# Comparing `tmp/ecoengine-1.5.9.tar.gz` & `tmp/ecoengine-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-1.5.9.tar", last modified: Wed Apr 24 23:01:50 2024, max compression
+gzip compressed data, was "ecoengine-1.6.0.tar", last modified: Thu May 16 22:09:22 2024, max compression
```

## Comparing `ecoengine-1.5.9.tar` & `ecoengine-1.6.0.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.253154 ecoengine-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 23:00:11.000000 ecoengine-1.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-24 23:01:50.253154 ecoengine-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 23:00:11.000000 ecoengine-1.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 23:00:11.000000 ecoengine-1.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-24 23:01:50.253154 ecoengine-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 23:00:11.000000 ecoengine-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.157153 ecoengine-1.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.161153 ecoengine-1.5.9/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.161153 ecoengine-1.5.9/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.161153 ecoengine-1.5.9/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.169153 ecoengine-1.5.9/src/ecoengine/data/climate_data/
--rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.173153 ecoengine-1.5.9/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.173153 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/maps.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.249154 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.249154 ecoengine-1.5.9/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    43027 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/engine/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.253154 ecoengine-1.5.9/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/PrefMapTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/SimulationRun.py
--rw-r--r--   0 runner    (1001) docker     (127)    48934 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/UtilityCostTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.253154 ecoengine-1.5.9/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/MultiPass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/MultiPassRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/PrimaryWithRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/SwingTankER.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:00:11.000000 ecoengine-1.5.9/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.253154 ecoengine-1.5.9/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-24 23:01:50.000000 ecoengine-1.5.9/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-04-24 23:01:50.000000 ecoengine-1.5.9/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:01:50.000000 ecoengine-1.5.9/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 23:01:50.000000 ecoengine-1.5.9/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 23:01:50.000000 ecoengine-1.5.9/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.982072 ecoengine-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 22:07:42.000000 ecoengine-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 22:09:22.982072 ecoengine-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-16 22:07:42.000000 ecoengine-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 22:07:42.000000 ecoengine-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-16 22:09:22.982072 ecoengine-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 22:07:42.000000 ecoengine-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.886070 ecoengine-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.890071 ecoengine-1.6.0/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.890071 ecoengine-1.6.0/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.890071 ecoengine-1.6.0/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.894071 ecoengine-1.6.0/src/ecoengine/data/climate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.902071 ecoengine-1.6.0/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.902071 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/maps.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.974072 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.978072 ecoengine-1.6.0/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43027 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/engine/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.978072 ecoengine-1.6.0/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/PrefMapTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/SimulationRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48934 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/UtilityCostTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.982072 ecoengine-1.6.0/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/MultiPass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/MultiPassRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/PrimaryWithRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/SwingTankER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:07:42.000000 ecoengine-1.6.0/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:09:22.982072 ecoengine-1.6.0/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 22:09:22.000000 ecoengine-1.6.0/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-16 22:09:22.000000 ecoengine-1.6.0/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:09:22.000000 ecoengine-1.6.0/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 22:09:22.000000 ecoengine-1.6.0/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 22:09:22.000000 ecoengine-1.6.0/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-1.5.9/PKG-INFO` & `ecoengine-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.5.9
+Version: 1.6.0
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.5.9/README.md` & `ecoengine-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/setup.cfg` & `ecoengine-1.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 1.5.9
+version = 1.6.0
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-1.5.9/src/ecoengine/__init__.py` & `ecoengine-1.6.0/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/constants/Constants.py` & `ecoengine-1.6.0/src/ecoengine/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv` & `ecoengine-1.6.0/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv` & `ecoengine-1.6.0/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv` & `ecoengine-1.6.0/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv` & `ecoengine-1.6.0/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv` & `ecoengine-1.6.0/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-1.6.0/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/maps.json` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/maps.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,93 @@
-00000000: 8004 9511 0400 0000 0000 005d 9428 5d94  ...........].(].
+00000000: 8004 95bb 0500 0000 0000 005d 9428 5d94  ...........].(].
 00000010: 288c 156e 756d 7079 2e63 6f72 652e 6d75  (..numpy.core.mu
 00000020: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
 00000030: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
 00000040: 7970 6594 9394 8c02 6638 9489 8887 9452  ype.....f8.....R
 00000050: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
 00000060: 4aff ffff ff4b 0074 9462 4308 0000 0000  J....K.t.bC.....
-00000070: 0080 4640 9486 9452 9468 0468 0a43 08cd  ..F@...R.h.h.C..
-00000080: cccc cccc ac50 4094 8694 5294 6804 680a  .....P@...R.h.h.
-00000090: 4308 3333 3333 3313 5640 9486 9452 9468  C.33333.V@...R.h
-000000a0: 0468 0a43 0800 0000 0000 805b 4094 8694  .h.C.......[@...
-000000b0: 5294 655d 9428 5d94 285d 9428 6804 680a  R.e].(].(].(h.h.
-000000c0: 4308 0000 0000 0000 4e40 9486 9452 945d  C.......N@...R.]
-000000d0: 9468 0468 0a43 08cd cccc cccc 8c50 4094  .h.h.C.......P@.
-000000e0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-000000f0: 0000 0000 0054 4094 8694 5294 5d94 6804  .....T@...R.].h.
-00000100: 680a 4308 0ad7 a370 3d9a 5540 9486 9452  h.C....p=.U@...R
-00000110: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
-00000120: 0000 5940 9486 9452 945d 9468 0468 0a43  ..Y@...R.].h.h.C
-00000130: 0800 0000 0000 805a 4094 8694 5294 6165  .......Z@...R.ae
-00000140: 5d94 2868 0468 0a43 0800 0000 0000 005e  ].(h.h.C.......^
-00000150: 4094 8694 5294 5d94 6804 680a 4308 48e1  @...R.].h.h.C.H.
-00000160: 7a14 ae87 5f40 9486 9452 9461 655d 9428  z..._@...R.ae].(
-00000170: 6804 680a 4308 0000 0000 0080 6140 9486  h.h.C.......a@..
-00000180: 9452 945d 9468 0468 0a43 08ae 47e1 7a14  .R.].h.h.C..G.z.
-00000190: 3e62 4094 8694 5294 6165 655d 9428 5d94  >b@...R.aee].(].
-000001a0: 2868 0468 0a43 0800 0000 0000 004e 4094  (h.h.C.......N@.
-000001b0: 8694 5294 5d94 6804 680a 4308 ec51 b81e  ..R.].h.h.C..Q..
-000001c0: 850b 5140 9486 9452 9461 655d 9428 6804  ..Q@...R.ae].(h.
-000001d0: 680a 4308 0000 0000 0000 5440 9486 9452  h.C.......T@...R
-000001e0: 945d 9468 0468 0a43 08a4 703d 0ad7 c355  .].h.h.C..p=...U
-000001f0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000200: 0800 0000 0000 0059 4094 8694 5294 5d94  .......Y@...R.].
-00000210: 6804 680a 4308 5c8f c2f5 28dc 5a40 9486  h.h.C.\...(.Z@..
-00000220: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-00000230: 0000 0000 5e40 9486 9452 945d 9468 0468  ....^@...R.].h.h
-00000240: 0a43 08ae 47e1 7a14 ce5f 4094 8694 5294  .C..G.z.._@...R.
-00000250: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
-00000260: 8061 4094 8694 5294 5d94 6804 680a 4308  .a@...R.].h.h.C.
-00000270: c3f5 285c 8f6a 6240 9486 9452 9461 6565  ..(\.jb@...R.aee
-00000280: 5d94 285d 9428 6804 680a 4308 0000 0000  ].(].(h.h.C.....
-00000290: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
-000002a0: 0848 e17a 14ae 9756 4094 8694 5294 6165  .H.z...V@...R.ae
-000002b0: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
-000002c0: 4094 8694 5294 5d94 6804 680a 4308 5c8f  @...R.].h.h.C.\.
-000002d0: c2f5 285c 5b40 9486 9452 9461 655d 9428  ..(\[@...R.ae].(
-000002e0: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
-000002f0: 9452 945d 9468 0468 0a43 08f6 285c 8fc2  .R.].h.h.C..(\..
-00000300: 1560 4094 8694 5294 6165 5d94 2868 0468  .`@...R.ae].(h.h
-00000310: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
-00000320: 5d94 6804 680a 4308 cdcc cccc cc74 6240  ].h.h.C......tb@
-00000330: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
-00000340: 680a 4308 0000 0000 0000 5440 9486 9452  h.C.......T@...R
-00000350: 945d 9468 0468 0a43 0848 e17a 14ae 1757  .].h.h.C.H.z...W
-00000360: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000370: 0800 0000 0000 0059 4094 8694 5294 5d94  .......Y@...R.].
-00000380: 6804 680a 4308 1f85 eb51 b89e 5b40 9486  h.h.C....Q..[@..
-00000390: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-000003a0: 0000 0000 5e40 9486 9452 945d 9468 0468  ....^@...R.].h.h
-000003b0: 0a43 0848 e17a 14ae 2760 4094 8694 5294  .C.H.z..'`@...R.
-000003c0: 6165 6565 5d94 2868 0468 0a43 0800 0000  aeee].(h.h.C....
-000003d0: 0000 004e 4094 8694 5294 6804 680a 4308  ...N@...R.h.h.C.
-000003e0: 0000 0000 0080 6140 9486 9452 9465 5d94  ......a@...R.e].
-000003f0: 2847 404b 8666 6666 6666 4740 2a28 f5c2  (G@K.fffffG@*(..
-00000400: 8f5c 2965 5d94 2847 403c e3d7 0a3d 70a4  .\)e].(G@<...=p.
-00000410: 4740 2d00 0000 0000 0065 652e            G@-......ee.
+00000070: 0000 4140 9486 9452 9468 0468 0a43 0800  ..A@...R.h.h.C..
+00000080: 0000 0000 8046 4094 8694 5294 6804 680a  .....F@...R.h.h.
+00000090: 4308 cdcc cccc ccac 5040 9486 9452 9468  C.......P@...R.h
+000000a0: 0468 0a43 0800 0000 0000 0051 4094 8694  .h.C.......Q@...
+000000b0: 5294 6804 680a 4308 3333 3333 3313 5640  R.h.h.C.33333.V@
+000000c0: 9486 9452 9468 0468 0a43 0800 0000 0000  ...R.h.h.C......
+000000d0: c057 4094 8694 5294 6804 680a 4308 0000  .W@...R.h.h.C...
+000000e0: 0000 0080 5b40 9486 9452 9465 5d94 285d  ....[@...R.e].(]
+000000f0: 945d 9428 6804 680a 4308 0000 0000 0040  .].(h.h.C......@
+00000100: 5f40 9486 9452 945d 9468 0468 0a43 0800  _@...R.].h.h.C..
+00000110: 0000 0000 8061 4094 8694 5294 6165 615d  .....a@...R.aea]
+00000120: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
+00000130: 0044 4094 8694 5294 5d94 6804 680a 4308  .D@...R.].h.h.C.
+00000140: ec51 b81e 85cb 4640 9486 9452 9461 655d  .Q....F@...R.ae]
+00000150: 9428 6804 680a 4308 0000 0000 0000 4e40  .(h.h.C.......N@
+00000160: 9486 9452 945d 9468 0468 0a43 0852 b81e  ...R.].h.h.C.R..
+00000170: 85eb 3150 4094 8694 5294 6165 5d94 2868  ..1P@...R.ae].(h
+00000180: 0468 0a43 0800 0000 0000 0054 4094 8694  .h.C.......T@...
+00000190: 5294 5d94 6804 680a 4308 0ad7 a370 3d7a  R.].h.h.C....p=z
+000001a0: 5540 9486 9452 9461 655d 9428 6804 680a  U@...R.ae].(h.h.
+000001b0: 4308 0000 0000 0000 5940 9486 9452 945d  C.......Y@...R.]
+000001c0: 9468 0468 0a43 08c3 f528 5c8f 225a 4094  .h.h.C...(\."Z@.
+000001d0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+000001e0: 0000 0000 005e 4094 8694 5294 5d94 6804  .....^@...R.].h.
+000001f0: 680a 4308 f628 5c8f c225 5f40 9486 9452  h.C..(\..%_@...R
+00000200: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+00000210: 0080 6140 9486 9452 945d 9468 0468 0a43  ..a@...R.].h.h.C
+00000220: 08cd cccc cccc 2c62 4094 8694 5294 6165  ......,b@...R.ae
+00000230: 655d 9428 5d94 2868 0468 0a43 0800 0000  e].(].(h.h.C....
+00000240: 0000 0044 4094 8694 5294 5d94 6804 680a  ...D@...R.].h.h.
+00000250: 4308 7b14 ae47 e1ba 4740 9486 9452 9461  C.{..G..G@...R.a
+00000260: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000270: 4e40 9486 9452 945d 9468 0468 0a43 0829  N@...R.].h.h.C.)
+00000280: 5c8f c2f5 d850 4094 8694 5294 6165 5d94  \....P@...R.ae].
+00000290: 2868 0468 0a43 0800 0000 0000 0054 4094  (h.h.C.......T@.
+000002a0: 8694 5294 5d94 6804 680a 4308 e17a 14ae  ..R.].h.h.C..z..
+000002b0: 47a1 5540 9486 9452 9461 655d 9428 6804  G.U@...R.ae].(h.
+000002c0: 680a 4308 0000 0000 0000 5940 9486 9452  h.C.......Y@...R
+000002d0: 945d 9468 0468 0a43 089a 9999 9999 c95a  .].h.h.C.......Z
+000002e0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
+000002f0: 0800 0000 0000 005e 4094 8694 5294 5d94  .......^@...R.].
+00000300: 6804 680a 4308 85eb 51b8 1ec5 5f40 9486  h.h.C...Q..._@..
+00000310: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
+00000320: 0000 0080 6140 9486 9452 945d 9468 0468  ....a@...R.].h.h
+00000330: 0a43 0848 e17a 14ae 6762 4094 8694 5294  .C.H.z..gb@...R.
+00000340: 6165 655d 945d 9428 6804 680a 4308 0000  aee].].(h.h.C...
+00000350: 0000 0040 5f40 9486 9452 945d 9468 0468  ...@_@...R.].h.h
+00000360: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
+00000370: 6165 615d 9428 5d94 2868 0468 0a43 0800  aea].(].(h.h.C..
+00000380: 0000 0000 004e 4094 8694 5294 5d94 6804  .....N@...R.].h.
+00000390: 680a 4308 8fc2 f528 5c4f 5140 9486 9452  h.C....(\OQ@...R
+000003a0: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+000003b0: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
+000003c0: 0885 eb51 b81e 3556 4094 8694 5294 6165  ...Q..5V@...R.ae
+000003d0: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
+000003e0: 4094 8694 5294 5d94 6804 680a 4308 ae47  @...R.].h.h.C..G
+000003f0: e17a 142e 5b40 9486 9452 9461 655d 9428  .z..[@...R.ae].(
+00000400: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
+00000410: 9452 945d 9468 0468 0a43 0866 6666 6666  .R.].h.h.C.fffff
+00000420: e65f 4094 8694 5294 6165 5d94 2868 0468  ._@...R.ae].(h.h
+00000430: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
+00000440: 5d94 6804 680a 4308 c3f5 285c 8f8a 6240  ].h.h.C...(\..b@
+00000450: 9486 9452 9461 6565 5d94 5d94 2868 0468  ...R.aee].].(h.h
+00000460: 0a43 0800 0000 0000 405f 4094 8694 5294  .C......@_@...R.
+00000470: 5d94 6804 680a 4308 0000 0000 0080 6140  ].h.h.C.......a@
+00000480: 9486 9452 9461 6561 5d94 285d 9428 6804  ...R.aea].(].(h.
+00000490: 680a 4308 0000 0000 0000 4e40 9486 9452  h.C.......N@...R
+000004a0: 945d 9468 0468 0a43 08ae 47e1 7a14 ce51  .].h.h.C..G.z..Q
+000004b0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
+000004c0: 0800 0000 0000 0054 4094 8694 5294 5d94  .......T@...R.].
+000004d0: 6804 680a 4308 1f85 eb51 b8ae 5640 9486  h.h.C....Q..V@..
+000004e0: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
+000004f0: 0000 0000 5940 9486 9452 945d 9468 0468  ....Y@...R.].h.h
+00000500: 0a43 0866 6666 6666 665b 4094 8694 5294  .C.ffffff[@...R.
+00000510: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
+00000520: 005e 4094 8694 5294 5d94 6804 680a 4308  .^@...R.].h.h.C.
+00000530: a470 3d0a d743 6040 9486 9452 9461 655d  .p=..C`@...R.ae]
+00000540: 9428 6804 680a 4308 0000 0000 0080 6140  .(h.h.C.......a@
+00000550: 9486 9452 945d 9468 0468 0a43 0833 3333  ...R.].h.h.C.333
+00000560: 3333 bb62 4094 8694 5294 6165 6565 5d94  33.b@...R.aeee].
+00000570: 2868 0468 0a43 0800 0000 0000 0044 4094  (h.h.C.......D@.
+00000580: 8694 5294 6804 680a 4308 0000 0000 0080  ..R.h.h.C.......
+00000590: 6140 9486 9452 9465 5d94 2847 4036 ae14  a@...R.e].(G@6..
+000005a0: 7ae1 47ae 4740 1a5c 28f5 c28f 5c65 5d94  z.G.G@.\(...\e].
+000005b0: 2847 4026 3333 3333 3333 4740 1333 3333  (G@&333333G@.333
+000005c0: 3333 3365 652e                           333ee.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9530 0a00 0000 0000 008c 1a73 6369  ...0.........sci
+00000000: 8004 955e 0c00 0000 0000 008c 1a73 6369  ...^.........sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,154 +11,189 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 4010 5798 851e 998c 0973 696d 706c  G.@.W......simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 154b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 1d4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 43fc 0c00 0000 0d00  ..K.t.b.C.......
-00000150: 0000 1000 0000 0600 0000 0a00 0000 0500  ................
-00000160: 0000 0500 0000 0a00 0000 0e00 0000 0100  ................
-00000170: 0000 0500 0000 0000 0000 0100 0000 0600  ................
-00000180: 0000 0500 0000 0600 0000 0100 0000 0700  ................
-00000190: 0000 0100 0000 0200 0000 0700 0000 0300  ................
-000001a0: 0000 0800 0000 0200 0000 0200 0000 0800  ................
-000001b0: 0000 0700 0000 0b00 0000 0c00 0000 1000  ................
-000001c0: 0000 0f00 0000 0b00 0000 1000 0000 0b00  ................
-000001d0: 0000 0f00 0000 0e00 0000 0a00 0000 0b00  ................
-000001e0: 0000 0e00 0000 0800 0000 0b00 0000 0700  ................
-000001f0: 0000 0b00 0000 0800 0000 0c00 0000 0b00  ................
-00000200: 0000 0600 0000 0700 0000 0b00 0000 0a00  ................
-00000210: 0000 0600 0000 0900 0000 0300 0000 0400  ................
-00000220: 0000 0900 0000 0800 0000 0300 0000 0800  ................
-00000230: 0000 0900 0000 0c00 0000 0c00 0000 0900  ................
-00000240: 0000 0d00 0000 9474 9462 8c09 6e65 6967  .......t.b..neig
-00000250: 6862 6f72 7394 6811 6814 4b00 8594 6816  hbors.h.h.K...h.
-00000260: 8794 5294 284b 014b 154b 0386 9468 1e89  ..R.(K.K.K...h..
-00000270: 43fc ffff ffff 0900 0000 1400 0000 0200  C...............
-00000280: 0000 0400 0000 1000 0000 0c00 0000 ffff  ................
-00000290: ffff 0100 0000 ffff ffff ffff ffff 0400  ................
-000002a0: 0000 0100 0000 0300 0000 0500 0000 0600  ................
-000002b0: 0000 0f00 0000 0400 0000 0800 0000 0500  ................
-000002c0: 0000 ffff ffff 0800 0000 ffff ffff 1200  ................
-000002d0: 0000 0d00 0000 0600 0000 0700 0000 0000  ................
-000002e0: 0000 0a00 0000 0e00 0000 0900 0000 ffff  ................
-000002f0: ffff 0b00 0000 ffff ffff 0c00 0000 0a00  ................
-00000300: 0000 0b00 0000 0200 0000 1000 0000 0f00  ................
-00000310: 0000 0800 0000 0e00 0000 1300 0000 0900  ................
-00000320: 0000 0d00 0000 0500 0000 0d00 0000 1000  ................
-00000330: 0000 0100 0000 0f00 0000 0c00 0000 ffff  ................
-00000340: ffff ffff ffff 1200 0000 0700 0000 1100  ................
-00000350: 0000 1300 0000 1400 0000 0e00 0000 1200  ................
-00000360: 0000 ffff ffff 0000 0000 1300 0000 9474  ...............t
-00000370: 9462 8c09 6571 7561 7469 6f6e 7394 6811  .b..equations.h.
-00000380: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000390: 154b 0486 9468 1b8c 0266 3894 8988 8794  .K...h...f8.....
-000003a0: 5294 284b 0368 1f4e 4e4e 4aff ffff ff4a  R.(K.h.NNNJ....J
-000003b0: ffff ffff 4b00 7494 6289 42a0 0200 0067  ....K.t.b.B....g
-000003c0: f1b8 d95c 6ee6 3fc9 8c40 e6a7 1be1 3f7a  ...\n.?..@....?z
-000003d0: 4ef2 c8c1 35de bf95 e31c 6750 a955 c0de  N...5.....gP.U..
-000003e0: f909 3617 70e0 3f36 7966 20f5 32e2 3f87  ..6.p.?6yf .2.?.
-000003f0: 4fa6 6d99 8ee4 bffa 3a60 8434 ee4d c068  O.m.....:`.4.M.h
-00000400: 9364 6146 46d5 3f80 fcc6 08bc 9fe6 3f9b  .daFF.?.......?.
-00000410: febe eda0 f9e3 bf2f 788f 33da 3a4d c013  ......./x.3.:M..
-00000420: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000430: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c013  ..[.^.....1..J..
-00000440: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000450: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c0b6  ..[.^.....1..J..
-00000460: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000470: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b6  ....b...S...?N..
-00000480: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000490: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b5  ....b...S...?N..
-000004a0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004b0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0b5  t*......s..^.Q..
-000004c0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004d0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0d5  t*......s..^.Q..
-000004e0: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-000004f0: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0d5  .U,.H......C.S..
-00000500: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-00000510: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0ca  .U,.H......C.S..
-00000520: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000530: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c0ca  ........7.. <R..
-00000540: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000550: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c048  ........7.. <R.H
-00000560: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000570: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c048  ...Ts..!.:ohOR.H
-00000580: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000590: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c06c  ...Ts..!.:ohOR.l
-000005a0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005b0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c06c  ...s.......].P.l
-000005c0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005d0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c006  ...s.......].P..
-000005e0: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-000005f0: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c006  .G.6......mC.S..
-00000600: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-00000610: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c06b  .G.6......mC.S.k
-00000620: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000630: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c06b  :.Z....v...4>T.k
-00000640: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000650: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c094  :.Z....v...4>T..
-00000660: 7494 628c 0863 6f70 6c61 6e61 7294 6811  t.b..coplanar.h.
-00000670: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000680: 004b 0386 9468 1e89 4300 9474 9462 8c04  .K...h..C..t.b..
-00000690: 676f 6f64 9468 1168 144b 0085 9468 1687  good.h.h.K...h..
-000006a0: 9452 9428 4b01 4b15 8594 681e 8943 5401  .R.(K.K...h..CT.
-000006b0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006c0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006d0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006e0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006f0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-00000700: 0000 0094 7494 628c 086e 7369 6d70 6c65  ....t.b..nsimple
-00000710: 7894 4b15 8c0a 5f74 7261 6e73 666f 726d  x.K..._transform
-00000720: 944e 8c12 5f76 6572 7465 785f 746f 5f73  .N.._vertex_to_s
-00000730: 696d 706c 6578 944e 8c19 5f76 6572 7465  implex.N.._verte
-00000740: 785f 6e65 6967 6862 6f72 5f76 6572 7469  x_neighbor_verti
-00000750: 6365 7394 4e8c 095f 7665 7274 6963 6573  ces.N.._vertices
-00000760: 9468 188c 075f 706f 696e 7473 9468 1168  .h..._points.h.h
-00000770: 144b 0085 9468 1687 9452 9428 4b01 4b11  .K...h...R.(K.K.
-00000780: 4b02 8694 6831 8942 1001 0000 0000 0000  K...h1.B........
-00000790: 0000 4e40 0000 0000 0080 4640 0000 0000  ..N@......F@....
-000007a0: 0000 5440 0000 0000 0080 4640 0000 0000  ..T@......F@....
-000007b0: 0000 5940 0000 0000 0080 4640 0000 0000  ..Y@......F@....
-000007c0: 0000 5e40 0000 0000 0080 4640 0000 0000  ..^@......F@....
-000007d0: 0080 6140 0000 0000 0080 4640 0000 0000  ..a@......F@....
-000007e0: 0000 4e40 cdcc cccc ccac 5040 0000 0000  ..N@......P@....
-000007f0: 0000 5440 cdcc cccc ccac 5040 0000 0000  ..T@......P@....
-00000800: 0000 5940 cdcc cccc ccac 5040 0000 0000  ..Y@......P@....
-00000810: 0000 5e40 cdcc cccc ccac 5040 0000 0000  ..^@......P@....
-00000820: 0080 6140 cdcc cccc ccac 5040 0000 0000  ..a@......P@....
-00000830: 0000 5440 3333 3333 3313 5640 0000 0000  ..T@33333.V@....
-00000840: 0000 5940 3333 3333 3313 5640 0000 0000  ..Y@33333.V@....
-00000850: 0000 5e40 3333 3333 3313 5640 0000 0000  ..^@33333.V@....
-00000860: 0080 6140 3333 3333 3313 5640 0000 0000  ..a@33333.V@....
-00000870: 0000 5440 0000 0000 0080 5b40 0000 0000  ..T@......[@....
-00000880: 0000 5940 0000 0000 0080 5b40 0000 0000  ..Y@......[@....
-00000890: 0000 5e40 0000 0000 0080 5b40 9474 9462  ..^@......[@.t.b
-000008a0: 8c04 6e64 696d 944b 028c 076e 706f 696e  ..ndim.K...npoin
-000008b0: 7473 944b 118c 096d 696e 5f62 6f75 6e64  ts.K...min_bound
-000008c0: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
-000008d0: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
-000008e0: 004e 4000 0000 0000 8046 4094 7494 628c  .N@......F@.t.b.
-000008f0: 096d 6178 5f62 6f75 6e64 9468 1168 144b  .max_bound.h.h.K
-00000900: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000910: 6831 8943 1000 0000 0000 8061 4000 0000  h1.C.......a@...
-00000920: 0000 805b 4094 7494 628c 0d66 7572 7468  ...[@.t.b..furth
-00000930: 6573 745f 7369 7465 9489 7562 8c0c 7661  est_site..ub..va
-00000940: 6c75 6573 5f73 6861 7065 944b 0185 948c  lues_shape.K....
-00000950: 0676 616c 7565 7394 6811 6814 4b00 8594  .values.h.h.K...
-00000960: 6816 8794 5294 284b 014b 114b 0186 9468  h...R.(K.K.K...h
-00000970: 3189 4388 1f85 eb51 b89e 3f40 85eb 51b8  1.C....Q..?@..Q.
-00000980: 1ec5 3e40 9a99 9999 9919 3e40 0000 0000  ..>@......>@....
-00000990: 0000 3d40 a470 3d0a d7e3 3c40 a470 3d0a  ..=@.p=...<@.p=.
-000009a0: d743 4440 0ad7 a370 3d6a 4340 a470 3d0a  .CD@...p=jC@.p=.
-000009b0: d783 4240 8fc2 f528 5c0f 4240 14ae 47e1  ..B@...(\.B@..G.
-000009c0: 7a74 4140 e17a 14ae 4741 4840 ae47 e17a  ztA@.z..GAH@.G.z
-000009d0: 140e 4740 6666 6666 66e6 4540 ec51 b81e  ..G@fffff.E@.Q..
-000009e0: 85eb 4440 8fc2 f528 5c0f 4d40 7b14 ae47  ..D@...(\.M@{..G
-000009f0: e19a 4c40 6666 6666 6686 4b40 9474 9462  ..L@fffff.K@.t.b
-00000a00: 8c0a 6973 5f63 6f6d 706c 6578 9489 8c0a  ..is_complex....
-00000a10: 6669 6c6c 5f76 616c 7565 9447 7ff8 0000  fill_value.G....
-00000a20: 0000 0000 8c05 7363 616c 6594 4e8c 0670  ......scale.N..p
-00000a30: 6f69 6e74 7394 684b 7562 2e              oints.hKub.
+00000140: ffff 4b00 7494 6289 425c 0100 000d 0000  ..K.t.b.B\......
+00000150: 000c 0000 0012 0000 0012 0000 0003 0000  ................
+00000160: 0004 0000 0006 0000 000a 0000 0005 0000  ................
+00000170: 0005 0000 000a 0000 000e 0000 0009 0000  ................
+00000180: 0012 0000 0004 0000 0009 0000 000d 0000  ................
+00000190: 0012 0000 000c 0000 0008 0000 0012 0000  ................
+000001a0: 0008 0000 0003 0000 0012 0000 0013 0000  ................
+000001b0: 000d 0000 0010 0000 000c 0000 0013 0000  ................
+000001c0: 0010 0000 0013 0000 000c 0000 000d 0000  ................
+000001d0: 0003 0000 0011 0000 0004 0000 0011 0000  ................
+000001e0: 0003 0000 0002 0000 0001 0000 0011 0000  ................
+000001f0: 0002 0000 0011 0000 0001 0000 0000 0000  ................
+00000200: 0001 0000 0005 0000 0000 0000 0001 0000  ................
+00000210: 0006 0000 0005 0000 0006 0000 0001 0000  ................
+00000220: 0007 0000 0001 0000 0002 0000 0007 0000  ................
+00000230: 0003 0000 0008 0000 0002 0000 0002 0000  ................
+00000240: 0008 0000 0007 0000 000b 0000 000c 0000  ................
+00000250: 0010 0000 000f 0000 000b 0000 0010 0000  ................
+00000260: 000b 0000 000f 0000 000e 0000 000a 0000  ................
+00000270: 000b 0000 000e 0000 0008 0000 000b 0000  ................
+00000280: 0007 0000 000b 0000 0008 0000 000c 0000  ................
+00000290: 000b 0000 0006 0000 0007 0000 000b 0000  ................
+000002a0: 000a 0000 0006 0000 0094 7494 628c 096e  ..........t.b..n
+000002b0: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+000002c0: 9468 1687 9452 9428 4b01 4b1d 4b03 8694  .h...R.(K.K.K...
+000002d0: 681e 8942 5c01 0000 0600 0000 0500 0000  h..B\...........
+000002e0: 0a00 0000 0b00 0000 0400 0000 0700 0000  ................
+000002f0: 0300 0000 1000 0000 1c00 0000 1800 0000  ................
+00000300: ffff ffff 0200 0000 0100 0000 ffff ffff  ................
+00000310: 0500 0000 0000 0000 0400 0000 ffff ffff  ................
+00000320: 0700 0000 0000 0000 1a00 0000 0100 0000  ................
+00000330: 0600 0000 1300 0000 ffff ffff 0900 0000  ................
+00000340: 0a00 0000 0800 0000 1500 0000 0a00 0000  ................
+00000350: 0000 0000 0800 0000 0900 0000 ffff ffff  ................
+00000360: 0100 0000 0c00 0000 1300 0000 0d00 0000  ................
+00000370: 0b00 0000 0c00 0000 1200 0000 0e00 0000  ................
+00000380: 0f00 0000 ffff ffff 0d00 0000 ffff ffff  ................
+00000390: 0e00 0000 1000 0000 0200 0000 0f00 0000  ................
+000003a0: 1100 0000 1200 0000 1b00 0000 1000 0000  ................
+000003b0: 1400 0000 1100 0000 0d00 0000 1400 0000  ................
+000003c0: 0c00 0000 0700 0000 1900 0000 1200 0000  ................
+000003d0: 1300 0000 0900 0000 1600 0000 1a00 0000  ................
+000003e0: 1500 0000 ffff ffff 1700 0000 ffff ffff  ................
+000003f0: 1800 0000 1600 0000 1700 0000 0300 0000  ................
+00000400: 1c00 0000 1b00 0000 1400 0000 1a00 0000  ................
+00000410: 0600 0000 1500 0000 1900 0000 1100 0000  ................
+00000420: 1900 0000 1c00 0000 0200 0000 1b00 0000  ................
+00000430: 1800 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000440: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000450: 5294 284b 014b 1d4b 0486 9468 1b8c 0266  R.(K.K.K...h...f
+00000460: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000470: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000480: 42a0 0300 0079 af00 802c a4e7 3f85 710a  B....y...,..?.q.
+00000490: ba93 18dd 3fee d2ff ec01 d7df bf71 a24b  ....?........q.K
+000004a0: b263 6d54 c0c2 9c32 1d4f 0de9 3f3b 04d8  .cmT...2.O..?;..
+000004b0: cec6 25d5 3faa f025 bfb0 dee0 bf5f 2669  ..%.?..%....._&i
+000004c0: 22e0 1253 c0de f909 3617 70e0 3f36 7966  "..S....6.p.?6yf
+000004d0: 20f5 32e2 3f87 4fa6 6d99 8ee4 bffa 3a60   .2.?.O.m.....:`
+000004e0: 8434 ee4d c068 9364 6146 46d5 3f80 fcc6  .4.M.h.daFF.?...
+000004f0: 08bc 9fe6 3f9b febe eda0 f9e3 bf2f 788f  ....?......../x.
+00000500: 33da 3a4d c02e d28d 1c40 1de9 3fcb 70c0  3.:M.....@..?.p.
+00000510: bc0e 55d5 3f2d ed30 84ee b7e0 bf75 7a21  ..U.?-.0.....uz!
+00000520: 544b 4853 c0ae 70e0 f649 10e8 3fd7 6ce7  TKHS..p..I..?.l.
+00000530: 21d9 f6db 3f12 41e6 f363 96df bf83 27c3  !...?.A..c....'.
+00000540: 2018 9f54 c089 e33d 252c e8e6 3f84 4f54   ..T...=%,..?.OT
+00000550: 1157 9fdd 3f68 6780 e6f0 bae0 bf73 5285  .W..?hg......sR.
+00000560: 543a 5253 c021 2e77 446a a7e8 3f04 13e8  T:RS.!.wDj..?...
+00000570: c8db f1d5 3f6f c7fe cbd1 32e1 bf30 e296  ....?o....2..0..
+00000580: 3fae ae52 c084 732f a49e aee6 3fc9 4cb2  ?..R..s/....?.L.
+00000590: 3040 8ee1 3fb7 dc50 60a3 60dc bf90 e2fd  0@..?..P`.`.....
+000005a0: b085 2257 c0fb 6e1a ab32 bae4 3f8f 46a6  .."W..n..2..?.F.
+000005b0: c59b 46e2 3f7d 6a5b 49d4 22e0 bfb6 d591  ..F.?}j[I.".....
+000005c0: 1275 1b54 c0ed 0077 dc3a 44e7 3f1f c760  .u.T...w.:D.?..`
+000005d0: d667 cdde 3faf d20c 8eca 55df bfc6 2c83  .g..?.....U...,.
+000005e0: ace3 d954 c0b4 8f00 85cb 99e9 3f0b 9233  ...T........?..3
+000005f0: db6b e6d0 3f0d 3f9d ff4a 3de1 bfc4 68c0  .k..?.?..J=...h.
+00000600: a2da a952 c055 52b5 391c 58e8 3f28 9f8b  ...R.UR.9.X.?(..
+00000610: 51f3 efcd 3f36 be13 0eb4 5fe3 bfd4 c345  Q...?6...._....E
+00000620: 6e09 1e50 c0c0 e7c2 d436 d7e6 3fc6 dfd1  n..P.....6..?...
+00000630: 1007 a0b7 bf4b cee4 6f7a 37e6 bf4d 5eed  .....K..oz7..M^.
+00000640: 4141 ec44 c06e 742f 24cd b2de 3f22 a2b0  AA.D.nt/$...?"..
+00000650: 4a01 7ee4 bf8d 36d8 7a12 32e3 bf00 b0cd  J.~...6.z.2.....
+00000660: 37fe 22a3 3f13 1176 4512 e3e1 3faa 631a  7.".?..vE...?.c.
+00000670: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+00000680: 31b5 cd4a c013 1176 4512 e3e1 3faa 631a  1..J...vE...?.c.
+00000690: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+000006a0: 31b5 cd4a c0b6 9ffd 9f60 f5e4 3f48 3817  1..J.....`..?H8.
+000006b0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006c0: bbb3 3f4e c0b6 9ffd 9f60 f5e4 3f48 3817  ..?N.....`..?H8.
+000006d0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006e0: bbb3 3f4e c0b5 41aa 8704 45e7 3f26 517b  ..?N..A...E.?&Q{
+000006f0: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000700: 0c5e 0b51 c0b5 41aa 8704 45e7 3f26 517b  .^.Q..A...E.?&Q{
+00000710: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000720: 0c5e 0b51 c0d5 906a 752a 76e4 3f3e 6845  .^.Q...ju*v.?>hE
+00000730: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000740: 1243 dd53 c0d5 906a 752a 76e4 3f3e 6845  .C.S...ju*v.?>hE
+00000750: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000760: 1243 dd53 c0ca 8133 6685 00e2 3f15 176b  .C.S...3f...?..k
+00000770: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+00000780: b920 3c52 c0ca 8133 6685 00e2 3f15 176b  . <R...3f...?..k
+00000790: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+000007a0: b920 3c52 c048 25d3 cc6b ede5 3f5d fafa  . <R.H%..k..?]..
+000007b0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007c0: 6f68 4f52 c048 25d3 cc6b ede5 3f5d fafa  ohOR.H%..k..?]..
+000007d0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007e0: 6f68 4f52 c06c d244 aef5 84e3 3f6d 43bb  ohOR.l.D....?mC.
+000007f0: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000800: c55d 8850 c06c d244 aef5 84e3 3f6d 43bb  .].P.l.D....?mC.
+00000810: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000820: c55d 8850 c094 7494 628c 0863 6f70 6c61  .].P..t.b..copla
+00000830: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000840: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000850: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000860: 0085 9468 1687 9452 9428 4b01 4b1d 8594  ...h...R.(K.K...
+00000870: 681e 8943 7401 0000 0001 0000 0001 0000  h..Ct...........
+00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008a0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008b0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008c0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008d0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008e0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+000008f0: 7369 6d70 6c65 7894 4b1d 8c0a 5f74 7261  simplex.K..._tra
+00000900: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000910: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000920: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000930: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000940: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000950: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000960: 9428 4b01 4b14 4b02 8694 6831 8942 4001  .(K.K.K...h1.B@.
+00000970: 0000 0000 0000 0000 4e40 0000 0000 0080  ........N@......
+00000980: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000990: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+000009a0: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+000009b0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+000009c0: 4640 0000 0000 0000 4e40 cdcc cccc ccac  F@......N@......
+000009d0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+000009e0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+000009f0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000a00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000a10: 5040 0000 0000 0000 5440 3333 3333 3313  P@......T@33333.
+00000a20: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000a30: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000a40: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000a50: 5640 0000 0000 0000 5440 0000 0000 0080  V@......T@......
+00000a60: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000a70: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000a80: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000a90: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000aa0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ab0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000ac0: 076e 706f 696e 7473 944b 148c 096d 696e  .npoints.K...min
+00000ad0: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000ae0: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000af0: 1000 0000 0000 004e 4000 0000 0000 0041  .......N@......A
+00000b00: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000b10: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000b20: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000b30: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000b40: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000b50: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000b60: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000b70: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000b80: 144b 0186 9468 3189 43a0 1f85 eb51 b89e  .K...h1.C....Q..
+00000b90: 3f40 85eb 51b8 1ec5 3e40 9a99 9999 9919  ?@..Q...>@......
+00000ba0: 3e40 0000 0000 0000 3d40 a470 3d0a d7e3  >@......=@.p=...
+00000bb0: 3c40 a470 3d0a d743 4440 0ad7 a370 3d6a  <@.p=..CD@...p=j
+00000bc0: 4340 a470 3d0a d783 4240 8fc2 f528 5c0f  C@.p=...B@...(\.
+00000bd0: 4240 14ae 47e1 7a74 4140 e17a 14ae 4741  B@..G.ztA@.z..GA
+00000be0: 4840 ae47 e17a 140e 4740 6666 6666 66e6  H@.G.z..G@fffff.
+00000bf0: 4540 ec51 b81e 85eb 4440 8fc2 f528 5c0f  E@.Q....D@...(\.
+00000c00: 4d40 7b14 ae47 e19a 4c40 6666 6666 6686  M@{..G..L@fffff.
+00000c10: 4b40 cdcc cccc cccc 3640 9a99 9999 9999  K@......6@......
+00000c20: 4040 0000 0000 00c0 4340 9474 9462 8c0a  @@......C@.t.b..
+00000c30: 6973 5f63 6f6d 706c 6578 9489 8c0a 6669  is_complex....fi
+00000c40: 6c6c 5f76 616c 7565 9447 7ff8 0000 0000  ll_value.G......
+00000c50: 0000 8c05 7363 616c 6594 4e8c 0670 6f69  ....scale.N..poi
+00000c60: 6e74 7394 684b 7562 2e                   nts.hKub.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9530 0a00 0000 0000 008c 1a73 6369  ...0.........sci
+00000000: 8004 955e 0c00 0000 0000 008c 1a73 6369  ...^.........sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,154 +11,189 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 4010 5798 851e 998c 0973 696d 706c  G.@.W......simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 154b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 1d4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 43fc 0c00 0000 0d00  ..K.t.b.C.......
-00000150: 0000 1000 0000 0600 0000 0a00 0000 0500  ................
-00000160: 0000 0500 0000 0a00 0000 0e00 0000 0100  ................
-00000170: 0000 0500 0000 0000 0000 0100 0000 0600  ................
-00000180: 0000 0500 0000 0600 0000 0100 0000 0700  ................
-00000190: 0000 0100 0000 0200 0000 0700 0000 0300  ................
-000001a0: 0000 0800 0000 0200 0000 0200 0000 0800  ................
-000001b0: 0000 0700 0000 0b00 0000 0c00 0000 1000  ................
-000001c0: 0000 0f00 0000 0b00 0000 1000 0000 0b00  ................
-000001d0: 0000 0f00 0000 0e00 0000 0a00 0000 0b00  ................
-000001e0: 0000 0e00 0000 0800 0000 0b00 0000 0700  ................
-000001f0: 0000 0b00 0000 0800 0000 0c00 0000 0b00  ................
-00000200: 0000 0600 0000 0700 0000 0b00 0000 0a00  ................
-00000210: 0000 0600 0000 0900 0000 0300 0000 0400  ................
-00000220: 0000 0900 0000 0800 0000 0300 0000 0800  ................
-00000230: 0000 0900 0000 0c00 0000 0c00 0000 0900  ................
-00000240: 0000 0d00 0000 9474 9462 8c09 6e65 6967  .......t.b..neig
-00000250: 6862 6f72 7394 6811 6814 4b00 8594 6816  hbors.h.h.K...h.
-00000260: 8794 5294 284b 014b 154b 0386 9468 1e89  ..R.(K.K.K...h..
-00000270: 43fc ffff ffff 0900 0000 1400 0000 0200  C...............
-00000280: 0000 0400 0000 1000 0000 0c00 0000 ffff  ................
-00000290: ffff 0100 0000 ffff ffff ffff ffff 0400  ................
-000002a0: 0000 0100 0000 0300 0000 0500 0000 0600  ................
-000002b0: 0000 0f00 0000 0400 0000 0800 0000 0500  ................
-000002c0: 0000 ffff ffff 0800 0000 ffff ffff 1200  ................
-000002d0: 0000 0d00 0000 0600 0000 0700 0000 0000  ................
-000002e0: 0000 0a00 0000 0e00 0000 0900 0000 ffff  ................
-000002f0: ffff 0b00 0000 ffff ffff 0c00 0000 0a00  ................
-00000300: 0000 0b00 0000 0200 0000 1000 0000 0f00  ................
-00000310: 0000 0800 0000 0e00 0000 1300 0000 0900  ................
-00000320: 0000 0d00 0000 0500 0000 0d00 0000 1000  ................
-00000330: 0000 0100 0000 0f00 0000 0c00 0000 ffff  ................
-00000340: ffff ffff ffff 1200 0000 0700 0000 1100  ................
-00000350: 0000 1300 0000 1400 0000 0e00 0000 1200  ................
-00000360: 0000 ffff ffff 0000 0000 1300 0000 9474  ...............t
-00000370: 9462 8c09 6571 7561 7469 6f6e 7394 6811  .b..equations.h.
-00000380: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000390: 154b 0486 9468 1b8c 0266 3894 8988 8794  .K...h...f8.....
-000003a0: 5294 284b 0368 1f4e 4e4e 4aff ffff ff4a  R.(K.h.NNNJ....J
-000003b0: ffff ffff 4b00 7494 6289 42a0 0200 0067  ....K.t.b.B....g
-000003c0: f1b8 d95c 6ee6 3fc9 8c40 e6a7 1be1 3f7a  ...\n.?..@....?z
-000003d0: 4ef2 c8c1 35de bf95 e31c 6750 a955 c0de  N...5.....gP.U..
-000003e0: f909 3617 70e0 3f36 7966 20f5 32e2 3f87  ..6.p.?6yf .2.?.
-000003f0: 4fa6 6d99 8ee4 bffa 3a60 8434 ee4d c068  O.m.....:`.4.M.h
-00000400: 9364 6146 46d5 3f80 fcc6 08bc 9fe6 3f9b  .daFF.?.......?.
-00000410: febe eda0 f9e3 bf2f 788f 33da 3a4d c013  ......./x.3.:M..
-00000420: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000430: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c013  ..[.^.....1..J..
-00000440: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000450: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c0b6  ..[.^.....1..J..
-00000460: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000470: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b6  ....b...S...?N..
-00000480: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000490: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b5  ....b...S...?N..
-000004a0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004b0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0b5  t*......s..^.Q..
-000004c0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004d0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0d5  t*......s..^.Q..
-000004e0: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-000004f0: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0d5  .U,.H......C.S..
-00000500: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-00000510: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0ca  .U,.H......C.S..
-00000520: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000530: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c0ca  ........7.. <R..
-00000540: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000550: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c048  ........7.. <R.H
-00000560: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000570: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c048  ...Ts..!.:ohOR.H
-00000580: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000590: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c06c  ...Ts..!.:ohOR.l
-000005a0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005b0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c06c  ...s.......].P.l
-000005c0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005d0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c006  ...s.......].P..
-000005e0: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-000005f0: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c006  .G.6......mC.S..
-00000600: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-00000610: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c06b  .G.6......mC.S.k
-00000620: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000630: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c06b  :.Z....v...4>T.k
-00000640: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000650: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c094  :.Z....v...4>T..
-00000660: 7494 628c 0863 6f70 6c61 6e61 7294 6811  t.b..coplanar.h.
-00000670: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000680: 004b 0386 9468 1e89 4300 9474 9462 8c04  .K...h..C..t.b..
-00000690: 676f 6f64 9468 1168 144b 0085 9468 1687  good.h.h.K...h..
-000006a0: 9452 9428 4b01 4b15 8594 681e 8943 5401  .R.(K.K...h..CT.
-000006b0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006c0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006d0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006e0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006f0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-00000700: 0000 0094 7494 628c 086e 7369 6d70 6c65  ....t.b..nsimple
-00000710: 7894 4b15 8c0a 5f74 7261 6e73 666f 726d  x.K..._transform
-00000720: 944e 8c12 5f76 6572 7465 785f 746f 5f73  .N.._vertex_to_s
-00000730: 696d 706c 6578 944e 8c19 5f76 6572 7465  implex.N.._verte
-00000740: 785f 6e65 6967 6862 6f72 5f76 6572 7469  x_neighbor_verti
-00000750: 6365 7394 4e8c 095f 7665 7274 6963 6573  ces.N.._vertices
-00000760: 9468 188c 075f 706f 696e 7473 9468 1168  .h..._points.h.h
-00000770: 144b 0085 9468 1687 9452 9428 4b01 4b11  .K...h...R.(K.K.
-00000780: 4b02 8694 6831 8942 1001 0000 0000 0000  K...h1.B........
-00000790: 0000 4e40 0000 0000 0080 4640 0000 0000  ..N@......F@....
-000007a0: 0000 5440 0000 0000 0080 4640 0000 0000  ..T@......F@....
-000007b0: 0000 5940 0000 0000 0080 4640 0000 0000  ..Y@......F@....
-000007c0: 0000 5e40 0000 0000 0080 4640 0000 0000  ..^@......F@....
-000007d0: 0080 6140 0000 0000 0080 4640 0000 0000  ..a@......F@....
-000007e0: 0000 4e40 cdcc cccc ccac 5040 0000 0000  ..N@......P@....
-000007f0: 0000 5440 cdcc cccc ccac 5040 0000 0000  ..T@......P@....
-00000800: 0000 5940 cdcc cccc ccac 5040 0000 0000  ..Y@......P@....
-00000810: 0000 5e40 cdcc cccc ccac 5040 0000 0000  ..^@......P@....
-00000820: 0080 6140 cdcc cccc ccac 5040 0000 0000  ..a@......P@....
-00000830: 0000 5440 3333 3333 3313 5640 0000 0000  ..T@33333.V@....
-00000840: 0000 5940 3333 3333 3313 5640 0000 0000  ..Y@33333.V@....
-00000850: 0000 5e40 3333 3333 3313 5640 0000 0000  ..^@33333.V@....
-00000860: 0080 6140 3333 3333 3313 5640 0000 0000  ..a@33333.V@....
-00000870: 0000 5440 0000 0000 0080 5b40 0000 0000  ..T@......[@....
-00000880: 0000 5940 0000 0000 0080 5b40 0000 0000  ..Y@......[@....
-00000890: 0000 5e40 0000 0000 0080 5b40 9474 9462  ..^@......[@.t.b
-000008a0: 8c04 6e64 696d 944b 028c 076e 706f 696e  ..ndim.K...npoin
-000008b0: 7473 944b 118c 096d 696e 5f62 6f75 6e64  ts.K...min_bound
-000008c0: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
-000008d0: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
-000008e0: 004e 4000 0000 0000 8046 4094 7494 628c  .N@......F@.t.b.
-000008f0: 096d 6178 5f62 6f75 6e64 9468 1168 144b  .max_bound.h.h.K
-00000900: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000910: 6831 8943 1000 0000 0000 8061 4000 0000  h1.C.......a@...
-00000920: 0000 805b 4094 7494 628c 0d66 7572 7468  ...[@.t.b..furth
-00000930: 6573 745f 7369 7465 9489 7562 8c0c 7661  est_site..ub..va
-00000940: 6c75 6573 5f73 6861 7065 944b 0185 948c  lues_shape.K....
-00000950: 0676 616c 7565 7394 6811 6814 4b00 8594  .values.h.h.K...
-00000960: 6816 8794 5294 284b 014b 114b 0186 9468  h...R.(K.K.K...h
-00000970: 3189 4388 e17a 14ae 47e1 1c40 0000 0000  1.C..z..G..@....
-00000980: 0000 2140 713d 0ad7 a3f0 2340 52b8 1e85  ..!@q=....#@R...
-00000990: ebd1 2740 0000 0000 0000 2d40 e17a 14ae  ..'@......-@.z..
-000009a0: 47e1 1e40 14ae 47e1 7a94 2140 c3f5 285c  G..@..G.z.!@..(\
-000009b0: 8fc2 2440 14ae 47e1 7a94 2840 0000 0000  ..$@..G.z.(@....
-000009c0: 0080 2d40 9a99 9999 9999 2240 85eb 51b8  ..-@......"@..Q.
-000009d0: 1e45 3340 48e1 7a14 ae47 2940 d7a3 703d  .E3@H.z..G)@..p=
-000009e0: 0ad7 2d40 14ae 47e1 7a94 2340 52b8 1e85  ..-@..G.z.#@R...
-000009f0: eb51 2640 295c 8fc2 f528 2a40 9474 9462  .Q&@)\...(*@.t.b
-00000a00: 8c0a 6973 5f63 6f6d 706c 6578 9489 8c0a  ..is_complex....
-00000a10: 6669 6c6c 5f76 616c 7565 9447 7ff8 0000  fill_value.G....
-00000a20: 0000 0000 8c05 7363 616c 6594 4e8c 0670  ......scale.N..p
-00000a30: 6f69 6e74 7394 684b 7562 2e              oints.hKub.
+00000140: ffff 4b00 7494 6289 425c 0100 000d 0000  ..K.t.b.B\......
+00000150: 000c 0000 0012 0000 0012 0000 0003 0000  ................
+00000160: 0004 0000 0006 0000 000a 0000 0005 0000  ................
+00000170: 0005 0000 000a 0000 000e 0000 0009 0000  ................
+00000180: 0012 0000 0004 0000 0009 0000 000d 0000  ................
+00000190: 0012 0000 000c 0000 0008 0000 0012 0000  ................
+000001a0: 0008 0000 0003 0000 0012 0000 0013 0000  ................
+000001b0: 000d 0000 0010 0000 000c 0000 0013 0000  ................
+000001c0: 0010 0000 0013 0000 000c 0000 000d 0000  ................
+000001d0: 0003 0000 0011 0000 0004 0000 0011 0000  ................
+000001e0: 0003 0000 0002 0000 0001 0000 0011 0000  ................
+000001f0: 0002 0000 0011 0000 0001 0000 0000 0000  ................
+00000200: 0001 0000 0005 0000 0000 0000 0001 0000  ................
+00000210: 0006 0000 0005 0000 0006 0000 0001 0000  ................
+00000220: 0007 0000 0001 0000 0002 0000 0007 0000  ................
+00000230: 0003 0000 0008 0000 0002 0000 0002 0000  ................
+00000240: 0008 0000 0007 0000 000b 0000 000c 0000  ................
+00000250: 0010 0000 000f 0000 000b 0000 0010 0000  ................
+00000260: 000b 0000 000f 0000 000e 0000 000a 0000  ................
+00000270: 000b 0000 000e 0000 0008 0000 000b 0000  ................
+00000280: 0007 0000 000b 0000 0008 0000 000c 0000  ................
+00000290: 000b 0000 0006 0000 0007 0000 000b 0000  ................
+000002a0: 000a 0000 0006 0000 0094 7494 628c 096e  ..........t.b..n
+000002b0: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+000002c0: 9468 1687 9452 9428 4b01 4b1d 4b03 8694  .h...R.(K.K.K...
+000002d0: 681e 8942 5c01 0000 0600 0000 0500 0000  h..B\...........
+000002e0: 0a00 0000 0b00 0000 0400 0000 0700 0000  ................
+000002f0: 0300 0000 1000 0000 1c00 0000 1800 0000  ................
+00000300: ffff ffff 0200 0000 0100 0000 ffff ffff  ................
+00000310: 0500 0000 0000 0000 0400 0000 ffff ffff  ................
+00000320: 0700 0000 0000 0000 1a00 0000 0100 0000  ................
+00000330: 0600 0000 1300 0000 ffff ffff 0900 0000  ................
+00000340: 0a00 0000 0800 0000 1500 0000 0a00 0000  ................
+00000350: 0000 0000 0800 0000 0900 0000 ffff ffff  ................
+00000360: 0100 0000 0c00 0000 1300 0000 0d00 0000  ................
+00000370: 0b00 0000 0c00 0000 1200 0000 0e00 0000  ................
+00000380: 0f00 0000 ffff ffff 0d00 0000 ffff ffff  ................
+00000390: 0e00 0000 1000 0000 0200 0000 0f00 0000  ................
+000003a0: 1100 0000 1200 0000 1b00 0000 1000 0000  ................
+000003b0: 1400 0000 1100 0000 0d00 0000 1400 0000  ................
+000003c0: 0c00 0000 0700 0000 1900 0000 1200 0000  ................
+000003d0: 1300 0000 0900 0000 1600 0000 1a00 0000  ................
+000003e0: 1500 0000 ffff ffff 1700 0000 ffff ffff  ................
+000003f0: 1800 0000 1600 0000 1700 0000 0300 0000  ................
+00000400: 1c00 0000 1b00 0000 1400 0000 1a00 0000  ................
+00000410: 0600 0000 1500 0000 1900 0000 1100 0000  ................
+00000420: 1900 0000 1c00 0000 0200 0000 1b00 0000  ................
+00000430: 1800 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000440: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000450: 5294 284b 014b 1d4b 0486 9468 1b8c 0266  R.(K.K.K...h...f
+00000460: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000470: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000480: 42a0 0300 0079 af00 802c a4e7 3f85 710a  B....y...,..?.q.
+00000490: ba93 18dd 3fee d2ff ec01 d7df bf71 a24b  ....?........q.K
+000004a0: b263 6d54 c0c2 9c32 1d4f 0de9 3f3b 04d8  .cmT...2.O..?;..
+000004b0: cec6 25d5 3faa f025 bfb0 dee0 bf5f 2669  ..%.?..%....._&i
+000004c0: 22e0 1253 c0de f909 3617 70e0 3f36 7966  "..S....6.p.?6yf
+000004d0: 20f5 32e2 3f87 4fa6 6d99 8ee4 bffa 3a60   .2.?.O.m.....:`
+000004e0: 8434 ee4d c068 9364 6146 46d5 3f80 fcc6  .4.M.h.daFF.?...
+000004f0: 08bc 9fe6 3f9b febe eda0 f9e3 bf2f 788f  ....?......../x.
+00000500: 33da 3a4d c02e d28d 1c40 1de9 3fcb 70c0  3.:M.....@..?.p.
+00000510: bc0e 55d5 3f2d ed30 84ee b7e0 bf75 7a21  ..U.?-.0.....uz!
+00000520: 544b 4853 c0ae 70e0 f649 10e8 3fd7 6ce7  TKHS..p..I..?.l.
+00000530: 21d9 f6db 3f12 41e6 f363 96df bf83 27c3  !...?.A..c....'.
+00000540: 2018 9f54 c089 e33d 252c e8e6 3f84 4f54   ..T...=%,..?.OT
+00000550: 1157 9fdd 3f68 6780 e6f0 bae0 bf73 5285  .W..?hg......sR.
+00000560: 543a 5253 c021 2e77 446a a7e8 3f04 13e8  T:RS.!.wDj..?...
+00000570: c8db f1d5 3f6f c7fe cbd1 32e1 bf30 e296  ....?o....2..0..
+00000580: 3fae ae52 c084 732f a49e aee6 3fc9 4cb2  ?..R..s/....?.L.
+00000590: 3040 8ee1 3fb7 dc50 60a3 60dc bf90 e2fd  0@..?..P`.`.....
+000005a0: b085 2257 c0fb 6e1a ab32 bae4 3f8f 46a6  .."W..n..2..?.F.
+000005b0: c59b 46e2 3f7d 6a5b 49d4 22e0 bfb6 d591  ..F.?}j[I.".....
+000005c0: 1275 1b54 c0ed 0077 dc3a 44e7 3f1f c760  .u.T...w.:D.?..`
+000005d0: d667 cdde 3faf d20c 8eca 55df bfc6 2c83  .g..?.....U...,.
+000005e0: ace3 d954 c0b4 8f00 85cb 99e9 3f0b 9233  ...T........?..3
+000005f0: db6b e6d0 3f0d 3f9d ff4a 3de1 bfc4 68c0  .k..?.?..J=...h.
+00000600: a2da a952 c055 52b5 391c 58e8 3f28 9f8b  ...R.UR.9.X.?(..
+00000610: 51f3 efcd 3f36 be13 0eb4 5fe3 bfd4 c345  Q...?6...._....E
+00000620: 6e09 1e50 c0c0 e7c2 d436 d7e6 3fc6 dfd1  n..P.....6..?...
+00000630: 1007 a0b7 bf4b cee4 6f7a 37e6 bf4d 5eed  .....K..oz7..M^.
+00000640: 4141 ec44 c06e 742f 24cd b2de 3f22 a2b0  AA.D.nt/$...?"..
+00000650: 4a01 7ee4 bf8d 36d8 7a12 32e3 bf00 b0cd  J.~...6.z.2.....
+00000660: 37fe 22a3 3f13 1176 4512 e3e1 3faa 631a  7.".?..vE...?.c.
+00000670: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+00000680: 31b5 cd4a c013 1176 4512 e3e1 3faa 631a  1..J...vE...?.c.
+00000690: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+000006a0: 31b5 cd4a c0b6 9ffd 9f60 f5e4 3f48 3817  1..J.....`..?H8.
+000006b0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006c0: bbb3 3f4e c0b6 9ffd 9f60 f5e4 3f48 3817  ..?N.....`..?H8.
+000006d0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006e0: bbb3 3f4e c0b5 41aa 8704 45e7 3f26 517b  ..?N..A...E.?&Q{
+000006f0: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000700: 0c5e 0b51 c0b5 41aa 8704 45e7 3f26 517b  .^.Q..A...E.?&Q{
+00000710: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000720: 0c5e 0b51 c0d5 906a 752a 76e4 3f3e 6845  .^.Q...ju*v.?>hE
+00000730: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000740: 1243 dd53 c0d5 906a 752a 76e4 3f3e 6845  .C.S...ju*v.?>hE
+00000750: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000760: 1243 dd53 c0ca 8133 6685 00e2 3f15 176b  .C.S...3f...?..k
+00000770: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+00000780: b920 3c52 c0ca 8133 6685 00e2 3f15 176b  . <R...3f...?..k
+00000790: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+000007a0: b920 3c52 c048 25d3 cc6b ede5 3f5d fafa  . <R.H%..k..?]..
+000007b0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007c0: 6f68 4f52 c048 25d3 cc6b ede5 3f5d fafa  ohOR.H%..k..?]..
+000007d0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007e0: 6f68 4f52 c06c d244 aef5 84e3 3f6d 43bb  ohOR.l.D....?mC.
+000007f0: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000800: c55d 8850 c06c d244 aef5 84e3 3f6d 43bb  .].P.l.D....?mC.
+00000810: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000820: c55d 8850 c094 7494 628c 0863 6f70 6c61  .].P..t.b..copla
+00000830: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000840: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000850: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000860: 0085 9468 1687 9452 9428 4b01 4b1d 8594  ...h...R.(K.K...
+00000870: 681e 8943 7401 0000 0001 0000 0001 0000  h..Ct...........
+00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008a0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008b0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008c0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008d0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008e0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+000008f0: 7369 6d70 6c65 7894 4b1d 8c0a 5f74 7261  simplex.K..._tra
+00000900: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000910: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000920: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000930: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000940: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000950: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000960: 9428 4b01 4b14 4b02 8694 6831 8942 4001  .(K.K.K...h1.B@.
+00000970: 0000 0000 0000 0000 4e40 0000 0000 0080  ........N@......
+00000980: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000990: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+000009a0: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+000009b0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+000009c0: 4640 0000 0000 0000 4e40 cdcc cccc ccac  F@......N@......
+000009d0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+000009e0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+000009f0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000a00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000a10: 5040 0000 0000 0000 5440 3333 3333 3313  P@......T@33333.
+00000a20: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000a30: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000a40: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000a50: 5640 0000 0000 0000 5440 0000 0000 0080  V@......T@......
+00000a60: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000a70: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000a80: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000a90: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000aa0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ab0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000ac0: 076e 706f 696e 7473 944b 148c 096d 696e  .npoints.K...min
+00000ad0: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000ae0: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000af0: 1000 0000 0000 004e 4000 0000 0000 0041  .......N@......A
+00000b00: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000b10: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000b20: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000b30: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000b40: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000b50: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000b60: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000b70: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000b80: 144b 0186 9468 3189 43a0 e17a 14ae 47e1  .K...h1.C..z..G.
+00000b90: 1c40 0000 0000 0000 2140 713d 0ad7 a3f0  .@......!@q=....
+00000ba0: 2340 52b8 1e85 ebd1 2740 0000 0000 0000  #@R.....'@......
+00000bb0: 2d40 e17a 14ae 47e1 1e40 14ae 47e1 7a94  -@.z..G..@..G.z.
+00000bc0: 2140 c3f5 285c 8fc2 2440 14ae 47e1 7a94  !@..(\..$@..G.z.
+00000bd0: 2840 0000 0000 0080 2d40 9a99 9999 9999  (@......-@......
+00000be0: 2240 85eb 51b8 1e45 3340 48e1 7a14 ae47  "@..Q..E3@H.z..G
+00000bf0: 2940 d7a3 703d 0ad7 2d40 14ae 47e1 7a94  )@..p=..-@..G.z.
+00000c00: 2340 52b8 1e85 eb51 2640 295c 8fc2 f528  #@R....Q&@)\...(
+00000c10: 2a40 3333 3333 3333 2540 9a99 9999 9999  *@333333%@......
+00000c20: 2640 0000 0000 0000 2640 9474 9462 8c0a  &@......&@.t.b..
+00000c30: 6973 5f63 6f6d 706c 6578 9489 8c0a 6669  is_complex....fi
+00000c40: 6c6c 5f76 616c 7565 9447 7ff8 0000 0000  ll_value.G......
+00000c50: 0000 8c05 7363 616c 6594 4e8c 0670 6f69  ....scale.N..poi
+00000c60: 6e74 7394 684b 7562 2e                   nts.hKub.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,93 @@
-00000000: 8004 9511 0400 0000 0000 005d 9428 5d94  ...........].(].
+00000000: 8004 95bb 0500 0000 0000 005d 9428 5d94  ...........].(].
 00000010: 288c 156e 756d 7079 2e63 6f72 652e 6d75  (..numpy.core.mu
 00000020: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
 00000030: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
 00000040: 7970 6594 9394 8c02 6638 9489 8887 9452  ype.....f8.....R
 00000050: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
 00000060: 4aff ffff ff4b 0074 9462 4308 0000 0000  J....K.t.bC.....
-00000070: 0080 4640 9486 9452 9468 0468 0a43 08cd  ..F@...R.h.h.C..
-00000080: cccc cccc ac50 4094 8694 5294 6804 680a  .....P@...R.h.h.
-00000090: 4308 3333 3333 3313 5640 9486 9452 9468  C.33333.V@...R.h
-000000a0: 0468 0a43 0800 0000 0000 805b 4094 8694  .h.C.......[@...
-000000b0: 5294 655d 9428 5d94 285d 9428 6804 680a  R.e].(].(].(h.h.
-000000c0: 4308 0000 0000 0000 4e40 9486 9452 945d  C.......N@...R.]
-000000d0: 9468 0468 0a43 08cd cccc cccc 8c50 4094  .h.h.C.......P@.
-000000e0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-000000f0: 0000 0000 0054 4094 8694 5294 5d94 6804  .....T@...R.].h.
-00000100: 680a 4308 0ad7 a370 3d9a 5540 9486 9452  h.C....p=.U@...R
-00000110: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
-00000120: 0000 5940 9486 9452 945d 9468 0468 0a43  ..Y@...R.].h.h.C
-00000130: 0800 0000 0000 805a 4094 8694 5294 6165  .......Z@...R.ae
-00000140: 5d94 2868 0468 0a43 0800 0000 0000 005e  ].(h.h.C.......^
-00000150: 4094 8694 5294 5d94 6804 680a 4308 48e1  @...R.].h.h.C.H.
-00000160: 7a14 ae87 5f40 9486 9452 9461 655d 9428  z..._@...R.ae].(
-00000170: 6804 680a 4308 0000 0000 0080 6140 9486  h.h.C.......a@..
-00000180: 9452 945d 9468 0468 0a43 08ae 47e1 7a14  .R.].h.h.C..G.z.
-00000190: 3e62 4094 8694 5294 6165 655d 9428 5d94  >b@...R.aee].(].
-000001a0: 2868 0468 0a43 0800 0000 0000 004e 4094  (h.h.C.......N@.
-000001b0: 8694 5294 5d94 6804 680a 4308 ec51 b81e  ..R.].h.h.C..Q..
-000001c0: 850b 5140 9486 9452 9461 655d 9428 6804  ..Q@...R.ae].(h.
-000001d0: 680a 4308 0000 0000 0000 5440 9486 9452  h.C.......T@...R
-000001e0: 945d 9468 0468 0a43 08a4 703d 0ad7 c355  .].h.h.C..p=...U
-000001f0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000200: 0800 0000 0000 0059 4094 8694 5294 5d94  .......Y@...R.].
-00000210: 6804 680a 4308 5c8f c2f5 28dc 5a40 9486  h.h.C.\...(.Z@..
-00000220: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-00000230: 0000 0000 5e40 9486 9452 945d 9468 0468  ....^@...R.].h.h
-00000240: 0a43 08ae 47e1 7a14 ce5f 4094 8694 5294  .C..G.z.._@...R.
-00000250: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
-00000260: 8061 4094 8694 5294 5d94 6804 680a 4308  .a@...R.].h.h.C.
-00000270: c3f5 285c 8f6a 6240 9486 9452 9461 6565  ..(\.jb@...R.aee
-00000280: 5d94 285d 9428 6804 680a 4308 0000 0000  ].(].(h.h.C.....
-00000290: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
-000002a0: 0848 e17a 14ae 9756 4094 8694 5294 6165  .H.z...V@...R.ae
-000002b0: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
-000002c0: 4094 8694 5294 5d94 6804 680a 4308 5c8f  @...R.].h.h.C.\.
-000002d0: c2f5 285c 5b40 9486 9452 9461 655d 9428  ..(\[@...R.ae].(
-000002e0: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
-000002f0: 9452 945d 9468 0468 0a43 08f6 285c 8fc2  .R.].h.h.C..(\..
-00000300: 1560 4094 8694 5294 6165 5d94 2868 0468  .`@...R.ae].(h.h
-00000310: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
-00000320: 5d94 6804 680a 4308 cdcc cccc cc74 6240  ].h.h.C......tb@
-00000330: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
-00000340: 680a 4308 0000 0000 0000 5440 9486 9452  h.C.......T@...R
-00000350: 945d 9468 0468 0a43 0848 e17a 14ae 1757  .].h.h.C.H.z...W
-00000360: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000370: 0800 0000 0000 0059 4094 8694 5294 5d94  .......Y@...R.].
-00000380: 6804 680a 4308 1f85 eb51 b89e 5b40 9486  h.h.C....Q..[@..
-00000390: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-000003a0: 0000 0000 5e40 9486 9452 945d 9468 0468  ....^@...R.].h.h
-000003b0: 0a43 0848 e17a 14ae 2760 4094 8694 5294  .C.H.z..'`@...R.
-000003c0: 6165 6565 5d94 2868 0468 0a43 0800 0000  aeee].(h.h.C....
-000003d0: 0000 004e 4094 8694 5294 6804 680a 4308  ...N@...R.h.h.C.
-000003e0: 0000 0000 0080 6140 9486 9452 9465 5d94  ......a@...R.e].
-000003f0: 2847 404b 8666 6666 6666 4740 2a28 f5c2  (G@K.fffffG@*(..
-00000400: 8f5c 2965 5d94 2847 403c e3d7 0a3d 70a4  .\)e].(G@<...=p.
-00000410: 4740 2d00 0000 0000 0065 652e            G@-......ee.
+00000070: 0000 4140 9486 9452 9468 0468 0a43 0800  ..A@...R.h.h.C..
+00000080: 0000 0000 8046 4094 8694 5294 6804 680a  .....F@...R.h.h.
+00000090: 4308 cdcc cccc ccac 5040 9486 9452 9468  C.......P@...R.h
+000000a0: 0468 0a43 0800 0000 0000 0051 4094 8694  .h.C.......Q@...
+000000b0: 5294 6804 680a 4308 3333 3333 3313 5640  R.h.h.C.33333.V@
+000000c0: 9486 9452 9468 0468 0a43 0800 0000 0000  ...R.h.h.C......
+000000d0: c057 4094 8694 5294 6804 680a 4308 0000  .W@...R.h.h.C...
+000000e0: 0000 0080 5b40 9486 9452 9465 5d94 285d  ....[@...R.e].(]
+000000f0: 945d 9428 6804 680a 4308 0000 0000 0040  .].(h.h.C......@
+00000100: 5f40 9486 9452 945d 9468 0468 0a43 0800  _@...R.].h.h.C..
+00000110: 0000 0000 8061 4094 8694 5294 6165 615d  .....a@...R.aea]
+00000120: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
+00000130: 0044 4094 8694 5294 5d94 6804 680a 4308  .D@...R.].h.h.C.
+00000140: ec51 b81e 85cb 4640 9486 9452 9461 655d  .Q....F@...R.ae]
+00000150: 9428 6804 680a 4308 0000 0000 0000 4e40  .(h.h.C.......N@
+00000160: 9486 9452 945d 9468 0468 0a43 0852 b81e  ...R.].h.h.C.R..
+00000170: 85eb 3150 4094 8694 5294 6165 5d94 2868  ..1P@...R.ae].(h
+00000180: 0468 0a43 0800 0000 0000 0054 4094 8694  .h.C.......T@...
+00000190: 5294 5d94 6804 680a 4308 0ad7 a370 3d7a  R.].h.h.C....p=z
+000001a0: 5540 9486 9452 9461 655d 9428 6804 680a  U@...R.ae].(h.h.
+000001b0: 4308 0000 0000 0000 5940 9486 9452 945d  C.......Y@...R.]
+000001c0: 9468 0468 0a43 08c3 f528 5c8f 225a 4094  .h.h.C...(\."Z@.
+000001d0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+000001e0: 0000 0000 005e 4094 8694 5294 5d94 6804  .....^@...R.].h.
+000001f0: 680a 4308 f628 5c8f c225 5f40 9486 9452  h.C..(\..%_@...R
+00000200: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+00000210: 0080 6140 9486 9452 945d 9468 0468 0a43  ..a@...R.].h.h.C
+00000220: 08cd cccc cccc 2c62 4094 8694 5294 6165  ......,b@...R.ae
+00000230: 655d 9428 5d94 2868 0468 0a43 0800 0000  e].(].(h.h.C....
+00000240: 0000 0044 4094 8694 5294 5d94 6804 680a  ...D@...R.].h.h.
+00000250: 4308 7b14 ae47 e1ba 4740 9486 9452 9461  C.{..G..G@...R.a
+00000260: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000270: 4e40 9486 9452 945d 9468 0468 0a43 0829  N@...R.].h.h.C.)
+00000280: 5c8f c2f5 d850 4094 8694 5294 6165 5d94  \....P@...R.ae].
+00000290: 2868 0468 0a43 0800 0000 0000 0054 4094  (h.h.C.......T@.
+000002a0: 8694 5294 5d94 6804 680a 4308 e17a 14ae  ..R.].h.h.C..z..
+000002b0: 47a1 5540 9486 9452 9461 655d 9428 6804  G.U@...R.ae].(h.
+000002c0: 680a 4308 0000 0000 0000 5940 9486 9452  h.C.......Y@...R
+000002d0: 945d 9468 0468 0a43 089a 9999 9999 c95a  .].h.h.C.......Z
+000002e0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
+000002f0: 0800 0000 0000 005e 4094 8694 5294 5d94  .......^@...R.].
+00000300: 6804 680a 4308 85eb 51b8 1ec5 5f40 9486  h.h.C...Q..._@..
+00000310: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
+00000320: 0000 0080 6140 9486 9452 945d 9468 0468  ....a@...R.].h.h
+00000330: 0a43 0848 e17a 14ae 6762 4094 8694 5294  .C.H.z..gb@...R.
+00000340: 6165 655d 945d 9428 6804 680a 4308 0000  aee].].(h.h.C...
+00000350: 0000 0040 5f40 9486 9452 945d 9468 0468  ...@_@...R.].h.h
+00000360: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
+00000370: 6165 615d 9428 5d94 2868 0468 0a43 0800  aea].(].(h.h.C..
+00000380: 0000 0000 004e 4094 8694 5294 5d94 6804  .....N@...R.].h.
+00000390: 680a 4308 8fc2 f528 5c4f 5140 9486 9452  h.C....(\OQ@...R
+000003a0: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+000003b0: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
+000003c0: 0885 eb51 b81e 3556 4094 8694 5294 6165  ...Q..5V@...R.ae
+000003d0: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
+000003e0: 4094 8694 5294 5d94 6804 680a 4308 ae47  @...R.].h.h.C..G
+000003f0: e17a 142e 5b40 9486 9452 9461 655d 9428  .z..[@...R.ae].(
+00000400: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
+00000410: 9452 945d 9468 0468 0a43 0866 6666 6666  .R.].h.h.C.fffff
+00000420: e65f 4094 8694 5294 6165 5d94 2868 0468  ._@...R.ae].(h.h
+00000430: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
+00000440: 5d94 6804 680a 4308 c3f5 285c 8f8a 6240  ].h.h.C...(\..b@
+00000450: 9486 9452 9461 6565 5d94 5d94 2868 0468  ...R.aee].].(h.h
+00000460: 0a43 0800 0000 0000 405f 4094 8694 5294  .C......@_@...R.
+00000470: 5d94 6804 680a 4308 0000 0000 0080 6140  ].h.h.C.......a@
+00000480: 9486 9452 9461 6561 5d94 285d 9428 6804  ...R.aea].(].(h.
+00000490: 680a 4308 0000 0000 0000 4e40 9486 9452  h.C.......N@...R
+000004a0: 945d 9468 0468 0a43 08ae 47e1 7a14 ce51  .].h.h.C..G.z..Q
+000004b0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
+000004c0: 0800 0000 0000 0054 4094 8694 5294 5d94  .......T@...R.].
+000004d0: 6804 680a 4308 1f85 eb51 b8ae 5640 9486  h.h.C....Q..V@..
+000004e0: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
+000004f0: 0000 0000 5940 9486 9452 945d 9468 0468  ....Y@...R.].h.h
+00000500: 0a43 0866 6666 6666 665b 4094 8694 5294  .C.ffffff[@...R.
+00000510: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
+00000520: 005e 4094 8694 5294 5d94 6804 680a 4308  .^@...R.].h.h.C.
+00000530: a470 3d0a d743 6040 9486 9452 9461 655d  .p=..C`@...R.ae]
+00000540: 9428 6804 680a 4308 0000 0000 0080 6140  .(h.h.C.......a@
+00000550: 9486 9452 945d 9468 0468 0a43 0833 3333  ...R.].h.h.C.333
+00000560: 3333 bb62 4094 8694 5294 6165 6565 5d94  33.b@...R.aeee].
+00000570: 2868 0468 0a43 0800 0000 0000 0044 4094  (h.h.C.......D@.
+00000580: 8694 5294 6804 680a 4308 0000 0000 0080  ..R.h.h.C.......
+00000590: 6140 9486 9452 9465 5d94 2847 4036 ae14  a@...R.e].(G@6..
+000005a0: 7ae1 47ae 4740 1a5c 28f5 c28f 5c65 5d94  z.G.G@.\(...\e].
+000005b0: 2847 4026 3333 3333 3333 4740 1333 3333  (G@&333333G@.333
+000005c0: 3333 3365 652e                           333ee.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9530 0a00 0000 0000 008c 1a73 6369  ...0.........sci
+00000000: 8004 955e 0c00 0000 0000 008c 1a73 6369  ...^.........sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,154 +11,189 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 4010 5798 851e 998c 0973 696d 706c  G.@.W......simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 154b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 1d4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 43fc 0c00 0000 0d00  ..K.t.b.C.......
-00000150: 0000 1000 0000 0600 0000 0a00 0000 0500  ................
-00000160: 0000 0500 0000 0a00 0000 0e00 0000 0100  ................
-00000170: 0000 0500 0000 0000 0000 0100 0000 0600  ................
-00000180: 0000 0500 0000 0600 0000 0100 0000 0700  ................
-00000190: 0000 0100 0000 0200 0000 0700 0000 0300  ................
-000001a0: 0000 0800 0000 0200 0000 0200 0000 0800  ................
-000001b0: 0000 0700 0000 0b00 0000 0c00 0000 1000  ................
-000001c0: 0000 0f00 0000 0b00 0000 1000 0000 0b00  ................
-000001d0: 0000 0f00 0000 0e00 0000 0a00 0000 0b00  ................
-000001e0: 0000 0e00 0000 0800 0000 0b00 0000 0700  ................
-000001f0: 0000 0b00 0000 0800 0000 0c00 0000 0b00  ................
-00000200: 0000 0600 0000 0700 0000 0b00 0000 0a00  ................
-00000210: 0000 0600 0000 0900 0000 0300 0000 0400  ................
-00000220: 0000 0900 0000 0800 0000 0300 0000 0800  ................
-00000230: 0000 0900 0000 0c00 0000 0c00 0000 0900  ................
-00000240: 0000 0d00 0000 9474 9462 8c09 6e65 6967  .......t.b..neig
-00000250: 6862 6f72 7394 6811 6814 4b00 8594 6816  hbors.h.h.K...h.
-00000260: 8794 5294 284b 014b 154b 0386 9468 1e89  ..R.(K.K.K...h..
-00000270: 43fc ffff ffff 0900 0000 1400 0000 0200  C...............
-00000280: 0000 0400 0000 1000 0000 0c00 0000 ffff  ................
-00000290: ffff 0100 0000 ffff ffff ffff ffff 0400  ................
-000002a0: 0000 0100 0000 0300 0000 0500 0000 0600  ................
-000002b0: 0000 0f00 0000 0400 0000 0800 0000 0500  ................
-000002c0: 0000 ffff ffff 0800 0000 ffff ffff 1200  ................
-000002d0: 0000 0d00 0000 0600 0000 0700 0000 0000  ................
-000002e0: 0000 0a00 0000 0e00 0000 0900 0000 ffff  ................
-000002f0: ffff 0b00 0000 ffff ffff 0c00 0000 0a00  ................
-00000300: 0000 0b00 0000 0200 0000 1000 0000 0f00  ................
-00000310: 0000 0800 0000 0e00 0000 1300 0000 0900  ................
-00000320: 0000 0d00 0000 0500 0000 0d00 0000 1000  ................
-00000330: 0000 0100 0000 0f00 0000 0c00 0000 ffff  ................
-00000340: ffff ffff ffff 1200 0000 0700 0000 1100  ................
-00000350: 0000 1300 0000 1400 0000 0e00 0000 1200  ................
-00000360: 0000 ffff ffff 0000 0000 1300 0000 9474  ...............t
-00000370: 9462 8c09 6571 7561 7469 6f6e 7394 6811  .b..equations.h.
-00000380: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000390: 154b 0486 9468 1b8c 0266 3894 8988 8794  .K...h...f8.....
-000003a0: 5294 284b 0368 1f4e 4e4e 4aff ffff ff4a  R.(K.h.NNNJ....J
-000003b0: ffff ffff 4b00 7494 6289 42a0 0200 0067  ....K.t.b.B....g
-000003c0: f1b8 d95c 6ee6 3fc9 8c40 e6a7 1be1 3f7a  ...\n.?..@....?z
-000003d0: 4ef2 c8c1 35de bf95 e31c 6750 a955 c0de  N...5.....gP.U..
-000003e0: f909 3617 70e0 3f36 7966 20f5 32e2 3f87  ..6.p.?6yf .2.?.
-000003f0: 4fa6 6d99 8ee4 bffa 3a60 8434 ee4d c068  O.m.....:`.4.M.h
-00000400: 9364 6146 46d5 3f80 fcc6 08bc 9fe6 3f9b  .daFF.?.......?.
-00000410: febe eda0 f9e3 bf2f 788f 33da 3a4d c013  ......./x.3.:M..
-00000420: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000430: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c013  ..[.^.....1..J..
-00000440: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000450: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c0b6  ..[.^.....1..J..
-00000460: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000470: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b6  ....b...S...?N..
-00000480: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000490: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b5  ....b...S...?N..
-000004a0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004b0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0b5  t*......s..^.Q..
-000004c0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004d0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0d5  t*......s..^.Q..
-000004e0: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-000004f0: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0d5  .U,.H......C.S..
-00000500: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-00000510: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0ca  .U,.H......C.S..
-00000520: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000530: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c0ca  ........7.. <R..
-00000540: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000550: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c048  ........7.. <R.H
-00000560: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000570: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c048  ...Ts..!.:ohOR.H
-00000580: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000590: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c06c  ...Ts..!.:ohOR.l
-000005a0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005b0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c06c  ...s.......].P.l
-000005c0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005d0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c006  ...s.......].P..
-000005e0: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-000005f0: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c006  .G.6......mC.S..
-00000600: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-00000610: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c06b  .G.6......mC.S.k
-00000620: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000630: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c06b  :.Z....v...4>T.k
-00000640: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000650: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c094  :.Z....v...4>T..
-00000660: 7494 628c 0863 6f70 6c61 6e61 7294 6811  t.b..coplanar.h.
-00000670: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000680: 004b 0386 9468 1e89 4300 9474 9462 8c04  .K...h..C..t.b..
-00000690: 676f 6f64 9468 1168 144b 0085 9468 1687  good.h.h.K...h..
-000006a0: 9452 9428 4b01 4b15 8594 681e 8943 5401  .R.(K.K...h..CT.
-000006b0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006c0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006d0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006e0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006f0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-00000700: 0000 0094 7494 628c 086e 7369 6d70 6c65  ....t.b..nsimple
-00000710: 7894 4b15 8c0a 5f74 7261 6e73 666f 726d  x.K..._transform
-00000720: 944e 8c12 5f76 6572 7465 785f 746f 5f73  .N.._vertex_to_s
-00000730: 696d 706c 6578 944e 8c19 5f76 6572 7465  implex.N.._verte
-00000740: 785f 6e65 6967 6862 6f72 5f76 6572 7469  x_neighbor_verti
-00000750: 6365 7394 4e8c 095f 7665 7274 6963 6573  ces.N.._vertices
-00000760: 9468 188c 075f 706f 696e 7473 9468 1168  .h..._points.h.h
-00000770: 144b 0085 9468 1687 9452 9428 4b01 4b11  .K...h...R.(K.K.
-00000780: 4b02 8694 6831 8942 1001 0000 0000 0000  K...h1.B........
-00000790: 0000 4e40 0000 0000 0080 4640 0000 0000  ..N@......F@....
-000007a0: 0000 5440 0000 0000 0080 4640 0000 0000  ..T@......F@....
-000007b0: 0000 5940 0000 0000 0080 4640 0000 0000  ..Y@......F@....
-000007c0: 0000 5e40 0000 0000 0080 4640 0000 0000  ..^@......F@....
-000007d0: 0080 6140 0000 0000 0080 4640 0000 0000  ..a@......F@....
-000007e0: 0000 4e40 cdcc cccc ccac 5040 0000 0000  ..N@......P@....
-000007f0: 0000 5440 cdcc cccc ccac 5040 0000 0000  ..T@......P@....
-00000800: 0000 5940 cdcc cccc ccac 5040 0000 0000  ..Y@......P@....
-00000810: 0000 5e40 cdcc cccc ccac 5040 0000 0000  ..^@......P@....
-00000820: 0080 6140 cdcc cccc ccac 5040 0000 0000  ..a@......P@....
-00000830: 0000 5440 3333 3333 3313 5640 0000 0000  ..T@33333.V@....
-00000840: 0000 5940 3333 3333 3313 5640 0000 0000  ..Y@33333.V@....
-00000850: 0000 5e40 3333 3333 3313 5640 0000 0000  ..^@33333.V@....
-00000860: 0080 6140 3333 3333 3313 5640 0000 0000  ..a@33333.V@....
-00000870: 0000 5440 0000 0000 0080 5b40 0000 0000  ..T@......[@....
-00000880: 0000 5940 0000 0000 0080 5b40 0000 0000  ..Y@......[@....
-00000890: 0000 5e40 0000 0000 0080 5b40 9474 9462  ..^@......[@.t.b
-000008a0: 8c04 6e64 696d 944b 028c 076e 706f 696e  ..ndim.K...npoin
-000008b0: 7473 944b 118c 096d 696e 5f62 6f75 6e64  ts.K...min_bound
-000008c0: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
-000008d0: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
-000008e0: 004e 4000 0000 0000 8046 4094 7494 628c  .N@......F@.t.b.
-000008f0: 096d 6178 5f62 6f75 6e64 9468 1168 144b  .max_bound.h.h.K
-00000900: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000910: 6831 8943 1000 0000 0000 8061 4000 0000  h1.C.......a@...
-00000920: 0000 805b 4094 7494 628c 0d66 7572 7468  ...[@.t.b..furth
-00000930: 6573 745f 7369 7465 9489 7562 8c0c 7661  est_site..ub..va
-00000940: 6c75 6573 5f73 6861 7065 944b 0185 948c  lues_shape.K....
-00000950: 0676 616c 7565 7394 6811 6814 4b00 8594  .values.h.h.K...
-00000960: 6816 8794 5294 284b 014b 114b 0186 9468  h...R.(K.K.K...h
-00000970: 3189 4388 1f85 eb51 b89e 3f40 85eb 51b8  1.C....Q..?@..Q.
-00000980: 1ec5 3e40 9a99 9999 9919 3e40 0000 0000  ..>@......>@....
-00000990: 0000 3d40 a470 3d0a d7e3 3c40 a470 3d0a  ..=@.p=...<@.p=.
-000009a0: d743 4440 0ad7 a370 3d6a 4340 a470 3d0a  .CD@...p=jC@.p=.
-000009b0: d783 4240 8fc2 f528 5c0f 4240 14ae 47e1  ..B@...(\.B@..G.
-000009c0: 7a74 4140 e17a 14ae 4741 4840 ae47 e17a  ztA@.z..GAH@.G.z
-000009d0: 140e 4740 6666 6666 66e6 4540 ec51 b81e  ..G@fffff.E@.Q..
-000009e0: 85eb 4440 8fc2 f528 5c0f 4d40 7b14 ae47  ..D@...(\.M@{..G
-000009f0: e19a 4c40 6666 6666 6686 4b40 9474 9462  ..L@fffff.K@.t.b
-00000a00: 8c0a 6973 5f63 6f6d 706c 6578 9489 8c0a  ..is_complex....
-00000a10: 6669 6c6c 5f76 616c 7565 9447 7ff8 0000  fill_value.G....
-00000a20: 0000 0000 8c05 7363 616c 6594 4e8c 0670  ......scale.N..p
-00000a30: 6f69 6e74 7394 684b 7562 2e              oints.hKub.
+00000140: ffff 4b00 7494 6289 425c 0100 000d 0000  ..K.t.b.B\......
+00000150: 000c 0000 0012 0000 0012 0000 0003 0000  ................
+00000160: 0004 0000 0006 0000 000a 0000 0005 0000  ................
+00000170: 0005 0000 000a 0000 000e 0000 0009 0000  ................
+00000180: 0012 0000 0004 0000 0009 0000 000d 0000  ................
+00000190: 0012 0000 000c 0000 0008 0000 0012 0000  ................
+000001a0: 0008 0000 0003 0000 0012 0000 0013 0000  ................
+000001b0: 000d 0000 0010 0000 000c 0000 0013 0000  ................
+000001c0: 0010 0000 0013 0000 000c 0000 000d 0000  ................
+000001d0: 0003 0000 0011 0000 0004 0000 0011 0000  ................
+000001e0: 0003 0000 0002 0000 0001 0000 0011 0000  ................
+000001f0: 0002 0000 0011 0000 0001 0000 0000 0000  ................
+00000200: 0001 0000 0005 0000 0000 0000 0001 0000  ................
+00000210: 0006 0000 0005 0000 0006 0000 0001 0000  ................
+00000220: 0007 0000 0001 0000 0002 0000 0007 0000  ................
+00000230: 0003 0000 0008 0000 0002 0000 0002 0000  ................
+00000240: 0008 0000 0007 0000 000b 0000 000c 0000  ................
+00000250: 0010 0000 000f 0000 000b 0000 0010 0000  ................
+00000260: 000b 0000 000f 0000 000e 0000 000a 0000  ................
+00000270: 000b 0000 000e 0000 0008 0000 000b 0000  ................
+00000280: 0007 0000 000b 0000 0008 0000 000c 0000  ................
+00000290: 000b 0000 0006 0000 0007 0000 000b 0000  ................
+000002a0: 000a 0000 0006 0000 0094 7494 628c 096e  ..........t.b..n
+000002b0: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+000002c0: 9468 1687 9452 9428 4b01 4b1d 4b03 8694  .h...R.(K.K.K...
+000002d0: 681e 8942 5c01 0000 0600 0000 0500 0000  h..B\...........
+000002e0: 0a00 0000 0b00 0000 0400 0000 0700 0000  ................
+000002f0: 0300 0000 1000 0000 1c00 0000 1800 0000  ................
+00000300: ffff ffff 0200 0000 0100 0000 ffff ffff  ................
+00000310: 0500 0000 0000 0000 0400 0000 ffff ffff  ................
+00000320: 0700 0000 0000 0000 1a00 0000 0100 0000  ................
+00000330: 0600 0000 1300 0000 ffff ffff 0900 0000  ................
+00000340: 0a00 0000 0800 0000 1500 0000 0a00 0000  ................
+00000350: 0000 0000 0800 0000 0900 0000 ffff ffff  ................
+00000360: 0100 0000 0c00 0000 1300 0000 0d00 0000  ................
+00000370: 0b00 0000 0c00 0000 1200 0000 0e00 0000  ................
+00000380: 0f00 0000 ffff ffff 0d00 0000 ffff ffff  ................
+00000390: 0e00 0000 1000 0000 0200 0000 0f00 0000  ................
+000003a0: 1100 0000 1200 0000 1b00 0000 1000 0000  ................
+000003b0: 1400 0000 1100 0000 0d00 0000 1400 0000  ................
+000003c0: 0c00 0000 0700 0000 1900 0000 1200 0000  ................
+000003d0: 1300 0000 0900 0000 1600 0000 1a00 0000  ................
+000003e0: 1500 0000 ffff ffff 1700 0000 ffff ffff  ................
+000003f0: 1800 0000 1600 0000 1700 0000 0300 0000  ................
+00000400: 1c00 0000 1b00 0000 1400 0000 1a00 0000  ................
+00000410: 0600 0000 1500 0000 1900 0000 1100 0000  ................
+00000420: 1900 0000 1c00 0000 0200 0000 1b00 0000  ................
+00000430: 1800 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000440: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000450: 5294 284b 014b 1d4b 0486 9468 1b8c 0266  R.(K.K.K...h...f
+00000460: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000470: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000480: 42a0 0300 0079 af00 802c a4e7 3f85 710a  B....y...,..?.q.
+00000490: ba93 18dd 3fee d2ff ec01 d7df bf71 a24b  ....?........q.K
+000004a0: b263 6d54 c0c2 9c32 1d4f 0de9 3f3b 04d8  .cmT...2.O..?;..
+000004b0: cec6 25d5 3faa f025 bfb0 dee0 bf5f 2669  ..%.?..%....._&i
+000004c0: 22e0 1253 c0de f909 3617 70e0 3f36 7966  "..S....6.p.?6yf
+000004d0: 20f5 32e2 3f87 4fa6 6d99 8ee4 bffa 3a60   .2.?.O.m.....:`
+000004e0: 8434 ee4d c068 9364 6146 46d5 3f80 fcc6  .4.M.h.daFF.?...
+000004f0: 08bc 9fe6 3f9b febe eda0 f9e3 bf2f 788f  ....?......../x.
+00000500: 33da 3a4d c02e d28d 1c40 1de9 3fcb 70c0  3.:M.....@..?.p.
+00000510: bc0e 55d5 3f2d ed30 84ee b7e0 bf75 7a21  ..U.?-.0.....uz!
+00000520: 544b 4853 c0ae 70e0 f649 10e8 3fd7 6ce7  TKHS..p..I..?.l.
+00000530: 21d9 f6db 3f12 41e6 f363 96df bf83 27c3  !...?.A..c....'.
+00000540: 2018 9f54 c089 e33d 252c e8e6 3f84 4f54   ..T...=%,..?.OT
+00000550: 1157 9fdd 3f68 6780 e6f0 bae0 bf73 5285  .W..?hg......sR.
+00000560: 543a 5253 c021 2e77 446a a7e8 3f04 13e8  T:RS.!.wDj..?...
+00000570: c8db f1d5 3f6f c7fe cbd1 32e1 bf30 e296  ....?o....2..0..
+00000580: 3fae ae52 c084 732f a49e aee6 3fc9 4cb2  ?..R..s/....?.L.
+00000590: 3040 8ee1 3fb7 dc50 60a3 60dc bf90 e2fd  0@..?..P`.`.....
+000005a0: b085 2257 c0fb 6e1a ab32 bae4 3f8f 46a6  .."W..n..2..?.F.
+000005b0: c59b 46e2 3f7d 6a5b 49d4 22e0 bfb6 d591  ..F.?}j[I.".....
+000005c0: 1275 1b54 c0ed 0077 dc3a 44e7 3f1f c760  .u.T...w.:D.?..`
+000005d0: d667 cdde 3faf d20c 8eca 55df bfc6 2c83  .g..?.....U...,.
+000005e0: ace3 d954 c0b4 8f00 85cb 99e9 3f0b 9233  ...T........?..3
+000005f0: db6b e6d0 3f0d 3f9d ff4a 3de1 bfc4 68c0  .k..?.?..J=...h.
+00000600: a2da a952 c055 52b5 391c 58e8 3f28 9f8b  ...R.UR.9.X.?(..
+00000610: 51f3 efcd 3f36 be13 0eb4 5fe3 bfd4 c345  Q...?6...._....E
+00000620: 6e09 1e50 c0c0 e7c2 d436 d7e6 3fc6 dfd1  n..P.....6..?...
+00000630: 1007 a0b7 bf4b cee4 6f7a 37e6 bf4d 5eed  .....K..oz7..M^.
+00000640: 4141 ec44 c06e 742f 24cd b2de 3f22 a2b0  AA.D.nt/$...?"..
+00000650: 4a01 7ee4 bf8d 36d8 7a12 32e3 bf00 b0cd  J.~...6.z.2.....
+00000660: 37fe 22a3 3f13 1176 4512 e3e1 3faa 631a  7.".?..vE...?.c.
+00000670: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+00000680: 31b5 cd4a c013 1176 4512 e3e1 3faa 631a  1..J...vE...?.c.
+00000690: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+000006a0: 31b5 cd4a c0b6 9ffd 9f60 f5e4 3f48 3817  1..J.....`..?H8.
+000006b0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006c0: bbb3 3f4e c0b6 9ffd 9f60 f5e4 3f48 3817  ..?N.....`..?H8.
+000006d0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006e0: bbb3 3f4e c0b5 41aa 8704 45e7 3f26 517b  ..?N..A...E.?&Q{
+000006f0: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000700: 0c5e 0b51 c0b5 41aa 8704 45e7 3f26 517b  .^.Q..A...E.?&Q{
+00000710: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000720: 0c5e 0b51 c0d5 906a 752a 76e4 3f3e 6845  .^.Q...ju*v.?>hE
+00000730: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000740: 1243 dd53 c0d5 906a 752a 76e4 3f3e 6845  .C.S...ju*v.?>hE
+00000750: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000760: 1243 dd53 c0ca 8133 6685 00e2 3f15 176b  .C.S...3f...?..k
+00000770: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+00000780: b920 3c52 c0ca 8133 6685 00e2 3f15 176b  . <R...3f...?..k
+00000790: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+000007a0: b920 3c52 c048 25d3 cc6b ede5 3f5d fafa  . <R.H%..k..?]..
+000007b0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007c0: 6f68 4f52 c048 25d3 cc6b ede5 3f5d fafa  ohOR.H%..k..?]..
+000007d0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007e0: 6f68 4f52 c06c d244 aef5 84e3 3f6d 43bb  ohOR.l.D....?mC.
+000007f0: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000800: c55d 8850 c06c d244 aef5 84e3 3f6d 43bb  .].P.l.D....?mC.
+00000810: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000820: c55d 8850 c094 7494 628c 0863 6f70 6c61  .].P..t.b..copla
+00000830: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000840: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000850: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000860: 0085 9468 1687 9452 9428 4b01 4b1d 8594  ...h...R.(K.K...
+00000870: 681e 8943 7401 0000 0001 0000 0001 0000  h..Ct...........
+00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008a0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008b0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008c0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008d0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008e0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+000008f0: 7369 6d70 6c65 7894 4b1d 8c0a 5f74 7261  simplex.K..._tra
+00000900: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000910: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000920: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000930: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000940: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000950: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000960: 9428 4b01 4b14 4b02 8694 6831 8942 4001  .(K.K.K...h1.B@.
+00000970: 0000 0000 0000 0000 4e40 0000 0000 0080  ........N@......
+00000980: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000990: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+000009a0: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+000009b0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+000009c0: 4640 0000 0000 0000 4e40 cdcc cccc ccac  F@......N@......
+000009d0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+000009e0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+000009f0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000a00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000a10: 5040 0000 0000 0000 5440 3333 3333 3313  P@......T@33333.
+00000a20: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000a30: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000a40: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000a50: 5640 0000 0000 0000 5440 0000 0000 0080  V@......T@......
+00000a60: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000a70: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000a80: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000a90: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000aa0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ab0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000ac0: 076e 706f 696e 7473 944b 148c 096d 696e  .npoints.K...min
+00000ad0: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000ae0: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000af0: 1000 0000 0000 004e 4000 0000 0000 0041  .......N@......A
+00000b00: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000b10: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000b20: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000b30: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000b40: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000b50: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000b60: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000b70: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000b80: 144b 0186 9468 3189 43a0 1f85 eb51 b89e  .K...h1.C....Q..
+00000b90: 3f40 85eb 51b8 1ec5 3e40 9a99 9999 9919  ?@..Q...>@......
+00000ba0: 3e40 0000 0000 0000 3d40 a470 3d0a d7e3  >@......=@.p=...
+00000bb0: 3c40 a470 3d0a d743 4440 0ad7 a370 3d6a  <@.p=..CD@...p=j
+00000bc0: 4340 a470 3d0a d783 4240 8fc2 f528 5c0f  C@.p=...B@...(\.
+00000bd0: 4240 14ae 47e1 7a74 4140 e17a 14ae 4741  B@..G.ztA@.z..GA
+00000be0: 4840 ae47 e17a 140e 4740 6666 6666 66e6  H@.G.z..G@fffff.
+00000bf0: 4540 ec51 b81e 85eb 4440 8fc2 f528 5c0f  E@.Q....D@...(\.
+00000c00: 4d40 7b14 ae47 e19a 4c40 6666 6666 6686  M@{..G..L@fffff.
+00000c10: 4b40 cdcc cccc cccc 3640 9a99 9999 9999  K@......6@......
+00000c20: 4040 0000 0000 00c0 4340 9474 9462 8c0a  @@......C@.t.b..
+00000c30: 6973 5f63 6f6d 706c 6578 9489 8c0a 6669  is_complex....fi
+00000c40: 6c6c 5f76 616c 7565 9447 7ff8 0000 0000  ll_value.G......
+00000c50: 0000 8c05 7363 616c 6594 4e8c 0670 6f69  ....scale.N..poi
+00000c60: 6e74 7394 684b 7562 2e                   nts.hKub.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9530 0a00 0000 0000 008c 1a73 6369  ...0.........sci
+00000000: 8004 955e 0c00 0000 0000 008c 1a73 6369  ...^.........sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,154 +11,189 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 4010 5798 851e 998c 0973 696d 706c  G.@.W......simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 154b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 1d4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 43fc 0c00 0000 0d00  ..K.t.b.C.......
-00000150: 0000 1000 0000 0600 0000 0a00 0000 0500  ................
-00000160: 0000 0500 0000 0a00 0000 0e00 0000 0100  ................
-00000170: 0000 0500 0000 0000 0000 0100 0000 0600  ................
-00000180: 0000 0500 0000 0600 0000 0100 0000 0700  ................
-00000190: 0000 0100 0000 0200 0000 0700 0000 0300  ................
-000001a0: 0000 0800 0000 0200 0000 0200 0000 0800  ................
-000001b0: 0000 0700 0000 0b00 0000 0c00 0000 1000  ................
-000001c0: 0000 0f00 0000 0b00 0000 1000 0000 0b00  ................
-000001d0: 0000 0f00 0000 0e00 0000 0a00 0000 0b00  ................
-000001e0: 0000 0e00 0000 0800 0000 0b00 0000 0700  ................
-000001f0: 0000 0b00 0000 0800 0000 0c00 0000 0b00  ................
-00000200: 0000 0600 0000 0700 0000 0b00 0000 0a00  ................
-00000210: 0000 0600 0000 0900 0000 0300 0000 0400  ................
-00000220: 0000 0900 0000 0800 0000 0300 0000 0800  ................
-00000230: 0000 0900 0000 0c00 0000 0c00 0000 0900  ................
-00000240: 0000 0d00 0000 9474 9462 8c09 6e65 6967  .......t.b..neig
-00000250: 6862 6f72 7394 6811 6814 4b00 8594 6816  hbors.h.h.K...h.
-00000260: 8794 5294 284b 014b 154b 0386 9468 1e89  ..R.(K.K.K...h..
-00000270: 43fc ffff ffff 0900 0000 1400 0000 0200  C...............
-00000280: 0000 0400 0000 1000 0000 0c00 0000 ffff  ................
-00000290: ffff 0100 0000 ffff ffff ffff ffff 0400  ................
-000002a0: 0000 0100 0000 0300 0000 0500 0000 0600  ................
-000002b0: 0000 0f00 0000 0400 0000 0800 0000 0500  ................
-000002c0: 0000 ffff ffff 0800 0000 ffff ffff 1200  ................
-000002d0: 0000 0d00 0000 0600 0000 0700 0000 0000  ................
-000002e0: 0000 0a00 0000 0e00 0000 0900 0000 ffff  ................
-000002f0: ffff 0b00 0000 ffff ffff 0c00 0000 0a00  ................
-00000300: 0000 0b00 0000 0200 0000 1000 0000 0f00  ................
-00000310: 0000 0800 0000 0e00 0000 1300 0000 0900  ................
-00000320: 0000 0d00 0000 0500 0000 0d00 0000 1000  ................
-00000330: 0000 0100 0000 0f00 0000 0c00 0000 ffff  ................
-00000340: ffff ffff ffff 1200 0000 0700 0000 1100  ................
-00000350: 0000 1300 0000 1400 0000 0e00 0000 1200  ................
-00000360: 0000 ffff ffff 0000 0000 1300 0000 9474  ...............t
-00000370: 9462 8c09 6571 7561 7469 6f6e 7394 6811  .b..equations.h.
-00000380: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000390: 154b 0486 9468 1b8c 0266 3894 8988 8794  .K...h...f8.....
-000003a0: 5294 284b 0368 1f4e 4e4e 4aff ffff ff4a  R.(K.h.NNNJ....J
-000003b0: ffff ffff 4b00 7494 6289 42a0 0200 0067  ....K.t.b.B....g
-000003c0: f1b8 d95c 6ee6 3fc9 8c40 e6a7 1be1 3f7a  ...\n.?..@....?z
-000003d0: 4ef2 c8c1 35de bf95 e31c 6750 a955 c0de  N...5.....gP.U..
-000003e0: f909 3617 70e0 3f36 7966 20f5 32e2 3f87  ..6.p.?6yf .2.?.
-000003f0: 4fa6 6d99 8ee4 bffa 3a60 8434 ee4d c068  O.m.....:`.4.M.h
-00000400: 9364 6146 46d5 3f80 fcc6 08bc 9fe6 3f9b  .daFF.?.......?.
-00000410: febe eda0 f9e3 bf2f 788f 33da 3a4d c013  ......./x.3.:M..
-00000420: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000430: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c013  ..[.^.....1..J..
-00000440: 1176 4512 e3e1 3faa 631a bde3 8adc 3fff  .vE...?.c.....?.
-00000450: 83f6 5b8b 5ee6 bf0c f799 31b5 cd4a c0b6  ..[.^.....1..J..
-00000460: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000470: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b6  ....b...S...?N..
-00000480: 9ffd 9f60 f5e4 3f48 3817 9107 03da 3f89  ...`..?H8.....?.
-00000490: deb6 f2cd 62e4 bf80 53e3 bbb3 3f4e c0b5  ....b...S...?N..
-000004a0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004b0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0b5  t*......s..^.Q..
-000004c0: 41aa 8704 45e7 3f26 517b a814 a1d7 3fe9  A...E.?&Q{....?.
-000004d0: 742a bbc6 84e2 bf1e 73c5 0c5e 0b51 c0d5  t*......s..^.Q..
-000004e0: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-000004f0: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0d5  .U,.H......C.S..
-00000500: 906a 752a 76e4 3f3e 6845 027e 71e2 3f46  .ju*v.?>hE.~q.?F
-00000510: bd55 2cb1 48e0 bf8d dfe5 1243 dd53 c0ca  .U,.H......C.S..
-00000520: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000530: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c0ca  ........7.. <R..
-00000540: 8133 6685 00e2 3f15 176b d70d d5e3 3f6d  .3f...?..k....?m
-00000550: 05d6 c89f 82e1 bfb5 3780 b920 3c52 c048  ........7.. <R.H
-00000560: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000570: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c048  ...Ts..!.:ohOR.H
-00000580: 25d3 cc6b ede5 3f5d fafa 14d2 e5de 3f14  %..k..?]......?.
-00000590: bf90 e654 73e1 bf21 ea3a 6f68 4f52 c06c  ...Ts..!.:ohOR.l
-000005a0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005b0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c06c  ...s.......].P.l
-000005c0: d244 aef5 84e3 3f6d 43bb 00f0 cee0 3f79  .D....?mC.....?y
-000005d0: cff7 8673 fce2 bf9a 0ad0 c55d 8850 c006  ...s.......].P..
-000005e0: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-000005f0: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c006  .G.6......mC.S..
-00000600: 6d12 e9b8 00e9 3fd1 14b3 92b2 7bd5 3f38  m.....?.....{.?8
-00000610: 9a47 ee36 d6e0 bf08 8bbb 6d43 1a53 c06b  .G.6......mC.S.k
-00000620: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000630: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c06b  :.Z....v...4>T.k
-00000640: 9843 d0fb cae7 3f5a 0eb3 9f53 5edc 3fc2  .C....?Z...S^.?.
-00000650: 3a86 5aa3 05e0 bf76 03aa d134 3e54 c094  :.Z....v...4>T..
-00000660: 7494 628c 0863 6f70 6c61 6e61 7294 6811  t.b..coplanar.h.
-00000670: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
-00000680: 004b 0386 9468 1e89 4300 9474 9462 8c04  .K...h..C..t.b..
-00000690: 676f 6f64 9468 1168 144b 0085 9468 1687  good.h.h.K...h..
-000006a0: 9452 9428 4b01 4b15 8594 681e 8943 5401  .R.(K.K...h..CT.
-000006b0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006c0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006d0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006e0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-000006f0: 0000 0001 0000 0001 0000 0001 0000 0001  ................
-00000700: 0000 0094 7494 628c 086e 7369 6d70 6c65  ....t.b..nsimple
-00000710: 7894 4b15 8c0a 5f74 7261 6e73 666f 726d  x.K..._transform
-00000720: 944e 8c12 5f76 6572 7465 785f 746f 5f73  .N.._vertex_to_s
-00000730: 696d 706c 6578 944e 8c19 5f76 6572 7465  implex.N.._verte
-00000740: 785f 6e65 6967 6862 6f72 5f76 6572 7469  x_neighbor_verti
-00000750: 6365 7394 4e8c 095f 7665 7274 6963 6573  ces.N.._vertices
-00000760: 9468 188c 075f 706f 696e 7473 9468 1168  .h..._points.h.h
-00000770: 144b 0085 9468 1687 9452 9428 4b01 4b11  .K...h...R.(K.K.
-00000780: 4b02 8694 6831 8942 1001 0000 0000 0000  K...h1.B........
-00000790: 0000 4e40 0000 0000 0080 4640 0000 0000  ..N@......F@....
-000007a0: 0000 5440 0000 0000 0080 4640 0000 0000  ..T@......F@....
-000007b0: 0000 5940 0000 0000 0080 4640 0000 0000  ..Y@......F@....
-000007c0: 0000 5e40 0000 0000 0080 4640 0000 0000  ..^@......F@....
-000007d0: 0080 6140 0000 0000 0080 4640 0000 0000  ..a@......F@....
-000007e0: 0000 4e40 cdcc cccc ccac 5040 0000 0000  ..N@......P@....
-000007f0: 0000 5440 cdcc cccc ccac 5040 0000 0000  ..T@......P@....
-00000800: 0000 5940 cdcc cccc ccac 5040 0000 0000  ..Y@......P@....
-00000810: 0000 5e40 cdcc cccc ccac 5040 0000 0000  ..^@......P@....
-00000820: 0080 6140 cdcc cccc ccac 5040 0000 0000  ..a@......P@....
-00000830: 0000 5440 3333 3333 3313 5640 0000 0000  ..T@33333.V@....
-00000840: 0000 5940 3333 3333 3313 5640 0000 0000  ..Y@33333.V@....
-00000850: 0000 5e40 3333 3333 3313 5640 0000 0000  ..^@33333.V@....
-00000860: 0080 6140 3333 3333 3313 5640 0000 0000  ..a@33333.V@....
-00000870: 0000 5440 0000 0000 0080 5b40 0000 0000  ..T@......[@....
-00000880: 0000 5940 0000 0000 0080 5b40 0000 0000  ..Y@......[@....
-00000890: 0000 5e40 0000 0000 0080 5b40 9474 9462  ..^@......[@.t.b
-000008a0: 8c04 6e64 696d 944b 028c 076e 706f 696e  ..ndim.K...npoin
-000008b0: 7473 944b 118c 096d 696e 5f62 6f75 6e64  ts.K...min_bound
-000008c0: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
-000008d0: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
-000008e0: 004e 4000 0000 0000 8046 4094 7494 628c  .N@......F@.t.b.
-000008f0: 096d 6178 5f62 6f75 6e64 9468 1168 144b  .max_bound.h.h.K
-00000900: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000910: 6831 8943 1000 0000 0000 8061 4000 0000  h1.C.......a@...
-00000920: 0000 805b 4094 7494 628c 0d66 7572 7468  ...[@.t.b..furth
-00000930: 6573 745f 7369 7465 9489 7562 8c0c 7661  est_site..ub..va
-00000940: 6c75 6573 5f73 6861 7065 944b 0185 948c  lues_shape.K....
-00000950: 0676 616c 7565 7394 6811 6814 4b00 8594  .values.h.h.K...
-00000960: 6816 8794 5294 284b 014b 114b 0186 9468  h...R.(K.K.K...h
-00000970: 3189 4388 e17a 14ae 47e1 1c40 0000 0000  1.C..z..G..@....
-00000980: 0000 2140 713d 0ad7 a3f0 2340 52b8 1e85  ..!@q=....#@R...
-00000990: ebd1 2740 0000 0000 0000 2d40 e17a 14ae  ..'@......-@.z..
-000009a0: 47e1 1e40 14ae 47e1 7a94 2140 c3f5 285c  G..@..G.z.!@..(\
-000009b0: 8fc2 2440 14ae 47e1 7a94 2840 0000 0000  ..$@..G.z.(@....
-000009c0: 0080 2d40 9a99 9999 9999 2240 85eb 51b8  ..-@......"@..Q.
-000009d0: 1e45 3340 48e1 7a14 ae47 2940 d7a3 703d  .E3@H.z..G)@..p=
-000009e0: 0ad7 2d40 14ae 47e1 7a94 2340 52b8 1e85  ..-@..G.z.#@R...
-000009f0: eb51 2640 295c 8fc2 f528 2a40 9474 9462  .Q&@)\...(*@.t.b
-00000a00: 8c0a 6973 5f63 6f6d 706c 6578 9489 8c0a  ..is_complex....
-00000a10: 6669 6c6c 5f76 616c 7565 9447 7ff8 0000  fill_value.G....
-00000a20: 0000 0000 8c05 7363 616c 6594 4e8c 0670  ......scale.N..p
-00000a30: 6f69 6e74 7394 684b 7562 2e              oints.hKub.
+00000140: ffff 4b00 7494 6289 425c 0100 000d 0000  ..K.t.b.B\......
+00000150: 000c 0000 0012 0000 0012 0000 0003 0000  ................
+00000160: 0004 0000 0006 0000 000a 0000 0005 0000  ................
+00000170: 0005 0000 000a 0000 000e 0000 0009 0000  ................
+00000180: 0012 0000 0004 0000 0009 0000 000d 0000  ................
+00000190: 0012 0000 000c 0000 0008 0000 0012 0000  ................
+000001a0: 0008 0000 0003 0000 0012 0000 0013 0000  ................
+000001b0: 000d 0000 0010 0000 000c 0000 0013 0000  ................
+000001c0: 0010 0000 0013 0000 000c 0000 000d 0000  ................
+000001d0: 0003 0000 0011 0000 0004 0000 0011 0000  ................
+000001e0: 0003 0000 0002 0000 0001 0000 0011 0000  ................
+000001f0: 0002 0000 0011 0000 0001 0000 0000 0000  ................
+00000200: 0001 0000 0005 0000 0000 0000 0001 0000  ................
+00000210: 0006 0000 0005 0000 0006 0000 0001 0000  ................
+00000220: 0007 0000 0001 0000 0002 0000 0007 0000  ................
+00000230: 0003 0000 0008 0000 0002 0000 0002 0000  ................
+00000240: 0008 0000 0007 0000 000b 0000 000c 0000  ................
+00000250: 0010 0000 000f 0000 000b 0000 0010 0000  ................
+00000260: 000b 0000 000f 0000 000e 0000 000a 0000  ................
+00000270: 000b 0000 000e 0000 0008 0000 000b 0000  ................
+00000280: 0007 0000 000b 0000 0008 0000 000c 0000  ................
+00000290: 000b 0000 0006 0000 0007 0000 000b 0000  ................
+000002a0: 000a 0000 0006 0000 0094 7494 628c 096e  ..........t.b..n
+000002b0: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+000002c0: 9468 1687 9452 9428 4b01 4b1d 4b03 8694  .h...R.(K.K.K...
+000002d0: 681e 8942 5c01 0000 0600 0000 0500 0000  h..B\...........
+000002e0: 0a00 0000 0b00 0000 0400 0000 0700 0000  ................
+000002f0: 0300 0000 1000 0000 1c00 0000 1800 0000  ................
+00000300: ffff ffff 0200 0000 0100 0000 ffff ffff  ................
+00000310: 0500 0000 0000 0000 0400 0000 ffff ffff  ................
+00000320: 0700 0000 0000 0000 1a00 0000 0100 0000  ................
+00000330: 0600 0000 1300 0000 ffff ffff 0900 0000  ................
+00000340: 0a00 0000 0800 0000 1500 0000 0a00 0000  ................
+00000350: 0000 0000 0800 0000 0900 0000 ffff ffff  ................
+00000360: 0100 0000 0c00 0000 1300 0000 0d00 0000  ................
+00000370: 0b00 0000 0c00 0000 1200 0000 0e00 0000  ................
+00000380: 0f00 0000 ffff ffff 0d00 0000 ffff ffff  ................
+00000390: 0e00 0000 1000 0000 0200 0000 0f00 0000  ................
+000003a0: 1100 0000 1200 0000 1b00 0000 1000 0000  ................
+000003b0: 1400 0000 1100 0000 0d00 0000 1400 0000  ................
+000003c0: 0c00 0000 0700 0000 1900 0000 1200 0000  ................
+000003d0: 1300 0000 0900 0000 1600 0000 1a00 0000  ................
+000003e0: 1500 0000 ffff ffff 1700 0000 ffff ffff  ................
+000003f0: 1800 0000 1600 0000 1700 0000 0300 0000  ................
+00000400: 1c00 0000 1b00 0000 1400 0000 1a00 0000  ................
+00000410: 0600 0000 1500 0000 1900 0000 1100 0000  ................
+00000420: 1900 0000 1c00 0000 0200 0000 1b00 0000  ................
+00000430: 1800 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000440: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000450: 5294 284b 014b 1d4b 0486 9468 1b8c 0266  R.(K.K.K...h...f
+00000460: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000470: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000480: 42a0 0300 0079 af00 802c a4e7 3f85 710a  B....y...,..?.q.
+00000490: ba93 18dd 3fee d2ff ec01 d7df bf71 a24b  ....?........q.K
+000004a0: b263 6d54 c0c2 9c32 1d4f 0de9 3f3b 04d8  .cmT...2.O..?;..
+000004b0: cec6 25d5 3faa f025 bfb0 dee0 bf5f 2669  ..%.?..%....._&i
+000004c0: 22e0 1253 c0de f909 3617 70e0 3f36 7966  "..S....6.p.?6yf
+000004d0: 20f5 32e2 3f87 4fa6 6d99 8ee4 bffa 3a60   .2.?.O.m.....:`
+000004e0: 8434 ee4d c068 9364 6146 46d5 3f80 fcc6  .4.M.h.daFF.?...
+000004f0: 08bc 9fe6 3f9b febe eda0 f9e3 bf2f 788f  ....?......../x.
+00000500: 33da 3a4d c02e d28d 1c40 1de9 3fcb 70c0  3.:M.....@..?.p.
+00000510: bc0e 55d5 3f2d ed30 84ee b7e0 bf75 7a21  ..U.?-.0.....uz!
+00000520: 544b 4853 c0ae 70e0 f649 10e8 3fd7 6ce7  TKHS..p..I..?.l.
+00000530: 21d9 f6db 3f12 41e6 f363 96df bf83 27c3  !...?.A..c....'.
+00000540: 2018 9f54 c089 e33d 252c e8e6 3f84 4f54   ..T...=%,..?.OT
+00000550: 1157 9fdd 3f68 6780 e6f0 bae0 bf73 5285  .W..?hg......sR.
+00000560: 543a 5253 c021 2e77 446a a7e8 3f04 13e8  T:RS.!.wDj..?...
+00000570: c8db f1d5 3f6f c7fe cbd1 32e1 bf30 e296  ....?o....2..0..
+00000580: 3fae ae52 c084 732f a49e aee6 3fc9 4cb2  ?..R..s/....?.L.
+00000590: 3040 8ee1 3fb7 dc50 60a3 60dc bf90 e2fd  0@..?..P`.`.....
+000005a0: b085 2257 c0fb 6e1a ab32 bae4 3f8f 46a6  .."W..n..2..?.F.
+000005b0: c59b 46e2 3f7d 6a5b 49d4 22e0 bfb6 d591  ..F.?}j[I.".....
+000005c0: 1275 1b54 c0ed 0077 dc3a 44e7 3f1f c760  .u.T...w.:D.?..`
+000005d0: d667 cdde 3faf d20c 8eca 55df bfc6 2c83  .g..?.....U...,.
+000005e0: ace3 d954 c0b4 8f00 85cb 99e9 3f0b 9233  ...T........?..3
+000005f0: db6b e6d0 3f0d 3f9d ff4a 3de1 bfc4 68c0  .k..?.?..J=...h.
+00000600: a2da a952 c055 52b5 391c 58e8 3f28 9f8b  ...R.UR.9.X.?(..
+00000610: 51f3 efcd 3f36 be13 0eb4 5fe3 bfd4 c345  Q...?6...._....E
+00000620: 6e09 1e50 c0c0 e7c2 d436 d7e6 3fc6 dfd1  n..P.....6..?...
+00000630: 1007 a0b7 bf4b cee4 6f7a 37e6 bf4d 5eed  .....K..oz7..M^.
+00000640: 4141 ec44 c06e 742f 24cd b2de 3f22 a2b0  AA.D.nt/$...?"..
+00000650: 4a01 7ee4 bf8d 36d8 7a12 32e3 bf00 b0cd  J.~...6.z.2.....
+00000660: 37fe 22a3 3f13 1176 4512 e3e1 3faa 631a  7.".?..vE...?.c.
+00000670: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+00000680: 31b5 cd4a c013 1176 4512 e3e1 3faa 631a  1..J...vE...?.c.
+00000690: bde3 8adc 3fff 83f6 5b8b 5ee6 bf0c f799  ....?...[.^.....
+000006a0: 31b5 cd4a c0b6 9ffd 9f60 f5e4 3f48 3817  1..J.....`..?H8.
+000006b0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006c0: bbb3 3f4e c0b6 9ffd 9f60 f5e4 3f48 3817  ..?N.....`..?H8.
+000006d0: 9107 03da 3f89 deb6 f2cd 62e4 bf80 53e3  ....?.....b...S.
+000006e0: bbb3 3f4e c0b5 41aa 8704 45e7 3f26 517b  ..?N..A...E.?&Q{
+000006f0: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000700: 0c5e 0b51 c0b5 41aa 8704 45e7 3f26 517b  .^.Q..A...E.?&Q{
+00000710: a814 a1d7 3fe9 742a bbc6 84e2 bf1e 73c5  ....?.t*......s.
+00000720: 0c5e 0b51 c0d5 906a 752a 76e4 3f3e 6845  .^.Q...ju*v.?>hE
+00000730: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000740: 1243 dd53 c0d5 906a 752a 76e4 3f3e 6845  .C.S...ju*v.?>hE
+00000750: 027e 71e2 3f46 bd55 2cb1 48e0 bf8d dfe5  .~q.?F.U,.H.....
+00000760: 1243 dd53 c0ca 8133 6685 00e2 3f15 176b  .C.S...3f...?..k
+00000770: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+00000780: b920 3c52 c0ca 8133 6685 00e2 3f15 176b  . <R...3f...?..k
+00000790: d70d d5e3 3f6d 05d6 c89f 82e1 bfb5 3780  ....?m........7.
+000007a0: b920 3c52 c048 25d3 cc6b ede5 3f5d fafa  . <R.H%..k..?]..
+000007b0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007c0: 6f68 4f52 c048 25d3 cc6b ede5 3f5d fafa  ohOR.H%..k..?]..
+000007d0: 14d2 e5de 3f14 bf90 e654 73e1 bf21 ea3a  ....?....Ts..!.:
+000007e0: 6f68 4f52 c06c d244 aef5 84e3 3f6d 43bb  ohOR.l.D....?mC.
+000007f0: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000800: c55d 8850 c06c d244 aef5 84e3 3f6d 43bb  .].P.l.D....?mC.
+00000810: 00f0 cee0 3f79 cff7 8673 fce2 bf9a 0ad0  ....?y...s......
+00000820: c55d 8850 c094 7494 628c 0863 6f70 6c61  .].P..t.b..copla
+00000830: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000840: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000850: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000860: 0085 9468 1687 9452 9428 4b01 4b1d 8594  ...h...R.(K.K...
+00000870: 681e 8943 7401 0000 0001 0000 0001 0000  h..Ct...........
+00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008a0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008b0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008c0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008d0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+000008e0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+000008f0: 7369 6d70 6c65 7894 4b1d 8c0a 5f74 7261  simplex.K..._tra
+00000900: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000910: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000920: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000930: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000940: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000950: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000960: 9428 4b01 4b14 4b02 8694 6831 8942 4001  .(K.K.K...h1.B@.
+00000970: 0000 0000 0000 0000 4e40 0000 0000 0080  ........N@......
+00000980: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000990: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+000009a0: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+000009b0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+000009c0: 4640 0000 0000 0000 4e40 cdcc cccc ccac  F@......N@......
+000009d0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+000009e0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+000009f0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000a00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000a10: 5040 0000 0000 0000 5440 3333 3333 3313  P@......T@33333.
+00000a20: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000a30: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000a40: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000a50: 5640 0000 0000 0000 5440 0000 0000 0080  V@......T@......
+00000a60: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000a70: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000a80: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000a90: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000aa0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ab0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000ac0: 076e 706f 696e 7473 944b 148c 096d 696e  .npoints.K...min
+00000ad0: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000ae0: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000af0: 1000 0000 0000 004e 4000 0000 0000 0041  .......N@......A
+00000b00: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000b10: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000b20: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000b30: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000b40: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000b50: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000b60: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000b70: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000b80: 144b 0186 9468 3189 43a0 e17a 14ae 47e1  .K...h1.C..z..G.
+00000b90: 1c40 0000 0000 0000 2140 713d 0ad7 a3f0  .@......!@q=....
+00000ba0: 2340 52b8 1e85 ebd1 2740 0000 0000 0000  #@R.....'@......
+00000bb0: 2d40 e17a 14ae 47e1 1e40 14ae 47e1 7a94  -@.z..G..@..G.z.
+00000bc0: 2140 c3f5 285c 8fc2 2440 14ae 47e1 7a94  !@..(\..$@..G.z.
+00000bd0: 2840 0000 0000 0080 2d40 9a99 9999 9999  (@......-@......
+00000be0: 2240 85eb 51b8 1e45 3340 48e1 7a14 ae47  "@..Q..E3@H.z..G
+00000bf0: 2940 d7a3 703d 0ad7 2d40 14ae 47e1 7a94  )@..p=..-@..G.z.
+00000c00: 2340 52b8 1e85 eb51 2640 295c 8fc2 f528  #@R....Q&@)\...(
+00000c10: 2a40 3333 3333 3333 2540 9a99 9999 9999  *@333333%@......
+00000c20: 2640 0000 0000 0000 2640 9474 9462 8c0a  &@......&@.t.b..
+00000c30: 6973 5f63 6f6d 706c 6578 9489 8c0a 6669  is_complex....fi
+00000c40: 6c6c 5f76 616c 7565 9447 7ff8 0000 0000  ll_value.G......
+00000c50: 0000 8c05 7363 616c 6594 4e8c 0670 6f69  ....scale.N..poi
+00000c60: 6e74 7394 684b 7562 2e                   nts.hKub.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,69 @@
-00000000: 8004 95f2 0400 0000 0000 005d 9428 5d94  ...........].(].
+00000000: 8004 9540 0400 0000 0000 005d 9428 5d94  ...@.......].(].
 00000010: 288c 156e 756d 7079 2e63 6f72 652e 6d75  (..numpy.core.mu
 00000020: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
 00000030: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
 00000040: 7970 6594 9394 8c02 6638 9489 8887 9452  ype.....f8.....R
 00000050: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
 00000060: 4aff ffff ff4b 0074 9462 4308 0000 0000  J....K.t.bC.....
-00000070: 0080 4640 9486 9452 9468 0468 0a43 08cd  ..F@...R.h.h.C..
-00000080: cccc cccc ac50 4094 8694 5294 6804 680a  .....P@...R.h.h.
-00000090: 4308 3333 3333 3313 5640 9486 9452 9468  C.33333.V@...R.h
-000000a0: 0468 0a43 0800 0000 0000 805b 4094 8694  .h.C.......[@...
-000000b0: 5294 655d 9428 5d94 285d 9428 6804 680a  R.e].(].(].(h.h.
-000000c0: 4308 0000 0000 0000 4440 9486 9452 945d  C.......D@...R.]
-000000d0: 9468 0468 0a43 08ec 51b8 1e85 cb46 4094  .h.h.C..Q....F@.
-000000e0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-000000f0: 0000 0000 004e 4094 8694 5294 5d94 6804  .....N@...R.].h.
-00000100: 680a 4308 52b8 1e85 eb31 5040 9486 9452  h.C.R....1P@...R
-00000110: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
-00000120: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
-00000130: 080a d7a3 703d 7a55 4094 8694 5294 6165  ....p=zU@...R.ae
-00000140: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
-00000150: 4094 8694 5294 5d94 6804 680a 4308 c3f5  @...R.].h.h.C...
-00000160: 285c 8f22 5a40 9486 9452 9461 655d 9428  (\."Z@...R.ae].(
-00000170: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
-00000180: 9452 945d 9468 0468 0a43 08f6 285c 8fc2  .R.].h.h.C..(\..
-00000190: 255f 4094 8694 5294 6165 5d94 2868 0468  %_@...R.ae].(h.h
-000001a0: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
-000001b0: 5d94 6804 680a 4308 cdcc cccc cc2c 6240  ].h.h.C......,b@
-000001c0: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
-000001d0: 680a 4308 0000 0000 0000 4440 9486 9452  h.C.......D@...R
-000001e0: 945d 9468 0468 0a43 087b 14ae 47e1 ba47  .].h.h.C.{..G..G
-000001f0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000200: 0800 0000 0000 004e 4094 8694 5294 5d94  .......N@...R.].
-00000210: 6804 680a 4308 295c 8fc2 f5d8 5040 9486  h.h.C.)\....P@..
-00000220: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-00000230: 0000 0000 5440 9486 9452 945d 9468 0468  ....T@...R.].h.h
-00000240: 0a43 08e1 7a14 ae47 a155 4094 8694 5294  .C..z..G.U@...R.
-00000250: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
-00000260: 0059 4094 8694 5294 5d94 6804 680a 4308  .Y@...R.].h.h.C.
-00000270: 9a99 9999 99c9 5a40 9486 9452 9461 655d  ......Z@...R.ae]
-00000280: 9428 6804 680a 4308 0000 0000 0000 5e40  .(h.h.C.......^@
-00000290: 9486 9452 945d 9468 0468 0a43 0885 eb51  ...R.].h.h.C...Q
-000002a0: b81e c55f 4094 8694 5294 6165 5d94 2868  ..._@...R.ae].(h
-000002b0: 0468 0a43 0800 0000 0000 8061 4094 8694  .h.C.......a@...
-000002c0: 5294 5d94 6804 680a 4308 48e1 7a14 ae67  R.].h.h.C.H.z..g
-000002d0: 6240 9486 9452 9461 6565 5d94 285d 9428  b@...R.aee].(].(
-000002e0: 6804 680a 4308 0000 0000 0000 4e40 9486  h.h.C.......N@..
-000002f0: 9452 945d 9468 0468 0a43 088f c2f5 285c  .R.].h.h.C....(\
-00000300: 4f51 4094 8694 5294 6165 5d94 2868 0468  OQ@...R.ae].(h.h
-00000310: 0a43 0800 0000 0000 0054 4094 8694 5294  .C.......T@...R.
-00000320: 5d94 6804 680a 4308 85eb 51b8 1e35 5640  ].h.h.C...Q..5V@
-00000330: 9486 9452 9461 655d 9428 6804 680a 4308  ...R.ae].(h.h.C.
-00000340: 0000 0000 0000 5940 9486 9452 945d 9468  ......Y@...R.].h
-00000350: 0468 0a43 08ae 47e1 7a14 2e5b 4094 8694  .h.C..G.z..[@...
-00000360: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
-00000370: 0000 005e 4094 8694 5294 5d94 6804 680a  ...^@...R.].h.h.
-00000380: 4308 6666 6666 66e6 5f40 9486 9452 9461  C.fffff._@...R.a
-00000390: 655d 9428 6804 680a 4308 0000 0000 0080  e].(h.h.C.......
-000003a0: 6140 9486 9452 945d 9468 0468 0a43 08c3  a@...R.].h.h.C..
-000003b0: f528 5c8f 8a62 4094 8694 5294 6165 655d  .(\..b@...R.aee]
-000003c0: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
-000003d0: 004e 4094 8694 5294 5d94 6804 680a 4308  .N@...R.].h.h.C.
-000003e0: ae47 e17a 14ce 5140 9486 9452 9461 655d  .G.z..Q@...R.ae]
-000003f0: 9428 6804 680a 4308 0000 0000 0000 5440  .(h.h.C.......T@
-00000400: 9486 9452 945d 9468 0468 0a43 081f 85eb  ...R.].h.h.C....
-00000410: 51b8 ae56 4094 8694 5294 6165 5d94 2868  Q..V@...R.ae].(h
-00000420: 0468 0a43 0800 0000 0000 0059 4094 8694  .h.C.......Y@...
-00000430: 5294 5d94 6804 680a 4308 6666 6666 6666  R.].h.h.C.ffffff
-00000440: 5b40 9486 9452 9461 655d 9428 6804 680a  [@...R.ae].(h.h.
-00000450: 4308 0000 0000 0000 5e40 9486 9452 945d  C.......^@...R.]
-00000460: 9468 0468 0a43 08a4 703d 0ad7 4360 4094  .h.h.C..p=..C`@.
-00000470: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-00000480: 0000 0000 8061 4094 8694 5294 5d94 6804  .....a@...R.].h.
-00000490: 680a 4308 3333 3333 33bb 6240 9486 9452  h.C.33333.b@...R
-000004a0: 9461 6565 655d 9428 6804 680a 4308 0000  .aeee].(h.h.C...
-000004b0: 0000 0000 4440 9486 9452 9468 0468 0a43  ....D@...R.h.h.C
-000004c0: 0800 0000 0000 8061 4094 8694 5294 655d  .......a@...R.e]
-000004d0: 9428 4740 36ae 147a e147 ae47 401a 5c28  .(G@6..z.G.G@.\(
-000004e0: f5c2 8f5c 655d 9428 4740 281e b851 eb85  ...\e].(G@(..Q..
-000004f0: 1f47 4018 851e b851 eb85 6565 2e         .G@....Q..ee.
+00000070: 0000 3940 9486 9452 9468 0468 0a43 0800  ..9@...R.h.h.C..
+00000080: 0000 0000 8041 4094 8694 5294 6804 680a  .....A@...R.h.h.
+00000090: 4308 0000 0000 0080 4640 9486 9452 9468  C.......F@...R.h
+000000a0: 0468 0a43 0800 0000 0000 804b 4094 8694  .h.C.......K@...
+000000b0: 5294 6804 680a 4308 0000 0000 0040 5040  R.h.h.C......@P@
+000000c0: 9486 9452 9468 0468 0a43 0800 0000 0000  ...R.h.h.C......
+000000d0: c052 4094 8694 5294 6804 680a 4308 0000  .R@...R.h.h.C...
+000000e0: 0000 0040 5540 9486 9452 9468 0468 0a43  ...@U@...R.h.h.C
+000000f0: 0800 0000 0000 c057 4094 8694 5294 655d  .......W@...R.e]
+00000100: 9428 5d94 285d 9428 6804 680a 4308 0000  .(].(].(h.h.C...
+00000110: 0000 0000 4440 9486 9452 945d 9468 0468  ....D@...R.].h.h
+00000120: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
+00000130: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
+00000140: 0049 4094 8694 5294 5d94 6804 680a 4308  .I@...R.].h.h.C.
+00000150: 0000 0000 0080 6140 9486 9452 9461 6565  ......a@...R.aee
+00000160: 5d94 285d 9428 6804 680a 4308 0000 0000  ].(].(h.h.C.....
+00000170: 0000 4440 9486 9452 945d 9468 0468 0a43  ..D@...R.].h.h.C
+00000180: 0800 0000 0000 8061 4094 8694 5294 6165  .......a@...R.ae
+00000190: 5d94 2868 0468 0a43 0800 0000 0000 0049  ].(h.h.C.......I
+000001a0: 4094 8694 5294 5d94 6804 680a 4308 0000  @...R.].h.h.C...
+000001b0: 0000 0080 6140 9486 9452 9461 6565 5d94  ....a@...R.aee].
+000001c0: 285d 9428 6804 680a 4308 0000 0000 0000  (].(h.h.C.......
+000001d0: 4440 9486 9452 945d 9468 0468 0a43 0800  D@...R.].h.h.C..
+000001e0: 0000 0000 8061 4094 8694 5294 6165 5d94  .....a@...R.ae].
+000001f0: 2868 0468 0a43 0800 0000 0000 0049 4094  (h.h.C.......I@.
+00000200: 8694 5294 5d94 6804 680a 4308 0000 0000  ..R.].h.h.C.....
+00000210: 0080 6140 9486 9452 9461 6565 5d94 285d  ..a@...R.aee].(]
+00000220: 9428 6804 680a 4308 0000 0000 0000 4440  .(h.h.C.......D@
+00000230: 9486 9452 945d 9468 0468 0a43 0800 0000  ...R.].h.h.C....
+00000240: 0000 8061 4094 8694 5294 6165 5d94 2868  ...a@...R.ae].(h
+00000250: 0468 0a43 0800 0000 0000 0049 4094 8694  .h.C.......I@...
+00000260: 5294 5d94 6804 680a 4308 0000 0000 0080  R.].h.h.C.......
+00000270: 6140 9486 9452 9461 6565 5d94 285d 9428  a@...R.aee].(].(
+00000280: 6804 680a 4308 0000 0000 0000 4440 9486  h.h.C.......D@..
+00000290: 9452 945d 9468 0468 0a43 0800 0000 0000  .R.].h.h.C......
+000002a0: 8061 4094 8694 5294 6165 5d94 2868 0468  .a@...R.ae].(h.h
+000002b0: 0a43 0800 0000 0000 0049 4094 8694 5294  .C.......I@...R.
+000002c0: 5d94 6804 680a 4308 0000 0000 0080 6140  ].h.h.C.......a@
+000002d0: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
+000002e0: 680a 4308 0000 0000 0000 4440 9486 9452  h.C.......D@...R
+000002f0: 945d 9468 0468 0a43 0800 0000 0000 8061  .].h.h.C.......a
+00000300: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
+00000310: 0800 0000 0000 0049 4094 8694 5294 5d94  .......I@...R.].
+00000320: 6804 680a 4308 0000 0000 0080 6140 9486  h.h.C.......a@..
+00000330: 9452 9461 6565 5d94 285d 9428 6804 680a  .R.aee].(].(h.h.
+00000340: 4308 0000 0000 0000 4440 9486 9452 945d  C.......D@...R.]
+00000350: 9468 0468 0a43 0800 0000 0000 8061 4094  .h.h.C.......a@.
+00000360: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+00000370: 0000 0000 0049 4094 8694 5294 5d94 6804  .....I@...R.].h.
+00000380: 680a 4308 0000 0000 0080 6140 9486 9452  h.C.......a@...R
+00000390: 9461 6565 5d94 285d 9428 6804 680a 4308  .aee].(].(h.h.C.
+000003a0: 0000 0000 0000 4440 9486 9452 945d 9468  ......D@...R.].h
+000003b0: 0468 0a43 0800 0000 0000 8061 4094 8694  .h.C.......a@...
+000003c0: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
+000003d0: 0000 0049 4094 8694 5294 5d94 6804 680a  ...I@...R.].h.h.
+000003e0: 4308 0000 0000 0080 6140 9486 9452 9461  C.......a@...R.a
+000003f0: 6565 655d 9428 6804 680a 4308 0000 0000  eee].(h.h.C.....
+00000400: 0000 4440 9486 9452 9468 0468 0a43 0800  ..D@...R.h.h.C..
+00000410: 0000 0000 0049 4094 8694 5294 655d 9428  .....I@...R.e].(
+00000420: 4740 3561 19ce 075f 7047 4013 7ae1 47ae  G@5a..._pG@.z.G.
+00000430: 147b 655d 9428 4740 25a9 6bb9 8c7e 2847  .{e].(G@%.k..~(G
+00000440: 4012 47ae 147a e148 6565 2e              @.G..z.Hee.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9552 0c00 0000 0000 008c 1a73 6369  ...R.........sci
+00000000: 8004 95b6 0e00 0000 0000 008c 1a73 6369  .............sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,188 +11,227 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 303e 1af4 bbf4 5e8c 0973 696d 706c  G.0>....^..simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 1c4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 254b 0386 9468 128c 0564 7479 7065  .K%K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 4250 0100 0006 0000  ..K.t.b.BP......
-00000150: 000c 0000 0011 0000 0007 0000 000c 0000  ................
-00000160: 0006 0000 0002 0000 0007 0000 0001 0000  ................
-00000170: 0007 0000 0002 0000 0008 0000 0001 0000  ................
-00000180: 0007 0000 0000 0000 0007 0000 0006 0000  ................
-00000190: 0000 0000 000d 0000 0007 0000 0008 0000  ................
-000001a0: 0007 0000 000d 0000 000c 0000 000b 0000  ................
-000001b0: 0004 0000 0005 0000 0004 0000 000b 0000  ................
-000001c0: 000a 0000 000d 0000 0012 0000 000c 0000  ................
-000001d0: 000c 0000 0012 0000 0011 0000 0012 0000  ................
-000001e0: 000e 0000 0013 0000 000e 0000 0012 0000  ................
-000001f0: 000d 0000 0009 0000 000d 0000 0008 0000  ................
-00000200: 0009 0000 000e 0000 000d 0000 0009 0000  ................
-00000210: 0002 0000 0003 0000 0002 0000 0009 0000  ................
-00000220: 0008 0000 0004 0000 0009 0000 0003 0000  ................
-00000230: 0009 0000 0004 0000 000a 0000 000f 0000  ................
-00000240: 0014 0000 0013 0000 000e 0000 000f 0000  ................
-00000250: 0013 0000 0014 0000 000f 0000 0015 0000  ................
-00000260: 000f 0000 0010 0000 0015 0000 0009 0000  ................
-00000270: 000f 0000 000e 0000 000f 0000 0009 0000  ................
-00000280: 000a 0000 000b 0000 000f 0000 000a 0000  ................
-00000290: 0010 0000 000f 0000 000b 0000 0094 7494  ..............t.
-000002a0: 628c 096e 6569 6768 626f 7273 9468 1168  b..neighbors.h.h
-000002b0: 144b 0085 9468 1687 9452 9428 4b01 4b1c  .K...h...R.(K.K.
-000002c0: 4b03 8694 681e 8942 5001 0000 0b00 0000  K...h..BP.......
-000002d0: ffff ffff 0100 0000 0000 0000 0500 0000  ................
-000002e0: 0700 0000 0400 0000 ffff ffff 0300 0000  ................
-000002f0: 1100 0000 0600 0000 0200 0000 0500 0000  ................
-00000300: ffff ffff 0200 0000 ffff ffff 0400 0000  ................
-00000310: 0100 0000 0300 0000 0e00 0000 0700 0000  ................
-00000320: 0a00 0000 0100 0000 0600 0000 ffff ffff  ................
-00000330: ffff ffff 0900 0000 1a00 0000 1300 0000  ................
-00000340: 0800 0000 0b00 0000 0700 0000 0d00 0000  ................
-00000350: ffff ffff 0000 0000 0a00 0000 1500 0000  ................
-00000360: ffff ffff 0d00 0000 0a00 0000 0f00 0000  ................
-00000370: 0c00 0000 0600 0000 1100 0000 0f00 0000  ................
-00000380: 0d00 0000 0e00 0000 1800 0000 ffff ffff  ................
-00000390: 1200 0000 1100 0000 0e00 0000 0300 0000  ................
-000003a0: 1000 0000 1000 0000 ffff ffff 1300 0000  ................
-000003b0: 0900 0000 1900 0000 1200 0000 ffff ffff  ................
-000003c0: 1500 0000 1600 0000 1400 0000 0c00 0000  ................
-000003d0: 1800 0000 1700 0000 ffff ffff 1400 0000  ................
-000003e0: ffff ffff 1600 0000 1b00 0000 1500 0000  ................
-000003f0: 0f00 0000 1900 0000 1300 0000 1a00 0000  ................
-00000400: 1800 0000 1900 0000 0900 0000 1b00 0000  ................
-00000410: 1a00 0000 ffff ffff 1700 0000 9474 9462  .............t.b
-00000420: 8c09 6571 7561 7469 6f6e 7394 6811 6814  ..equations.h.h.
-00000430: 4b00 8594 6816 8794 5294 284b 014b 1c4b  K...h...R.(K.K.K
-00000440: 0486 9468 1b8c 0266 3894 8988 8794 5294  ...h...f8.....R.
-00000450: 284b 0368 1f4e 4e4e 4aff ffff ff4a ffff  (K.h.NNNJ....J..
-00000460: ffff 4b00 7494 6289 4280 0300 0053 a8b3  ..K.t.b.B....S..
-00000470: 4d50 78c6 3fbd 52c2 3abb ece4 3f00 5ea5  MPx.?.R.:...?.^.
-00000480: 6dc8 8ce7 bf59 6b06 b36f 5245 c02a 4aba  m....Yk..oRE.*J.
-00000490: 3e9f 1ad6 3f7e f969 9d6e 21e1 3f51 b23f  >...?~.i.n!.?Q.?
-000004a0: 7a6a aae8 bfa6 a95a 7f35 9344 c0cd ecaf  zj.....Z.5.D....
-000004b0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004c0: 1f16 f5e8 bfec e5e7 1629 f743 c0cd ecaf  .........).C....
-000004d0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004e0: 1f16 f5e8 bfec e5e7 1629 f743 c07d 409c  .........).C.}@.
-000004f0: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000500: 011f 90ea bfd6 3798 cb60 c940 c07d 409c  ......7..`.@.}@.
-00000510: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000520: 011f 90ea bfd6 3798 cb60 c940 c044 0f45  ......7..`.@.D.E
-00000530: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000540: a63b 5de7 bff8 e8ec 534a 6a47 c044 0f45  .;].....SJjG.D.E
-00000550: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000560: a63b 5de7 bff8 e8ec 534a 6a47 c022 c659  .;].....SJjG.".Y
-00000570: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-00000580: 6bf7 d0e3 bf02 98b8 5e21 4050 c022 c659  k.......^!@P.".Y
-00000590: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-000005a0: 6bf7 d0e3 bf02 98b8 5e21 4050 c0d0 ab7f  k.......^!@P....
-000005b0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005c0: 4987 a8e5 bfbd 4052 e4ca 804b c0d0 ab7f  I.....@R...K....
-000005d0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005e0: 4987 a8e5 bfbd 4052 e4ca 804b c058 fe98  I.....@R...K.X..
-000005f0: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000600: d76c 7ce4 bf4f 3a98 41a4 9a4e c058 fe98  .l|..O:.A..N.X..
-00000610: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000620: d76c 7ce4 bf4f 3a98 41a4 9a4e c049 3cb0  .l|..O:.A..N.I<.
-00000630: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000640: 9e55 e9e5 bfe4 5a46 9a45 de4a c049 3cb0  .U....ZF.E.J.I<.
-00000650: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000660: 9e55 e9e5 bfe4 5a46 9a45 de4a c0ba 8c7c  .U....ZF.E.J...|
-00000670: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-00000680: 948f 35e7 bf76 4df1 3045 c447 c0ba 8c7c  ..5..vM.0E.G...|
-00000690: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-000006a0: 948f 35e7 bf76 4df1 3045 c447 c036 6eb5  ..5..vM.0E.G.6n.
-000006b0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006c0: bd5e 77e5 bfda 189c f64f fe4b c036 6eb5  .^w......O.K.6n.
-000006d0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006e0: bd5e 77e5 bfda 189c f64f fe4b c0ab 5c88  .^w......O.K..\.
-000006f0: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000700: 82ef 41e3 bf8c 6c96 e3b6 1451 c0ab 5c88  ..A...l....Q..\.
-00000710: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000720: 82ef 41e3 bf8c 6c96 e3b6 1451 c094 32f3  ..A...l....Q..2.
-00000730: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000740: f71b 0ae2 bf08 e69e 8619 0853 c094 32f3  ...........S..2.
-00000750: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000760: f71b 0ae2 bf08 e69e 8619 0853 c028 b95b  ...........S.(.[
-00000770: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-00000780: 6b57 6de4 bfcf 2e5c 6bc4 c44e c028 b95b  kWm....\k..N.(.[
-00000790: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-000007a0: 6b57 6de4 bfcf 2e5c 6bc4 c44e c03c 0a19  kWm....\k..N.<..
-000007b0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007c0: c673 fde2 bf72 990a 512b 7e51 c03c 0a19  .s...r..Q+~Q.<..
-000007d0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007e0: c673 fde2 bf72 990a 512b 7e51 c094 7494  .s...r..Q+~Q..t.
-000007f0: 628c 0863 6f70 6c61 6e61 7294 6811 6814  b..coplanar.h.h.
-00000800: 4b00 8594 6816 8794 5294 284b 014b 004b  K...h...R.(K.K.K
-00000810: 0386 9468 1e89 4300 9474 9462 8c04 676f  ...h..C..t.b..go
-00000820: 6f64 9468 1168 144b 0085 9468 1687 9452  od.h.h.K...h...R
-00000830: 9428 4b01 4b1c 8594 681e 8943 7001 0000  .(K.K...h..Cp...
-00000840: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000850: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000860: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000870: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-000008a0: 0001 0000 0001 0000 0001 0000 0094 7494  ..............t.
-000008b0: 628c 086e 7369 6d70 6c65 7894 4b1c 8c0a  b..nsimplex.K...
-000008c0: 5f74 7261 6e73 666f 726d 944e 8c12 5f76  _transform.N.._v
-000008d0: 6572 7465 785f 746f 5f73 696d 706c 6578  ertex_to_simplex
-000008e0: 944e 8c19 5f76 6572 7465 785f 6e65 6967  .N.._vertex_neig
-000008f0: 6862 6f72 5f76 6572 7469 6365 7394 4e8c  hbor_vertices.N.
-00000900: 095f 7665 7274 6963 6573 9468 188c 075f  ._vertices.h..._
-00000910: 706f 696e 7473 9468 1168 144b 0085 9468  points.h.h.K...h
-00000920: 1687 9452 9428 4b01 4b16 4b02 8694 6831  ...R.(K.K.K...h1
-00000930: 8942 6001 0000 0000 0000 0000 4440 0000  .B`.........D@..
-00000940: 0000 0080 4640 0000 0000 0000 4e40 0000  ....F@......N@..
-00000950: 0000 0080 4640 0000 0000 0000 5440 0000  ....F@......T@..
-00000960: 0000 0080 4640 0000 0000 0000 5940 0000  ....F@......Y@..
-00000970: 0000 0080 4640 0000 0000 0000 5e40 0000  ....F@......^@..
-00000980: 0000 0080 4640 0000 0000 0080 6140 0000  ....F@......a@..
-00000990: 0000 0080 4640 0000 0000 0000 4440 cdcc  ....F@......D@..
-000009a0: cccc ccac 5040 0000 0000 0000 4e40 cdcc  ....P@......N@..
-000009b0: cccc ccac 5040 0000 0000 0000 5440 cdcc  ....P@......T@..
-000009c0: cccc ccac 5040 0000 0000 0000 5940 cdcc  ....P@......Y@..
-000009d0: cccc ccac 5040 0000 0000 0000 5e40 cdcc  ....P@......^@..
-000009e0: cccc ccac 5040 0000 0000 0080 6140 cdcc  ....P@......a@..
-000009f0: cccc ccac 5040 0000 0000 0000 4e40 3333  ....P@......N@33
-00000a00: 3333 3313 5640 0000 0000 0000 5440 3333  333.V@......T@33
-00000a10: 3333 3313 5640 0000 0000 0000 5940 3333  333.V@......Y@33
-00000a20: 3333 3313 5640 0000 0000 0000 5e40 3333  333.V@......^@33
-00000a30: 3333 3313 5640 0000 0000 0080 6140 3333  333.V@......a@33
-00000a40: 3333 3313 5640 0000 0000 0000 4e40 0000  333.V@......N@..
-00000a50: 0000 0080 5b40 0000 0000 0000 5440 0000  ....[@......T@..
-00000a60: 0000 0080 5b40 0000 0000 0000 5940 0000  ....[@......Y@..
-00000a70: 0000 0080 5b40 0000 0000 0000 5e40 0000  ....[@......^@..
-00000a80: 0000 0080 5b40 0000 0000 0080 6140 0000  ....[@......a@..
-00000a90: 0000 0080 5b40 9474 9462 8c04 6e64 696d  ....[@.t.b..ndim
-00000aa0: 944b 028c 076e 706f 696e 7473 944b 168c  .K...npoints.K..
-00000ab0: 096d 696e 5f62 6f75 6e64 9468 1168 144b  .min_bound.h.h.K
-00000ac0: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000ad0: 6831 8943 1000 0000 0000 0044 4000 0000  h1.C.......D@...
-00000ae0: 0000 8046 4094 7494 628c 096d 6178 5f62  ...F@.t.b..max_b
-00000af0: 6f75 6e64 9468 1168 144b 0085 9468 1687  ound.h.h.K...h..
-00000b00: 9452 9428 4b01 4b02 8594 6831 8943 1000  .R.(K.K...h1.C..
-00000b10: 0000 0000 8061 4000 0000 0000 805b 4094  .....a@......[@.
-00000b20: 7494 628c 0d66 7572 7468 6573 745f 7369  t.b..furthest_si
-00000b30: 7465 9489 7562 8c0c 7661 6c75 6573 5f73  te..ub..values_s
-00000b40: 6861 7065 944b 0185 948c 0676 616c 7565  hape.K.....value
-00000b50: 7394 6811 6814 4b00 8594 6816 8794 5294  s.h.h.K...h...R.
-00000b60: 284b 014b 164b 0186 9468 3189 43b0 85eb  (K.K.K...h1.C...
-00000b70: 51b8 1e85 2940 3d0a d7a3 70bd 2740 0ad7  Q...)@=...p.'@..
-00000b80: a370 3d8a 2a40 e17a 14ae 47e1 2740 52b8  .p=.*@.z..G.'@R.
-00000b90: 1e85 eb51 2940 1f85 eb51 b81e 2840 c3f5  ...Q)@...Q..(@..
-00000ba0: 285c 8f42 3140 52b8 1e85 eb51 3140 a470  (\.B1@R....Q1@.p
-00000bb0: 3d0a d723 3140 cdcc cccc cc8c 3040 295c  =..#1@......0@)\
-00000bc0: 8fc2 f568 3040 8fc2 f528 5c8f 2f40 ae47  ...h0@...(\./@.G
-00000bd0: e17a 14ae 3540 c3f5 285c 8f02 3540 a470  .z..5@..(\..5@.p
-00000be0: 3d0a d763 3440 48e1 7a14 ae07 3440 1f85  =..c4@H.z...4@..
-00000bf0: eb51 b89e 3340 3d0a d7a3 70fd 3940 52b8  .Q..3@=...p.9@R.
-00000c00: 1e85 eb91 3840 0000 0000 0040 3840 713d  ....8@.....@8@q=
-00000c10: 0ad7 a330 3740 ae47 e17a 14ae 3640 9474  ...07@.G.z..6@.t
-00000c20: 9462 8c0a 6973 5f63 6f6d 706c 6578 9489  .b..is_complex..
-00000c30: 8c0a 6669 6c6c 5f76 616c 7565 9447 7ff8  ..fill_value.G..
-00000c40: 0000 0000 0000 8c05 7363 616c 6594 4e8c  ........scale.N.
-00000c50: 0670 6f69 6e74 7394 684b 7562 2e         .points.hKub.
+00000140: ffff 4b00 7494 6289 42bc 0100 0016 0000  ..K.t.b.B.......
+00000150: 0001 0000 0000 0000 0006 0000 000c 0000  ................
+00000160: 0011 0000 0002 0000 0016 0000 0003 0000  ................
+00000170: 0002 0000 0001 0000 0016 0000 0007 0000  ................
+00000180: 000c 0000 0006 0000 0016 0000 0004 0000  ................
+00000190: 0003 0000 0004 0000 0016 0000 0005 0000  ................
+000001a0: 0014 0000 0018 0000 0015 0000 0018 0000  ................
+000001b0: 0010 0000 0015 0000 000f 0000 0010 0000  ................
+000001c0: 0018 0000 0014 0000 000f 0000 0018 0000  ................
+000001d0: 0010 0000 0017 0000 000b 0000 0017 0000  ................
+000001e0: 000f 0000 000a 0000 000f 0000 0017 0000  ................
+000001f0: 0010 0000 000b 0000 0017 0000 0005 0000  ................
+00000200: 0004 0000 0017 0000 000a 0000 0017 0000  ................
+00000210: 0004 0000 0005 0000 0002 0000 0007 0000  ................
+00000220: 0001 0000 0007 0000 0002 0000 0008 0000  ................
+00000230: 0007 0000 0006 0000 0000 0000 0001 0000  ................
+00000240: 0007 0000 0000 0000 000d 0000 0007 0000  ................
+00000250: 0008 0000 0007 0000 000d 0000 000c 0000  ................
+00000260: 000d 0000 0012 0000 000c 0000 000c 0000  ................
+00000270: 0012 0000 0011 0000 0012 0000 000e 0000  ................
+00000280: 0013 0000 000e 0000 0012 0000 000d 0000  ................
+00000290: 0009 0000 000d 0000 0008 0000 0009 0000  ................
+000002a0: 000e 0000 000d 0000 0002 0000 0009 0000  ................
+000002b0: 0008 0000 0009 0000 0002 0000 0003 0000  ................
+000002c0: 0009 0000 0004 0000 000a 0000 0004 0000  ................
+000002d0: 0009 0000 0003 0000 0009 0000 000f 0000  ................
+000002e0: 000e 0000 000f 0000 0009 0000 000a 0000  ................
+000002f0: 000e 0000 000f 0000 0013 0000 000f 0000  ................
+00000300: 0014 0000 0013 0000 0094 7494 628c 096e  ..........t.b..n
+00000310: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+00000320: 9468 1687 9452 9428 4b01 4b25 4b03 8694  .h...R.(K.K%K...
+00000330: 681e 8942 bc01 0000 1400 0000 ffff ffff  h..B............
+00000340: 0300 0000 1800 0000 ffff ffff 0400 0000  ................
+00000350: 0500 0000 1e00 0000 0300 0000 0000 0000  ................
+00000360: 0200 0000 1100 0000 0100 0000 1300 0000  ................
+00000370: 1600 0000 2000 0000 0200 0000 0600 0000  .... ...........
+00000380: ffff ffff 1000 0000 0500 0000 0800 0000  ................
+00000390: ffff ffff 0a00 0000 ffff ffff 0700 0000  ................
+000003a0: 0900 0000 0800 0000 0a00 0000 0d00 0000  ................
+000003b0: 0900 0000 0700 0000 2400 0000 0e00 0000  ........$.......
+000003c0: ffff ffff 0d00 0000 2200 0000 0f00 0000  ........".......
+000003d0: 0d00 0000 0b00 0000 0900 0000 0c00 0000  ................
+000003e0: 1000 0000 ffff ffff 0b00 0000 0c00 0000  ................
+000003f0: 1f00 0000 1000 0000 0600 0000 0e00 0000  ................
+00000400: 0f00 0000 1400 0000 0300 0000 1200 0000  ................
+00000410: 1d00 0000 1500 0000 1100 0000 ffff ffff  ................
+00000420: 1400 0000 0400 0000 1300 0000 0000 0000  ................
+00000430: 1100 0000 1200 0000 1b00 0000 1600 0000  ................
+00000440: 1700 0000 0400 0000 1500 0000 1800 0000  ................
+00000450: 1600 0000 1a00 0000 ffff ffff 0100 0000  ................
+00000460: 1700 0000 2300 0000 ffff ffff 1a00 0000  ....#...........
+00000470: 1700 0000 1c00 0000 1900 0000 1500 0000  ................
+00000480: 1d00 0000 1c00 0000 1a00 0000 1b00 0000  ................
+00000490: 2100 0000 1b00 0000 1200 0000 1e00 0000  !...............
+000004a0: 0200 0000 2000 0000 1d00 0000 0f00 0000  .... ...........
+000004b0: 2200 0000 2000 0000 1e00 0000 0500 0000  "... ...........
+000004c0: 1f00 0000 2300 0000 1c00 0000 2200 0000  ....#......."...
+000004d0: 1f00 0000 0c00 0000 2100 0000 2400 0000  ........!...$...
+000004e0: 1900 0000 2100 0000 ffff ffff 2300 0000  ....!.......#...
+000004f0: 0a00 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000500: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000510: 5294 284b 014b 254b 0486 9468 1b8c 0266  R.(K.K%K...h...f
+00000520: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000530: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000540: 42a0 0400 006c 9d0b 2029 2fca 3fef f2f5  B....l.. )/.?...
+00000550: a729 b5eb bf94 0759 5302 38dd bf6f 3c2e  .).....YS.8..o<.
+00000560: ba05 c83e 4053 a8b3 4d50 78c6 3fbd 52c2  ...>@S..MPx.?.R.
+00000570: 3abb ece4 3f00 5ea5 6dc8 8ce7 bf59 6b06  :...?.^.m....Yk.
+00000580: b36f 5245 c076 abab 32fd 05e4 3f49 03bf  .oRE.v..2...?I..
+00000590: 7a08 b6b4 bf19 51ac be9d d3e8 bfda 3435  z.....Q.......45
+000005a0: 2c51 bb3d c0cd 41e7 aaec bcdb 3f87 bd0c  ,Q.=..A.....?...
+000005b0: ff18 84e2 bf0c 2c16 65e8 1be6 bf82 c9c9  ......,.e.......
+000005c0: 8db1 e618 402a 4aba 3e9f 1ad6 3f7e f969  ....@*J.>...?~.i
+000005d0: 9d6e 21e1 3f51 b23f 7a6a aae8 bfa6 a95a  .n!.?Q.?zj.....Z
+000005e0: 7f35 9344 c0ac 2dbe c07c f5e5 3fa1 85cd  .5.D..-..|..?...
+000005f0: 1f09 01cb 3ffe 0c91 f4b4 46e6 bfe2 a394  ....?.....F.....
+00000600: 1a07 f549 c026 be92 60ca 8de7 3fd0 aeff  ...I.&..`...?...
+00000610: 9902 19cf 3f6b bf14 a7d8 37e4 bf11 bf51  ....?k....7....Q
+00000620: 02f4 824f c02f b392 2edf b3e4 3f4a 2e8a  ...O./......?J..
+00000630: 6aaa b8e0 3fc4 a1f0 9e4c c5e1 bfac d48d  j...?....L......
+00000640: 1676 8c53 c0c4 c014 b0c6 89e5 3fbc 35e8  .v.S........?.5.
+00000650: f572 70df 3faf 1eea cb19 b1e1 bfd0 7da8  .rp.?.........}.
+00000660: 09e4 ad53 c066 6a97 64b6 b2e5 3feb 87a2  ...S.fj.d...?...
+00000670: ffd6 b9dc 3fe3 a3f2 980c a0e2 bf62 5e51  ....?........b^Q
+00000680: fb3c 2452 c007 8b11 bf0c 41e3 3f19 978d  .<$R......A.?...
+00000690: 4511 fae0 3f1d cbb4 6652 1be3 bf9e ebc7  E...?...fR......
+000006a0: 0725 5751 c009 13e8 3df9 6ae6 3fed 2483  .%WQ....=.j.?.$.
+000006b0: 3f3d 0dda 3f9e 2c27 2964 c1e2 bff2 acb7  ?=..?.,')d......
+000006c0: 00e5 e551 c0af 873e 5392 2be5 3f1d b5c5  ...Q...>S.+.?...
+000006d0: e465 60db 3ff9 5462 e78f b5e3 bf2a 792d  .e`.?.Tb.....*y-
+000006e0: f8f9 7950 c086 3415 5449 00e6 3f7b 4074  ..yP..4.TI..?{@t
+000006f0: 61cf 13db 3fc8 c3d2 17a3 e2e2 bf55 1a4e  a...?........U.N
+00000700: 3c1b b051 c093 6cc4 916a 36e7 3f5f c433  <..Q..l..j6.?_.3
+00000710: 6489 b7d3 3f56 72fe 9f88 b2e3 bf79 3328  d...?Vr......y3(
+00000720: bc79 7150 c0da 9258 75e7 b0e6 3f2d 2b7d  .yqP...Xu...?-+}
+00000730: 6f91 32d4 3f2d 4c72 7371 2de4 bfeb 9fb3  o.2.?-Lrsq-.....
+00000740: d17e 904f c0de 0080 23d7 1fe7 3f1d f11c  .~.O....#...?...
+00000750: 6837 85d3 3fc5 7598 a677 d9e3 bfde 1615  h7..?.u..w......
+00000760: d767 3750 c0cd ecaf a5c0 4fdf 3f08 44ab  .g7P......O.?.D.
+00000770: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+00000780: 1629 f743 c0cd ecaf a5c0 4fdf 3f08 44ab  .).C......O.?.D.
+00000790: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+000007a0: 1629 f743 c07d 409c 2fe2 cdd7 3f44 7c8c  .).C.}@./...?D|.
+000007b0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007c0: cb60 c940 c07d 409c 2fe2 cdd7 3f44 7c8c  .`.@.}@./...?D|.
+000007d0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007e0: cb60 c940 c044 0f45 310f 50dd 3f2d 16fd  .`.@.D.E1.P.?-..
+000007f0: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000800: 534a 6a47 c044 0f45 310f 50dd 3f2d 16fd  SJjG.D.E1.P.?-..
+00000810: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000820: 534a 6a47 c0d0 ab7f 642b 2cdb 3f56 8bd0  SJjG....d+,.?V..
+00000830: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000840: e4ca 804b c0d0 ab7f 642b 2cdb 3f56 8bd0  ...K....d+,.?V..
+00000850: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000860: e4ca 804b c058 fe98 fdc7 85e0 3f79 f9a8  ...K.X......?y..
+00000870: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+00000880: 41a4 9a4e c058 fe98 fdc7 85e0 3f79 f9a8  A..N.X......?y..
+00000890: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+000008a0: 41a4 9a4e c049 3cb0 5517 ace1 3fef 2e5a  A..N.I<.U...?..Z
+000008b0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008c0: 9a45 de4a c049 3cb0 5517 ace1 3fef 2e5a  .E.J.I<.U...?..Z
+000008d0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008e0: 9a45 de4a c0ba 8c7c 990a b8e2 3f5c cd68  .E.J...|....?\.h
+000008f0: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000900: 3045 c447 c0ba 8c7c 990a b8e2 3f5c cd68  0E.G...|....?\.h
+00000910: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000920: 3045 c447 c036 6eb5 7d1a 29e5 3ffc cfb3  0E.G.6n.}.).?...
+00000930: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000940: f64f fe4b c036 6eb5 7d1a 29e5 3ffc cfb3  .O.K.6n.}.).?...
+00000950: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000960: f64f fe4b c028 b95b 1edd 22e4 3fef 8498  .O.K.(.[..".?...
+00000970: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+00000980: 6bc4 c44e c028 b95b 1edd 22e4 3fef 8498  k..N.(.[..".?...
+00000990: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+000009a0: 6bc4 c44e c0ab 5c88 d9b8 fbe2 3fd9 4116  k..N..\.....?.A.
+000009b0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009c0: e3b6 1451 c0ab 5c88 d9b8 fbe2 3fd9 4116  ...Q..\.....?.A.
+000009d0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009e0: e3b6 1451 c094 7494 628c 0863 6f70 6c61  ...Q..t.b..copla
+000009f0: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000a00: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000a10: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000a20: 0085 9468 1687 9452 9428 4b01 4b25 8594  ...h...R.(K.K%..
+00000a30: 681e 8943 9401 0000 0001 0000 0001 0000  h..C............
+00000a40: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a50: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a60: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a70: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a80: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a90: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000aa0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ab0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ac0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+00000ad0: 7369 6d70 6c65 7894 4b25 8c0a 5f74 7261  simplex.K%.._tra
+00000ae0: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000af0: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000b00: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000b10: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000b20: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000b30: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000b40: 9428 4b01 4b19 4b02 8694 6831 8942 9001  .(K.K.K...h1.B..
+00000b50: 0000 0000 0000 0000 4440 0000 0000 0080  ........D@......
+00000b60: 4640 0000 0000 0000 4e40 0000 0000 0080  F@......N@......
+00000b70: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000b80: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+00000b90: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+00000ba0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+00000bb0: 4640 0000 0000 0000 4440 cdcc cccc ccac  F@......D@......
+00000bc0: 5040 0000 0000 0000 4e40 cdcc cccc ccac  P@......N@......
+00000bd0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+00000be0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+00000bf0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000c00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000c10: 5040 0000 0000 0000 4e40 3333 3333 3313  P@......N@33333.
+00000c20: 5640 0000 0000 0000 5440 3333 3333 3313  V@......T@33333.
+00000c30: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000c40: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000c50: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000c60: 5640 0000 0000 0000 4e40 0000 0000 0080  V@......N@......
+00000c70: 5b40 0000 0000 0000 5440 0000 0000 0080  [@......T@......
+00000c80: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000c90: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000ca0: 5b40 0000 0000 0080 6140 0000 0000 0080  [@......a@......
+00000cb0: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000cc0: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000cd0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ce0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000cf0: 076e 706f 696e 7473 944b 198c 096d 696e  .npoints.K...min
+00000d00: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000d10: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000d20: 1000 0000 0000 0044 4000 0000 0000 0041  .......D@......A
+00000d30: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000d40: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000d50: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000d60: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000d70: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000d80: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000d90: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000da0: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000db0: 194b 0186 9468 3189 43c8 85eb 51b8 1e85  .K...h1.C...Q...
+00000dc0: 2940 3d0a d7a3 70bd 2740 0ad7 a370 3d8a  )@=...p.'@...p=.
+00000dd0: 2a40 e17a 14ae 47e1 2740 52b8 1e85 eb51  *@.z..G.'@R....Q
+00000de0: 2940 1f85 eb51 b81e 2840 c3f5 285c 8f42  )@...Q..(@..(\.B
+00000df0: 3140 52b8 1e85 eb51 3140 a470 3d0a d723  1@R....Q1@.p=..#
+00000e00: 3140 cdcc cccc cc8c 3040 295c 8fc2 f568  1@......0@)\...h
+00000e10: 3040 8fc2 f528 5c8f 2f40 ae47 e17a 14ae  0@...(\./@.G.z..
+00000e20: 3540 c3f5 285c 8f02 3540 a470 3d0a d763  5@..(\..5@.p=..c
+00000e30: 3440 48e1 7a14 ae07 3440 1f85 eb51 b89e  4@H.z...4@...Q..
+00000e40: 3340 3d0a d7a3 70fd 3940 52b8 1e85 eb91  3@=...p.9@R.....
+00000e50: 3840 0000 0000 0040 3840 713d 0ad7 a330  8@.....@8@q=...0
+00000e60: 3740 ae47 e17a 14ae 3640 3333 3333 3333  7@.G.z..6@333333
+00000e70: 2640 9a99 9999 9919 3040 3333 3333 3333  &@......0@333333
+00000e80: 3340 9474 9462 8c0a 6973 5f63 6f6d 706c  3@.t.b..is_compl
+00000e90: 6578 9489 8c0a 6669 6c6c 5f76 616c 7565  ex....fill_value
+00000ea0: 9447 7ff8 0000 0000 0000 8c05 7363 616c  .G..........scal
+00000eb0: 6594 4e8c 0670 6f69 6e74 7394 684b 7562  e.N..points.hKub
+00000ec0: 2e                                       .
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9552 0c00 0000 0000 008c 1a73 6369  ...R.........sci
+00000000: 8004 95b6 0e00 0000 0000 008c 1a73 6369  .............sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,188 +11,227 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 303e 1af4 bbf4 5e8c 0973 696d 706c  G.0>....^..simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 1c4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 254b 0386 9468 128c 0564 7479 7065  .K%K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 4250 0100 0006 0000  ..K.t.b.BP......
-00000150: 000c 0000 0011 0000 0007 0000 000c 0000  ................
-00000160: 0006 0000 0002 0000 0007 0000 0001 0000  ................
-00000170: 0007 0000 0002 0000 0008 0000 0001 0000  ................
-00000180: 0007 0000 0000 0000 0007 0000 0006 0000  ................
-00000190: 0000 0000 000d 0000 0007 0000 0008 0000  ................
-000001a0: 0007 0000 000d 0000 000c 0000 000b 0000  ................
-000001b0: 0004 0000 0005 0000 0004 0000 000b 0000  ................
-000001c0: 000a 0000 000d 0000 0012 0000 000c 0000  ................
-000001d0: 000c 0000 0012 0000 0011 0000 0012 0000  ................
-000001e0: 000e 0000 0013 0000 000e 0000 0012 0000  ................
-000001f0: 000d 0000 0009 0000 000d 0000 0008 0000  ................
-00000200: 0009 0000 000e 0000 000d 0000 0009 0000  ................
-00000210: 0002 0000 0003 0000 0002 0000 0009 0000  ................
-00000220: 0008 0000 0004 0000 0009 0000 0003 0000  ................
-00000230: 0009 0000 0004 0000 000a 0000 000f 0000  ................
-00000240: 0014 0000 0013 0000 000e 0000 000f 0000  ................
-00000250: 0013 0000 0014 0000 000f 0000 0015 0000  ................
-00000260: 000f 0000 0010 0000 0015 0000 0009 0000  ................
-00000270: 000f 0000 000e 0000 000f 0000 0009 0000  ................
-00000280: 000a 0000 000b 0000 000f 0000 000a 0000  ................
-00000290: 0010 0000 000f 0000 000b 0000 0094 7494  ..............t.
-000002a0: 628c 096e 6569 6768 626f 7273 9468 1168  b..neighbors.h.h
-000002b0: 144b 0085 9468 1687 9452 9428 4b01 4b1c  .K...h...R.(K.K.
-000002c0: 4b03 8694 681e 8942 5001 0000 0b00 0000  K...h..BP.......
-000002d0: ffff ffff 0100 0000 0000 0000 0500 0000  ................
-000002e0: 0700 0000 0400 0000 ffff ffff 0300 0000  ................
-000002f0: 1100 0000 0600 0000 0200 0000 0500 0000  ................
-00000300: ffff ffff 0200 0000 ffff ffff 0400 0000  ................
-00000310: 0100 0000 0300 0000 0e00 0000 0700 0000  ................
-00000320: 0a00 0000 0100 0000 0600 0000 ffff ffff  ................
-00000330: ffff ffff 0900 0000 1a00 0000 1300 0000  ................
-00000340: 0800 0000 0b00 0000 0700 0000 0d00 0000  ................
-00000350: ffff ffff 0000 0000 0a00 0000 1500 0000  ................
-00000360: ffff ffff 0d00 0000 0a00 0000 0f00 0000  ................
-00000370: 0c00 0000 0600 0000 1100 0000 0f00 0000  ................
-00000380: 0d00 0000 0e00 0000 1800 0000 ffff ffff  ................
-00000390: 1200 0000 1100 0000 0e00 0000 0300 0000  ................
-000003a0: 1000 0000 1000 0000 ffff ffff 1300 0000  ................
-000003b0: 0900 0000 1900 0000 1200 0000 ffff ffff  ................
-000003c0: 1500 0000 1600 0000 1400 0000 0c00 0000  ................
-000003d0: 1800 0000 1700 0000 ffff ffff 1400 0000  ................
-000003e0: ffff ffff 1600 0000 1b00 0000 1500 0000  ................
-000003f0: 0f00 0000 1900 0000 1300 0000 1a00 0000  ................
-00000400: 1800 0000 1900 0000 0900 0000 1b00 0000  ................
-00000410: 1a00 0000 ffff ffff 1700 0000 9474 9462  .............t.b
-00000420: 8c09 6571 7561 7469 6f6e 7394 6811 6814  ..equations.h.h.
-00000430: 4b00 8594 6816 8794 5294 284b 014b 1c4b  K...h...R.(K.K.K
-00000440: 0486 9468 1b8c 0266 3894 8988 8794 5294  ...h...f8.....R.
-00000450: 284b 0368 1f4e 4e4e 4aff ffff ff4a ffff  (K.h.NNNJ....J..
-00000460: ffff 4b00 7494 6289 4280 0300 0053 a8b3  ..K.t.b.B....S..
-00000470: 4d50 78c6 3fbd 52c2 3abb ece4 3f00 5ea5  MPx.?.R.:...?.^.
-00000480: 6dc8 8ce7 bf59 6b06 b36f 5245 c02a 4aba  m....Yk..oRE.*J.
-00000490: 3e9f 1ad6 3f7e f969 9d6e 21e1 3f51 b23f  >...?~.i.n!.?Q.?
-000004a0: 7a6a aae8 bfa6 a95a 7f35 9344 c0cd ecaf  zj.....Z.5.D....
-000004b0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004c0: 1f16 f5e8 bfec e5e7 1629 f743 c0cd ecaf  .........).C....
-000004d0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004e0: 1f16 f5e8 bfec e5e7 1629 f743 c07d 409c  .........).C.}@.
-000004f0: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000500: 011f 90ea bfd6 3798 cb60 c940 c07d 409c  ......7..`.@.}@.
-00000510: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000520: 011f 90ea bfd6 3798 cb60 c940 c044 0f45  ......7..`.@.D.E
-00000530: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000540: a63b 5de7 bff8 e8ec 534a 6a47 c044 0f45  .;].....SJjG.D.E
-00000550: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000560: a63b 5de7 bff8 e8ec 534a 6a47 c022 c659  .;].....SJjG.".Y
-00000570: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-00000580: 6bf7 d0e3 bf02 98b8 5e21 4050 c022 c659  k.......^!@P.".Y
-00000590: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-000005a0: 6bf7 d0e3 bf02 98b8 5e21 4050 c0d0 ab7f  k.......^!@P....
-000005b0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005c0: 4987 a8e5 bfbd 4052 e4ca 804b c0d0 ab7f  I.....@R...K....
-000005d0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005e0: 4987 a8e5 bfbd 4052 e4ca 804b c058 fe98  I.....@R...K.X..
-000005f0: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000600: d76c 7ce4 bf4f 3a98 41a4 9a4e c058 fe98  .l|..O:.A..N.X..
-00000610: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000620: d76c 7ce4 bf4f 3a98 41a4 9a4e c049 3cb0  .l|..O:.A..N.I<.
-00000630: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000640: 9e55 e9e5 bfe4 5a46 9a45 de4a c049 3cb0  .U....ZF.E.J.I<.
-00000650: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000660: 9e55 e9e5 bfe4 5a46 9a45 de4a c0ba 8c7c  .U....ZF.E.J...|
-00000670: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-00000680: 948f 35e7 bf76 4df1 3045 c447 c0ba 8c7c  ..5..vM.0E.G...|
-00000690: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-000006a0: 948f 35e7 bf76 4df1 3045 c447 c036 6eb5  ..5..vM.0E.G.6n.
-000006b0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006c0: bd5e 77e5 bfda 189c f64f fe4b c036 6eb5  .^w......O.K.6n.
-000006d0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006e0: bd5e 77e5 bfda 189c f64f fe4b c0ab 5c88  .^w......O.K..\.
-000006f0: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000700: 82ef 41e3 bf8c 6c96 e3b6 1451 c0ab 5c88  ..A...l....Q..\.
-00000710: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000720: 82ef 41e3 bf8c 6c96 e3b6 1451 c094 32f3  ..A...l....Q..2.
-00000730: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000740: f71b 0ae2 bf08 e69e 8619 0853 c094 32f3  ...........S..2.
-00000750: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000760: f71b 0ae2 bf08 e69e 8619 0853 c028 b95b  ...........S.(.[
-00000770: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-00000780: 6b57 6de4 bfcf 2e5c 6bc4 c44e c028 b95b  kWm....\k..N.(.[
-00000790: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-000007a0: 6b57 6de4 bfcf 2e5c 6bc4 c44e c03c 0a19  kWm....\k..N.<..
-000007b0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007c0: c673 fde2 bf72 990a 512b 7e51 c03c 0a19  .s...r..Q+~Q.<..
-000007d0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007e0: c673 fde2 bf72 990a 512b 7e51 c094 7494  .s...r..Q+~Q..t.
-000007f0: 628c 0863 6f70 6c61 6e61 7294 6811 6814  b..coplanar.h.h.
-00000800: 4b00 8594 6816 8794 5294 284b 014b 004b  K...h...R.(K.K.K
-00000810: 0386 9468 1e89 4300 9474 9462 8c04 676f  ...h..C..t.b..go
-00000820: 6f64 9468 1168 144b 0085 9468 1687 9452  od.h.h.K...h...R
-00000830: 9428 4b01 4b1c 8594 681e 8943 7001 0000  .(K.K...h..Cp...
-00000840: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000850: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000860: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000870: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-000008a0: 0001 0000 0001 0000 0001 0000 0094 7494  ..............t.
-000008b0: 628c 086e 7369 6d70 6c65 7894 4b1c 8c0a  b..nsimplex.K...
-000008c0: 5f74 7261 6e73 666f 726d 944e 8c12 5f76  _transform.N.._v
-000008d0: 6572 7465 785f 746f 5f73 696d 706c 6578  ertex_to_simplex
-000008e0: 944e 8c19 5f76 6572 7465 785f 6e65 6967  .N.._vertex_neig
-000008f0: 6862 6f72 5f76 6572 7469 6365 7394 4e8c  hbor_vertices.N.
-00000900: 095f 7665 7274 6963 6573 9468 188c 075f  ._vertices.h..._
-00000910: 706f 696e 7473 9468 1168 144b 0085 9468  points.h.h.K...h
-00000920: 1687 9452 9428 4b01 4b16 4b02 8694 6831  ...R.(K.K.K...h1
-00000930: 8942 6001 0000 0000 0000 0000 4440 0000  .B`.........D@..
-00000940: 0000 0080 4640 0000 0000 0000 4e40 0000  ....F@......N@..
-00000950: 0000 0080 4640 0000 0000 0000 5440 0000  ....F@......T@..
-00000960: 0000 0080 4640 0000 0000 0000 5940 0000  ....F@......Y@..
-00000970: 0000 0080 4640 0000 0000 0000 5e40 0000  ....F@......^@..
-00000980: 0000 0080 4640 0000 0000 0080 6140 0000  ....F@......a@..
-00000990: 0000 0080 4640 0000 0000 0000 4440 cdcc  ....F@......D@..
-000009a0: cccc ccac 5040 0000 0000 0000 4e40 cdcc  ....P@......N@..
-000009b0: cccc ccac 5040 0000 0000 0000 5440 cdcc  ....P@......T@..
-000009c0: cccc ccac 5040 0000 0000 0000 5940 cdcc  ....P@......Y@..
-000009d0: cccc ccac 5040 0000 0000 0000 5e40 cdcc  ....P@......^@..
-000009e0: cccc ccac 5040 0000 0000 0080 6140 cdcc  ....P@......a@..
-000009f0: cccc ccac 5040 0000 0000 0000 4e40 3333  ....P@......N@33
-00000a00: 3333 3313 5640 0000 0000 0000 5440 3333  333.V@......T@33
-00000a10: 3333 3313 5640 0000 0000 0000 5940 3333  333.V@......Y@33
-00000a20: 3333 3313 5640 0000 0000 0000 5e40 3333  333.V@......^@33
-00000a30: 3333 3313 5640 0000 0000 0080 6140 3333  333.V@......a@33
-00000a40: 3333 3313 5640 0000 0000 0000 4e40 0000  333.V@......N@..
-00000a50: 0000 0080 5b40 0000 0000 0000 5440 0000  ....[@......T@..
-00000a60: 0000 0080 5b40 0000 0000 0000 5940 0000  ....[@......Y@..
-00000a70: 0000 0080 5b40 0000 0000 0000 5e40 0000  ....[@......^@..
-00000a80: 0000 0080 5b40 0000 0000 0080 6140 0000  ....[@......a@..
-00000a90: 0000 0080 5b40 9474 9462 8c04 6e64 696d  ....[@.t.b..ndim
-00000aa0: 944b 028c 076e 706f 696e 7473 944b 168c  .K...npoints.K..
-00000ab0: 096d 696e 5f62 6f75 6e64 9468 1168 144b  .min_bound.h.h.K
-00000ac0: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000ad0: 6831 8943 1000 0000 0000 0044 4000 0000  h1.C.......D@...
-00000ae0: 0000 8046 4094 7494 628c 096d 6178 5f62  ...F@.t.b..max_b
-00000af0: 6f75 6e64 9468 1168 144b 0085 9468 1687  ound.h.h.K...h..
-00000b00: 9452 9428 4b01 4b02 8594 6831 8943 1000  .R.(K.K...h1.C..
-00000b10: 0000 0000 8061 4000 0000 0000 805b 4094  .....a@......[@.
-00000b20: 7494 628c 0d66 7572 7468 6573 745f 7369  t.b..furthest_si
-00000b30: 7465 9489 7562 8c0c 7661 6c75 6573 5f73  te..ub..values_s
-00000b40: 6861 7065 944b 0185 948c 0676 616c 7565  hape.K.....value
-00000b50: 7394 6811 6814 4b00 8594 6816 8794 5294  s.h.h.K...h...R.
-00000b60: 284b 014b 164b 0186 9468 3189 43b0 d7a3  (K.K.K...h1.C...
-00000b70: 703d 0ad7 0140 e17a 14ae 47e1 0440 5c8f  p=...@.z..G..@\.
-00000b80: c2f5 285c 0940 e17a 14ae 47e1 0e40 14ae  ..(\.@.z..G..@..
-00000b90: 47e1 7a14 1340 85eb 51b8 1e85 1840 713d  G.z..@..Q....@q=
-00000ba0: 0ad7 a370 0340 6666 6666 6666 0640 3d0a  ...p.@ffffff.@=.
-00000bb0: d7a3 703d 0a40 1f85 eb51 b81e 1040 0ad7  ..p=.@...Q...@..
-00000bc0: a370 3d0a 1440 52b8 1e85 eb51 1940 3d0a  .p=..@R....Q.@=.
-00000bd0: d7a3 703d 0840 14ae 47e1 7a14 0c40 e17a  ..p=.@..G.z..@.z
-00000be0: 14ae 47e1 1040 6666 6666 6666 1440 b81e  ..G..@ffffff.@..
-00000bf0: 85eb 51b8 1940 0000 0000 0000 0a40 ae47  ..Q..@.......@.G
-00000c00: e17a 14ae 0d40 7b14 ae47 e17a 1140 3d0a  .z...@{..G.z.@=.
-00000c10: d7a3 703d 1540 5c8f c2f5 285c 1a40 9474  ..p=.@\...(\.@.t
-00000c20: 9462 8c0a 6973 5f63 6f6d 706c 6578 9489  .b..is_complex..
-00000c30: 8c0a 6669 6c6c 5f76 616c 7565 9447 7ff8  ..fill_value.G..
-00000c40: 0000 0000 0000 8c05 7363 616c 6594 4e8c  ........scale.N.
-00000c50: 0670 6f69 6e74 7394 684b 7562 2e         .points.hKub.
+00000140: ffff 4b00 7494 6289 42bc 0100 0016 0000  ..K.t.b.B.......
+00000150: 0001 0000 0000 0000 0006 0000 000c 0000  ................
+00000160: 0011 0000 0002 0000 0016 0000 0003 0000  ................
+00000170: 0002 0000 0001 0000 0016 0000 0007 0000  ................
+00000180: 000c 0000 0006 0000 0016 0000 0004 0000  ................
+00000190: 0003 0000 0004 0000 0016 0000 0005 0000  ................
+000001a0: 0014 0000 0018 0000 0015 0000 0018 0000  ................
+000001b0: 0010 0000 0015 0000 000f 0000 0010 0000  ................
+000001c0: 0018 0000 0014 0000 000f 0000 0018 0000  ................
+000001d0: 0010 0000 0017 0000 000b 0000 0017 0000  ................
+000001e0: 000f 0000 000a 0000 000f 0000 0017 0000  ................
+000001f0: 0010 0000 000b 0000 0017 0000 0005 0000  ................
+00000200: 0004 0000 0017 0000 000a 0000 0017 0000  ................
+00000210: 0004 0000 0005 0000 0002 0000 0007 0000  ................
+00000220: 0001 0000 0007 0000 0002 0000 0008 0000  ................
+00000230: 0007 0000 0006 0000 0000 0000 0001 0000  ................
+00000240: 0007 0000 0000 0000 000d 0000 0007 0000  ................
+00000250: 0008 0000 0007 0000 000d 0000 000c 0000  ................
+00000260: 000d 0000 0012 0000 000c 0000 000c 0000  ................
+00000270: 0012 0000 0011 0000 0012 0000 000e 0000  ................
+00000280: 0013 0000 000e 0000 0012 0000 000d 0000  ................
+00000290: 0009 0000 000d 0000 0008 0000 0009 0000  ................
+000002a0: 000e 0000 000d 0000 0002 0000 0009 0000  ................
+000002b0: 0008 0000 0009 0000 0002 0000 0003 0000  ................
+000002c0: 0009 0000 0004 0000 000a 0000 0004 0000  ................
+000002d0: 0009 0000 0003 0000 0009 0000 000f 0000  ................
+000002e0: 000e 0000 000f 0000 0009 0000 000a 0000  ................
+000002f0: 000e 0000 000f 0000 0013 0000 000f 0000  ................
+00000300: 0014 0000 0013 0000 0094 7494 628c 096e  ..........t.b..n
+00000310: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+00000320: 9468 1687 9452 9428 4b01 4b25 4b03 8694  .h...R.(K.K%K...
+00000330: 681e 8942 bc01 0000 1400 0000 ffff ffff  h..B............
+00000340: 0300 0000 1800 0000 ffff ffff 0400 0000  ................
+00000350: 0500 0000 1e00 0000 0300 0000 0000 0000  ................
+00000360: 0200 0000 1100 0000 0100 0000 1300 0000  ................
+00000370: 1600 0000 2000 0000 0200 0000 0600 0000  .... ...........
+00000380: ffff ffff 1000 0000 0500 0000 0800 0000  ................
+00000390: ffff ffff 0a00 0000 ffff ffff 0700 0000  ................
+000003a0: 0900 0000 0800 0000 0a00 0000 0d00 0000  ................
+000003b0: 0900 0000 0700 0000 2400 0000 0e00 0000  ........$.......
+000003c0: ffff ffff 0d00 0000 2200 0000 0f00 0000  ........".......
+000003d0: 0d00 0000 0b00 0000 0900 0000 0c00 0000  ................
+000003e0: 1000 0000 ffff ffff 0b00 0000 0c00 0000  ................
+000003f0: 1f00 0000 1000 0000 0600 0000 0e00 0000  ................
+00000400: 0f00 0000 1400 0000 0300 0000 1200 0000  ................
+00000410: 1d00 0000 1500 0000 1100 0000 ffff ffff  ................
+00000420: 1400 0000 0400 0000 1300 0000 0000 0000  ................
+00000430: 1100 0000 1200 0000 1b00 0000 1600 0000  ................
+00000440: 1700 0000 0400 0000 1500 0000 1800 0000  ................
+00000450: 1600 0000 1a00 0000 ffff ffff 0100 0000  ................
+00000460: 1700 0000 2300 0000 ffff ffff 1a00 0000  ....#...........
+00000470: 1700 0000 1c00 0000 1900 0000 1500 0000  ................
+00000480: 1d00 0000 1c00 0000 1a00 0000 1b00 0000  ................
+00000490: 2100 0000 1b00 0000 1200 0000 1e00 0000  !...............
+000004a0: 0200 0000 2000 0000 1d00 0000 0f00 0000  .... ...........
+000004b0: 2200 0000 2000 0000 1e00 0000 0500 0000  "... ...........
+000004c0: 1f00 0000 2300 0000 1c00 0000 2200 0000  ....#......."...
+000004d0: 1f00 0000 0c00 0000 2100 0000 2400 0000  ........!...$...
+000004e0: 1900 0000 2100 0000 ffff ffff 2300 0000  ....!.......#...
+000004f0: 0a00 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000500: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000510: 5294 284b 014b 254b 0486 9468 1b8c 0266  R.(K.K%K...h...f
+00000520: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000530: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000540: 42a0 0400 006c 9d0b 2029 2fca 3fef f2f5  B....l.. )/.?...
+00000550: a729 b5eb bf94 0759 5302 38dd bf6f 3c2e  .).....YS.8..o<.
+00000560: ba05 c83e 4053 a8b3 4d50 78c6 3fbd 52c2  ...>@S..MPx.?.R.
+00000570: 3abb ece4 3f00 5ea5 6dc8 8ce7 bf59 6b06  :...?.^.m....Yk.
+00000580: b36f 5245 c076 abab 32fd 05e4 3f49 03bf  .oRE.v..2...?I..
+00000590: 7a08 b6b4 bf19 51ac be9d d3e8 bfda 3435  z.....Q.......45
+000005a0: 2c51 bb3d c0cd 41e7 aaec bcdb 3f87 bd0c  ,Q.=..A.....?...
+000005b0: ff18 84e2 bf0c 2c16 65e8 1be6 bf82 c9c9  ......,.e.......
+000005c0: 8db1 e618 402a 4aba 3e9f 1ad6 3f7e f969  ....@*J.>...?~.i
+000005d0: 9d6e 21e1 3f51 b23f 7a6a aae8 bfa6 a95a  .n!.?Q.?zj.....Z
+000005e0: 7f35 9344 c0ac 2dbe c07c f5e5 3fa1 85cd  .5.D..-..|..?...
+000005f0: 1f09 01cb 3ffe 0c91 f4b4 46e6 bfe2 a394  ....?.....F.....
+00000600: 1a07 f549 c026 be92 60ca 8de7 3fd0 aeff  ...I.&..`...?...
+00000610: 9902 19cf 3f6b bf14 a7d8 37e4 bf11 bf51  ....?k....7....Q
+00000620: 02f4 824f c02f b392 2edf b3e4 3f4a 2e8a  ...O./......?J..
+00000630: 6aaa b8e0 3fc4 a1f0 9e4c c5e1 bfac d48d  j...?....L......
+00000640: 1676 8c53 c0c4 c014 b0c6 89e5 3fbc 35e8  .v.S........?.5.
+00000650: f572 70df 3faf 1eea cb19 b1e1 bfd0 7da8  .rp.?.........}.
+00000660: 09e4 ad53 c066 6a97 64b6 b2e5 3feb 87a2  ...S.fj.d...?...
+00000670: ffd6 b9dc 3fe3 a3f2 980c a0e2 bf62 5e51  ....?........b^Q
+00000680: fb3c 2452 c007 8b11 bf0c 41e3 3f19 978d  .<$R......A.?...
+00000690: 4511 fae0 3f1d cbb4 6652 1be3 bf9e ebc7  E...?...fR......
+000006a0: 0725 5751 c009 13e8 3df9 6ae6 3fed 2483  .%WQ....=.j.?.$.
+000006b0: 3f3d 0dda 3f9e 2c27 2964 c1e2 bff2 acb7  ?=..?.,')d......
+000006c0: 00e5 e551 c0af 873e 5392 2be5 3f1d b5c5  ...Q...>S.+.?...
+000006d0: e465 60db 3ff9 5462 e78f b5e3 bf2a 792d  .e`.?.Tb.....*y-
+000006e0: f8f9 7950 c086 3415 5449 00e6 3f7b 4074  ..yP..4.TI..?{@t
+000006f0: 61cf 13db 3fc8 c3d2 17a3 e2e2 bf55 1a4e  a...?........U.N
+00000700: 3c1b b051 c093 6cc4 916a 36e7 3f5f c433  <..Q..l..j6.?_.3
+00000710: 6489 b7d3 3f56 72fe 9f88 b2e3 bf79 3328  d...?Vr......y3(
+00000720: bc79 7150 c0da 9258 75e7 b0e6 3f2d 2b7d  .yqP...Xu...?-+}
+00000730: 6f91 32d4 3f2d 4c72 7371 2de4 bfeb 9fb3  o.2.?-Lrsq-.....
+00000740: d17e 904f c0de 0080 23d7 1fe7 3f1d f11c  .~.O....#...?...
+00000750: 6837 85d3 3fc5 7598 a677 d9e3 bfde 1615  h7..?.u..w......
+00000760: d767 3750 c0cd ecaf a5c0 4fdf 3f08 44ab  .g7P......O.?.D.
+00000770: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+00000780: 1629 f743 c0cd ecaf a5c0 4fdf 3f08 44ab  .).C......O.?.D.
+00000790: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+000007a0: 1629 f743 c07d 409c 2fe2 cdd7 3f44 7c8c  .).C.}@./...?D|.
+000007b0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007c0: cb60 c940 c07d 409c 2fe2 cdd7 3f44 7c8c  .`.@.}@./...?D|.
+000007d0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007e0: cb60 c940 c044 0f45 310f 50dd 3f2d 16fd  .`.@.D.E1.P.?-..
+000007f0: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000800: 534a 6a47 c044 0f45 310f 50dd 3f2d 16fd  SJjG.D.E1.P.?-..
+00000810: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000820: 534a 6a47 c0d0 ab7f 642b 2cdb 3f56 8bd0  SJjG....d+,.?V..
+00000830: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000840: e4ca 804b c0d0 ab7f 642b 2cdb 3f56 8bd0  ...K....d+,.?V..
+00000850: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000860: e4ca 804b c058 fe98 fdc7 85e0 3f79 f9a8  ...K.X......?y..
+00000870: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+00000880: 41a4 9a4e c058 fe98 fdc7 85e0 3f79 f9a8  A..N.X......?y..
+00000890: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+000008a0: 41a4 9a4e c049 3cb0 5517 ace1 3fef 2e5a  A..N.I<.U...?..Z
+000008b0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008c0: 9a45 de4a c049 3cb0 5517 ace1 3fef 2e5a  .E.J.I<.U...?..Z
+000008d0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008e0: 9a45 de4a c0ba 8c7c 990a b8e2 3f5c cd68  .E.J...|....?\.h
+000008f0: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000900: 3045 c447 c0ba 8c7c 990a b8e2 3f5c cd68  0E.G...|....?\.h
+00000910: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000920: 3045 c447 c036 6eb5 7d1a 29e5 3ffc cfb3  0E.G.6n.}.).?...
+00000930: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000940: f64f fe4b c036 6eb5 7d1a 29e5 3ffc cfb3  .O.K.6n.}.).?...
+00000950: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000960: f64f fe4b c028 b95b 1edd 22e4 3fef 8498  .O.K.(.[..".?...
+00000970: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+00000980: 6bc4 c44e c028 b95b 1edd 22e4 3fef 8498  k..N.(.[..".?...
+00000990: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+000009a0: 6bc4 c44e c0ab 5c88 d9b8 fbe2 3fd9 4116  k..N..\.....?.A.
+000009b0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009c0: e3b6 1451 c0ab 5c88 d9b8 fbe2 3fd9 4116  ...Q..\.....?.A.
+000009d0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009e0: e3b6 1451 c094 7494 628c 0863 6f70 6c61  ...Q..t.b..copla
+000009f0: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000a00: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000a10: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000a20: 0085 9468 1687 9452 9428 4b01 4b25 8594  ...h...R.(K.K%..
+00000a30: 681e 8943 9401 0000 0001 0000 0001 0000  h..C............
+00000a40: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a50: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a60: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a70: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a80: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a90: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000aa0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ab0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ac0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+00000ad0: 7369 6d70 6c65 7894 4b25 8c0a 5f74 7261  simplex.K%.._tra
+00000ae0: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000af0: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000b00: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000b10: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000b20: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000b30: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000b40: 9428 4b01 4b19 4b02 8694 6831 8942 9001  .(K.K.K...h1.B..
+00000b50: 0000 0000 0000 0000 4440 0000 0000 0080  ........D@......
+00000b60: 4640 0000 0000 0000 4e40 0000 0000 0080  F@......N@......
+00000b70: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000b80: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+00000b90: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+00000ba0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+00000bb0: 4640 0000 0000 0000 4440 cdcc cccc ccac  F@......D@......
+00000bc0: 5040 0000 0000 0000 4e40 cdcc cccc ccac  P@......N@......
+00000bd0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+00000be0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+00000bf0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000c00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000c10: 5040 0000 0000 0000 4e40 3333 3333 3313  P@......N@33333.
+00000c20: 5640 0000 0000 0000 5440 3333 3333 3313  V@......T@33333.
+00000c30: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000c40: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000c50: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000c60: 5640 0000 0000 0000 4e40 0000 0000 0080  V@......N@......
+00000c70: 5b40 0000 0000 0000 5440 0000 0000 0080  [@......T@......
+00000c80: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000c90: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000ca0: 5b40 0000 0000 0080 6140 0000 0000 0080  [@......a@......
+00000cb0: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000cc0: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000cd0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ce0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000cf0: 076e 706f 696e 7473 944b 198c 096d 696e  .npoints.K...min
+00000d00: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000d10: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000d20: 1000 0000 0000 0044 4000 0000 0000 0041  .......D@......A
+00000d30: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000d40: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000d50: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000d60: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000d70: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000d80: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000d90: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000da0: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000db0: 194b 0186 9468 3189 43c8 d7a3 703d 0ad7  .K...h1.C...p=..
+00000dc0: 0140 e17a 14ae 47e1 0440 5c8f c2f5 285c  .@.z..G..@\...(\
+00000dd0: 0940 e17a 14ae 47e1 0e40 14ae 47e1 7a14  .@.z..G..@..G.z.
+00000de0: 1340 85eb 51b8 1e85 1840 713d 0ad7 a370  .@..Q....@q=...p
+00000df0: 0340 6666 6666 6666 0640 3d0a d7a3 703d  .@ffffff.@=...p=
+00000e00: 0a40 1f85 eb51 b81e 1040 0ad7 a370 3d0a  .@...Q...@...p=.
+00000e10: 1440 52b8 1e85 eb51 1940 3d0a d7a3 703d  .@R....Q.@=...p=
+00000e20: 0840 14ae 47e1 7a14 0c40 e17a 14ae 47e1  .@..G.z..@.z..G.
+00000e30: 1040 6666 6666 6666 1440 b81e 85eb 51b8  .@ffffff.@....Q.
+00000e40: 1940 0000 0000 0000 0a40 ae47 e17a 14ae  .@.......@.G.z..
+00000e50: 0d40 7b14 ae47 e17a 1140 3d0a d7a3 703d  .@{..G.z.@=...p=
+00000e60: 1540 5c8f c2f5 285c 1a40 3333 3333 3333  .@\...(\.@333333
+00000e70: 1340 0000 0000 0000 1440 cdcc cccc cccc  .@.......@......
+00000e80: 1440 9474 9462 8c0a 6973 5f63 6f6d 706c  .@.t.b..is_compl
+00000e90: 6578 9489 8c0a 6669 6c6c 5f76 616c 7565  ex....fill_value
+00000ea0: 9447 7ff8 0000 0000 0000 8c05 7363 616c  .G..........scal
+00000eb0: 6594 4e8c 0670 6f69 6e74 7394 684b 7562  e.N..points.hKub
+00000ec0: 2e                                       .
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,79 @@
-00000000: 8004 95f2 0400 0000 0000 005d 9428 5d94  ...........].(].
+00000000: 8004 95da 0400 0000 0000 005d 9428 5d94  ...........].(].
 00000010: 288c 156e 756d 7079 2e63 6f72 652e 6d75  (..numpy.core.mu
 00000020: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
 00000030: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
 00000040: 7970 6594 9394 8c02 6638 9489 8887 9452  ype.....f8.....R
 00000050: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
 00000060: 4aff ffff ff4b 0074 9462 4308 0000 0000  J....K.t.bC.....
-00000070: 0080 4640 9486 9452 9468 0468 0a43 08cd  ..F@...R.h.h.C..
-00000080: cccc cccc ac50 4094 8694 5294 6804 680a  .....P@...R.h.h.
-00000090: 4308 3333 3333 3313 5640 9486 9452 9468  C.33333.V@...R.h
-000000a0: 0468 0a43 0800 0000 0000 805b 4094 8694  .h.C.......[@...
-000000b0: 5294 655d 9428 5d94 285d 9428 6804 680a  R.e].(].(].(h.h.
-000000c0: 4308 0000 0000 0000 4440 9486 9452 945d  C.......D@...R.]
-000000d0: 9468 0468 0a43 08ec 51b8 1e85 cb46 4094  .h.h.C..Q....F@.
-000000e0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-000000f0: 0000 0000 004e 4094 8694 5294 5d94 6804  .....N@...R.].h.
-00000100: 680a 4308 52b8 1e85 eb31 5040 9486 9452  h.C.R....1P@...R
-00000110: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
-00000120: 0000 5440 9486 9452 945d 9468 0468 0a43  ..T@...R.].h.h.C
-00000130: 080a d7a3 703d 7a55 4094 8694 5294 6165  ....p=zU@...R.ae
-00000140: 5d94 2868 0468 0a43 0800 0000 0000 0059  ].(h.h.C.......Y
-00000150: 4094 8694 5294 5d94 6804 680a 4308 c3f5  @...R.].h.h.C...
-00000160: 285c 8f22 5a40 9486 9452 9461 655d 9428  (\."Z@...R.ae].(
-00000170: 6804 680a 4308 0000 0000 0000 5e40 9486  h.h.C.......^@..
-00000180: 9452 945d 9468 0468 0a43 08f6 285c 8fc2  .R.].h.h.C..(\..
-00000190: 255f 4094 8694 5294 6165 5d94 2868 0468  %_@...R.ae].(h.h
-000001a0: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
-000001b0: 5d94 6804 680a 4308 cdcc cccc cc2c 6240  ].h.h.C......,b@
-000001c0: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
-000001d0: 680a 4308 0000 0000 0000 4440 9486 9452  h.C.......D@...R
-000001e0: 945d 9468 0468 0a43 087b 14ae 47e1 ba47  .].h.h.C.{..G..G
-000001f0: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000200: 0800 0000 0000 004e 4094 8694 5294 5d94  .......N@...R.].
-00000210: 6804 680a 4308 295c 8fc2 f5d8 5040 9486  h.h.C.)\....P@..
-00000220: 9452 9461 655d 9428 6804 680a 4308 0000  .R.ae].(h.h.C...
-00000230: 0000 0000 5440 9486 9452 945d 9468 0468  ....T@...R.].h.h
-00000240: 0a43 08e1 7a14 ae47 a155 4094 8694 5294  .C..z..G.U@...R.
-00000250: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
-00000260: 0059 4094 8694 5294 5d94 6804 680a 4308  .Y@...R.].h.h.C.
-00000270: 9a99 9999 99c9 5a40 9486 9452 9461 655d  ......Z@...R.ae]
-00000280: 9428 6804 680a 4308 0000 0000 0000 5e40  .(h.h.C.......^@
-00000290: 9486 9452 945d 9468 0468 0a43 0885 eb51  ...R.].h.h.C...Q
-000002a0: b81e c55f 4094 8694 5294 6165 5d94 2868  ..._@...R.ae].(h
-000002b0: 0468 0a43 0800 0000 0000 8061 4094 8694  .h.C.......a@...
-000002c0: 5294 5d94 6804 680a 4308 48e1 7a14 ae67  R.].h.h.C.H.z..g
-000002d0: 6240 9486 9452 9461 6565 5d94 285d 9428  b@...R.aee].(].(
-000002e0: 6804 680a 4308 0000 0000 0000 4e40 9486  h.h.C.......N@..
-000002f0: 9452 945d 9468 0468 0a43 088f c2f5 285c  .R.].h.h.C....(\
-00000300: 4f51 4094 8694 5294 6165 5d94 2868 0468  OQ@...R.ae].(h.h
-00000310: 0a43 0800 0000 0000 0054 4094 8694 5294  .C.......T@...R.
-00000320: 5d94 6804 680a 4308 85eb 51b8 1e35 5640  ].h.h.C...Q..5V@
-00000330: 9486 9452 9461 655d 9428 6804 680a 4308  ...R.ae].(h.h.C.
-00000340: 0000 0000 0000 5940 9486 9452 945d 9468  ......Y@...R.].h
-00000350: 0468 0a43 08ae 47e1 7a14 2e5b 4094 8694  .h.C..G.z..[@...
-00000360: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
-00000370: 0000 005e 4094 8694 5294 5d94 6804 680a  ...^@...R.].h.h.
-00000380: 4308 6666 6666 66e6 5f40 9486 9452 9461  C.fffff._@...R.a
-00000390: 655d 9428 6804 680a 4308 0000 0000 0080  e].(h.h.C.......
-000003a0: 6140 9486 9452 945d 9468 0468 0a43 08c3  a@...R.].h.h.C..
-000003b0: f528 5c8f 8a62 4094 8694 5294 6165 655d  .(\..b@...R.aee]
-000003c0: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
-000003d0: 004e 4094 8694 5294 5d94 6804 680a 4308  .N@...R.].h.h.C.
-000003e0: ae47 e17a 14ce 5140 9486 9452 9461 655d  .G.z..Q@...R.ae]
-000003f0: 9428 6804 680a 4308 0000 0000 0000 5440  .(h.h.C.......T@
-00000400: 9486 9452 945d 9468 0468 0a43 081f 85eb  ...R.].h.h.C....
-00000410: 51b8 ae56 4094 8694 5294 6165 5d94 2868  Q..V@...R.ae].(h
-00000420: 0468 0a43 0800 0000 0000 0059 4094 8694  .h.C.......Y@...
-00000430: 5294 5d94 6804 680a 4308 6666 6666 6666  R.].h.h.C.ffffff
-00000440: 5b40 9486 9452 9461 655d 9428 6804 680a  [@...R.ae].(h.h.
-00000450: 4308 0000 0000 0000 5e40 9486 9452 945d  C.......^@...R.]
-00000460: 9468 0468 0a43 08a4 703d 0ad7 4360 4094  .h.h.C..p=..C`@.
-00000470: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-00000480: 0000 0000 8061 4094 8694 5294 5d94 6804  .....a@...R.].h.
-00000490: 680a 4308 3333 3333 33bb 6240 9486 9452  h.C.33333.b@...R
-000004a0: 9461 6565 655d 9428 6804 680a 4308 0000  .aeee].(h.h.C...
-000004b0: 0000 0000 4440 9486 9452 9468 0468 0a43  ....D@...R.h.h.C
-000004c0: 0800 0000 0000 8061 4094 8694 5294 655d  .......a@...R.e]
-000004d0: 9428 4740 36ae 147a e147 ae47 401a 5c28  .(G@6..z.G.G@.\(
-000004e0: f5c2 8f5c 655d 9428 4740 281e b851 eb85  ...\e].(G@(..Q..
-000004f0: 1f47 4018 851e b851 eb85 6565 2e         .G@....Q..ee.
+00000070: 0000 4140 9486 9452 9468 0468 0a43 0800  ..A@...R.h.h.C..
+00000080: 0000 0000 8046 4094 8694 5294 6804 680a  .....F@...R.h.h.
+00000090: 4308 cdcc cccc ccac 5040 9486 9452 9468  C.......P@...R.h
+000000a0: 0468 0a43 0800 0000 0000 0051 4094 8694  .h.C.......Q@...
+000000b0: 5294 6804 680a 4308 3333 3333 3313 5640  R.h.h.C.33333.V@
+000000c0: 9486 9452 9468 0468 0a43 0800 0000 0000  ...R.h.h.C......
+000000d0: c057 4094 8694 5294 6804 680a 4308 0000  .W@...R.h.h.C...
+000000e0: 0000 0080 5b40 9486 9452 9465 5d94 285d  ....[@...R.e].(]
+000000f0: 945d 9428 6804 680a 4308 0000 0000 0040  .].(h.h.C......@
+00000100: 5f40 9486 9452 945d 9468 0468 0a43 0800  _@...R.].h.h.C..
+00000110: 0000 0000 8061 4094 8694 5294 6165 615d  .....a@...R.aea]
+00000120: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
+00000130: 004e 4094 8694 5294 5d94 6804 680a 4308  .N@...R.].h.h.C.
+00000140: cdcc cccc cc8c 5040 9486 9452 9461 655d  ......P@...R.ae]
+00000150: 9428 6804 680a 4308 0000 0000 0000 5440  .(h.h.C.......T@
+00000160: 9486 9452 945d 9468 0468 0a43 080a d7a3  ...R.].h.h.C....
+00000170: 703d 9a55 4094 8694 5294 6165 5d94 2868  p=.U@...R.ae].(h
+00000180: 0468 0a43 0800 0000 0000 0059 4094 8694  .h.C.......Y@...
+00000190: 5294 5d94 6804 680a 4308 0000 0000 0080  R.].h.h.C.......
+000001a0: 5a40 9486 9452 9461 655d 9428 6804 680a  Z@...R.ae].(h.h.
+000001b0: 4308 0000 0000 0000 5e40 9486 9452 945d  C.......^@...R.]
+000001c0: 9468 0468 0a43 0848 e17a 14ae 875f 4094  .h.h.C.H.z..._@.
+000001d0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+000001e0: 0000 0000 8061 4094 8694 5294 5d94 6804  .....a@...R.].h.
+000001f0: 680a 4308 ae47 e17a 143e 6240 9486 9452  h.C..G.z.>b@...R
+00000200: 9461 6565 5d94 285d 9428 6804 680a 4308  .aee].(].(h.h.C.
+00000210: 0000 0000 0000 4e40 9486 9452 945d 9468  ......N@...R.].h
+00000220: 0468 0a43 08ec 51b8 1e85 0b51 4094 8694  .h.C..Q....Q@...
+00000230: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
+00000240: 0000 0054 4094 8694 5294 5d94 6804 680a  ...T@...R.].h.h.
+00000250: 4308 a470 3d0a d7c3 5540 9486 9452 9461  C..p=...U@...R.a
+00000260: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000270: 5940 9486 9452 945d 9468 0468 0a43 085c  Y@...R.].h.h.C.\
+00000280: 8fc2 f528 dc5a 4094 8694 5294 6165 5d94  ...(.Z@...R.ae].
+00000290: 2868 0468 0a43 0800 0000 0000 005e 4094  (h.h.C.......^@.
+000002a0: 8694 5294 5d94 6804 680a 4308 ae47 e17a  ..R.].h.h.C..G.z
+000002b0: 14ce 5f40 9486 9452 9461 655d 9428 6804  .._@...R.ae].(h.
+000002c0: 680a 4308 0000 0000 0080 6140 9486 9452  h.C.......a@...R
+000002d0: 945d 9468 0468 0a43 08c3 f528 5c8f 6a62  .].h.h.C...(\.jb
+000002e0: 4094 8694 5294 6165 655d 945d 9428 6804  @...R.aee].].(h.
+000002f0: 680a 4308 0000 0000 0040 5f40 9486 9452  h.C......@_@...R
+00000300: 945d 9468 0468 0a43 0800 0000 0000 8061  .].h.h.C.......a
+00000310: 4094 8694 5294 6165 615d 9428 5d94 2868  @...R.aea].(].(h
+00000320: 0468 0a43 0800 0000 0000 0054 4094 8694  .h.C.......T@...
+00000330: 5294 5d94 6804 680a 4308 48e1 7a14 ae97  R.].h.h.C.H.z...
+00000340: 5640 9486 9452 9461 655d 9428 6804 680a  V@...R.ae].(h.h.
+00000350: 4308 0000 0000 0000 5940 9486 9452 945d  C.......Y@...R.]
+00000360: 9468 0468 0a43 085c 8fc2 f528 5c5b 4094  .h.h.C.\...(\[@.
+00000370: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+00000380: 0000 0000 005e 4094 8694 5294 5d94 6804  .....^@...R.].h.
+00000390: 680a 4308 f628 5c8f c215 6040 9486 9452  h.C..(\...`@...R
+000003a0: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+000003b0: 0080 6140 9486 9452 945d 9468 0468 0a43  ..a@...R.].h.h.C
+000003c0: 08cd cccc cccc 7462 4094 8694 5294 6165  ......tb@...R.ae
+000003d0: 655d 945d 9428 6804 680a 4308 0000 0000  e].].(h.h.C.....
+000003e0: 0040 5f40 9486 9452 945d 9468 0468 0a43  .@_@...R.].h.h.C
+000003f0: 0800 0000 0000 8061 4094 8694 5294 6165  .......a@...R.ae
+00000400: 615d 9428 5d94 2868 0468 0a43 0800 0000  a].(].(h.h.C....
+00000410: 0000 0054 4094 8694 5294 5d94 6804 680a  ...T@...R.].h.h.
+00000420: 4308 48e1 7a14 ae17 5740 9486 9452 9461  C.H.z...W@...R.a
+00000430: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000440: 5940 9486 9452 945d 9468 0468 0a43 081f  Y@...R.].h.h.C..
+00000450: 85eb 51b8 9e5b 4094 8694 5294 6165 5d94  ..Q..[@...R.ae].
+00000460: 2868 0468 0a43 0800 0000 0000 005e 4094  (h.h.C.......^@.
+00000470: 8694 5294 5d94 6804 680a 4308 48e1 7a14  ..R.].h.h.C.H.z.
+00000480: ae27 6040 9486 9452 9461 6565 655d 9428  .'`@...R.aeee].(
+00000490: 6804 680a 4308 0000 0000 0000 4e40 9486  h.h.C.......N@..
+000004a0: 9452 9468 0468 0a43 0800 0000 0000 8061  .R.h.h.C.......a
+000004b0: 4094 8694 5294 655d 9428 4740 4b86 6666  @...R.e].(G@K.ff
+000004c0: 6666 6647 402a 28f5 c28f 5c29 655d 9428  fffG@*(...\)e].(
+000004d0: 4740 36cc cccc cccc cd47 4025 3333 3333  G@6......G@%3333
+000004e0: 3333 6565 2e                             33ee.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9552 0c00 0000 0000 008c 1a73 6369  ...R.........sci
+00000000: 8004 95b6 0e00 0000 0000 008c 1a73 6369  .............sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,188 +11,227 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 303e 1af4 bbf4 5e8c 0973 696d 706c  G.0>....^..simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 1c4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 254b 0386 9468 128c 0564 7479 7065  .K%K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 4250 0100 0006 0000  ..K.t.b.BP......
-00000150: 000c 0000 0011 0000 0007 0000 000c 0000  ................
-00000160: 0006 0000 0002 0000 0007 0000 0001 0000  ................
-00000170: 0007 0000 0002 0000 0008 0000 0001 0000  ................
-00000180: 0007 0000 0000 0000 0007 0000 0006 0000  ................
-00000190: 0000 0000 000d 0000 0007 0000 0008 0000  ................
-000001a0: 0007 0000 000d 0000 000c 0000 000b 0000  ................
-000001b0: 0004 0000 0005 0000 0004 0000 000b 0000  ................
-000001c0: 000a 0000 000d 0000 0012 0000 000c 0000  ................
-000001d0: 000c 0000 0012 0000 0011 0000 0012 0000  ................
-000001e0: 000e 0000 0013 0000 000e 0000 0012 0000  ................
-000001f0: 000d 0000 0009 0000 000d 0000 0008 0000  ................
-00000200: 0009 0000 000e 0000 000d 0000 0009 0000  ................
-00000210: 0002 0000 0003 0000 0002 0000 0009 0000  ................
-00000220: 0008 0000 0004 0000 0009 0000 0003 0000  ................
-00000230: 0009 0000 0004 0000 000a 0000 000f 0000  ................
-00000240: 0014 0000 0013 0000 000e 0000 000f 0000  ................
-00000250: 0013 0000 0014 0000 000f 0000 0015 0000  ................
-00000260: 000f 0000 0010 0000 0015 0000 0009 0000  ................
-00000270: 000f 0000 000e 0000 000f 0000 0009 0000  ................
-00000280: 000a 0000 000b 0000 000f 0000 000a 0000  ................
-00000290: 0010 0000 000f 0000 000b 0000 0094 7494  ..............t.
-000002a0: 628c 096e 6569 6768 626f 7273 9468 1168  b..neighbors.h.h
-000002b0: 144b 0085 9468 1687 9452 9428 4b01 4b1c  .K...h...R.(K.K.
-000002c0: 4b03 8694 681e 8942 5001 0000 0b00 0000  K...h..BP.......
-000002d0: ffff ffff 0100 0000 0000 0000 0500 0000  ................
-000002e0: 0700 0000 0400 0000 ffff ffff 0300 0000  ................
-000002f0: 1100 0000 0600 0000 0200 0000 0500 0000  ................
-00000300: ffff ffff 0200 0000 ffff ffff 0400 0000  ................
-00000310: 0100 0000 0300 0000 0e00 0000 0700 0000  ................
-00000320: 0a00 0000 0100 0000 0600 0000 ffff ffff  ................
-00000330: ffff ffff 0900 0000 1a00 0000 1300 0000  ................
-00000340: 0800 0000 0b00 0000 0700 0000 0d00 0000  ................
-00000350: ffff ffff 0000 0000 0a00 0000 1500 0000  ................
-00000360: ffff ffff 0d00 0000 0a00 0000 0f00 0000  ................
-00000370: 0c00 0000 0600 0000 1100 0000 0f00 0000  ................
-00000380: 0d00 0000 0e00 0000 1800 0000 ffff ffff  ................
-00000390: 1200 0000 1100 0000 0e00 0000 0300 0000  ................
-000003a0: 1000 0000 1000 0000 ffff ffff 1300 0000  ................
-000003b0: 0900 0000 1900 0000 1200 0000 ffff ffff  ................
-000003c0: 1500 0000 1600 0000 1400 0000 0c00 0000  ................
-000003d0: 1800 0000 1700 0000 ffff ffff 1400 0000  ................
-000003e0: ffff ffff 1600 0000 1b00 0000 1500 0000  ................
-000003f0: 0f00 0000 1900 0000 1300 0000 1a00 0000  ................
-00000400: 1800 0000 1900 0000 0900 0000 1b00 0000  ................
-00000410: 1a00 0000 ffff ffff 1700 0000 9474 9462  .............t.b
-00000420: 8c09 6571 7561 7469 6f6e 7394 6811 6814  ..equations.h.h.
-00000430: 4b00 8594 6816 8794 5294 284b 014b 1c4b  K...h...R.(K.K.K
-00000440: 0486 9468 1b8c 0266 3894 8988 8794 5294  ...h...f8.....R.
-00000450: 284b 0368 1f4e 4e4e 4aff ffff ff4a ffff  (K.h.NNNJ....J..
-00000460: ffff 4b00 7494 6289 4280 0300 0053 a8b3  ..K.t.b.B....S..
-00000470: 4d50 78c6 3fbd 52c2 3abb ece4 3f00 5ea5  MPx.?.R.:...?.^.
-00000480: 6dc8 8ce7 bf59 6b06 b36f 5245 c02a 4aba  m....Yk..oRE.*J.
-00000490: 3e9f 1ad6 3f7e f969 9d6e 21e1 3f51 b23f  >...?~.i.n!.?Q.?
-000004a0: 7a6a aae8 bfa6 a95a 7f35 9344 c0cd ecaf  zj.....Z.5.D....
-000004b0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004c0: 1f16 f5e8 bfec e5e7 1629 f743 c0cd ecaf  .........).C....
-000004d0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004e0: 1f16 f5e8 bfec e5e7 1629 f743 c07d 409c  .........).C.}@.
-000004f0: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000500: 011f 90ea bfd6 3798 cb60 c940 c07d 409c  ......7..`.@.}@.
-00000510: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000520: 011f 90ea bfd6 3798 cb60 c940 c044 0f45  ......7..`.@.D.E
-00000530: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000540: a63b 5de7 bff8 e8ec 534a 6a47 c044 0f45  .;].....SJjG.D.E
-00000550: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000560: a63b 5de7 bff8 e8ec 534a 6a47 c022 c659  .;].....SJjG.".Y
-00000570: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-00000580: 6bf7 d0e3 bf02 98b8 5e21 4050 c022 c659  k.......^!@P.".Y
-00000590: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-000005a0: 6bf7 d0e3 bf02 98b8 5e21 4050 c0d0 ab7f  k.......^!@P....
-000005b0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005c0: 4987 a8e5 bfbd 4052 e4ca 804b c0d0 ab7f  I.....@R...K....
-000005d0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005e0: 4987 a8e5 bfbd 4052 e4ca 804b c058 fe98  I.....@R...K.X..
-000005f0: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000600: d76c 7ce4 bf4f 3a98 41a4 9a4e c058 fe98  .l|..O:.A..N.X..
-00000610: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000620: d76c 7ce4 bf4f 3a98 41a4 9a4e c049 3cb0  .l|..O:.A..N.I<.
-00000630: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000640: 9e55 e9e5 bfe4 5a46 9a45 de4a c049 3cb0  .U....ZF.E.J.I<.
-00000650: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000660: 9e55 e9e5 bfe4 5a46 9a45 de4a c0ba 8c7c  .U....ZF.E.J...|
-00000670: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-00000680: 948f 35e7 bf76 4df1 3045 c447 c0ba 8c7c  ..5..vM.0E.G...|
-00000690: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-000006a0: 948f 35e7 bf76 4df1 3045 c447 c036 6eb5  ..5..vM.0E.G.6n.
-000006b0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006c0: bd5e 77e5 bfda 189c f64f fe4b c036 6eb5  .^w......O.K.6n.
-000006d0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006e0: bd5e 77e5 bfda 189c f64f fe4b c0ab 5c88  .^w......O.K..\.
-000006f0: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000700: 82ef 41e3 bf8c 6c96 e3b6 1451 c0ab 5c88  ..A...l....Q..\.
-00000710: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000720: 82ef 41e3 bf8c 6c96 e3b6 1451 c094 32f3  ..A...l....Q..2.
-00000730: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000740: f71b 0ae2 bf08 e69e 8619 0853 c094 32f3  ...........S..2.
-00000750: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000760: f71b 0ae2 bf08 e69e 8619 0853 c028 b95b  ...........S.(.[
-00000770: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-00000780: 6b57 6de4 bfcf 2e5c 6bc4 c44e c028 b95b  kWm....\k..N.(.[
-00000790: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-000007a0: 6b57 6de4 bfcf 2e5c 6bc4 c44e c03c 0a19  kWm....\k..N.<..
-000007b0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007c0: c673 fde2 bf72 990a 512b 7e51 c03c 0a19  .s...r..Q+~Q.<..
-000007d0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007e0: c673 fde2 bf72 990a 512b 7e51 c094 7494  .s...r..Q+~Q..t.
-000007f0: 628c 0863 6f70 6c61 6e61 7294 6811 6814  b..coplanar.h.h.
-00000800: 4b00 8594 6816 8794 5294 284b 014b 004b  K...h...R.(K.K.K
-00000810: 0386 9468 1e89 4300 9474 9462 8c04 676f  ...h..C..t.b..go
-00000820: 6f64 9468 1168 144b 0085 9468 1687 9452  od.h.h.K...h...R
-00000830: 9428 4b01 4b1c 8594 681e 8943 7001 0000  .(K.K...h..Cp...
-00000840: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000850: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000860: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000870: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-000008a0: 0001 0000 0001 0000 0001 0000 0094 7494  ..............t.
-000008b0: 628c 086e 7369 6d70 6c65 7894 4b1c 8c0a  b..nsimplex.K...
-000008c0: 5f74 7261 6e73 666f 726d 944e 8c12 5f76  _transform.N.._v
-000008d0: 6572 7465 785f 746f 5f73 696d 706c 6578  ertex_to_simplex
-000008e0: 944e 8c19 5f76 6572 7465 785f 6e65 6967  .N.._vertex_neig
-000008f0: 6862 6f72 5f76 6572 7469 6365 7394 4e8c  hbor_vertices.N.
-00000900: 095f 7665 7274 6963 6573 9468 188c 075f  ._vertices.h..._
-00000910: 706f 696e 7473 9468 1168 144b 0085 9468  points.h.h.K...h
-00000920: 1687 9452 9428 4b01 4b16 4b02 8694 6831  ...R.(K.K.K...h1
-00000930: 8942 6001 0000 0000 0000 0000 4440 0000  .B`.........D@..
-00000940: 0000 0080 4640 0000 0000 0000 4e40 0000  ....F@......N@..
-00000950: 0000 0080 4640 0000 0000 0000 5440 0000  ....F@......T@..
-00000960: 0000 0080 4640 0000 0000 0000 5940 0000  ....F@......Y@..
-00000970: 0000 0080 4640 0000 0000 0000 5e40 0000  ....F@......^@..
-00000980: 0000 0080 4640 0000 0000 0080 6140 0000  ....F@......a@..
-00000990: 0000 0080 4640 0000 0000 0000 4440 cdcc  ....F@......D@..
-000009a0: cccc ccac 5040 0000 0000 0000 4e40 cdcc  ....P@......N@..
-000009b0: cccc ccac 5040 0000 0000 0000 5440 cdcc  ....P@......T@..
-000009c0: cccc ccac 5040 0000 0000 0000 5940 cdcc  ....P@......Y@..
-000009d0: cccc ccac 5040 0000 0000 0000 5e40 cdcc  ....P@......^@..
-000009e0: cccc ccac 5040 0000 0000 0080 6140 cdcc  ....P@......a@..
-000009f0: cccc ccac 5040 0000 0000 0000 4e40 3333  ....P@......N@33
-00000a00: 3333 3313 5640 0000 0000 0000 5440 3333  333.V@......T@33
-00000a10: 3333 3313 5640 0000 0000 0000 5940 3333  333.V@......Y@33
-00000a20: 3333 3313 5640 0000 0000 0000 5e40 3333  333.V@......^@33
-00000a30: 3333 3313 5640 0000 0000 0080 6140 3333  333.V@......a@33
-00000a40: 3333 3313 5640 0000 0000 0000 4e40 0000  333.V@......N@..
-00000a50: 0000 0080 5b40 0000 0000 0000 5440 0000  ....[@......T@..
-00000a60: 0000 0080 5b40 0000 0000 0000 5940 0000  ....[@......Y@..
-00000a70: 0000 0080 5b40 0000 0000 0000 5e40 0000  ....[@......^@..
-00000a80: 0000 0080 5b40 0000 0000 0080 6140 0000  ....[@......a@..
-00000a90: 0000 0080 5b40 9474 9462 8c04 6e64 696d  ....[@.t.b..ndim
-00000aa0: 944b 028c 076e 706f 696e 7473 944b 168c  .K...npoints.K..
-00000ab0: 096d 696e 5f62 6f75 6e64 9468 1168 144b  .min_bound.h.h.K
-00000ac0: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000ad0: 6831 8943 1000 0000 0000 0044 4000 0000  h1.C.......D@...
-00000ae0: 0000 8046 4094 7494 628c 096d 6178 5f62  ...F@.t.b..max_b
-00000af0: 6f75 6e64 9468 1168 144b 0085 9468 1687  ound.h.h.K...h..
-00000b00: 9452 9428 4b01 4b02 8594 6831 8943 1000  .R.(K.K...h1.C..
-00000b10: 0000 0000 8061 4000 0000 0000 805b 4094  .....a@......[@.
-00000b20: 7494 628c 0d66 7572 7468 6573 745f 7369  t.b..furthest_si
-00000b30: 7465 9489 7562 8c0c 7661 6c75 6573 5f73  te..ub..values_s
-00000b40: 6861 7065 944b 0185 948c 0676 616c 7565  hape.K.....value
-00000b50: 7394 6811 6814 4b00 8594 6816 8794 5294  s.h.h.K...h...R.
-00000b60: 284b 014b 164b 0186 9468 3189 43b0 85eb  (K.K.K...h1.C...
-00000b70: 51b8 1e85 2940 3d0a d7a3 70bd 2740 0ad7  Q...)@=...p.'@..
-00000b80: a370 3d8a 2a40 e17a 14ae 47e1 2740 52b8  .p=.*@.z..G.'@R.
-00000b90: 1e85 eb51 2940 1f85 eb51 b81e 2840 c3f5  ...Q)@...Q..(@..
-00000ba0: 285c 8f42 3140 52b8 1e85 eb51 3140 a470  (\.B1@R....Q1@.p
-00000bb0: 3d0a d723 3140 cdcc cccc cc8c 3040 295c  =..#1@......0@)\
-00000bc0: 8fc2 f568 3040 8fc2 f528 5c8f 2f40 ae47  ...h0@...(\./@.G
-00000bd0: e17a 14ae 3540 c3f5 285c 8f02 3540 a470  .z..5@..(\..5@.p
-00000be0: 3d0a d763 3440 48e1 7a14 ae07 3440 1f85  =..c4@H.z...4@..
-00000bf0: eb51 b89e 3340 3d0a d7a3 70fd 3940 52b8  .Q..3@=...p.9@R.
-00000c00: 1e85 eb91 3840 0000 0000 0040 3840 713d  ....8@.....@8@q=
-00000c10: 0ad7 a330 3740 ae47 e17a 14ae 3640 9474  ...07@.G.z..6@.t
-00000c20: 9462 8c0a 6973 5f63 6f6d 706c 6578 9489  .b..is_complex..
-00000c30: 8c0a 6669 6c6c 5f76 616c 7565 9447 7ff8  ..fill_value.G..
-00000c40: 0000 0000 0000 8c05 7363 616c 6594 4e8c  ........scale.N.
-00000c50: 0670 6f69 6e74 7394 684b 7562 2e         .points.hKub.
+00000140: ffff 4b00 7494 6289 42bc 0100 0016 0000  ..K.t.b.B.......
+00000150: 0001 0000 0000 0000 0006 0000 000c 0000  ................
+00000160: 0011 0000 0002 0000 0016 0000 0003 0000  ................
+00000170: 0002 0000 0001 0000 0016 0000 0007 0000  ................
+00000180: 000c 0000 0006 0000 0016 0000 0004 0000  ................
+00000190: 0003 0000 0004 0000 0016 0000 0005 0000  ................
+000001a0: 0014 0000 0018 0000 0015 0000 0018 0000  ................
+000001b0: 0010 0000 0015 0000 000f 0000 0010 0000  ................
+000001c0: 0018 0000 0014 0000 000f 0000 0018 0000  ................
+000001d0: 0010 0000 0017 0000 000b 0000 0017 0000  ................
+000001e0: 000f 0000 000a 0000 000f 0000 0017 0000  ................
+000001f0: 0010 0000 000b 0000 0017 0000 0005 0000  ................
+00000200: 0004 0000 0017 0000 000a 0000 0017 0000  ................
+00000210: 0004 0000 0005 0000 0002 0000 0007 0000  ................
+00000220: 0001 0000 0007 0000 0002 0000 0008 0000  ................
+00000230: 0007 0000 0006 0000 0000 0000 0001 0000  ................
+00000240: 0007 0000 0000 0000 000d 0000 0007 0000  ................
+00000250: 0008 0000 0007 0000 000d 0000 000c 0000  ................
+00000260: 000d 0000 0012 0000 000c 0000 000c 0000  ................
+00000270: 0012 0000 0011 0000 0012 0000 000e 0000  ................
+00000280: 0013 0000 000e 0000 0012 0000 000d 0000  ................
+00000290: 0009 0000 000d 0000 0008 0000 0009 0000  ................
+000002a0: 000e 0000 000d 0000 0002 0000 0009 0000  ................
+000002b0: 0008 0000 0009 0000 0002 0000 0003 0000  ................
+000002c0: 0009 0000 0004 0000 000a 0000 0004 0000  ................
+000002d0: 0009 0000 0003 0000 0009 0000 000f 0000  ................
+000002e0: 000e 0000 000f 0000 0009 0000 000a 0000  ................
+000002f0: 000e 0000 000f 0000 0013 0000 000f 0000  ................
+00000300: 0014 0000 0013 0000 0094 7494 628c 096e  ..........t.b..n
+00000310: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+00000320: 9468 1687 9452 9428 4b01 4b25 4b03 8694  .h...R.(K.K%K...
+00000330: 681e 8942 bc01 0000 1400 0000 ffff ffff  h..B............
+00000340: 0300 0000 1800 0000 ffff ffff 0400 0000  ................
+00000350: 0500 0000 1e00 0000 0300 0000 0000 0000  ................
+00000360: 0200 0000 1100 0000 0100 0000 1300 0000  ................
+00000370: 1600 0000 2000 0000 0200 0000 0600 0000  .... ...........
+00000380: ffff ffff 1000 0000 0500 0000 0800 0000  ................
+00000390: ffff ffff 0a00 0000 ffff ffff 0700 0000  ................
+000003a0: 0900 0000 0800 0000 0a00 0000 0d00 0000  ................
+000003b0: 0900 0000 0700 0000 2400 0000 0e00 0000  ........$.......
+000003c0: ffff ffff 0d00 0000 2200 0000 0f00 0000  ........".......
+000003d0: 0d00 0000 0b00 0000 0900 0000 0c00 0000  ................
+000003e0: 1000 0000 ffff ffff 0b00 0000 0c00 0000  ................
+000003f0: 1f00 0000 1000 0000 0600 0000 0e00 0000  ................
+00000400: 0f00 0000 1400 0000 0300 0000 1200 0000  ................
+00000410: 1d00 0000 1500 0000 1100 0000 ffff ffff  ................
+00000420: 1400 0000 0400 0000 1300 0000 0000 0000  ................
+00000430: 1100 0000 1200 0000 1b00 0000 1600 0000  ................
+00000440: 1700 0000 0400 0000 1500 0000 1800 0000  ................
+00000450: 1600 0000 1a00 0000 ffff ffff 0100 0000  ................
+00000460: 1700 0000 2300 0000 ffff ffff 1a00 0000  ....#...........
+00000470: 1700 0000 1c00 0000 1900 0000 1500 0000  ................
+00000480: 1d00 0000 1c00 0000 1a00 0000 1b00 0000  ................
+00000490: 2100 0000 1b00 0000 1200 0000 1e00 0000  !...............
+000004a0: 0200 0000 2000 0000 1d00 0000 0f00 0000  .... ...........
+000004b0: 2200 0000 2000 0000 1e00 0000 0500 0000  "... ...........
+000004c0: 1f00 0000 2300 0000 1c00 0000 2200 0000  ....#......."...
+000004d0: 1f00 0000 0c00 0000 2100 0000 2400 0000  ........!...$...
+000004e0: 1900 0000 2100 0000 ffff ffff 2300 0000  ....!.......#...
+000004f0: 0a00 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000500: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000510: 5294 284b 014b 254b 0486 9468 1b8c 0266  R.(K.K%K...h...f
+00000520: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000530: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000540: 42a0 0400 006c 9d0b 2029 2fca 3fef f2f5  B....l.. )/.?...
+00000550: a729 b5eb bf94 0759 5302 38dd bf6f 3c2e  .).....YS.8..o<.
+00000560: ba05 c83e 4053 a8b3 4d50 78c6 3fbd 52c2  ...>@S..MPx.?.R.
+00000570: 3abb ece4 3f00 5ea5 6dc8 8ce7 bf59 6b06  :...?.^.m....Yk.
+00000580: b36f 5245 c076 abab 32fd 05e4 3f49 03bf  .oRE.v..2...?I..
+00000590: 7a08 b6b4 bf19 51ac be9d d3e8 bfda 3435  z.....Q.......45
+000005a0: 2c51 bb3d c0cd 41e7 aaec bcdb 3f87 bd0c  ,Q.=..A.....?...
+000005b0: ff18 84e2 bf0c 2c16 65e8 1be6 bf82 c9c9  ......,.e.......
+000005c0: 8db1 e618 402a 4aba 3e9f 1ad6 3f7e f969  ....@*J.>...?~.i
+000005d0: 9d6e 21e1 3f51 b23f 7a6a aae8 bfa6 a95a  .n!.?Q.?zj.....Z
+000005e0: 7f35 9344 c0ac 2dbe c07c f5e5 3fa1 85cd  .5.D..-..|..?...
+000005f0: 1f09 01cb 3ffe 0c91 f4b4 46e6 bfe2 a394  ....?.....F.....
+00000600: 1a07 f549 c026 be92 60ca 8de7 3fd0 aeff  ...I.&..`...?...
+00000610: 9902 19cf 3f6b bf14 a7d8 37e4 bf11 bf51  ....?k....7....Q
+00000620: 02f4 824f c02f b392 2edf b3e4 3f4a 2e8a  ...O./......?J..
+00000630: 6aaa b8e0 3fc4 a1f0 9e4c c5e1 bfac d48d  j...?....L......
+00000640: 1676 8c53 c0c4 c014 b0c6 89e5 3fbc 35e8  .v.S........?.5.
+00000650: f572 70df 3faf 1eea cb19 b1e1 bfd0 7da8  .rp.?.........}.
+00000660: 09e4 ad53 c066 6a97 64b6 b2e5 3feb 87a2  ...S.fj.d...?...
+00000670: ffd6 b9dc 3fe3 a3f2 980c a0e2 bf62 5e51  ....?........b^Q
+00000680: fb3c 2452 c007 8b11 bf0c 41e3 3f19 978d  .<$R......A.?...
+00000690: 4511 fae0 3f1d cbb4 6652 1be3 bf9e ebc7  E...?...fR......
+000006a0: 0725 5751 c009 13e8 3df9 6ae6 3fed 2483  .%WQ....=.j.?.$.
+000006b0: 3f3d 0dda 3f9e 2c27 2964 c1e2 bff2 acb7  ?=..?.,')d......
+000006c0: 00e5 e551 c0af 873e 5392 2be5 3f1d b5c5  ...Q...>S.+.?...
+000006d0: e465 60db 3ff9 5462 e78f b5e3 bf2a 792d  .e`.?.Tb.....*y-
+000006e0: f8f9 7950 c086 3415 5449 00e6 3f7b 4074  ..yP..4.TI..?{@t
+000006f0: 61cf 13db 3fc8 c3d2 17a3 e2e2 bf55 1a4e  a...?........U.N
+00000700: 3c1b b051 c093 6cc4 916a 36e7 3f5f c433  <..Q..l..j6.?_.3
+00000710: 6489 b7d3 3f56 72fe 9f88 b2e3 bf79 3328  d...?Vr......y3(
+00000720: bc79 7150 c0da 9258 75e7 b0e6 3f2d 2b7d  .yqP...Xu...?-+}
+00000730: 6f91 32d4 3f2d 4c72 7371 2de4 bfeb 9fb3  o.2.?-Lrsq-.....
+00000740: d17e 904f c0de 0080 23d7 1fe7 3f1d f11c  .~.O....#...?...
+00000750: 6837 85d3 3fc5 7598 a677 d9e3 bfde 1615  h7..?.u..w......
+00000760: d767 3750 c0cd ecaf a5c0 4fdf 3f08 44ab  .g7P......O.?.D.
+00000770: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+00000780: 1629 f743 c0cd ecaf a5c0 4fdf 3f08 44ab  .).C......O.?.D.
+00000790: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+000007a0: 1629 f743 c07d 409c 2fe2 cdd7 3f44 7c8c  .).C.}@./...?D|.
+000007b0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007c0: cb60 c940 c07d 409c 2fe2 cdd7 3f44 7c8c  .`.@.}@./...?D|.
+000007d0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007e0: cb60 c940 c044 0f45 310f 50dd 3f2d 16fd  .`.@.D.E1.P.?-..
+000007f0: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000800: 534a 6a47 c044 0f45 310f 50dd 3f2d 16fd  SJjG.D.E1.P.?-..
+00000810: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000820: 534a 6a47 c0d0 ab7f 642b 2cdb 3f56 8bd0  SJjG....d+,.?V..
+00000830: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000840: e4ca 804b c0d0 ab7f 642b 2cdb 3f56 8bd0  ...K....d+,.?V..
+00000850: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000860: e4ca 804b c058 fe98 fdc7 85e0 3f79 f9a8  ...K.X......?y..
+00000870: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+00000880: 41a4 9a4e c058 fe98 fdc7 85e0 3f79 f9a8  A..N.X......?y..
+00000890: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+000008a0: 41a4 9a4e c049 3cb0 5517 ace1 3fef 2e5a  A..N.I<.U...?..Z
+000008b0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008c0: 9a45 de4a c049 3cb0 5517 ace1 3fef 2e5a  .E.J.I<.U...?..Z
+000008d0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008e0: 9a45 de4a c0ba 8c7c 990a b8e2 3f5c cd68  .E.J...|....?\.h
+000008f0: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000900: 3045 c447 c0ba 8c7c 990a b8e2 3f5c cd68  0E.G...|....?\.h
+00000910: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000920: 3045 c447 c036 6eb5 7d1a 29e5 3ffc cfb3  0E.G.6n.}.).?...
+00000930: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000940: f64f fe4b c036 6eb5 7d1a 29e5 3ffc cfb3  .O.K.6n.}.).?...
+00000950: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000960: f64f fe4b c028 b95b 1edd 22e4 3fef 8498  .O.K.(.[..".?...
+00000970: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+00000980: 6bc4 c44e c028 b95b 1edd 22e4 3fef 8498  k..N.(.[..".?...
+00000990: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+000009a0: 6bc4 c44e c0ab 5c88 d9b8 fbe2 3fd9 4116  k..N..\.....?.A.
+000009b0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009c0: e3b6 1451 c0ab 5c88 d9b8 fbe2 3fd9 4116  ...Q..\.....?.A.
+000009d0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009e0: e3b6 1451 c094 7494 628c 0863 6f70 6c61  ...Q..t.b..copla
+000009f0: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000a00: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000a10: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000a20: 0085 9468 1687 9452 9428 4b01 4b25 8594  ...h...R.(K.K%..
+00000a30: 681e 8943 9401 0000 0001 0000 0001 0000  h..C............
+00000a40: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a50: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a60: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a70: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a80: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a90: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000aa0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ab0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ac0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+00000ad0: 7369 6d70 6c65 7894 4b25 8c0a 5f74 7261  simplex.K%.._tra
+00000ae0: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000af0: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000b00: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000b10: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000b20: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000b30: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000b40: 9428 4b01 4b19 4b02 8694 6831 8942 9001  .(K.K.K...h1.B..
+00000b50: 0000 0000 0000 0000 4440 0000 0000 0080  ........D@......
+00000b60: 4640 0000 0000 0000 4e40 0000 0000 0080  F@......N@......
+00000b70: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000b80: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+00000b90: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+00000ba0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+00000bb0: 4640 0000 0000 0000 4440 cdcc cccc ccac  F@......D@......
+00000bc0: 5040 0000 0000 0000 4e40 cdcc cccc ccac  P@......N@......
+00000bd0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+00000be0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+00000bf0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000c00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000c10: 5040 0000 0000 0000 4e40 3333 3333 3313  P@......N@33333.
+00000c20: 5640 0000 0000 0000 5440 3333 3333 3313  V@......T@33333.
+00000c30: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000c40: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000c50: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000c60: 5640 0000 0000 0000 4e40 0000 0000 0080  V@......N@......
+00000c70: 5b40 0000 0000 0000 5440 0000 0000 0080  [@......T@......
+00000c80: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000c90: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000ca0: 5b40 0000 0000 0080 6140 0000 0000 0080  [@......a@......
+00000cb0: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000cc0: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000cd0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ce0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000cf0: 076e 706f 696e 7473 944b 198c 096d 696e  .npoints.K...min
+00000d00: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000d10: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000d20: 1000 0000 0000 0044 4000 0000 0000 0041  .......D@......A
+00000d30: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000d40: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000d50: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000d60: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000d70: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000d80: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000d90: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000da0: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000db0: 194b 0186 9468 3189 43c8 85eb 51b8 1e85  .K...h1.C...Q...
+00000dc0: 2940 3d0a d7a3 70bd 2740 0ad7 a370 3d8a  )@=...p.'@...p=.
+00000dd0: 2a40 e17a 14ae 47e1 2740 52b8 1e85 eb51  *@.z..G.'@R....Q
+00000de0: 2940 1f85 eb51 b81e 2840 c3f5 285c 8f42  )@...Q..(@..(\.B
+00000df0: 3140 52b8 1e85 eb51 3140 a470 3d0a d723  1@R....Q1@.p=..#
+00000e00: 3140 cdcc cccc cc8c 3040 295c 8fc2 f568  1@......0@)\...h
+00000e10: 3040 8fc2 f528 5c8f 2f40 ae47 e17a 14ae  0@...(\./@.G.z..
+00000e20: 3540 c3f5 285c 8f02 3540 a470 3d0a d763  5@..(\..5@.p=..c
+00000e30: 3440 48e1 7a14 ae07 3440 1f85 eb51 b89e  4@H.z...4@...Q..
+00000e40: 3340 3d0a d7a3 70fd 3940 52b8 1e85 eb91  3@=...p.9@R.....
+00000e50: 3840 0000 0000 0040 3840 713d 0ad7 a330  8@.....@8@q=...0
+00000e60: 3740 ae47 e17a 14ae 3640 3333 3333 3333  7@.G.z..6@333333
+00000e70: 2640 9a99 9999 9919 3040 3333 3333 3333  &@......0@333333
+00000e80: 3340 9474 9462 8c0a 6973 5f63 6f6d 706c  3@.t.b..is_compl
+00000e90: 6578 9489 8c0a 6669 6c6c 5f76 616c 7565  ex....fill_value
+00000ea0: 9447 7ff8 0000 0000 0000 8c05 7363 616c  .G..........scal
+00000eb0: 6594 4e8c 0670 6f69 6e74 7394 684b 7562  e.N..points.hKub
+00000ec0: 2e                                       .
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9552 0c00 0000 0000 008c 1a73 6369  ...R.........sci
+00000000: 8004 95b6 0e00 0000 0000 008c 1a73 6369  .............sci
 00000010: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
 00000020: 6e74 6572 706e 6494 8c14 4c69 6e65 6172  nterpnd...Linear
 00000030: 4e44 496e 7465 7270 6f6c 6174 6f72 9493  NDInterpolator..
 00000040: 9429 8194 7d94 288c 0374 7269 948c 1473  .)..}.(..tri...s
 00000050: 6369 7079 2e73 7061 7469 616c 2e5f 7168  cipy.spatial._qh
 00000060: 756c 6c94 8c08 4465 6c61 756e 6179 9493  ull...Delaunay..
 00000070: 9429 8194 7d94 288c 065f 7168 756c 6c94  .)..}.(.._qhull.
@@ -11,188 +11,227 @@
 000000a0: 6172 6162 6f6c 6f69 645f 7368 6966 7494  araboloid_shift.
 000000b0: 47c0 303e 1af4 bbf4 5e8c 0973 696d 706c  G.0>....^..simpl
 000000c0: 6963 6573 948c 156e 756d 7079 2e63 6f72  ices...numpy.cor
 000000d0: 652e 6d75 6c74 6961 7272 6179 948c 0c5f  e.multiarray..._
 000000e0: 7265 636f 6e73 7472 7563 7494 9394 8c05  reconstruct.....
 000000f0: 6e75 6d70 7994 8c07 6e64 6172 7261 7994  numpy...ndarray.
 00000100: 9394 4b00 8594 4301 6294 8794 5294 284b  ..K...C.b...R.(K
-00000110: 014b 1c4b 0386 9468 128c 0564 7479 7065  .K.K...h...dtype
+00000110: 014b 254b 0386 9468 128c 0564 7479 7065  .K%K...h...dtype
 00000120: 9493 948c 0269 3494 8988 8794 5294 284b  .....i4.....R.(K
 00000130: 038c 013c 944e 4e4e 4aff ffff ff4a ffff  ...<.NNNJ....J..
-00000140: ffff 4b00 7494 6289 4250 0100 0006 0000  ..K.t.b.BP......
-00000150: 000c 0000 0011 0000 0007 0000 000c 0000  ................
-00000160: 0006 0000 0002 0000 0007 0000 0001 0000  ................
-00000170: 0007 0000 0002 0000 0008 0000 0001 0000  ................
-00000180: 0007 0000 0000 0000 0007 0000 0006 0000  ................
-00000190: 0000 0000 000d 0000 0007 0000 0008 0000  ................
-000001a0: 0007 0000 000d 0000 000c 0000 000b 0000  ................
-000001b0: 0004 0000 0005 0000 0004 0000 000b 0000  ................
-000001c0: 000a 0000 000d 0000 0012 0000 000c 0000  ................
-000001d0: 000c 0000 0012 0000 0011 0000 0012 0000  ................
-000001e0: 000e 0000 0013 0000 000e 0000 0012 0000  ................
-000001f0: 000d 0000 0009 0000 000d 0000 0008 0000  ................
-00000200: 0009 0000 000e 0000 000d 0000 0009 0000  ................
-00000210: 0002 0000 0003 0000 0002 0000 0009 0000  ................
-00000220: 0008 0000 0004 0000 0009 0000 0003 0000  ................
-00000230: 0009 0000 0004 0000 000a 0000 000f 0000  ................
-00000240: 0014 0000 0013 0000 000e 0000 000f 0000  ................
-00000250: 0013 0000 0014 0000 000f 0000 0015 0000  ................
-00000260: 000f 0000 0010 0000 0015 0000 0009 0000  ................
-00000270: 000f 0000 000e 0000 000f 0000 0009 0000  ................
-00000280: 000a 0000 000b 0000 000f 0000 000a 0000  ................
-00000290: 0010 0000 000f 0000 000b 0000 0094 7494  ..............t.
-000002a0: 628c 096e 6569 6768 626f 7273 9468 1168  b..neighbors.h.h
-000002b0: 144b 0085 9468 1687 9452 9428 4b01 4b1c  .K...h...R.(K.K.
-000002c0: 4b03 8694 681e 8942 5001 0000 0b00 0000  K...h..BP.......
-000002d0: ffff ffff 0100 0000 0000 0000 0500 0000  ................
-000002e0: 0700 0000 0400 0000 ffff ffff 0300 0000  ................
-000002f0: 1100 0000 0600 0000 0200 0000 0500 0000  ................
-00000300: ffff ffff 0200 0000 ffff ffff 0400 0000  ................
-00000310: 0100 0000 0300 0000 0e00 0000 0700 0000  ................
-00000320: 0a00 0000 0100 0000 0600 0000 ffff ffff  ................
-00000330: ffff ffff 0900 0000 1a00 0000 1300 0000  ................
-00000340: 0800 0000 0b00 0000 0700 0000 0d00 0000  ................
-00000350: ffff ffff 0000 0000 0a00 0000 1500 0000  ................
-00000360: ffff ffff 0d00 0000 0a00 0000 0f00 0000  ................
-00000370: 0c00 0000 0600 0000 1100 0000 0f00 0000  ................
-00000380: 0d00 0000 0e00 0000 1800 0000 ffff ffff  ................
-00000390: 1200 0000 1100 0000 0e00 0000 0300 0000  ................
-000003a0: 1000 0000 1000 0000 ffff ffff 1300 0000  ................
-000003b0: 0900 0000 1900 0000 1200 0000 ffff ffff  ................
-000003c0: 1500 0000 1600 0000 1400 0000 0c00 0000  ................
-000003d0: 1800 0000 1700 0000 ffff ffff 1400 0000  ................
-000003e0: ffff ffff 1600 0000 1b00 0000 1500 0000  ................
-000003f0: 0f00 0000 1900 0000 1300 0000 1a00 0000  ................
-00000400: 1800 0000 1900 0000 0900 0000 1b00 0000  ................
-00000410: 1a00 0000 ffff ffff 1700 0000 9474 9462  .............t.b
-00000420: 8c09 6571 7561 7469 6f6e 7394 6811 6814  ..equations.h.h.
-00000430: 4b00 8594 6816 8794 5294 284b 014b 1c4b  K...h...R.(K.K.K
-00000440: 0486 9468 1b8c 0266 3894 8988 8794 5294  ...h...f8.....R.
-00000450: 284b 0368 1f4e 4e4e 4aff ffff ff4a ffff  (K.h.NNNJ....J..
-00000460: ffff 4b00 7494 6289 4280 0300 0053 a8b3  ..K.t.b.B....S..
-00000470: 4d50 78c6 3fbd 52c2 3abb ece4 3f00 5ea5  MPx.?.R.:...?.^.
-00000480: 6dc8 8ce7 bf59 6b06 b36f 5245 c02a 4aba  m....Yk..oRE.*J.
-00000490: 3e9f 1ad6 3f7e f969 9d6e 21e1 3f51 b23f  >...?~.i.n!.?Q.?
-000004a0: 7a6a aae8 bfa6 a95a 7f35 9344 c0cd ecaf  zj.....Z.5.D....
-000004b0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004c0: 1f16 f5e8 bfec e5e7 1629 f743 c0cd ecaf  .........).C....
-000004d0: a5c0 4fdf 3f08 44ab e76c fbd8 3fac e4c0  ..O.?.D..l..?...
-000004e0: 1f16 f5e8 bfec e5e7 1629 f743 c07d 409c  .........).C.}@.
-000004f0: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000500: 011f 90ea bfd6 3798 cb60 c940 c07d 409c  ......7..`.@.}@.
-00000510: 2fe2 cdd7 3f44 7c8c 2fde 96da 3f46 be49  /...?D|./...?F.I
-00000520: 011f 90ea bfd6 3798 cb60 c940 c044 0f45  ......7..`.@.D.E
-00000530: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000540: a63b 5de7 bff8 e8ec 534a 6a47 c044 0f45  .;].....SJjG.D.E
-00000550: 310f 50dd 3f2d 16fd 6808 3ae0 3f66 36fa  1.P.?-..h.:.?f6.
-00000560: a63b 5de7 bff8 e8ec 534a 6a47 c022 c659  .;].....SJjG.".Y
-00000570: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-00000580: 6bf7 d0e3 bf02 98b8 5e21 4050 c022 c659  k.......^!@P.".Y
-00000590: dcef 15e7 3fa3 41d2 eaff d5d3 3f7e e3ce  ....?.A.....?~..
-000005a0: 6bf7 d0e3 bf02 98b8 5e21 4050 c0d0 ab7f  k.......^!@P....
-000005b0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005c0: 4987 a8e5 bfbd 4052 e4ca 804b c0d0 ab7f  I.....@R...K....
-000005d0: 642b 2cdb 3f56 8bd0 6775 3ee3 3f4f c6ee  d+,.?V..gu>.?O..
-000005e0: 4987 a8e5 bfbd 4052 e4ca 804b c058 fe98  I.....@R...K.X..
-000005f0: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000600: d76c 7ce4 bf4f 3a98 41a4 9a4e c058 fe98  .l|..O:.A..N.X..
-00000610: fdc7 85e0 3f79 f9a8 18cf 33e2 3f6d 1a3b  ....?y....3.?m.;
-00000620: d76c 7ce4 bf4f 3a98 41a4 9a4e c049 3cb0  .l|..O:.A..N.I<.
-00000630: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000640: 9e55 e9e5 bfe4 5a46 9a45 de4a c049 3cb0  .U....ZF.E.J.I<.
-00000650: 5517 ace1 3fef 2e5a 857d 6fde 3f70 9134  U...?..Z.}o.?p.4
-00000660: 9e55 e9e5 bfe4 5a46 9a45 de4a c0ba 8c7c  .U....ZF.E.J...|
-00000670: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-00000680: 948f 35e7 bf76 4df1 3045 c447 c0ba 8c7c  ..5..vM.0E.G...|
-00000690: 990a b8e2 3f5c cd68 b174 3bd7 3f76 798d  ....?\.h.t;.?vy.
-000006a0: 948f 35e7 bf76 4df1 3045 c447 c036 6eb5  ..5..vM.0E.G.6n.
-000006b0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006c0: bd5e 77e5 bfda 189c f64f fe4b c036 6eb5  .^w......O.K.6n.
-000006d0: 7d1a 29e5 3ffc cfb3 85d2 7cd5 3f68 541d  }.).?.....|.?hT.
-000006e0: bd5e 77e5 bfda 189c f64f fe4b c0ab 5c88  .^w......O.K..\.
-000006f0: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000700: 82ef 41e3 bf8c 6c96 e3b6 1451 c0ab 5c88  ..A...l....Q..\.
-00000710: d9b8 fbe2 3fd9 4116 7360 1ce1 3fcd ae93  ....?.A.s`..?...
-00000720: 82ef 41e3 bf8c 6c96 e3b6 1451 c094 32f3  ..A...l....Q..2.
-00000730: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000740: f71b 0ae2 bf08 e69e 8619 0853 c094 32f3  ...........S..2.
-00000750: d108 04e5 3f8e c8ac 964f 07e0 3fa9 ac73  ....?....O..?..s
-00000760: f71b 0ae2 bf08 e69e 8619 0853 c028 b95b  ...........S.(.[
-00000770: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-00000780: 6b57 6de4 bfcf 2e5c 6bc4 c44e c028 b95b  kWm....\k..N.(.[
-00000790: 1edd 22e4 3fef 8498 f0ab 5fdc 3f88 e478  ..".?....._.?..x
-000007a0: 6b57 6de4 bfcf 2e5c 6bc4 c44e c03c 0a19  kWm....\k..N.<..
-000007b0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007c0: c673 fde2 bf72 990a 512b 7e51 c03c 0a19  .s...r..Q+~Q.<..
-000007d0: 9786 1fe6 3f2b 8cb1 51aa 60da 3fe4 4c8d  ....?+..Q.`.?.L.
-000007e0: c673 fde2 bf72 990a 512b 7e51 c094 7494  .s...r..Q+~Q..t.
-000007f0: 628c 0863 6f70 6c61 6e61 7294 6811 6814  b..coplanar.h.h.
-00000800: 4b00 8594 6816 8794 5294 284b 014b 004b  K...h...R.(K.K.K
-00000810: 0386 9468 1e89 4300 9474 9462 8c04 676f  ...h..C..t.b..go
-00000820: 6f64 9468 1168 144b 0085 9468 1687 9452  od.h.h.K...h...R
-00000830: 9428 4b01 4b1c 8594 681e 8943 7001 0000  .(K.K...h..Cp...
-00000840: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000850: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000860: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000870: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000880: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-00000890: 0001 0000 0001 0000 0001 0000 0001 0000  ................
-000008a0: 0001 0000 0001 0000 0001 0000 0094 7494  ..............t.
-000008b0: 628c 086e 7369 6d70 6c65 7894 4b1c 8c0a  b..nsimplex.K...
-000008c0: 5f74 7261 6e73 666f 726d 944e 8c12 5f76  _transform.N.._v
-000008d0: 6572 7465 785f 746f 5f73 696d 706c 6578  ertex_to_simplex
-000008e0: 944e 8c19 5f76 6572 7465 785f 6e65 6967  .N.._vertex_neig
-000008f0: 6862 6f72 5f76 6572 7469 6365 7394 4e8c  hbor_vertices.N.
-00000900: 095f 7665 7274 6963 6573 9468 188c 075f  ._vertices.h..._
-00000910: 706f 696e 7473 9468 1168 144b 0085 9468  points.h.h.K...h
-00000920: 1687 9452 9428 4b01 4b16 4b02 8694 6831  ...R.(K.K.K...h1
-00000930: 8942 6001 0000 0000 0000 0000 4440 0000  .B`.........D@..
-00000940: 0000 0080 4640 0000 0000 0000 4e40 0000  ....F@......N@..
-00000950: 0000 0080 4640 0000 0000 0000 5440 0000  ....F@......T@..
-00000960: 0000 0080 4640 0000 0000 0000 5940 0000  ....F@......Y@..
-00000970: 0000 0080 4640 0000 0000 0000 5e40 0000  ....F@......^@..
-00000980: 0000 0080 4640 0000 0000 0080 6140 0000  ....F@......a@..
-00000990: 0000 0080 4640 0000 0000 0000 4440 cdcc  ....F@......D@..
-000009a0: cccc ccac 5040 0000 0000 0000 4e40 cdcc  ....P@......N@..
-000009b0: cccc ccac 5040 0000 0000 0000 5440 cdcc  ....P@......T@..
-000009c0: cccc ccac 5040 0000 0000 0000 5940 cdcc  ....P@......Y@..
-000009d0: cccc ccac 5040 0000 0000 0000 5e40 cdcc  ....P@......^@..
-000009e0: cccc ccac 5040 0000 0000 0080 6140 cdcc  ....P@......a@..
-000009f0: cccc ccac 5040 0000 0000 0000 4e40 3333  ....P@......N@33
-00000a00: 3333 3313 5640 0000 0000 0000 5440 3333  333.V@......T@33
-00000a10: 3333 3313 5640 0000 0000 0000 5940 3333  333.V@......Y@33
-00000a20: 3333 3313 5640 0000 0000 0000 5e40 3333  333.V@......^@33
-00000a30: 3333 3313 5640 0000 0000 0080 6140 3333  333.V@......a@33
-00000a40: 3333 3313 5640 0000 0000 0000 4e40 0000  333.V@......N@..
-00000a50: 0000 0080 5b40 0000 0000 0000 5440 0000  ....[@......T@..
-00000a60: 0000 0080 5b40 0000 0000 0000 5940 0000  ....[@......Y@..
-00000a70: 0000 0080 5b40 0000 0000 0000 5e40 0000  ....[@......^@..
-00000a80: 0000 0080 5b40 0000 0000 0080 6140 0000  ....[@......a@..
-00000a90: 0000 0080 5b40 9474 9462 8c04 6e64 696d  ....[@.t.b..ndim
-00000aa0: 944b 028c 076e 706f 696e 7473 944b 168c  .K...npoints.K..
-00000ab0: 096d 696e 5f62 6f75 6e64 9468 1168 144b  .min_bound.h.h.K
-00000ac0: 0085 9468 1687 9452 9428 4b01 4b02 8594  ...h...R.(K.K...
-00000ad0: 6831 8943 1000 0000 0000 0044 4000 0000  h1.C.......D@...
-00000ae0: 0000 8046 4094 7494 628c 096d 6178 5f62  ...F@.t.b..max_b
-00000af0: 6f75 6e64 9468 1168 144b 0085 9468 1687  ound.h.h.K...h..
-00000b00: 9452 9428 4b01 4b02 8594 6831 8943 1000  .R.(K.K...h1.C..
-00000b10: 0000 0000 8061 4000 0000 0000 805b 4094  .....a@......[@.
-00000b20: 7494 628c 0d66 7572 7468 6573 745f 7369  t.b..furthest_si
-00000b30: 7465 9489 7562 8c0c 7661 6c75 6573 5f73  te..ub..values_s
-00000b40: 6861 7065 944b 0185 948c 0676 616c 7565  hape.K.....value
-00000b50: 7394 6811 6814 4b00 8594 6816 8794 5294  s.h.h.K...h...R.
-00000b60: 284b 014b 164b 0186 9468 3189 43b0 d7a3  (K.K.K...h1.C...
-00000b70: 703d 0ad7 0140 e17a 14ae 47e1 0440 5c8f  p=...@.z..G..@\.
-00000b80: c2f5 285c 0940 e17a 14ae 47e1 0e40 14ae  ..(\.@.z..G..@..
-00000b90: 47e1 7a14 1340 85eb 51b8 1e85 1840 713d  G.z..@..Q....@q=
-00000ba0: 0ad7 a370 0340 6666 6666 6666 0640 3d0a  ...p.@ffffff.@=.
-00000bb0: d7a3 703d 0a40 1f85 eb51 b81e 1040 0ad7  ..p=.@...Q...@..
-00000bc0: a370 3d0a 1440 52b8 1e85 eb51 1940 3d0a  .p=..@R....Q.@=.
-00000bd0: d7a3 703d 0840 14ae 47e1 7a14 0c40 e17a  ..p=.@..G.z..@.z
-00000be0: 14ae 47e1 1040 6666 6666 6666 1440 b81e  ..G..@ffffff.@..
-00000bf0: 85eb 51b8 1940 0000 0000 0000 0a40 ae47  ..Q..@.......@.G
-00000c00: e17a 14ae 0d40 7b14 ae47 e17a 1140 3d0a  .z...@{..G.z.@=.
-00000c10: d7a3 703d 1540 5c8f c2f5 285c 1a40 9474  ..p=.@\...(\.@.t
-00000c20: 9462 8c0a 6973 5f63 6f6d 706c 6578 9489  .b..is_complex..
-00000c30: 8c0a 6669 6c6c 5f76 616c 7565 9447 7ff8  ..fill_value.G..
-00000c40: 0000 0000 0000 8c05 7363 616c 6594 4e8c  ........scale.N.
-00000c50: 0670 6f69 6e74 7394 684b 7562 2e         .points.hKub.
+00000140: ffff 4b00 7494 6289 42bc 0100 0016 0000  ..K.t.b.B.......
+00000150: 0001 0000 0000 0000 0006 0000 000c 0000  ................
+00000160: 0011 0000 0002 0000 0016 0000 0003 0000  ................
+00000170: 0002 0000 0001 0000 0016 0000 0007 0000  ................
+00000180: 000c 0000 0006 0000 0016 0000 0004 0000  ................
+00000190: 0003 0000 0004 0000 0016 0000 0005 0000  ................
+000001a0: 0014 0000 0018 0000 0015 0000 0018 0000  ................
+000001b0: 0010 0000 0015 0000 000f 0000 0010 0000  ................
+000001c0: 0018 0000 0014 0000 000f 0000 0018 0000  ................
+000001d0: 0010 0000 0017 0000 000b 0000 0017 0000  ................
+000001e0: 000f 0000 000a 0000 000f 0000 0017 0000  ................
+000001f0: 0010 0000 000b 0000 0017 0000 0005 0000  ................
+00000200: 0004 0000 0017 0000 000a 0000 0017 0000  ................
+00000210: 0004 0000 0005 0000 0002 0000 0007 0000  ................
+00000220: 0001 0000 0007 0000 0002 0000 0008 0000  ................
+00000230: 0007 0000 0006 0000 0000 0000 0001 0000  ................
+00000240: 0007 0000 0000 0000 000d 0000 0007 0000  ................
+00000250: 0008 0000 0007 0000 000d 0000 000c 0000  ................
+00000260: 000d 0000 0012 0000 000c 0000 000c 0000  ................
+00000270: 0012 0000 0011 0000 0012 0000 000e 0000  ................
+00000280: 0013 0000 000e 0000 0012 0000 000d 0000  ................
+00000290: 0009 0000 000d 0000 0008 0000 0009 0000  ................
+000002a0: 000e 0000 000d 0000 0002 0000 0009 0000  ................
+000002b0: 0008 0000 0009 0000 0002 0000 0003 0000  ................
+000002c0: 0009 0000 0004 0000 000a 0000 0004 0000  ................
+000002d0: 0009 0000 0003 0000 0009 0000 000f 0000  ................
+000002e0: 000e 0000 000f 0000 0009 0000 000a 0000  ................
+000002f0: 000e 0000 000f 0000 0013 0000 000f 0000  ................
+00000300: 0014 0000 0013 0000 0094 7494 628c 096e  ..........t.b..n
+00000310: 6569 6768 626f 7273 9468 1168 144b 0085  eighbors.h.h.K..
+00000320: 9468 1687 9452 9428 4b01 4b25 4b03 8694  .h...R.(K.K%K...
+00000330: 681e 8942 bc01 0000 1400 0000 ffff ffff  h..B............
+00000340: 0300 0000 1800 0000 ffff ffff 0400 0000  ................
+00000350: 0500 0000 1e00 0000 0300 0000 0000 0000  ................
+00000360: 0200 0000 1100 0000 0100 0000 1300 0000  ................
+00000370: 1600 0000 2000 0000 0200 0000 0600 0000  .... ...........
+00000380: ffff ffff 1000 0000 0500 0000 0800 0000  ................
+00000390: ffff ffff 0a00 0000 ffff ffff 0700 0000  ................
+000003a0: 0900 0000 0800 0000 0a00 0000 0d00 0000  ................
+000003b0: 0900 0000 0700 0000 2400 0000 0e00 0000  ........$.......
+000003c0: ffff ffff 0d00 0000 2200 0000 0f00 0000  ........".......
+000003d0: 0d00 0000 0b00 0000 0900 0000 0c00 0000  ................
+000003e0: 1000 0000 ffff ffff 0b00 0000 0c00 0000  ................
+000003f0: 1f00 0000 1000 0000 0600 0000 0e00 0000  ................
+00000400: 0f00 0000 1400 0000 0300 0000 1200 0000  ................
+00000410: 1d00 0000 1500 0000 1100 0000 ffff ffff  ................
+00000420: 1400 0000 0400 0000 1300 0000 0000 0000  ................
+00000430: 1100 0000 1200 0000 1b00 0000 1600 0000  ................
+00000440: 1700 0000 0400 0000 1500 0000 1800 0000  ................
+00000450: 1600 0000 1a00 0000 ffff ffff 0100 0000  ................
+00000460: 1700 0000 2300 0000 ffff ffff 1a00 0000  ....#...........
+00000470: 1700 0000 1c00 0000 1900 0000 1500 0000  ................
+00000480: 1d00 0000 1c00 0000 1a00 0000 1b00 0000  ................
+00000490: 2100 0000 1b00 0000 1200 0000 1e00 0000  !...............
+000004a0: 0200 0000 2000 0000 1d00 0000 0f00 0000  .... ...........
+000004b0: 2200 0000 2000 0000 1e00 0000 0500 0000  "... ...........
+000004c0: 1f00 0000 2300 0000 1c00 0000 2200 0000  ....#......."...
+000004d0: 1f00 0000 0c00 0000 2100 0000 2400 0000  ........!...$...
+000004e0: 1900 0000 2100 0000 ffff ffff 2300 0000  ....!.......#...
+000004f0: 0a00 0000 9474 9462 8c09 6571 7561 7469  .....t.b..equati
+00000500: 6f6e 7394 6811 6814 4b00 8594 6816 8794  ons.h.h.K...h...
+00000510: 5294 284b 014b 254b 0486 9468 1b8c 0266  R.(K.K%K...h...f
+00000520: 3894 8988 8794 5294 284b 0368 1f4e 4e4e  8.....R.(K.h.NNN
+00000530: 4aff ffff ff4a ffff ffff 4b00 7494 6289  J....J....K.t.b.
+00000540: 42a0 0400 006c 9d0b 2029 2fca 3fef f2f5  B....l.. )/.?...
+00000550: a729 b5eb bf94 0759 5302 38dd bf6f 3c2e  .).....YS.8..o<.
+00000560: ba05 c83e 4053 a8b3 4d50 78c6 3fbd 52c2  ...>@S..MPx.?.R.
+00000570: 3abb ece4 3f00 5ea5 6dc8 8ce7 bf59 6b06  :...?.^.m....Yk.
+00000580: b36f 5245 c076 abab 32fd 05e4 3f49 03bf  .oRE.v..2...?I..
+00000590: 7a08 b6b4 bf19 51ac be9d d3e8 bfda 3435  z.....Q.......45
+000005a0: 2c51 bb3d c0cd 41e7 aaec bcdb 3f87 bd0c  ,Q.=..A.....?...
+000005b0: ff18 84e2 bf0c 2c16 65e8 1be6 bf82 c9c9  ......,.e.......
+000005c0: 8db1 e618 402a 4aba 3e9f 1ad6 3f7e f969  ....@*J.>...?~.i
+000005d0: 9d6e 21e1 3f51 b23f 7a6a aae8 bfa6 a95a  .n!.?Q.?zj.....Z
+000005e0: 7f35 9344 c0ac 2dbe c07c f5e5 3fa1 85cd  .5.D..-..|..?...
+000005f0: 1f09 01cb 3ffe 0c91 f4b4 46e6 bfe2 a394  ....?.....F.....
+00000600: 1a07 f549 c026 be92 60ca 8de7 3fd0 aeff  ...I.&..`...?...
+00000610: 9902 19cf 3f6b bf14 a7d8 37e4 bf11 bf51  ....?k....7....Q
+00000620: 02f4 824f c02f b392 2edf b3e4 3f4a 2e8a  ...O./......?J..
+00000630: 6aaa b8e0 3fc4 a1f0 9e4c c5e1 bfac d48d  j...?....L......
+00000640: 1676 8c53 c0c4 c014 b0c6 89e5 3fbc 35e8  .v.S........?.5.
+00000650: f572 70df 3faf 1eea cb19 b1e1 bfd0 7da8  .rp.?.........}.
+00000660: 09e4 ad53 c066 6a97 64b6 b2e5 3feb 87a2  ...S.fj.d...?...
+00000670: ffd6 b9dc 3fe3 a3f2 980c a0e2 bf62 5e51  ....?........b^Q
+00000680: fb3c 2452 c007 8b11 bf0c 41e3 3f19 978d  .<$R......A.?...
+00000690: 4511 fae0 3f1d cbb4 6652 1be3 bf9e ebc7  E...?...fR......
+000006a0: 0725 5751 c009 13e8 3df9 6ae6 3fed 2483  .%WQ....=.j.?.$.
+000006b0: 3f3d 0dda 3f9e 2c27 2964 c1e2 bff2 acb7  ?=..?.,')d......
+000006c0: 00e5 e551 c0af 873e 5392 2be5 3f1d b5c5  ...Q...>S.+.?...
+000006d0: e465 60db 3ff9 5462 e78f b5e3 bf2a 792d  .e`.?.Tb.....*y-
+000006e0: f8f9 7950 c086 3415 5449 00e6 3f7b 4074  ..yP..4.TI..?{@t
+000006f0: 61cf 13db 3fc8 c3d2 17a3 e2e2 bf55 1a4e  a...?........U.N
+00000700: 3c1b b051 c093 6cc4 916a 36e7 3f5f c433  <..Q..l..j6.?_.3
+00000710: 6489 b7d3 3f56 72fe 9f88 b2e3 bf79 3328  d...?Vr......y3(
+00000720: bc79 7150 c0da 9258 75e7 b0e6 3f2d 2b7d  .yqP...Xu...?-+}
+00000730: 6f91 32d4 3f2d 4c72 7371 2de4 bfeb 9fb3  o.2.?-Lrsq-.....
+00000740: d17e 904f c0de 0080 23d7 1fe7 3f1d f11c  .~.O....#...?...
+00000750: 6837 85d3 3fc5 7598 a677 d9e3 bfde 1615  h7..?.u..w......
+00000760: d767 3750 c0cd ecaf a5c0 4fdf 3f08 44ab  .g7P......O.?.D.
+00000770: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+00000780: 1629 f743 c0cd ecaf a5c0 4fdf 3f08 44ab  .).C......O.?.D.
+00000790: e76c fbd8 3fac e4c0 1f16 f5e8 bfec e5e7  .l..?...........
+000007a0: 1629 f743 c07d 409c 2fe2 cdd7 3f44 7c8c  .).C.}@./...?D|.
+000007b0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007c0: cb60 c940 c07d 409c 2fe2 cdd7 3f44 7c8c  .`.@.}@./...?D|.
+000007d0: 2fde 96da 3f46 be49 011f 90ea bfd6 3798  /...?F.I......7.
+000007e0: cb60 c940 c044 0f45 310f 50dd 3f2d 16fd  .`.@.D.E1.P.?-..
+000007f0: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000800: 534a 6a47 c044 0f45 310f 50dd 3f2d 16fd  SJjG.D.E1.P.?-..
+00000810: 6808 3ae0 3f66 36fa a63b 5de7 bff8 e8ec  h.:.?f6..;].....
+00000820: 534a 6a47 c0d0 ab7f 642b 2cdb 3f56 8bd0  SJjG....d+,.?V..
+00000830: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000840: e4ca 804b c0d0 ab7f 642b 2cdb 3f56 8bd0  ...K....d+,.?V..
+00000850: 6775 3ee3 3f4f c6ee 4987 a8e5 bfbd 4052  gu>.?O..I.....@R
+00000860: e4ca 804b c058 fe98 fdc7 85e0 3f79 f9a8  ...K.X......?y..
+00000870: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+00000880: 41a4 9a4e c058 fe98 fdc7 85e0 3f79 f9a8  A..N.X......?y..
+00000890: 18cf 33e2 3f6d 1a3b d76c 7ce4 bf4f 3a98  ..3.?m.;.l|..O:.
+000008a0: 41a4 9a4e c049 3cb0 5517 ace1 3fef 2e5a  A..N.I<.U...?..Z
+000008b0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008c0: 9a45 de4a c049 3cb0 5517 ace1 3fef 2e5a  .E.J.I<.U...?..Z
+000008d0: 857d 6fde 3f70 9134 9e55 e9e5 bfe4 5a46  .}o.?p.4.U....ZF
+000008e0: 9a45 de4a c0ba 8c7c 990a b8e2 3f5c cd68  .E.J...|....?\.h
+000008f0: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000900: 3045 c447 c0ba 8c7c 990a b8e2 3f5c cd68  0E.G...|....?\.h
+00000910: b174 3bd7 3f76 798d 948f 35e7 bf76 4df1  .t;.?vy...5..vM.
+00000920: 3045 c447 c036 6eb5 7d1a 29e5 3ffc cfb3  0E.G.6n.}.).?...
+00000930: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000940: f64f fe4b c036 6eb5 7d1a 29e5 3ffc cfb3  .O.K.6n.}.).?...
+00000950: 85d2 7cd5 3f68 541d bd5e 77e5 bfda 189c  ..|.?hT..^w.....
+00000960: f64f fe4b c028 b95b 1edd 22e4 3fef 8498  .O.K.(.[..".?...
+00000970: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+00000980: 6bc4 c44e c028 b95b 1edd 22e4 3fef 8498  k..N.(.[..".?...
+00000990: f0ab 5fdc 3f88 e478 6b57 6de4 bfcf 2e5c  .._.?..xkWm....\
+000009a0: 6bc4 c44e c0ab 5c88 d9b8 fbe2 3fd9 4116  k..N..\.....?.A.
+000009b0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009c0: e3b6 1451 c0ab 5c88 d9b8 fbe2 3fd9 4116  ...Q..\.....?.A.
+000009d0: 7360 1ce1 3fcd ae93 82ef 41e3 bf8b 6c96  s`..?.....A...l.
+000009e0: e3b6 1451 c094 7494 628c 0863 6f70 6c61  ...Q..t.b..copla
+000009f0: 6e61 7294 6811 6814 4b00 8594 6816 8794  nar.h.h.K...h...
+00000a00: 5294 284b 014b 004b 0386 9468 1e89 4300  R.(K.K.K...h..C.
+00000a10: 9474 9462 8c04 676f 6f64 9468 1168 144b  .t.b..good.h.h.K
+00000a20: 0085 9468 1687 9452 9428 4b01 4b25 8594  ...h...R.(K.K%..
+00000a30: 681e 8943 9401 0000 0001 0000 0001 0000  h..C............
+00000a40: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a50: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a60: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a70: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a80: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000a90: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000aa0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ab0: 0001 0000 0001 0000 0001 0000 0001 0000  ................
+00000ac0: 0001 0000 0001 0000 0094 7494 628c 086e  ..........t.b..n
+00000ad0: 7369 6d70 6c65 7894 4b25 8c0a 5f74 7261  simplex.K%.._tra
+00000ae0: 6e73 666f 726d 944e 8c12 5f76 6572 7465  nsform.N.._verte
+00000af0: 785f 746f 5f73 696d 706c 6578 944e 8c19  x_to_simplex.N..
+00000b00: 5f76 6572 7465 785f 6e65 6967 6862 6f72  _vertex_neighbor
+00000b10: 5f76 6572 7469 6365 7394 4e8c 095f 7665  _vertices.N.._ve
+00000b20: 7274 6963 6573 9468 188c 075f 706f 696e  rtices.h..._poin
+00000b30: 7473 9468 1168 144b 0085 9468 1687 9452  ts.h.h.K...h...R
+00000b40: 9428 4b01 4b19 4b02 8694 6831 8942 9001  .(K.K.K...h1.B..
+00000b50: 0000 0000 0000 0000 4440 0000 0000 0080  ........D@......
+00000b60: 4640 0000 0000 0000 4e40 0000 0000 0080  F@......N@......
+00000b70: 4640 0000 0000 0000 5440 0000 0000 0080  F@......T@......
+00000b80: 4640 0000 0000 0000 5940 0000 0000 0080  F@......Y@......
+00000b90: 4640 0000 0000 0000 5e40 0000 0000 0080  F@......^@......
+00000ba0: 4640 0000 0000 0080 6140 0000 0000 0080  F@......a@......
+00000bb0: 4640 0000 0000 0000 4440 cdcc cccc ccac  F@......D@......
+00000bc0: 5040 0000 0000 0000 4e40 cdcc cccc ccac  P@......N@......
+00000bd0: 5040 0000 0000 0000 5440 cdcc cccc ccac  P@......T@......
+00000be0: 5040 0000 0000 0000 5940 cdcc cccc ccac  P@......Y@......
+00000bf0: 5040 0000 0000 0000 5e40 cdcc cccc ccac  P@......^@......
+00000c00: 5040 0000 0000 0080 6140 cdcc cccc ccac  P@......a@......
+00000c10: 5040 0000 0000 0000 4e40 3333 3333 3313  P@......N@33333.
+00000c20: 5640 0000 0000 0000 5440 3333 3333 3313  V@......T@33333.
+00000c30: 5640 0000 0000 0000 5940 3333 3333 3313  V@......Y@33333.
+00000c40: 5640 0000 0000 0000 5e40 3333 3333 3313  V@......^@33333.
+00000c50: 5640 0000 0000 0080 6140 3333 3333 3313  V@......a@33333.
+00000c60: 5640 0000 0000 0000 4e40 0000 0000 0080  V@......N@......
+00000c70: 5b40 0000 0000 0000 5440 0000 0000 0080  [@......T@......
+00000c80: 5b40 0000 0000 0000 5940 0000 0000 0080  [@......Y@......
+00000c90: 5b40 0000 0000 0000 5e40 0000 0000 0080  [@......^@......
+00000ca0: 5b40 0000 0000 0080 6140 0000 0000 0080  [@......a@......
+00000cb0: 5b40 0000 0000 0040 5f40 0000 0000 0000  [@.....@_@......
+00000cc0: 4140 0000 0000 0040 5f40 0000 0000 0000  A@.....@_@......
+00000cd0: 5140 0000 0000 0040 5f40 0000 0000 00c0  Q@.....@_@......
+00000ce0: 5740 9474 9462 8c04 6e64 696d 944b 028c  W@.t.b..ndim.K..
+00000cf0: 076e 706f 696e 7473 944b 198c 096d 696e  .npoints.K...min
+00000d00: 5f62 6f75 6e64 9468 1168 144b 0085 9468  _bound.h.h.K...h
+00000d10: 1687 9452 9428 4b01 4b02 8594 6831 8943  ...R.(K.K...h1.C
+00000d20: 1000 0000 0000 0044 4000 0000 0000 0041  .......D@......A
+00000d30: 4094 7494 628c 096d 6178 5f62 6f75 6e64  @.t.b..max_bound
+00000d40: 9468 1168 144b 0085 9468 1687 9452 9428  .h.h.K...h...R.(
+00000d50: 4b01 4b02 8594 6831 8943 1000 0000 0000  K.K...h1.C......
+00000d60: 8061 4000 0000 0000 805b 4094 7494 628c  .a@......[@.t.b.
+00000d70: 0d66 7572 7468 6573 745f 7369 7465 9489  .furthest_site..
+00000d80: 7562 8c0c 7661 6c75 6573 5f73 6861 7065  ub..values_shape
+00000d90: 944b 0185 948c 0676 616c 7565 7394 6811  .K.....values.h.
+00000da0: 6814 4b00 8594 6816 8794 5294 284b 014b  h.K...h...R.(K.K
+00000db0: 194b 0186 9468 3189 43c8 d7a3 703d 0ad7  .K...h1.C...p=..
+00000dc0: 0140 e17a 14ae 47e1 0440 5c8f c2f5 285c  .@.z..G..@\...(\
+00000dd0: 0940 e17a 14ae 47e1 0e40 14ae 47e1 7a14  .@.z..G..@..G.z.
+00000de0: 1340 85eb 51b8 1e85 1840 713d 0ad7 a370  .@..Q....@q=...p
+00000df0: 0340 6666 6666 6666 0640 3d0a d7a3 703d  .@ffffff.@=...p=
+00000e00: 0a40 1f85 eb51 b81e 1040 0ad7 a370 3d0a  .@...Q...@...p=.
+00000e10: 1440 52b8 1e85 eb51 1940 3d0a d7a3 703d  .@R....Q.@=...p=
+00000e20: 0840 14ae 47e1 7a14 0c40 e17a 14ae 47e1  .@..G.z..@.z..G.
+00000e30: 1040 6666 6666 6666 1440 b81e 85eb 51b8  .@ffffff.@....Q.
+00000e40: 1940 0000 0000 0000 0a40 ae47 e17a 14ae  .@.......@.G.z..
+00000e50: 0d40 7b14 ae47 e17a 1140 3d0a d7a3 703d  .@{..G.z.@=...p=
+00000e60: 1540 5c8f c2f5 285c 1a40 3333 3333 3333  .@\...(\.@333333
+00000e70: 1340 0000 0000 0000 1440 cdcc cccc cccc  .@.......@......
+00000e80: 1440 9474 9462 8c0a 6973 5f63 6f6d 706c  .@.t.b..is_compl
+00000e90: 6578 9489 8c0a 6669 6c6c 5f76 616c 7565  ex....fill_value
+00000ea0: 9447 7ff8 0000 0000 0000 8c05 7363 616c  .G..........scal
+00000eb0: 6594 4e8c 0670 6f69 6e74 7394 684b 7562  e.N..points.hKub
+00000ec0: 2e                                       .
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,79 @@
-00000000: 8004 9540 0400 0000 0000 005d 9428 5d94  ...@.......].(].
+00000000: 8004 95da 0400 0000 0000 005d 9428 5d94  ...........].(].
 00000010: 288c 156e 756d 7079 2e63 6f72 652e 6d75  (..numpy.core.mu
 00000020: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
 00000030: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
 00000040: 7970 6594 9394 8c02 6638 9489 8887 9452  ype.....f8.....R
 00000050: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
 00000060: 4aff ffff ff4b 0074 9462 4308 0000 0000  J....K.t.bC.....
-00000070: 0000 3940 9486 9452 9468 0468 0a43 0800  ..9@...R.h.h.C..
-00000080: 0000 0000 8041 4094 8694 5294 6804 680a  .....A@...R.h.h.
-00000090: 4308 0000 0000 0080 4640 9486 9452 9468  C.......F@...R.h
-000000a0: 0468 0a43 0800 0000 0000 804b 4094 8694  .h.C.......K@...
-000000b0: 5294 6804 680a 4308 0000 0000 0040 5040  R.h.h.C......@P@
+00000070: 0000 4140 9486 9452 9468 0468 0a43 0800  ..A@...R.h.h.C..
+00000080: 0000 0000 8046 4094 8694 5294 6804 680a  .....F@...R.h.h.
+00000090: 4308 cdcc cccc ccac 5040 9486 9452 9468  C.......P@...R.h
+000000a0: 0468 0a43 0800 0000 0000 0051 4094 8694  .h.C.......Q@...
+000000b0: 5294 6804 680a 4308 3333 3333 3313 5640  R.h.h.C.33333.V@
 000000c0: 9486 9452 9468 0468 0a43 0800 0000 0000  ...R.h.h.C......
-000000d0: c052 4094 8694 5294 6804 680a 4308 0000  .R@...R.h.h.C...
-000000e0: 0000 0040 5540 9486 9452 9468 0468 0a43  ...@U@...R.h.h.C
-000000f0: 0800 0000 0000 c057 4094 8694 5294 655d  .......W@...R.e]
-00000100: 9428 5d94 285d 9428 6804 680a 4308 0000  .(].(].(h.h.C...
-00000110: 0000 0000 4440 9486 9452 945d 9468 0468  ....D@...R.].h.h
-00000120: 0a43 0800 0000 0000 8061 4094 8694 5294  .C.......a@...R.
-00000130: 6165 5d94 2868 0468 0a43 0800 0000 0000  ae].(h.h.C......
-00000140: 0049 4094 8694 5294 5d94 6804 680a 4308  .I@...R.].h.h.C.
-00000150: 0000 0000 0080 6140 9486 9452 9461 6565  ......a@...R.aee
-00000160: 5d94 285d 9428 6804 680a 4308 0000 0000  ].(].(h.h.C.....
-00000170: 0000 4440 9486 9452 945d 9468 0468 0a43  ..D@...R.].h.h.C
-00000180: 0800 0000 0000 8061 4094 8694 5294 6165  .......a@...R.ae
-00000190: 5d94 2868 0468 0a43 0800 0000 0000 0049  ].(h.h.C.......I
-000001a0: 4094 8694 5294 5d94 6804 680a 4308 0000  @...R.].h.h.C...
-000001b0: 0000 0080 6140 9486 9452 9461 6565 5d94  ....a@...R.aee].
-000001c0: 285d 9428 6804 680a 4308 0000 0000 0000  (].(h.h.C.......
-000001d0: 4440 9486 9452 945d 9468 0468 0a43 0800  D@...R.].h.h.C..
-000001e0: 0000 0000 8061 4094 8694 5294 6165 5d94  .....a@...R.ae].
-000001f0: 2868 0468 0a43 0800 0000 0000 0049 4094  (h.h.C.......I@.
-00000200: 8694 5294 5d94 6804 680a 4308 0000 0000  ..R.].h.h.C.....
-00000210: 0080 6140 9486 9452 9461 6565 5d94 285d  ..a@...R.aee].(]
-00000220: 9428 6804 680a 4308 0000 0000 0000 4440  .(h.h.C.......D@
-00000230: 9486 9452 945d 9468 0468 0a43 0800 0000  ...R.].h.h.C....
-00000240: 0000 8061 4094 8694 5294 6165 5d94 2868  ...a@...R.ae].(h
-00000250: 0468 0a43 0800 0000 0000 0049 4094 8694  .h.C.......I@...
-00000260: 5294 5d94 6804 680a 4308 0000 0000 0080  R.].h.h.C.......
-00000270: 6140 9486 9452 9461 6565 5d94 285d 9428  a@...R.aee].(].(
-00000280: 6804 680a 4308 0000 0000 0000 4440 9486  h.h.C.......D@..
-00000290: 9452 945d 9468 0468 0a43 0800 0000 0000  .R.].h.h.C......
-000002a0: 8061 4094 8694 5294 6165 5d94 2868 0468  .a@...R.ae].(h.h
-000002b0: 0a43 0800 0000 0000 0049 4094 8694 5294  .C.......I@...R.
-000002c0: 5d94 6804 680a 4308 0000 0000 0080 6140  ].h.h.C.......a@
-000002d0: 9486 9452 9461 6565 5d94 285d 9428 6804  ...R.aee].(].(h.
-000002e0: 680a 4308 0000 0000 0000 4440 9486 9452  h.C.......D@...R
-000002f0: 945d 9468 0468 0a43 0800 0000 0000 8061  .].h.h.C.......a
-00000300: 4094 8694 5294 6165 5d94 2868 0468 0a43  @...R.ae].(h.h.C
-00000310: 0800 0000 0000 0049 4094 8694 5294 5d94  .......I@...R.].
-00000320: 6804 680a 4308 0000 0000 0080 6140 9486  h.h.C.......a@..
-00000330: 9452 9461 6565 5d94 285d 9428 6804 680a  .R.aee].(].(h.h.
-00000340: 4308 0000 0000 0000 4440 9486 9452 945d  C.......D@...R.]
-00000350: 9468 0468 0a43 0800 0000 0000 8061 4094  .h.h.C.......a@.
-00000360: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
-00000370: 0000 0000 0049 4094 8694 5294 5d94 6804  .....I@...R.].h.
-00000380: 680a 4308 0000 0000 0080 6140 9486 9452  h.C.......a@...R
-00000390: 9461 6565 5d94 285d 9428 6804 680a 4308  .aee].(].(h.h.C.
-000003a0: 0000 0000 0000 4440 9486 9452 945d 9468  ......D@...R.].h
-000003b0: 0468 0a43 0800 0000 0000 8061 4094 8694  .h.C.......a@...
-000003c0: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
-000003d0: 0000 0049 4094 8694 5294 5d94 6804 680a  ...I@...R.].h.h.
-000003e0: 4308 0000 0000 0080 6140 9486 9452 9461  C.......a@...R.a
-000003f0: 6565 655d 9428 6804 680a 4308 0000 0000  eee].(h.h.C.....
-00000400: 0000 4440 9486 9452 9468 0468 0a43 0800  ..D@...R.h.h.C..
-00000410: 0000 0000 0049 4094 8694 5294 655d 9428  .....I@...R.e].(
-00000420: 4740 3561 19ce 075f 7047 4013 7ae1 47ae  G@5a..._pG@.z.G.
-00000430: 147b 655d 9428 4740 25a9 6bb9 8c7e 2847  .{e].(G@%.k..~(G
-00000440: 4012 47ae 147a e148 6565 2e              @.G..z.Hee.
+000000d0: c057 4094 8694 5294 6804 680a 4308 0000  .W@...R.h.h.C...
+000000e0: 0000 0080 5b40 9486 9452 9465 5d94 285d  ....[@...R.e].(]
+000000f0: 945d 9428 6804 680a 4308 0000 0000 0040  .].(h.h.C......@
+00000100: 5f40 9486 9452 945d 9468 0468 0a43 0800  _@...R.].h.h.C..
+00000110: 0000 0000 8061 4094 8694 5294 6165 615d  .....a@...R.aea]
+00000120: 9428 5d94 2868 0468 0a43 0800 0000 0000  .(].(h.h.C......
+00000130: 004e 4094 8694 5294 5d94 6804 680a 4308  .N@...R.].h.h.C.
+00000140: cdcc cccc cc8c 5040 9486 9452 9461 655d  ......P@...R.ae]
+00000150: 9428 6804 680a 4308 0000 0000 0000 5440  .(h.h.C.......T@
+00000160: 9486 9452 945d 9468 0468 0a43 080a d7a3  ...R.].h.h.C....
+00000170: 703d 9a55 4094 8694 5294 6165 5d94 2868  p=.U@...R.ae].(h
+00000180: 0468 0a43 0800 0000 0000 0059 4094 8694  .h.C.......Y@...
+00000190: 5294 5d94 6804 680a 4308 0000 0000 0080  R.].h.h.C.......
+000001a0: 5a40 9486 9452 9461 655d 9428 6804 680a  Z@...R.ae].(h.h.
+000001b0: 4308 0000 0000 0000 5e40 9486 9452 945d  C.......^@...R.]
+000001c0: 9468 0468 0a43 0848 e17a 14ae 875f 4094  .h.h.C.H.z..._@.
+000001d0: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+000001e0: 0000 0000 8061 4094 8694 5294 5d94 6804  .....a@...R.].h.
+000001f0: 680a 4308 ae47 e17a 143e 6240 9486 9452  h.C..G.z.>b@...R
+00000200: 9461 6565 5d94 285d 9428 6804 680a 4308  .aee].(].(h.h.C.
+00000210: 0000 0000 0000 4e40 9486 9452 945d 9468  ......N@...R.].h
+00000220: 0468 0a43 08ec 51b8 1e85 0b51 4094 8694  .h.C..Q....Q@...
+00000230: 5294 6165 5d94 2868 0468 0a43 0800 0000  R.ae].(h.h.C....
+00000240: 0000 0054 4094 8694 5294 5d94 6804 680a  ...T@...R.].h.h.
+00000250: 4308 a470 3d0a d7c3 5540 9486 9452 9461  C..p=...U@...R.a
+00000260: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000270: 5940 9486 9452 945d 9468 0468 0a43 085c  Y@...R.].h.h.C.\
+00000280: 8fc2 f528 dc5a 4094 8694 5294 6165 5d94  ...(.Z@...R.ae].
+00000290: 2868 0468 0a43 0800 0000 0000 005e 4094  (h.h.C.......^@.
+000002a0: 8694 5294 5d94 6804 680a 4308 ae47 e17a  ..R.].h.h.C..G.z
+000002b0: 14ce 5f40 9486 9452 9461 655d 9428 6804  .._@...R.ae].(h.
+000002c0: 680a 4308 0000 0000 0080 6140 9486 9452  h.C.......a@...R
+000002d0: 945d 9468 0468 0a43 08c3 f528 5c8f 6a62  .].h.h.C...(\.jb
+000002e0: 4094 8694 5294 6165 655d 945d 9428 6804  @...R.aee].].(h.
+000002f0: 680a 4308 0000 0000 0040 5f40 9486 9452  h.C......@_@...R
+00000300: 945d 9468 0468 0a43 0800 0000 0000 8061  .].h.h.C.......a
+00000310: 4094 8694 5294 6165 615d 9428 5d94 2868  @...R.aea].(].(h
+00000320: 0468 0a43 0800 0000 0000 0054 4094 8694  .h.C.......T@...
+00000330: 5294 5d94 6804 680a 4308 48e1 7a14 ae97  R.].h.h.C.H.z...
+00000340: 5640 9486 9452 9461 655d 9428 6804 680a  V@...R.ae].(h.h.
+00000350: 4308 0000 0000 0000 5940 9486 9452 945d  C.......Y@...R.]
+00000360: 9468 0468 0a43 085c 8fc2 f528 5c5b 4094  .h.h.C.\...(\[@.
+00000370: 8694 5294 6165 5d94 2868 0468 0a43 0800  ..R.ae].(h.h.C..
+00000380: 0000 0000 005e 4094 8694 5294 5d94 6804  .....^@...R.].h.
+00000390: 680a 4308 f628 5c8f c215 6040 9486 9452  h.C..(\...`@...R
+000003a0: 9461 655d 9428 6804 680a 4308 0000 0000  .ae].(h.h.C.....
+000003b0: 0080 6140 9486 9452 945d 9468 0468 0a43  ..a@...R.].h.h.C
+000003c0: 08cd cccc cccc 7462 4094 8694 5294 6165  ......tb@...R.ae
+000003d0: 655d 945d 9428 6804 680a 4308 0000 0000  e].].(h.h.C.....
+000003e0: 0040 5f40 9486 9452 945d 9468 0468 0a43  .@_@...R.].h.h.C
+000003f0: 0800 0000 0000 8061 4094 8694 5294 6165  .......a@...R.ae
+00000400: 615d 9428 5d94 2868 0468 0a43 0800 0000  a].(].(h.h.C....
+00000410: 0000 0054 4094 8694 5294 5d94 6804 680a  ...T@...R.].h.h.
+00000420: 4308 48e1 7a14 ae17 5740 9486 9452 9461  C.H.z...W@...R.a
+00000430: 655d 9428 6804 680a 4308 0000 0000 0000  e].(h.h.C.......
+00000440: 5940 9486 9452 945d 9468 0468 0a43 081f  Y@...R.].h.h.C..
+00000450: 85eb 51b8 9e5b 4094 8694 5294 6165 5d94  ..Q..[@...R.ae].
+00000460: 2868 0468 0a43 0800 0000 0000 005e 4094  (h.h.C.......^@.
+00000470: 8694 5294 5d94 6804 680a 4308 48e1 7a14  ..R.].h.h.C.H.z.
+00000480: ae27 6040 9486 9452 9461 6565 655d 9428  .'`@...R.aeee].(
+00000490: 6804 680a 4308 0000 0000 0000 4e40 9486  h.h.C.......N@..
+000004a0: 9452 9468 0468 0a43 0800 0000 0000 8061  .R.h.h.C.......a
+000004b0: 4094 8694 5294 655d 9428 4740 4b86 6666  @...R.e].(G@K.ff
+000004c0: 6666 6647 402a 28f5 c28f 5c29 655d 9428  fffG@*(...\)e].(
+000004d0: 4740 36cc cccc cccc cd47 4025 3333 3333  G@6......G@%3333
+000004e0: 3333 6565 2e                             33ee.
```

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.0/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-1.6.0/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-1.6.0/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/engine/Simulator.py` & `ecoengine-1.6.0/src/ecoengine/engine/Simulator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/engine/SystemCreator.py` & `ecoengine-1.6.0/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/engine/__init__.py` & `ecoengine-1.6.0/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/Building.py` & `ecoengine-1.6.0/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/PrefMapTracker.py` & `ecoengine-1.6.0/src/ecoengine/objects/PrefMapTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/SimulationRun.py` & `ecoengine-1.6.0/src/ecoengine/objects/SimulationRun.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/SystemConfig.py` & `ecoengine-1.6.0/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/UtilityCostTracker.py` & `ecoengine-1.6.0/src/ecoengine/objects/UtilityCostTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/__init__.py` & `ecoengine-1.6.0/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-1.6.0/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/MultiPass.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/MultiPass.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/MultiPassRecirc.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/MultiPassRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/PrimaryWithRecirc.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/PrimaryWithRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine/objects/systems/SwingTankER.py` & `ecoengine-1.6.0/src/ecoengine/objects/systems/SwingTankER.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.5.9/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-1.6.0/src/ecoengine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.5.9
+Version: 1.6.0
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.5.9/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-1.6.0/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

