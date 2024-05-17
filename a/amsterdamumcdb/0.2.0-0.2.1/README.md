# Comparing `tmp/amsterdamumcdb-0.2.0.tar.gz` & `tmp/amsterdamumcdb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amsterdamumcdb-0.2.0.tar", last modified: Wed Nov  2 01:34:44 2022, max compression
+gzip compressed data, was "amsterdamumcdb-0.2.1.tar", last modified: Tue Nov 22 21:26:36 2022, max compression
```

## Comparing `amsterdamumcdb-0.2.0.tar` & `amsterdamumcdb-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,76 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.871914 amsterdamumcdb-0.2.0/
--rw-rw-rw-   0        0        0     1097 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       20 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9114 2022-11-02 01:34:44.872936 amsterdamumcdb-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7880 2022-11-02 01:34:07.000000 amsterdamumcdb-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.807908 amsterdamumcdb-0.2.0/amsterdamumcdb/
--rw-rw-rw-   0        0        0      217 2022-10-30 20:35:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.826911 amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/
--rw-rw-rw-   0        0        0      295 2021-09-27 20:18:07.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      616 2021-09-27 20:18:08.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/dictionary.cpython-38.pyc
--rw-rw-rw-   0        0        0     1576 2021-09-27 20:18:07.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/fluidbalance.cpython-38.pyc
--rw-rw-rw-   0        0        0     4404 2021-09-27 20:18:08.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/plotting.cpython-38.pyc
--rw-rw-rw-   0        0        0      249 2022-04-27 11:43:59.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/amsterdamumcdb.py
--rw-rw-rw-   0        0        0     1794 2022-10-31 00:19:10.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/bigquery.py
--rw-rw-rw-   0        0        0    15675 2022-11-02 01:16:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/cohorts.py
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.828925 amsterdamumcdb-0.2.0/amsterdamumcdb/dictionary/
--rw-rw-rw-   0        0        0  1299133 2022-04-27 11:43:59.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/dictionary/dictionary.csv
--rw-rw-rw-   0        0        0      478 2022-04-27 11:43:59.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/dictionary.py
--rw-rw-rw-   0        0        0     1637 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/fluidbalance.py
--rw-rw-rw-   0        0        0     5500 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/plotting.py
--rw-rw-rw-   0        0        0    19292 2022-11-01 21:59:11.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/scores.py
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.781909 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.856908 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/
--rw-rw-rw-   0        0        0      650 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/bilirubin.sql
--rw-rw-rw-   0        0        0     2497 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/creatinine_acute_kidney_injury_failure.sql
--rw-rw-rw-   0        0        0     3971 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/gcs.sql
--rw-rw-rw-   0        0        0      430 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/heart_rate.sql
--rw-rw-rw-   0        0        0      664 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/hematocrit.sql
--rw-rw-rw-   0        0        0      661 2022-11-01 21:14:57.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/lactate.sql
--rw-rw-rw-   0        0        0      507 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/mean_abp.sql
--rw-rw-rw-   0        0        0      736 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/oxygen_device.sql
--rw-rw-rw-   0        0        0      934 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/pH.sql
--rw-rw-rw-   0        0        0     7079 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/pO2_FiO2_estimated.sql
--rw-rw-rw-   0        0        0     3035 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/pO2_pCO2_FiO2.sql
--rw-rw-rw-   0        0        0      717 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/platelets.sql
--rw-rw-rw-   0        0        0      718 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/potassium.sql
--rw-rw-rw-   0        0        0     2269 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/resp_rate.sql
--rw-rw-rw-   0        0        0      694 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/sodium.sql
--rw-rw-rw-   0        0        0      704 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/temperature.sql
--rw-rw-rw-   0        0        0      706 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/urine_output.sql
--rw-rw-rw-   0        0        0     2643 2022-10-29 12:15:30.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/vasopressors_inotropes.sql
--rw-rw-rw-   0        0        0      649 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/wbc.sql
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.857910 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/diagnosis/
--rw-rw-rw-   0        0        0    19439 2022-10-29 12:15:30.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/diagnosis/reason_for_admission.sql
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.867911 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/
--rw-rw-rw-   0        0        0    14826 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet.sql
--rw-rw-rw-   0        0        0    14825 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet_itemids.sql
--rw-rw-rw-   0        0        0    10597 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_nephrology_flowsheet_itemids.sql
--rw-rw-rw-   0        0        0     1033 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_CPP.sql
--rw-rw-rw-   0        0        0     5440 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_itemids.sql
--rw-rw-rw-   0        0        0    33827 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_respiration_flowsheet_itemids.sql
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.868911 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/functions/
--rw-rw-rw-   0        0        0     1491 2021-09-27 18:57:41.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/functions/get_fluidbalance.sql
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.869912 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/lifesupport/
--rw-rw-rw-   0        0        0     7426 2022-11-02 00:19:34.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql
--rw-rw-rw-   0        0        0     1189 2022-11-01 22:24:15.000000 amsterdamumcdb-0.2.0/amsterdamumcdb/util.py
-drwxrwxrwx   0        0        0        0 2022-11-02 01:34:44.821936 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/
--rw-rw-rw-   0        0        0     9114 2022-11-02 01:34:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2105 2022-11-02 01:34:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 01:34:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-11-02 01:34:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-02 01:34:44.000000 amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-09-27 18:57:42.000000 amsterdamumcdb-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1211 2022-11-02 01:34:44.878912 amsterdamumcdb-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      148 2021-09-27 18:57:42.000000 amsterdamumcdb-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.319785 amsterdamumcdb-0.2.1/
+-rw-rw-rw-   0        0        0     1097 2020-06-03 12:26:46.000000 amsterdamumcdb-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       20 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9114 2022-11-22 21:26:36.319785 amsterdamumcdb-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7880 2022-11-15 22:31:10.000000 amsterdamumcdb-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.233798 amsterdamumcdb-0.2.1/amsterdamumcdb/
+-rw-rw-rw-   0        0        0      217 2022-11-15 22:31:10.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.257785 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/
+-rw-rw-rw-   0        0        0      377 2022-11-16 15:13:42.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1090 2022-11-16 15:13:43.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/bigquery.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15736 2022-11-20 23:56:11.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/cohorts.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1885 2022-11-21 13:52:29.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/connections.cpython-310.pyc
+-rw-rw-rw-   0        0        0      651 2022-11-16 15:13:43.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/dictionary.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1569 2022-11-16 15:13:42.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/fluidbalance.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4423 2022-11-16 15:13:43.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/plotting.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11269 2022-11-21 14:21:19.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/scores.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4106 2022-11-20 23:56:11.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0      249 2022-09-26 20:50:06.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/amsterdamumcdb.py
+-rw-rw-rw-   0        0        0     1794 2022-11-15 22:31:10.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/bigquery.py
+-rw-rw-rw-   0        0        0    21606 2022-11-20 22:54:51.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/cohorts.py
+-rw-rw-rw-   0        0        0     2253 2022-11-20 23:23:57.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/connections.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.259793 amsterdamumcdb-0.2.1/amsterdamumcdb/dictionary/
+-rw-rw-rw-   0        0        0  1299133 2022-09-26 20:50:06.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/dictionary/dictionary.csv
+-rw-rw-rw-   0        0        0      478 2022-09-26 20:50:06.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/dictionary.py
+-rw-rw-rw-   0        0        0     1637 2021-10-31 22:56:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/fluidbalance.py
+-rw-rw-rw-   0        0        0     5500 2021-10-31 22:56:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/plotting.py
+-rw-rw-rw-   0        0        0    24005 2022-11-21 14:20:58.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/scores.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.205786 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.294796 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/
+-rw-rw-rw-   0        0        0      650 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/bilirubin.sql
+-rw-rw-rw-   0        0        0     2497 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/creatinine_acute_kidney_injury_failure.sql
+-rw-rw-rw-   0        0        0     8157 2022-11-19 20:41:04.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/gcs.sql
+-rw-rw-rw-   0        0        0      430 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/heart_rate.sql
+-rw-rw-rw-   0        0        0      664 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/hematocrit.sql
+-rw-rw-rw-   0        0        0      661 2022-11-15 22:31:10.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/lactate.sql
+-rw-rw-rw-   0        0        0      507 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/mean_abp.sql
+-rw-rw-rw-   0        0        0      736 2022-11-18 16:12:08.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/oxygen_device.sql
+-rw-rw-rw-   0        0        0      934 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/pH.sql
+-rw-rw-rw-   0        0        0     9232 2022-11-18 21:50:49.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/pO2_FiO2_estimated.sql
+-rw-rw-rw-   0        0        0     3049 2022-11-18 16:24:23.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/pO2_pCO2_FiO2.sql
+-rw-rw-rw-   0        0        0      717 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/platelets.sql
+-rw-rw-rw-   0        0        0      718 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/potassium.sql
+-rw-rw-rw-   0        0        0     2269 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/resp_rate.sql
+-rw-rw-rw-   0        0        0      694 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/sodium.sql
+-rw-rw-rw-   0        0        0      704 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/temperature.sql
+-rw-rw-rw-   0        0        0      706 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/urine_output.sql
+-rw-rw-rw-   0        0        0     2643 2022-10-17 20:52:48.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/vasopressors_inotropes.sql
+-rw-rw-rw-   0        0        0      649 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/wbc.sql
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.296789 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/diagnosis/
+-rw-rw-rw-   0        0        0    20046 2022-11-20 22:25:10.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/diagnosis/reason_for_admission.sql
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.307788 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/
+-rw-rw-rw-   0        0        0    14826 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet.sql
+-rw-rw-rw-   0        0        0    14825 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet_itemids.sql
+-rw-rw-rw-   0        0        0    10597 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_nephrology_flowsheet_itemids.sql
+-rw-rw-rw-   0        0        0     1033 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_CPP.sql
+-rw-rw-rw-   0        0        0     5440 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_itemids.sql
+-rw-rw-rw-   0        0        0    33827 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_respiration_flowsheet_itemids.sql
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.309790 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/functions/
+-rw-rw-rw-   0        0        0     1491 2021-04-29 13:11:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/functions/get_fluidbalance.sql
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.311788 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/lifesupport/
+-rw-rw-rw-   0        0        0     7426 2022-11-15 22:31:10.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql
+-rw-rw-rw-   0        0        0     5916 2022-11-20 23:34:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb/util.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.242787 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/
+-rw-rw-rw-   0        0        0     9114 2022-11-22 21:26:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2475 2022-11-22 21:26:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-22 21:26:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2022-11-22 21:26:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2022-11-22 21:26:36.000000 amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-29 13:11:37.000000 amsterdamumcdb-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1211 2022-11-22 21:26:36.321785 amsterdamumcdb-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      148 2021-04-29 13:11:37.000000 amsterdamumcdb-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:26:36.318785 amsterdamumcdb-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-16 16:26:23.000000 amsterdamumcdb-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     8073 2022-11-20 22:55:39.000000 amsterdamumcdb-0.2.1/tests/test_cohorts.py
+-rw-rw-rw-   0        0        0     5304 2022-11-20 00:05:18.000000 amsterdamumcdb-0.2.1/tests/test_scores.py
+-rw-rw-rw-   0        0        0     2890 2022-11-17 00:36:17.000000 amsterdamumcdb-0.2.1/tests/test_util.py
```

### Comparing `amsterdamumcdb-0.2.0/LICENSE` & `amsterdamumcdb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/PKG-INFO` & `amsterdamumcdb-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amsterdamumcdb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common functions for data exploration on AmsterdamUMCdb
 Home-page: https://github.com/AmsterdamUMC/AmsterdamUMCdb
 Author: Amsterdam UMC Laboratory for Critical Care Computational Intelligence
 Author-email: p.thoral@amsterdamumc.nl
 Project-URL: Bug Tracker, https://github.com/AmsterdamUMC/AmsterdamUMCdb/issues
 Keywords: AmsterdamUMCdb,Intensive Care unit,Critical Care,Medical,Patient Data
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amsterdamumcdb-0.2.0/README.md` & `amsterdamumcdb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/dictionary.cpython-38.pyc` & `amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/dictionary.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Sep 27 18:57:41 2021 UTC, .py size: 446 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-00000000: 550d 0d0a 0000 0000 2514 5261 be01 0000  U.......%.Ra....
+00000000: 6f0d 0d0a 0000 0000 7e10 3263 de01 0000  o.......~.2c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a03 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6300 0000 0000 0000 0000 0000 0004  .Nc.............
 00000060: 0000 0005 0000 0043 0000 0073 3400 0000  .......C...s4...
 00000070: 7400 6a01 a002 7400 6a01 a003 7404 a101  t.j...t.j...t...
 00000080: a101 7d00 6401 7d01 7400 6a01 a005 7c00  ..}.d.}.t.j...|.
 00000090: 7c01 a102 7d02 7406 a007 7c02 a101 7d03  |...}.t...|...}.
-000000a0: 7c03 5300 2902 7a96 0a20 2020 2047 6574  |.S.).z..    Get
+000000a0: 7c03 5300 2903 7ab6 0a20 2020 2047 6574  |.S.).z..    Get
 000000b0: 7320 6120 6469 6374 696f 6e61 7279 206f  s a dictionary o
 000000c0: 6620 616c 6c20 6974 656d 7320 696e 2041  f all items in A
-000000d0: 6d73 7465 7264 616d 2055 4d43 6462 2c20  msterdam UMCdb, 
-000000e0: 7769 7468 2028 776f 726b 2069 6e20 7072  with (work in pr
-000000f0: 6f67 7265 7373 2920 7472 616e 736c 6174  ogress) translat
-00000100: 6564 0a20 2020 206d 6564 6963 616c 2063  ed.    medical c
-00000110: 6f6e 6365 7074 732e 0a0a 2020 2020 5265  oncepts...    Re
-00000120: 7475 726e 733a 0a20 2020 2020 2020 2064  turns:.        d
-00000130: 6174 6166 7261 6d65 3a0a 2020 2020 7a1b  ataframe:.    z.
-00000140: 2e2f 6469 6374 696f 6e61 7279 2f64 6963  ./dictionary/dic
-00000150: 7469 6f6e 6172 792e 6373 7629 08da 026f  tionary.csv)...o
-00000160: 73da 0470 6174 68da 0764 6972 6e61 6d65  s..path..dirname
-00000170: da07 6162 7370 6174 68da 085f 5f66 696c  ..abspath..__fil
-00000180: 655f 5fda 046a 6f69 6eda 0270 64da 0872  e__..join..pd..r
-00000190: 6561 645f 6373 7629 0472 0400 0000 da08  ead_csv).r......
-000001a0: 6669 6c65 6e61 6d65 5a08 6469 6374 6669  filenameZ.dictfi
-000001b0: 6c65 da0a 6469 6374 696f 6e61 7279 a900  le..dictionary..
-000001c0: 720c 0000 00fa 3564 3a5c 6769 7468 7562  r.....5d:\github
-000001d0: 5c61 6d73 7465 7264 616d 756d 6364 625c  \amsterdamumcdb\
-000001e0: 616d 7374 6572 6461 6d75 6d63 6462 5c64  amsterdamumcdb\d
-000001f0: 6963 7469 6f6e 6172 792e 7079 da0e 6765  ictionary.py..ge
-00000200: 745f 6469 6374 696f 6e61 7279 0500 0000  t_dictionary....
-00000210: 730a 0000 0000 0814 0104 020e 020a 0172  s..............r
-00000220: 0e00 0000 2904 da06 7061 6e64 6173 7208  ....)...pandasr.
-00000230: 0000 0072 0200 0000 720e 0000 0072 0c00  ...r....r....r..
-00000240: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000250: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000260: 0400 0000 0801 0803                      ........
+000000d0: 6d73 7465 7264 616d 554d 4364 6220 7769  msterdamUMCdb wi
+000000e0: 7468 2074 7261 6e73 6c61 7465 6420 6d65  th translated me
+000000f0: 6469 6361 6c20 636f 6e63 6570 7473 206d  dical concepts m
+00000100: 6170 7065 6420 746f 204c 4f49 4e43 2c20  apped to LOINC, 
+00000110: 534e 4f4d 4544 2043 540a 2020 2020 6f72  SNOMED CT.    or
+00000120: 2041 5443 2028 776f 726b 2069 6e20 7072   ATC (work in pr
+00000130: 6f67 7265 7373 292e 0a0a 2020 2020 5265  ogress)...    Re
+00000140: 7475 726e 733a 0a20 2020 2020 2020 2064  turns:.        d
+00000150: 6174 6166 7261 6d65 3a0a 2020 2020 7a1b  ataframe:.    z.
+00000160: 2e2f 6469 6374 696f 6e61 7279 2f64 6963  ./dictionary/dic
+00000170: 7469 6f6e 6172 792e 6373 764e 2908 da02  tionary.csvN)...
+00000180: 6f73 da04 7061 7468 da07 6469 726e 616d  os..path..dirnam
+00000190: 65da 0761 6273 7061 7468 da08 5f5f 6669  e..abspath..__fi
+000001a0: 6c65 5f5f da04 6a6f 696e da02 7064 da08  le__..join..pd..
+000001b0: 7265 6164 5f63 7376 2904 7204 0000 00da  read_csv).r.....
+000001c0: 0866 696c 656e 616d 655a 0864 6963 7466  .filenameZ.dictf
+000001d0: 696c 65da 0a64 6963 7469 6f6e 6172 79a9  ile..dictionary.
+000001e0: 0072 0c00 0000 fa35 433a 5c47 6974 4875  .r.....5C:\GitHu
+000001f0: 625c 416d 7374 6572 6461 6d55 4d43 6462  b\AmsterdamUMCdb
+00000200: 5c61 6d73 7465 7264 616d 756d 6364 625c  \amsterdamumcdb\
+00000210: 6469 6374 696f 6e61 7279 2e70 79da 0e67  dictionary.py..g
+00000220: 6574 5f64 6963 7469 6f6e 6172 7905 0000  et_dictionary...
+00000230: 0073 0a00 0000 1408 0401 0e02 0a02 0401  .s..............
+00000240: 720e 0000 0029 04da 0670 616e 6461 7372  r....)...pandasr
+00000250: 0800 0000 7202 0000 0072 0e00 0000 720c  ....r....r....r.
+00000260: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000270: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000280: 7306 0000 0008 0008 010c 03              s..........
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/fluidbalance.cpython-38.pyc` & `amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/fluidbalance.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Sep 27 18:57:41 2021 UTC, .py size: 1637 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-00000000: 550d 0d0a 0000 0000 2514 5261 6506 0000  U.......%.Rae...
+00000000: 6f0d 0d0a 0000 0000 241f 7f61 6506 0000  o.......$..ae...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c04 5a04 6501 6a05 6402 9c01 6403  d.l.Z.e.j.d...d.
+00000040: 6401 6c04 5a04 6402 6501 6a05 6602 6403  d.l.Z.d.e.j.f.d.
 00000050: 6404 8404 5a06 6401 5300 2905 e900 0000  d...Z.d.S.).....
-00000060: 004e 2901 da06 7265 7475 726e 6304 0000  .N)...returnc...
-00000070: 0000 0000 0000 0000 000a 0000 0008 0000  ................
-00000080: 0043 0000 0073 0001 0000 7a0e 7400 a001  .C...s....z.t...
-00000090: 7c00 a101 7d00 5700 6e20 0400 7402 6b0a  |...}.W.n ..t.k.
-000000a0: 722e 0100 0100 0100 7403 6401 7c00 1600  r.......t.d.|...
-000000b0: 8301 8201 5900 6e02 5800 7a0e 7400 a001  ....Y.n.X.z.t...
-000000c0: 7c01 a101 7d01 5700 6e20 0400 7402 6b0a  |...}.W.n ..t.k.
-000000d0: 725e 0100 0100 0100 7403 6402 7c01 1600  r^......t.d.|...
-000000e0: 8301 8201 5900 6e02 5800 7a0e 7400 a001  ....Y.n.X.z.t...
-000000f0: 7c02 a101 7d02 5700 6e20 0400 7402 6b0a  |...}.W.n ..t.k.
-00000100: 728e 0100 0100 0100 7403 6403 7c02 1600  r.......t.d.|...
-00000110: 8301 8201 5900 6e02 5800 7404 6a05 a006  ....Y.n.X.t.j...
-00000120: 7404 6a05 a007 7408 a101 a101 7d04 6404  t.j...t.....}.d.
-00000130: 7d05 7404 6a05 a009 7c04 7c05 a102 7d06  }.t.j...|.|...}.
-00000140: 740a 7c06 6405 8302 7d07 7c07 a00b a100  t.|.d...}.|.....
-00000150: 6a0c 7c00 7c01 7c02 6406 8d03 7d08 740d  j.|.|.|.d...}.t.
-00000160: 7c03 8301 740e 6b08 72f0 740f 6a10 7c08  |...t.k.r.t.j.|.
-00000170: 7c03 6407 8d02 7d09 6e0c 740f a011 7c08  |.d...}.n.t...|.
-00000180: 7c03 a102 7d09 7c09 5300 2908 6121 0200  |...}.|.S.).a!..
-00000190: 0043 616c 6375 6c61 7465 2074 6865 2066  .Calculate the f
-000001a0: 6c75 6964 2062 616c 616e 6365 2028 692e  luid balance (i.
-000001b0: 652e 2066 6c75 6964 2069 6e70 7574 202d  e. fluid input -
-000001c0: 2066 6c75 6964 206f 7574 7075 7429 2066   fluid output) f
-000001d0: 6f72 2061 2073 7065 6369 6669 6320 7469  or a specific ti
-000001e0: 6d65 2069 6e74 6572 7661 6c2e 0a20 2020  me interval..   
-000001f0: 2054 7970 6963 616c 6c79 2074 6869 7320   Typically this 
-00000200: 7769 6c6c 2062 6520 7573 6564 2074 6f20  will be used to 
-00000210: 6361 6c63 756c 6174 6520 6461 696c 7920  calculate daily 
-00000220: 666c 7569 6420 6261 6c61 6e63 6573 2e0a  fluid balances..
-00000230: 0a20 2020 2041 7267 756d 656e 7473 3a0a  .    Arguments:.
-00000240: 2020 2020 2020 2020 6164 6d69 7373 696f          admissio
-00000250: 6e69 6420 2d2d 2074 6865 2061 646d 6973  nid -- the admis
-00000260: 7369 6f6e 6964 206f 6620 4943 5520 6164  sionid of ICU ad
-00000270: 6d69 7373 696f 6e0a 2020 2020 2020 2020  mission.        
-00000280: 6672 6f6d 5f64 6174 6520 2d2d 2074 6865  from_date -- the
-00000290: 2073 7461 7274 206f 6620 7468 6520 696e   start of the in
-000002a0: 7465 7276 616c 2c20 6578 7072 6573 7365  terval, expresse
-000002b0: 6420 6173 2074 6865 206e 756d 6265 7220  d as the number 
-000002c0: 6f66 206d 696c 6c69 7365 636f 6e64 7320  of milliseconds 
-000002d0: 6672 6f6d 2073 7461 7274 206f 6620 7468  from start of th
-000002e0: 6973 2049 4355 2061 646d 6973 7369 6f6e  is ICU admission
-000002f0: 0a20 2020 2020 2020 2074 6f5f 6461 7465  .        to_date
-00000300: 202d 2d20 7468 6520 656e 6420 6f66 2074   -- the end of t
-00000310: 6865 2069 6e74 6572 7661 6c2c 2065 7870  he interval, exp
-00000320: 7265 7373 6564 2061 7320 7468 6520 6e75  ressed as the nu
-00000330: 6d62 6572 206f 6620 6d69 6c6c 6973 6563  mber of millisec
-00000340: 6f6e 6473 2066 726f 6d20 7374 6172 7420  onds from start 
-00000350: 6f66 2074 6869 7320 4943 5520 6164 6d69  of this ICU admi
-00000360: 7373 696f 6e0a 2020 2020 2020 2020 636f  ssion.        co
-00000370: 6e20 2d2d 2070 7379 636f 7067 3220 636f  n -- psycopg2 co
-00000380: 6e6e 6563 7469 6f6e 206f 7220 7061 6e64  nnection or pand
-00000390: 6173 2d67 6271 2047 6f6f 676c 6520 4269  as-gbq Google Bi
-000003a0: 6751 7565 7279 2063 6f6e 6669 670a 2020  gQuery config.  
-000003b0: 2020 7a1f 6164 6d69 7373 696f 6e69 6420    z.admissionid 
-000003c0: 6973 206e 6f74 2061 206e 756d 6265 723a  is not a number:
-000003d0: 2025 727a 1d66 726f 6d5f 6461 7465 2069   %rz.from_date i
-000003e0: 7320 6e6f 7420 6120 6e75 6d62 6572 3a20  s not a number: 
-000003f0: 2572 7a1b 746f 5f64 6174 6520 6973 206e  %rz.to_date is n
-00000400: 6f74 2061 206e 756d 6265 723a 2025 727a  ot a number: %rz
-00000410: 242e 2f73 716c 2f66 756e 6374 696f 6e73  $./sql/functions
-00000420: 2f67 6574 5f66 6c75 6964 6261 6c61 6e63  /get_fluidbalanc
-00000430: 652e 7371 6cda 0172 2903 da0b 6164 6d69  e.sql..r)...admi
-00000440: 7373 696f 6e69 645a 0a6d 7366 726f 6d64  ssionidZ.msfromd
-00000450: 6174 655a 086d 7374 6f64 6174 6529 015a  ateZ.mstodate).Z
-00000460: 0d63 6f6e 6669 6775 7261 7469 6f6e 2912  .configuration).
-00000470: da02 6e70 da05 696e 7436 34da 0a56 616c  ..np..int64..Val
-00000480: 7565 4572 726f 72da 0945 7863 6570 7469  ueError..Excepti
-00000490: 6f6e da02 6f73 da04 7061 7468 da07 6469  on..os..path..di
-000004a0: 726e 616d 65da 0761 6273 7061 7468 da08  rname..abspath..
-000004b0: 5f5f 6669 6c65 5f5f da04 6a6f 696e da04  __file__..join..
-000004c0: 6f70 656e da04 7265 6164 da06 666f 726d  open..read..form
-000004d0: 6174 da04 7479 7065 da04 6469 6374 da02  at..type..dict..
-000004e0: 7064 5a08 7265 6164 5f67 6271 5a08 7265  pdZ.read_gbqZ.re
-000004f0: 6164 5f73 716c 290a 7204 0000 005a 0966  ad_sql).r....Z.f
-00000500: 726f 6d5f 6461 7465 5a07 746f 5f64 6174  rom_dateZ.to_dat
-00000510: 65da 0363 6f6e 720b 0000 00da 0866 696c  e..conr......fil
-00000520: 656e 616d 655a 0773 716c 6669 6c65 da04  enameZ.sqlfile..
-00000530: 6669 6c65 da03 7371 6cda 0672 6573 756c  file..sql..resul
-00000540: 74a9 0072 1a00 0000 fa37 643a 5c67 6974  t..r.....7d:\git
-00000550: 6875 625c 616d 7374 6572 6461 6d75 6d63  hub\amsterdamumc
-00000560: 6462 5c61 6d73 7465 7264 616d 756d 6364  db\amsterdamumcd
-00000570: 625c 666c 7569 6462 616c 616e 6365 2e70  b\fluidbalance.p
-00000580: 79da 1067 6574 5f66 6c75 6964 6261 6c61  y..get_fluidbala
-00000590: 6e63 6506 0000 0073 2a00 0000 000b 0201  nce....s*.......
-000005a0: 0e01 0e01 1202 0201 0e01 0e01 1202 0201  ................
-000005b0: 0e01 0e01 1203 1401 0401 0e02 0a02 1402  ................
-000005c0: 0c01 1002 0c02 721c 0000 0029 07da 0670  ......r....)...p
-000005d0: 616e 6461 7372 1400 0000 da05 6e75 6d70  andasr......nump
-000005e0: 7972 0500 0000 7209 0000 00da 0944 6174  yr....r......Dat
-000005f0: 6146 7261 6d65 721c 0000 0072 1a00 0000  aFramer....r....
-00000600: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000610: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-00000620: 0000 0801 0801 0803                      ........
+00000060: 004e da06 7265 7475 726e 6304 0000 0000  .N..returnc.....
+00000070: 0000 0000 0000 000a 0000 0008 0000 0043  ...............C
+00000080: 0000 0073 f000 0000 7a07 7400 a001 7c00  ...s....z.t...|.
+00000090: a101 7d00 5700 6e0d 0400 7402 7914 0100  ..}.W.n...t.y...
+000000a0: 0100 0100 7403 6401 7c00 1600 8301 8201  ....t.d.|.......
+000000b0: 7700 7a07 7400 a001 7c01 a101 7d01 5700  w.z.t...|...}.W.
+000000c0: 6e0d 0400 7402 7929 0100 0100 0100 7403  n...t.y)......t.
+000000d0: 6402 7c01 1600 8301 8201 7700 7a07 7400  d.|.......w.z.t.
+000000e0: a001 7c02 a101 7d02 5700 6e0d 0400 7402  ..|...}.W.n...t.
+000000f0: 793e 0100 0100 0100 7403 6403 7c02 1600  y>......t.d.|...
+00000100: 8301 8201 7700 7404 6a05 a006 7404 6a05  ....w.t.j...t.j.
+00000110: a007 7408 a101 a101 7d04 6404 7d05 7404  ..t.....}.d.}.t.
+00000120: 6a05 a009 7c04 7c05 a102 7d06 740a 7c06  j...|.|...}.t.|.
+00000130: 6405 8302 7d07 7c07 a00b a100 6a0c 7c00  d...}.|.....j.|.
+00000140: 7c01 7c02 6406 8d03 7d08 740d 7c03 8301  |.|.d...}.t.|...
+00000150: 740e 7500 7270 740f 6a10 7c08 7c03 6407  t.u.rpt.j.|.|.d.
+00000160: 8d02 7d09 7c09 5300 740f a011 7c08 7c03  ..}.|.S.t...|.|.
+00000170: a102 7d09 7c09 5300 2909 6121 0200 0043  ..}.|.S.).a!...C
+00000180: 616c 6375 6c61 7465 2074 6865 2066 6c75  alculate the flu
+00000190: 6964 2062 616c 616e 6365 2028 692e 652e  id balance (i.e.
+000001a0: 2066 6c75 6964 2069 6e70 7574 202d 2066   fluid input - f
+000001b0: 6c75 6964 206f 7574 7075 7429 2066 6f72  luid output) for
+000001c0: 2061 2073 7065 6369 6669 6320 7469 6d65   a specific time
+000001d0: 2069 6e74 6572 7661 6c2e 0a20 2020 2054   interval..    T
+000001e0: 7970 6963 616c 6c79 2074 6869 7320 7769  ypically this wi
+000001f0: 6c6c 2062 6520 7573 6564 2074 6f20 6361  ll be used to ca
+00000200: 6c63 756c 6174 6520 6461 696c 7920 666c  lculate daily fl
+00000210: 7569 6420 6261 6c61 6e63 6573 2e0a 0a20  uid balances... 
+00000220: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
+00000230: 2020 2020 2020 6164 6d69 7373 696f 6e69        admissioni
+00000240: 6420 2d2d 2074 6865 2061 646d 6973 7369  d -- the admissi
+00000250: 6f6e 6964 206f 6620 4943 5520 6164 6d69  onid of ICU admi
+00000260: 7373 696f 6e0a 2020 2020 2020 2020 6672  ssion.        fr
+00000270: 6f6d 5f64 6174 6520 2d2d 2074 6865 2073  om_date -- the s
+00000280: 7461 7274 206f 6620 7468 6520 696e 7465  tart of the inte
+00000290: 7276 616c 2c20 6578 7072 6573 7365 6420  rval, expressed 
+000002a0: 6173 2074 6865 206e 756d 6265 7220 6f66  as the number of
+000002b0: 206d 696c 6c69 7365 636f 6e64 7320 6672   milliseconds fr
+000002c0: 6f6d 2073 7461 7274 206f 6620 7468 6973  om start of this
+000002d0: 2049 4355 2061 646d 6973 7369 6f6e 0a20   ICU admission. 
+000002e0: 2020 2020 2020 2074 6f5f 6461 7465 202d         to_date -
+000002f0: 2d20 7468 6520 656e 6420 6f66 2074 6865  - the end of the
+00000300: 2069 6e74 6572 7661 6c2c 2065 7870 7265   interval, expre
+00000310: 7373 6564 2061 7320 7468 6520 6e75 6d62  ssed as the numb
+00000320: 6572 206f 6620 6d69 6c6c 6973 6563 6f6e  er of millisecon
+00000330: 6473 2066 726f 6d20 7374 6172 7420 6f66  ds from start of
+00000340: 2074 6869 7320 4943 5520 6164 6d69 7373   this ICU admiss
+00000350: 696f 6e0a 2020 2020 2020 2020 636f 6e20  ion.        con 
+00000360: 2d2d 2070 7379 636f 7067 3220 636f 6e6e  -- psycopg2 conn
+00000370: 6563 7469 6f6e 206f 7220 7061 6e64 6173  ection or pandas
+00000380: 2d67 6271 2047 6f6f 676c 6520 4269 6751  -gbq Google BigQ
+00000390: 7565 7279 2063 6f6e 6669 670a 2020 2020  uery config.    
+000003a0: 7a1f 6164 6d69 7373 696f 6e69 6420 6973  z.admissionid is
+000003b0: 206e 6f74 2061 206e 756d 6265 723a 2025   not a number: %
+000003c0: 727a 1d66 726f 6d5f 6461 7465 2069 7320  rz.from_date is 
+000003d0: 6e6f 7420 6120 6e75 6d62 6572 3a20 2572  not a number: %r
+000003e0: 7a1b 746f 5f64 6174 6520 6973 206e 6f74  z.to_date is not
+000003f0: 2061 206e 756d 6265 723a 2025 727a 242e   a number: %rz$.
+00000400: 2f73 716c 2f66 756e 6374 696f 6e73 2f67  /sql/functions/g
+00000410: 6574 5f66 6c75 6964 6261 6c61 6e63 652e  et_fluidbalance.
+00000420: 7371 6cda 0172 2903 da0b 6164 6d69 7373  sql..r)...admiss
+00000430: 696f 6e69 645a 0a6d 7366 726f 6d64 6174  ionidZ.msfromdat
+00000440: 655a 086d 7374 6f64 6174 6529 015a 0d63  eZ.mstodate).Z.c
+00000450: 6f6e 6669 6775 7261 7469 6f6e 4e29 12da  onfigurationN)..
+00000460: 026e 705a 0569 6e74 3634 da0a 5661 6c75  .npZ.int64..Valu
+00000470: 6545 7272 6f72 da09 4578 6365 7074 696f  eError..Exceptio
+00000480: 6eda 026f 73da 0470 6174 68da 0764 6972  n..os..path..dir
+00000490: 6e61 6d65 da07 6162 7370 6174 68da 085f  name..abspath.._
+000004a0: 5f66 696c 655f 5fda 046a 6f69 6eda 046f  _file__..join..o
+000004b0: 7065 6eda 0472 6561 64da 0666 6f72 6d61  pen..read..forma
+000004c0: 74da 0474 7970 65da 0464 6963 74da 0270  t..type..dict..p
+000004d0: 645a 0872 6561 645f 6762 715a 0872 6561  dZ.read_gbqZ.rea
+000004e0: 645f 7371 6c29 0a72 0400 0000 5a09 6672  d_sql).r....Z.fr
+000004f0: 6f6d 5f64 6174 655a 0774 6f5f 6461 7465  om_dateZ.to_date
+00000500: 5a03 636f 6e72 0a00 0000 da08 6669 6c65  Z.conr......file
+00000510: 6e61 6d65 5a07 7371 6c66 696c 65da 0466  nameZ.sqlfile..f
+00000520: 696c 655a 0373 716c da06 7265 7375 6c74  ileZ.sql..result
+00000530: a900 7217 0000 00fa 3743 3a5c 4769 7448  ..r.....7C:\GitH
+00000540: 7562 5c41 6d73 7465 7264 616d 554d 4364  ub\AmsterdamUMCd
+00000550: 625c 616d 7374 6572 6461 6d75 6d63 6462  b\amsterdamumcdb
+00000560: 5c66 6c75 6964 6261 6c61 6e63 652e 7079  \fluidbalance.py
+00000570: da10 6765 745f 666c 7569 6462 616c 616e  ..get_fluidbalan
+00000580: 6365 0600 0000 7332 0000 0002 0b0e 010c  ce....s2........
+00000590: 010c 0102 ff02 030e 010c 010c 0102 ff02  ................
+000005a0: 030e 010c 010c 0102 ff14 0404 010e 010a  ................
+000005b0: 0214 020c 020e 0104 040c fe04 0272 1900  .............r..
+000005c0: 0000 2907 5a06 7061 6e64 6173 7213 0000  ..).Z.pandasr...
+000005d0: 005a 056e 756d 7079 7205 0000 0072 0800  .Z.numpyr....r..
+000005e0: 0000 5a09 4461 7461 4672 616d 6572 1900  ..Z.DataFramer..
+000005f0: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000600: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000610: 0100 0000 7308 0000 0008 0008 0108 0114  ....s...........
+00000620: 03                                       .
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/__pycache__/plotting.cpython-38.pyc` & `amsterdamumcdb-0.2.1/amsterdamumcdb/__pycache__/plotting.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Sep 27 18:57:41 2021 UTC, .py size: 5500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-00000000: 550d 0d0a 0000 0000 2514 5261 7c15 0000  U.......%.Ra|...
+00000000: 6f0d 0d0a 0000 0000 241f 7f61 7c15 0000  o.......$..a|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 6400 6401 6c05 5a06 640f  m.Z...d.d.l.Z.d.
 00000050: 6403 6404 8401 5a07 6405 6406 8400 5a08  d.d...Z.d.d...Z.
 00000060: 6410 6408 6409 8401 5a09 6411 640b 640c  d.d.d...Z.d.d.d.
 00000070: 8401 5a0a 6412 640d 640e 8401 5a0b 6401  ..Z.d.d.d...Z.d.
 00000080: 5300 2913 e900 0000 004e e700 0000 0000  S.)......N......
 00000090: 0010 4063 0700 0000 0000 0000 0000 0000  ..@c............
-000000a0: 1300 0000 0900 0000 4b00 0000 7300 0200  ........K...s...
-000000b0: 007c 020c 007c 030c 0040 0072 1a74 007c  .|...|...@.r.t.|
-000000c0: 007c 0183 025c 027d 027d 037c 0272 2a7c  .|...\.}.}.|.r*|
-000000d0: 027c 00a0 01a1 006b 0072 387c 00a0 01a1  .|.....k.r8|....
-000000e0: 007d 0264 017d 086e 0464 027d 087c 0372  .}.d.}.n.d.}.|.r
-000000f0: 4c7c 037c 00a0 02a1 006b 0472 5a7c 00a0  L|.|.....k.rZ|..
-00000100: 02a1 007d 0364 017d 096e 0464 027d 097c  ...}.d.}.n.d.}.|
-00000110: 0473 c67c 0573 a474 037c 0083 017d 0a74  .s.|.s.t.|...}.t
+000000a0: 1300 0000 0900 0000 4b00 0000 73f6 0100  ........K...s...
+000000b0: 007c 020c 007c 030c 0040 0072 0d74 007c  .|...|...@.r.t.|
+000000c0: 007c 0183 025c 027d 027d 037c 0272 157c  .|...\.}.}.|.r.|
+000000d0: 027c 00a0 01a1 006b 0072 1c7c 00a0 01a1  .|.....k.r.|....
+000000e0: 007d 0264 017d 086e 0264 027d 087c 0372  .}.d.}.n.d.}.|.r
+000000f0: 267c 037c 00a0 02a1 006b 0472 2d7c 00a0  &|.|.....k.r-|..
+00000100: 02a1 007d 0364 017d 096e 0264 027d 097c  ...}.d.}.n.d.}.|
+00000110: 0473 637c 0573 5274 037c 0083 017d 0a74  .sc|.sRt.|...}.t
 00000120: 047c 027c 0374 037c 0083 017c 0683 047d  .|.|.t.|...|...}
 00000130: 0574 05a0 0674 077c 027c 0564 038d 0274  .t...t.|.|.d...t
 00000140: 077c 037c 0517 007c 0564 038d 027c 05a1  .|.|...|.d...|..
-00000150: 037d 046e 2274 05a0 0674 077c 027c 0564  .}.n"t...t.|.|.d
+00000150: 037d 046e 1174 05a0 0674 077c 027c 0564  .}.n.t...t.|.|.d
 00000160: 038d 0274 077c 037c 0517 007c 0564 038d  ...t.|.|...|.d..
 00000170: 027c 05a1 037d 0474 086a 097c 0066 017c  .|...}.t.j.|.f.|
-00000180: 027c 0366 027c 0464 049c 027c 0797 028e  .|.f.|.d...|....
+00000180: 027c 0366 027c 0464 049c 027c 07a4 018e  .|.f.|.d...|....
 00000190: 015c 037d 0b7d 047d 0c74 086a 0aa0 0b64  .\.}.}.}.t.j...d
 000001a0: 05a1 017d 0d7c 0b7c 0ba0 01a1 0018 007c  ...}.|.|.......|
 000001b0: 0ba0 02a1 007c 0ba0 01a1 0018 001b 007d  .....|.........}
-000001c0: 0e74 0c7c 0e7c 0c83 0244 005d 245c 027d  .t.|.|...D.]$\.}
+000001c0: 0e74 0c7c 0e7c 0c83 0244 005d 115c 027d  .t.|.|...D.].\.}
 000001d0: 0f7d 1074 08a0 0d7c 1064 067c 0d64 0764  .}.t...|.d.|.d.d
-000001e0: 087c 0f14 0017 0083 01a1 0301 0090 0171  .|.............q
-000001f0: 1a7c 0890 0172 947c 007c 026b 00a0 0ea1  .|...r.|.|.k....
-00000200: 007d 117c 0c64 0919 00a0 0f7c 0c64 0919  .}.|.d.....|.d..
-00000210: 00a0 10a1 007c 1117 00a1 0101 007c 0c64  .....|.......|.d
-00000220: 0919 00a0 1164 0aa1 0101 007c 0c64 0919  .....d.....|.d..
-00000230: 00a0 1264 0ba0 137c 00a0 01a1 007c 02a1  ...d...|.....|..
-00000240: 02a1 0101 007c 0990 0172 e87c 007c 036b  .....|...r.|.|.k
-00000250: 04a0 0ea1 007d 127c 0c64 0c19 00a0 0f7c  .....}.|.d.....|
-00000260: 0c64 0c19 00a0 10a1 007c 1217 00a1 0101  .d.......|......
-00000270: 007c 0c64 0c19 00a0 1164 0da1 0101 007c  .|.d.....d.....|
-00000280: 0c64 0c19 00a0 1264 0ea0 137c 037c 00a0  .d.....d...|.|..
-00000290: 02a1 00a1 02a1 0101 007c 0890 0173 f47c  .........|...s.|
-000002a0: 0990 0172 fc74 08a0 14a1 0001 0074 0853  ...r.t.......t.S
-000002b0: 0029 0f61 d603 0000 5265 7475 726e 2061  .).a....Return a
-000002c0: 2070 7970 6c6f 7420 6869 7374 6f67 7261   pyplot histogra
-000002d0: 6d2c 2077 6865 7265 2074 6865 2075 7070  m, where the upp
-000002e0: 6572 2061 6e64 2f6f 7220 6c6f 7765 7220  er and/or lower 
-000002f0: 6f75 746c 6965 7273 2061 7265 0a20 2020  outliers are.   
-00000300: 2062 696e 6e65 6420 746f 6765 7468 6572   binned together
-00000310: 2066 6f72 2061 206d 6f72 6520 6576 656e   for a more even
-00000320: 2064 6973 7472 6962 7574 696f 6e20 706c   distribution pl
-00000330: 6f74 2e20 4279 2064 6566 6175 6c74 2c20  ot. By default, 
-00000340: 7468 6520 6869 7374 6f67 7261 6d20 7769  the histogram wi
-00000350: 6c6c 2062 6520 6372 6561 7465 6420 7769  ll be created wi
-00000360: 7468 2062 696e 7320 7468 6174 2061 7265  th bins that are
-00000370: 206f 6e0a 2020 2020 626f 756e 6461 7269   on.    boundari
-00000380: 6573 2061 6c69 676e 6564 2077 6974 6820  es aligned with 
-00000390: 7468 6520 7079 706c 6f74 2061 7869 7320  the pyplot axis 
-000003a0: 7469 636b 732e 0a0a 2020 2020 4172 6775  ticks...    Argu
-000003b0: 6d65 6e74 733a 0a20 2020 2020 2020 2064  ments:.        d
-000003c0: 6174 6120 2d2d 2064 6174 6166 7261 6d65  ata -- dataframe
-000003d0: 2074 6f20 6372 6561 7465 2074 6865 2068   to create the h
-000003e0: 6973 746f 6772 616d 2066 6f72 2e0a 2020  istogram for..  
-000003f0: 2020 2020 2020 7a5f 7468 7265 7368 6f6c        z_threshol
-00000400: 6420 284f 7074 696f 6e61 6c29 202d 2d20  d (Optional) -- 
-00000410: 6e75 6d62 6572 206f 6620 7374 616e 6461  number of standa
-00000420: 7264 2064 6576 6961 7469 6f6e 7320 6672  rd deviations fr
-00000430: 6f6d 2074 6865 206d 6564 6961 6e20 746f  om the median to
-00000440: 2064 6574 6572 6d69 6e65 206f 7574 6c69   determine outli
-00000450: 6572 730a 2020 2020 2020 2020 6c6f 7765  ers.        lowe
-00000460: 7220 284f 7074 696f 6e61 6c29 202d 2d20  r (Optional) -- 
-00000470: 6c6f 7765 7220 7468 7265 7368 6f6c 6420  lower threshold 
-00000480: 666f 7220 6269 6e6e 696e 6720 6c6f 7765  for binning lowe
-00000490: 7220 6f75 746c 6965 7273 2074 6f67 6574  r outliers toget
-000004a0: 6865 720a 2020 2020 2020 2020 7570 7065  her.        uppe
-000004b0: 7220 284f 7074 696f 6e61 6c29 202d 2d20  r (Optional) -- 
-000004c0: 7570 7065 7220 7468 7265 7368 6f6c 6420  upper threshold 
-000004d0: 666f 7220 6269 6e6e 696e 6720 6869 6768  for binning high
-000004e0: 6572 206f 7574 6c69 6572 7320 746f 6765  er outliers toge
-000004f0: 7468 6572 0a20 2020 2020 2020 2062 696e  ther.        bin
-00000500: 7320 284f 7074 696f 6e61 6c29 202d 2d20  s (Optional) -- 
-00000510: 696e 7420 6f72 2073 6571 7565 6e63 6520  int or sequence 
-00000520: 6f72 2073 7472 2c20 616c 6c6f 7773 2073  or str, allows s
-00000530: 7065 6369 6679 696e 6720 7468 6520 6e75  pecifying the nu
-00000540: 6d62 6572 206f 6620 6269 6e73 2c20 7468  mber of bins, th
-00000550: 6520 6163 7475 616c 2062 696e 7320 6f72  e actual bins or
-00000560: 2061 2062 696e 6e69 6e67 2073 7472 6174   a binning strat
-00000570: 6567 790a 2020 2020 2020 2020 2020 2020  egy.            
-00000580: 2873 6565 3a20 6874 7470 733a 2f2f 6d61  (see: https://ma
-00000590: 7470 6c6f 746c 6962 2e6f 7267 2f73 7461  tplotlib.org/sta
-000005a0: 626c 652f 6170 692f 5f61 735f 6765 6e2f  ble/api/_as_gen/
-000005b0: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-000005c0: 742e 6869 7374 2e68 746d 6c29 0a20 2020  t.hist.html).   
-000005d0: 2020 2020 2062 696e 7769 6474 6820 284f       binwidth (O
-000005e0: 7074 696f 6e61 6c29 202d 2d20 666f 7263  ptional) -- forc
-000005f0: 6573 2061 2073 7065 6369 6669 6564 2073  es a specified s
-00000600: 697a 6520 6f66 2074 6865 2065 7175 616c  ize of the equal
-00000610: 6c79 2073 697a 6564 2062 696e 7320 6265  ly sized bins be
-00000620: 7477 6565 6e20 7468 6520 6c6f 7765 7220  tween the lower 
-00000630: 616e 6420 7570 7065 7220 7468 7265 7368  and upper thresh
-00000640: 6f6c 640a 2020 2020 2020 2020 6d61 7862  old.        maxb
-00000650: 696e 7320 2d2d 2074 6865 206d 6178 696d  ins -- the maxim
-00000660: 756d 206e 756d 6265 7220 6f66 2065 7175  um number of equ
-00000670: 616c 6c79 2073 697a 6564 2062 696e 7320  ally sized bins 
-00000680: 746f 2063 7265 6174 650a 2020 2020 4654  to create.    FT
-00000690: 2901 da04 6261 7365 2902 da05 7261 6e67  )...base)...rang
-000006a0: 65da 0462 696e 73da 056d 6167 6d61 da09  e..bins..magma..
-000006b0: 6661 6365 636f 6c6f 7267 3333 3333 3333  facecolorg333333
-000006c0: c33f 6733 3333 3333 33e3 3f72 0100 0000  .?g333333.?r....
-000006d0: da01 627a 204c 6f77 6572 206f 7574 6c69  ..bz Lower outli
-000006e0: 6572 733a 2028 7b3a 2e32 667d 2c20 7b3a  ers: ({:.2f}, {:
-000006f0: 2e32 667d 29e9 ffff ffff da01 727a 2055  .2f}).......rz U
-00000700: 7070 6572 206f 7574 6c69 6572 733a 2028  pper outliers: (
-00000710: 7b3a 2e32 667d 2c20 7b3a 2e32 667d 2929  {:.2f}, {:.2f}))
-00000720: 15da 077a 5f72 616e 6765 da03 6d69 6eda  ...z_range..min.
-00000730: 036d 6178 da03 6c65 6eda 0f70 7265 7474  .max..len..prett
-00000740: 795f 6269 6e77 6964 7468 da02 6e70 da06  y_binwidth..np..
-00000750: 6172 616e 6765 da0a 726f 756e 645f 6261  arange..round_ba
-00000760: 7365 da03 706c 74da 0468 6973 74da 0263  se..plt..hist..c
-00000770: 6dda 0867 6574 5f63 6d61 70da 037a 6970  m..get_cmap..zip
-00000780: da04 7365 7470 da03 7375 6dda 0a73 6574  ..setp..sum..set
-00000790: 5f68 6569 6768 74da 0a67 6574 5f68 6569  _height..get_hei
-000007a0: 6768 74da 0d73 6574 5f66 6163 6563 6f6c  ght..set_facecol
-000007b0: 6f72 da09 7365 745f 6c61 6265 6cda 0666  or..set_label..f
-000007c0: 6f72 6d61 74da 066c 6567 656e 6429 13da  ormat..legend)..
-000007d0: 0464 6174 615a 0b7a 5f74 6872 6573 686f  .dataZ.z_thresho
-000007e0: 6c64 da05 6c6f 7765 72da 0575 7070 6572  ld..lower..upper
-000007f0: 7205 0000 00da 0862 696e 7769 6474 68da  r......binwidth.
-00000800: 076d 6178 6269 6e73 da06 6b77 6172 6773  .maxbins..kwargs
-00000810: 5a0e 6c6f 7765 725f 6f75 746c 6965 7273  Z.lower_outliers
-00000820: 5a0e 7570 7065 725f 6f75 746c 6965 7273  Z.upper_outliers
-00000830: da05 636f 756e 74da 016e da07 7061 7463  ..count..n..patc
-00000840: 6865 7372 1500 0000 da03 636f 6cda 0163  hesr......col..c
-00000850: da01 705a 106e 5f6c 6f77 6572 5f6f 7574  ..pZ.n_lower_out
-00000860: 6c69 6572 735a 106e 5f75 7070 6572 5f6f  liersZ.n_upper_o
-00000870: 7574 6c69 6572 73a9 0072 2c00 0000 fa33  utliers..r,....3
-00000880: 643a 5c67 6974 6875 625c 616d 7374 6572  d:\github\amster
-00000890: 6461 6d75 6d63 6462 5c61 6d73 7465 7264  damumcdb\amsterd
-000008a0: 616d 756d 6364 625c 706c 6f74 7469 6e67  amumcdb\plotting
-000008b0: 2e70 79da 126f 7574 6c69 6572 735f 6869  .py..outliers_hi
-000008c0: 7374 6f67 7261 6d05 0000 0073 4400 0000  stogram....sD...
-000008d0: 000f 0c01 0e02 1001 0801 0602 0402 1001  ................
-000008e0: 0801 0602 0402 0403 0403 0801 1201 2402  ..............$.
-000008f0: 2202 2201 0c03 1c01 1201 1e02 0601 0c01  ".".............
-00000900: 1a01 0e01 1a02 0601 0c01 1a01 0e01 1a02  ................
-00000910: 0c01 0802 722e 0000 0063 0100 0000 0000  ....r....c......
-00000920: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-00000930: 0000 7326 0000 0074 00a0 017c 00a1 017d  ..s&...t...|...}
-00000940: 0174 00a0 027c 007c 0118 00a1 017d 0274  .t...|.|.....}.t
-00000950: 00a0 017c 02a1 017d 037c 0353 0029 017a  ...|...}.|.S.).z
-00000960: 9852 6574 7572 6e20 7468 6520 6d65 6469  .Return the medi
-00000970: 616e 2061 6273 6f6c 7574 6520 6465 7669  an absolute devi
-00000980: 6174 696f 6e20 666f 7220 7468 6520 6461  ation for the da
-00000990: 7461 7365 742e 0a0a 2020 2020 4172 6775  taset...    Argu
-000009a0: 6d65 6e74 733a 0a20 2020 2020 2020 2064  ments:.        d
-000009b0: 6174 6120 2d2d 2074 6865 2064 6174 6166  ata -- the dataf
-000009c0: 7261 6d65 2074 6f20 6361 6c63 756c 6174  rame to calculat
-000009d0: 6520 7468 6520 6d65 6469 616e 2061 6273  e the median abs
-000009e0: 6f6c 7574 6520 6465 7669 6174 696f 6e20  olute deviation 
-000009f0: 666f 722e 0a20 2020 2029 0372 1000 0000  for..    ).r....
-00000a00: da06 6d65 6469 616e da03 6162 7329 0472  ..median..abs).r
-00000a10: 2000 0000 722f 0000 00da 0464 6966 66da   ...r/.....diff.
-00000a20: 034d 4144 722c 0000 0072 2c00 0000 722d  .MADr,...r,...r-
-00000a30: 0000 00da 036d 6164 4900 0000 7308 0000  .....madI...s...
-00000a40: 0000 060a 010e 010a 0172 3300 0000 e904  .........r3.....
-00000a50: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000a60: 0500 0000 0300 0000 4300 0000 732e 0000  ........C...s...
-00000a70: 0074 007c 0083 017d 0274 01a0 027c 00a1  .t.|...}.t...|..
-00000a80: 017d 037c 017c 0214 0064 011b 007d 047c  .}.|.|...d...}.|
-00000a90: 037c 0418 007c 037c 0417 0066 0253 0029  .|...|.|...f.S.)
-00000aa0: 027a f443 616c 6375 6c61 7465 2074 6865  .z.Calculate the
-00000ab0: 2072 616e 6765 2066 6f72 2074 6865 2064   range for the d
-00000ac0: 6174 6173 6574 2062 6173 6564 206f 6e20  ataset based on 
-00000ad0: 7468 6520 7370 6563 6966 6965 6420 5a20  the specified Z 
-00000ae0: 7468 7265 7368 6f6c 643a 2074 6865 206e  threshold: the n
-00000af0: 756d 6265 7220 6f66 2073 7461 6e64 6172  umber of standar
-00000b00: 640a 2020 2020 6465 7669 6174 696f 6e73  d.    deviations
-00000b10: 2066 726f 6d20 7468 6520 6d65 6469 616e   from the median
-00000b20: 2e0a 0a20 2020 2041 7267 756d 656e 7473  ...    Arguments
-00000b30: 3a0a 2020 2020 2020 2020 6461 7461 202d  :.        data -
-00000b40: 2d20 7468 6520 6461 7461 6672 616d 6520  - the dataframe 
-00000b50: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00000b60: 205a 2072 616e 6765 2066 6f72 2e0a 2020   Z range for..  
-00000b70: 2020 2020 2020 7a5f 7468 7265 7368 202d        z_thresh -
-00000b80: 2d20 7468 6520 5a20 7468 7265 7368 6f6c  - the Z threshol
-00000b90: 642e 0a20 2020 2067 2fdd 2406 8195 e53f  d..    g/.$....?
-00000ba0: 2903 7233 0000 0072 1000 0000 722f 0000  ).r3...r....r/..
-00000bb0: 0029 0572 2000 0000 5a08 7a5f 7468 7265  .).r ...Z.z_thre
-00000bc0: 7368 7232 0000 0072 2f00 0000 da05 636f  shr2...r/.....co
-00000bd0: 6e73 7472 2c00 0000 722c 0000 0072 2d00  nstr,...r,...r-.
-00000be0: 0000 720b 0000 0055 0000 0073 0800 0000  ..r....U...s....
-00000bf0: 0008 0801 0a01 0c01 720b 0000 00e7 9a99  ........r.......
-00000c00: 9999 9999 a93f 6302 0000 0000 0000 0000  .....?c.........
-00000c10: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00000c20: 1400 0000 7c01 7400 7401 7c00 8301 7c01  ....|.t.t.|...|.
-00000c30: 1b00 8301 1400 5300 2901 7a28 2272 6f75  ......S.).z("rou
-00000c40: 6e64 7320 7468 6520 7661 6c75 6520 7570  nds the value up
-00000c50: 2074 6f20 7468 6520 6e65 6172 6573 7420   to the nearest 
-00000c60: 6261 7365 2902 da05 726f 756e 64da 0566  base)...round..f
-00000c70: 6c6f 6174 2902 da01 7872 0300 0000 722c  loat)...xr....r,
-00000c80: 0000 0072 2c00 0000 722d 0000 0072 1200  ...r,...r-...r..
-00000c90: 0000 6300 0000 7302 0000 0000 0272 1200  ..c...s......r..
-00000ca0: 0000 6304 0000 0000 0000 0000 0000 000b  ..c.............
-00000cb0: 0000 0004 0000 0043 0000 0073 a200 0000  .......C...s....
-00000cc0: 7400 a001 a100 7d04 7c04 6a02 7c00 7c01  t.....}.|.j.|.|.
-00000cd0: 6401 8d02 7d05 7c03 7238 7403 7c03 7404  d...}.|.r8t.|.t.
-00000ce0: 7c05 8301 1b00 8301 7d06 7c06 6402 6b02  |.......}.|.d.k.
-00000cf0: 728a 6403 7d06 6e52 7404 7c05 8301 7d07  r.d.}.nRt.|...}.
-00000d00: 6403 6404 6405 6406 6704 7d08 6402 7d09  d.d.d.d.g.}.d.}.
-00000d10: 7c08 6402 1900 7d06 7c09 7404 7c08 8301  |.d...}.|.t.|...
-00000d20: 6b00 728a 7c07 7c06 1400 6404 1300 7c02  k.r.|.|...d...|.
-00000d30: 6b00 728a 7c08 7c09 1900 7d06 6e02 718a  k.r.|.|...}.n.q.
-00000d40: 7c09 6403 3700 7d09 7158 7c05 6403 1900  |.d.7.}.qX|.d...
+000001e0: 087c 0f14 0017 0083 01a1 0301 0071 8d7c  .|...........q.|
+000001f0: 0872 c87c 007c 026b 00a0 0ea1 007d 117c  .r.|.|.k.....}.|
+00000200: 0c64 0919 00a0 0f7c 0c64 0919 00a0 10a1  .d.....|.d......
+00000210: 007c 1117 00a1 0101 007c 0c64 0919 00a0  .|.......|.d....
+00000220: 1164 0aa1 0101 007c 0c64 0919 00a0 1264  .d.....|.d.....d
+00000230: 0ba0 137c 00a0 01a1 007c 02a1 02a1 0101  ...|.....|......
+00000240: 007c 0972 f17c 007c 036b 04a0 0ea1 007d  .|.r.|.|.k.....}
+00000250: 127c 0c64 0c19 00a0 0f7c 0c64 0c19 00a0  .|.d.....|.d....
+00000260: 10a1 007c 1217 00a1 0101 007c 0c64 0c19  ...|.......|.d..
+00000270: 00a0 1164 0da1 0101 007c 0c64 0c19 00a0  ...d.....|.d....
+00000280: 1264 0ea0 137c 037c 00a0 02a1 00a1 02a1  .d...|.|........
+00000290: 0101 007c 0873 f57c 0972 f974 08a0 14a1  ...|.s.|.r.t....
+000002a0: 0001 0074 0853 0029 1061 d603 0000 5265  ...t.S.).a....Re
+000002b0: 7475 726e 2061 2070 7970 6c6f 7420 6869  turn a pyplot hi
+000002c0: 7374 6f67 7261 6d2c 2077 6865 7265 2074  stogram, where t
+000002d0: 6865 2075 7070 6572 2061 6e64 2f6f 7220  he upper and/or 
+000002e0: 6c6f 7765 7220 6f75 746c 6965 7273 2061  lower outliers a
+000002f0: 7265 0a20 2020 2062 696e 6e65 6420 746f  re.    binned to
+00000300: 6765 7468 6572 2066 6f72 2061 206d 6f72  gether for a mor
+00000310: 6520 6576 656e 2064 6973 7472 6962 7574  e even distribut
+00000320: 696f 6e20 706c 6f74 2e20 4279 2064 6566  ion plot. By def
+00000330: 6175 6c74 2c20 7468 6520 6869 7374 6f67  ault, the histog
+00000340: 7261 6d20 7769 6c6c 2062 6520 6372 6561  ram will be crea
+00000350: 7465 6420 7769 7468 2062 696e 7320 7468  ted with bins th
+00000360: 6174 2061 7265 206f 6e0a 2020 2020 626f  at are on.    bo
+00000370: 756e 6461 7269 6573 2061 6c69 676e 6564  undaries aligned
+00000380: 2077 6974 6820 7468 6520 7079 706c 6f74   with the pyplot
+00000390: 2061 7869 7320 7469 636b 732e 0a0a 2020   axis ticks...  
+000003a0: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+000003b0: 2020 2020 2064 6174 6120 2d2d 2064 6174       data -- dat
+000003c0: 6166 7261 6d65 2074 6f20 6372 6561 7465  aframe to create
+000003d0: 2074 6865 2068 6973 746f 6772 616d 2066   the histogram f
+000003e0: 6f72 2e0a 2020 2020 2020 2020 7a5f 7468  or..        z_th
+000003f0: 7265 7368 6f6c 6420 284f 7074 696f 6e61  reshold (Optiona
+00000400: 6c29 202d 2d20 6e75 6d62 6572 206f 6620  l) -- number of 
+00000410: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+00000420: 6f6e 7320 6672 6f6d 2074 6865 206d 6564  ons from the med
+00000430: 6961 6e20 746f 2064 6574 6572 6d69 6e65  ian to determine
+00000440: 206f 7574 6c69 6572 730a 2020 2020 2020   outliers.      
+00000450: 2020 6c6f 7765 7220 284f 7074 696f 6e61    lower (Optiona
+00000460: 6c29 202d 2d20 6c6f 7765 7220 7468 7265  l) -- lower thre
+00000470: 7368 6f6c 6420 666f 7220 6269 6e6e 696e  shold for binnin
+00000480: 6720 6c6f 7765 7220 6f75 746c 6965 7273  g lower outliers
+00000490: 2074 6f67 6574 6865 720a 2020 2020 2020   together.      
+000004a0: 2020 7570 7065 7220 284f 7074 696f 6e61    upper (Optiona
+000004b0: 6c29 202d 2d20 7570 7065 7220 7468 7265  l) -- upper thre
+000004c0: 7368 6f6c 6420 666f 7220 6269 6e6e 696e  shold for binnin
+000004d0: 6720 6869 6768 6572 206f 7574 6c69 6572  g higher outlier
+000004e0: 7320 746f 6765 7468 6572 0a20 2020 2020  s together.     
+000004f0: 2020 2062 696e 7320 284f 7074 696f 6e61     bins (Optiona
+00000500: 6c29 202d 2d20 696e 7420 6f72 2073 6571  l) -- int or seq
+00000510: 7565 6e63 6520 6f72 2073 7472 2c20 616c  uence or str, al
+00000520: 6c6f 7773 2073 7065 6369 6679 696e 6720  lows specifying 
+00000530: 7468 6520 6e75 6d62 6572 206f 6620 6269  the number of bi
+00000540: 6e73 2c20 7468 6520 6163 7475 616c 2062  ns, the actual b
+00000550: 696e 7320 6f72 2061 2062 696e 6e69 6e67  ins or a binning
+00000560: 2073 7472 6174 6567 790a 2020 2020 2020   strategy.      
+00000570: 2020 2020 2020 2873 6565 3a20 6874 7470        (see: http
+00000580: 733a 2f2f 6d61 7470 6c6f 746c 6962 2e6f  s://matplotlib.o
+00000590: 7267 2f73 7461 626c 652f 6170 692f 5f61  rg/stable/api/_a
+000005a0: 735f 6765 6e2f 6d61 7470 6c6f 746c 6962  s_gen/matplotlib
+000005b0: 2e70 7970 6c6f 742e 6869 7374 2e68 746d  .pyplot.hist.htm
+000005c0: 6c29 0a20 2020 2020 2020 2062 696e 7769  l).        binwi
+000005d0: 6474 6820 284f 7074 696f 6e61 6c29 202d  dth (Optional) -
+000005e0: 2d20 666f 7263 6573 2061 2073 7065 6369  - forces a speci
+000005f0: 6669 6564 2073 697a 6520 6f66 2074 6865  fied size of the
+00000600: 2065 7175 616c 6c79 2073 697a 6564 2062   equally sized b
+00000610: 696e 7320 6265 7477 6565 6e20 7468 6520  ins between the 
+00000620: 6c6f 7765 7220 616e 6420 7570 7065 7220  lower and upper 
+00000630: 7468 7265 7368 6f6c 640a 2020 2020 2020  threshold.      
+00000640: 2020 6d61 7862 696e 7320 2d2d 2074 6865    maxbins -- the
+00000650: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+00000660: 6f66 2065 7175 616c 6c79 2073 697a 6564  of equally sized
+00000670: 2062 696e 7320 746f 2063 7265 6174 650a   bins to create.
+00000680: 2020 2020 4654 2901 da04 6261 7365 2902      FT)...base).
+00000690: da05 7261 6e67 65da 0462 696e 735a 056d  ..range..binsZ.m
+000006a0: 6167 6d61 5a09 6661 6365 636f 6c6f 7267  agmaZ.facecolorg
+000006b0: 3333 3333 3333 c33f 6733 3333 3333 33e3  333333.?g333333.
+000006c0: 3f72 0100 0000 da01 627a 204c 6f77 6572  ?r......bz Lower
+000006d0: 206f 7574 6c69 6572 733a 2028 7b3a 2e32   outliers: ({:.2
+000006e0: 667d 2c20 7b3a 2e32 667d 29e9 ffff ffff  f}, {:.2f}).....
+000006f0: da01 727a 2055 7070 6572 206f 7574 6c69  ..rz Upper outli
+00000700: 6572 733a 2028 7b3a 2e32 667d 2c20 7b3a  ers: ({:.2f}, {:
+00000710: 2e32 667d 294e 2915 da07 7a5f 7261 6e67  .2f})N)...z_rang
+00000720: 65da 036d 696e da03 6d61 78da 036c 656e  e..min..max..len
+00000730: da0f 7072 6574 7479 5f62 696e 7769 6474  ..pretty_binwidt
+00000740: 68da 026e 70da 0661 7261 6e67 65da 0a72  h..np..arange..r
+00000750: 6f75 6e64 5f62 6173 65da 0370 6c74 da04  ound_base..plt..
+00000760: 6869 7374 da02 636d 5a08 6765 745f 636d  hist..cmZ.get_cm
+00000770: 6170 da03 7a69 705a 0473 6574 70da 0373  ap..zipZ.setp..s
+00000780: 756d 5a0a 7365 745f 6865 6967 6874 5a0a  umZ.set_heightZ.
+00000790: 6765 745f 6865 6967 6874 5a0d 7365 745f  get_heightZ.set_
+000007a0: 6661 6365 636f 6c6f 725a 0973 6574 5f6c  facecolorZ.set_l
+000007b0: 6162 656c da06 666f 726d 6174 da06 6c65  abel..format..le
+000007c0: 6765 6e64 2913 da04 6461 7461 5a0b 7a5f  gend)...dataZ.z_
+000007d0: 7468 7265 7368 6f6c 64da 056c 6f77 6572  threshold..lower
+000007e0: da05 7570 7065 7272 0500 0000 da08 6269  ..upperr......bi
+000007f0: 6e77 6964 7468 da07 6d61 7862 696e 73da  nwidth..maxbins.
+00000800: 066b 7761 7267 735a 0e6c 6f77 6572 5f6f  .kwargsZ.lower_o
+00000810: 7574 6c69 6572 735a 0e75 7070 6572 5f6f  utliersZ.upper_o
+00000820: 7574 6c69 6572 73da 0563 6f75 6e74 da01  utliers..count..
+00000830: 6e5a 0770 6174 6368 6573 7213 0000 00da  nZ.patchesr.....
+00000840: 0363 6f6c da01 63da 0170 5a10 6e5f 6c6f  .col..c..pZ.n_lo
+00000850: 7765 725f 6f75 746c 6965 7273 5a10 6e5f  wer_outliersZ.n_
+00000860: 7570 7065 725f 6f75 746c 6965 7273 a900  upper_outliers..
+00000870: 7223 0000 00fa 3343 3a5c 4769 7448 7562  r#....3C:\GitHub
+00000880: 5c41 6d73 7465 7264 616d 554d 4364 625c  \AmsterdamUMCdb\
+00000890: 616d 7374 6572 6461 6d75 6d63 6462 5c70  amsterdamumcdb\p
+000008a0: 6c6f 7474 696e 672e 7079 da12 6f75 746c  lotting.py..outl
+000008b0: 6965 7273 5f68 6973 746f 6772 616d 0500  iers_histogram..
+000008c0: 0000 7344 0000 000c 0f0e 0110 0208 0106  ..sD............
+000008d0: 0104 0210 0208 0106 0104 0204 0204 0308  ................
+000008e0: 0312 0124 0122 0222 020c 011c 0312 011c  ...$."."........
+000008f0: 0104 020c 011a 010e 011a 0104 020c 011a  ................
+00000900: 010e 011a 0108 0208 0104 0272 2500 0000  ...........r%...
+00000910: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000920: 0004 0000 0043 0000 0073 2600 0000 7400  .....C...s&...t.
+00000930: a001 7c00 a101 7d01 7400 a002 7c00 7c01  ..|...}.t...|.|.
+00000940: 1800 a101 7d02 7400 a001 7c02 a101 7d03  ....}.t...|...}.
+00000950: 7c03 5300 2902 7a98 5265 7475 726e 2074  |.S.).z.Return t
+00000960: 6865 206d 6564 6961 6e20 6162 736f 6c75  he median absolu
+00000970: 7465 2064 6576 6961 7469 6f6e 2066 6f72  te deviation for
+00000980: 2074 6865 2064 6174 6173 6574 2e0a 0a20   the dataset... 
+00000990: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
+000009a0: 2020 2020 2020 6461 7461 202d 2d20 7468        data -- th
+000009b0: 6520 6461 7461 6672 616d 6520 746f 2063  e dataframe to c
+000009c0: 616c 6375 6c61 7465 2074 6865 206d 6564  alculate the med
+000009d0: 6961 6e20 6162 736f 6c75 7465 2064 6576  ian absolute dev
+000009e0: 6961 7469 6f6e 2066 6f72 2e0a 2020 2020  iation for..    
+000009f0: 4e29 0372 0e00 0000 da06 6d65 6469 616e  N).r......median
+00000a00: da03 6162 7329 0472 1800 0000 7226 0000  ..abs).r....r&..
+00000a10: 00da 0464 6966 66da 034d 4144 7223 0000  ...diff..MADr#..
+00000a20: 0072 2300 0000 7224 0000 00da 036d 6164  .r#...r$.....mad
+00000a30: 4900 0000 7308 0000 000a 060e 010a 0104  I...s...........
+00000a40: 0172 2a00 0000 e904 0000 0063 0200 0000  .r*........c....
+00000a50: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000a60: 4300 0000 732e 0000 0074 007c 0083 017d  C...s....t.|...}
+00000a70: 0274 01a0 027c 00a1 017d 037c 017c 0214  .t...|...}.|.|..
+00000a80: 0064 011b 007d 047c 037c 0418 007c 037c  .d...}.|.|...|.|
+00000a90: 0417 0066 0253 0029 037a f443 616c 6375  ...f.S.).z.Calcu
+00000aa0: 6c61 7465 2074 6865 2072 616e 6765 2066  late the range f
+00000ab0: 6f72 2074 6865 2064 6174 6173 6574 2062  or the dataset b
+00000ac0: 6173 6564 206f 6e20 7468 6520 7370 6563  ased on the spec
+00000ad0: 6966 6965 6420 5a20 7468 7265 7368 6f6c  ified Z threshol
+00000ae0: 643a 2074 6865 206e 756d 6265 7220 6f66  d: the number of
+00000af0: 2073 7461 6e64 6172 640a 2020 2020 6465   standard.    de
+00000b00: 7669 6174 696f 6e73 2066 726f 6d20 7468  viations from th
+00000b10: 6520 6d65 6469 616e 2e0a 0a20 2020 2041  e median...    A
+00000b20: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+00000b30: 2020 6461 7461 202d 2d20 7468 6520 6461    data -- the da
+00000b40: 7461 6672 616d 6520 746f 2063 616c 6375  taframe to calcu
+00000b50: 6c61 7465 2074 6865 205a 2072 616e 6765  late the Z range
+00000b60: 2066 6f72 2e0a 2020 2020 2020 2020 7a5f   for..        z_
+00000b70: 7468 7265 7368 202d 2d20 7468 6520 5a20  thresh -- the Z 
+00000b80: 7468 7265 7368 6f6c 642e 0a20 2020 2067  threshold..    g
+00000b90: 2fdd 2406 8195 e53f 4e29 0372 2a00 0000  /.$....?N).r*...
+00000ba0: 720e 0000 0072 2600 0000 2905 7218 0000  r....r&...).r...
+00000bb0: 005a 087a 5f74 6872 6573 6872 2900 0000  .Z.z_threshr)...
+00000bc0: 7226 0000 00da 0563 6f6e 7374 7223 0000  r&.....constr#..
+00000bd0: 0072 2300 0000 7224 0000 0072 0900 0000  .r#...r$...r....
+00000be0: 5500 0000 7308 0000 0008 080a 010c 0110  U...s...........
+00000bf0: 0172 0900 0000 e79a 9999 9999 99a9 3f63  .r............?c
+00000c00: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000c10: 0400 0000 4300 0000 7314 0000 007c 0174  ....C...s....|.t
+00000c20: 0074 017c 0083 017c 011b 0083 0114 0053  .t.|...|.......S
+00000c30: 0029 027a 2822 726f 756e 6473 2074 6865  .).z("rounds the
+00000c40: 2076 616c 7565 2075 7020 746f 2074 6865   value up to the
+00000c50: 206e 6561 7265 7374 2062 6173 654e 2902   nearest baseN).
+00000c60: da05 726f 756e 64da 0566 6c6f 6174 2902  ..round..float).
+00000c70: da01 7872 0300 0000 7223 0000 0072 2300  ..xr....r#...r#.
+00000c80: 0000 7224 0000 0072 1000 0000 6300 0000  ..r$...r....c...
+00000c90: 7302 0000 0014 0272 1000 0000 6304 0000  s......r....c...
+00000ca0: 0000 0000 0000 0000 000b 0000 0004 0000  ................
+00000cb0: 0043 0000 0073 a800 0000 7400 a001 a100  .C...s....t.....
+00000cc0: 7d04 7c04 6a02 7c00 7c01 6401 8d02 7d05  }.|.j.|.|.d...}.
+00000cd0: 7c03 721c 7403 7c03 7404 7c05 8301 1b00  |.r.t.|.t.|.....
+00000ce0: 8301 7d06 7c06 6402 6b02 721b 6403 7d06  ..}.|.d.k.r.d.}.
+00000cf0: 6e2c 7404 7c05 8301 7d07 6700 6404 a201  n,t.|...}.g.d...
+00000d00: 7d08 6402 7d09 7c08 6402 1900 7d06 7c09  }.d.}.|.d...}.|.
+00000d10: 7404 7c08 8301 6b00 7248 7c07 7c06 1400  t.|...k.rH|.|...
+00000d20: 6405 1300 7c02 6b00 723d 7c08 7c09 1900  d...|.k.r=|.|...
+00000d30: 7d06 6e01 7148 7c09 6403 3700 7d09 7c09  }.n.qH|.d.7.}.|.
+00000d40: 7404 7c08 8301 6b00 7330 7c05 6403 1900  t.|...k.s0|.d...
 00000d50: 7c05 6402 1900 1800 7c06 1b00 7d0a 7c0a  |.d.....|...}.|.
 00000d60: 5300 2907 6121 0200 0075 7365 7320 7468  S.).a!...uses th
 00000d70: 6520 6d61 7470 6c6f 746c 6962 2e74 6963  e matplotlib.tic
 00000d80: 6b65 722e 4175 746f 4c6f 6361 746f 7220  ker.AutoLocator 
 00000d90: 2866 6f72 2067 656e 6572 6174 696e 6720  (for generating 
 00000da0: 7468 6520 7469 636b 7320 696e 2074 6865  the ticks in the
 00000db0: 0a20 2020 2070 6c6f 7429 2c20 746f 2064  .    plot), to d
@@ -242,35 +242,36 @@
 00000f10: 6620 7468 6520 6461 7461 7365 740a 2020  f the dataset.  
 00000f20: 2020 2020 2020 636f 756e 7420 2d2d 206e        count -- n
 00000f30: 756d 6265 7220 6f66 2069 7465 6d73 2069  umber of items i
 00000f40: 6e20 7468 6520 6461 7461 7365 740a 2020  n the dataset.  
 00000f50: 2020 2020 2020 6d61 7862 696e 7320 2d2d        maxbins --
 00000f60: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
 00000f70: 6265 7220 6f66 2062 696e 7320 746f 2063  ber of bins to c
-00000f80: 7265 6174 650a 2020 2020 2902 da04 766d  reate.    )...vm
-00000f90: 696e da04 766d 6178 7201 0000 00e9 0100  in..vmaxr.......
-00000fa0: 0000 e902 0000 0072 3400 0000 e905 0000  .......r4.......
-00000fb0: 0029 05da 0674 6963 6b65 72da 0b41 7574  .)...ticker..Aut
-00000fc0: 6f4c 6f63 6174 6f72 da0b 7469 636b 5f76  oLocator..tick_v
-00000fd0: 616c 7565 73da 0369 6e74 720e 0000 0029  alues..intr....)
-00000fe0: 0b72 2100 0000 7222 0000 0072 2600 0000  .r!...r"...r&...
-00000ff0: 7224 0000 00da 076c 6f63 6174 6f72 da05  r$.....locator..
-00001000: 7469 636b 735a 0d62 696e 735f 7065 725f  ticksZ.bins_per_
-00001010: 7469 636b 5a09 6e75 6d5f 7469 636b 735a  tickZ.num_ticksZ
-00001020: 1662 696e 735f 7065 725f 7469 636b 5f73  .bins_per_tick_s
-00001030: 7472 6174 6567 79da 0169 7223 0000 0072  trategy..ir#...r
-00001040: 2c00 0000 722c 0000 0072 2d00 0000 720f  ,...r,...r-...r.
-00001050: 0000 0068 0000 0073 2200 0000 000d 0801  ...h...s".......
-00001060: 0e02 0402 1001 0801 0603 0801 0c03 0401  ................
-00001070: 0801 0c01 1001 0a02 0201 0a02 1402 720f  ..............r.
-00001080: 0000 0029 0672 0200 0000 4e4e 4e4e 4e29  ...).r....NNNNN)
-00001090: 0172 3400 0000 2901 7236 0000 0029 014e  .r4...).r6...).N
-000010a0: 290c da11 6d61 7470 6c6f 746c 6962 2e70  )...matplotlib.p
-000010b0: 7970 6c6f 74da 0670 7970 6c6f 7472 1300  yplot..pyplotr..
-000010c0: 0000 da11 6d61 7470 6c6f 746c 6962 2e74  ....matplotlib.t
-000010d0: 6963 6b65 7272 3f00 0000 da05 6e75 6d70  ickerr?.....nump
-000010e0: 7972 1000 0000 722e 0000 0072 3300 0000  yr....r....r3...
-000010f0: 720b 0000 0072 1200 0000 720f 0000 0072  r....r....r....r
-00001100: 2c00 0000 722c 0000 0072 2c00 0000 722d  ,...r,...r,...r-
-00001110: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001120: 0073 0e00 0000 0c01 0c01 0802 0a44 080c  .s...........D..
-00001130: 0a0e 0a05                                ....
+00000f80: 7265 6174 650a 2020 2020 2902 5a04 766d  reate.    ).Z.vm
+00000f90: 696e 5a04 766d 6178 7201 0000 00e9 0100  inZ.vmaxr.......
+00000fa0: 0000 2904 7231 0000 00e9 0200 0000 722b  ..).r1........r+
+00000fb0: 0000 00e9 0500 0000 7232 0000 004e 2905  ........r2...N).
+00000fc0: da06 7469 636b 6572 5a0b 4175 746f 4c6f  ..tickerZ.AutoLo
+00000fd0: 6361 746f 725a 0b74 6963 6b5f 7661 6c75  catorZ.tick_valu
+00000fe0: 6573 da03 696e 7472 0c00 0000 290b 7219  es..intr....).r.
+00000ff0: 0000 0072 1a00 0000 721e 0000 0072 1c00  ...r....r....r..
+00001000: 0000 5a07 6c6f 6361 746f 725a 0574 6963  ..Z.locatorZ.tic
+00001010: 6b73 5a0d 6269 6e73 5f70 6572 5f74 6963  ksZ.bins_per_tic
+00001020: 6b5a 096e 756d 5f74 6963 6b73 5a16 6269  kZ.num_ticksZ.bi
+00001030: 6e73 5f70 6572 5f74 6963 6b5f 7374 7261  ns_per_tick_stra
+00001040: 7465 6779 da01 6972 1b00 0000 7223 0000  tegy..ir....r#..
+00001050: 0072 2300 0000 7224 0000 0072 0d00 0000  .r#...r$...r....
+00001060: 6800 0000 7326 0000 0008 0d0e 0104 0210  h...s&..........
+00001070: 0208 0104 0102 8008 0308 0104 0308 010c  ................
+00001080: 0110 010a 0102 0208 010c fb14 0704 0272  ...............r
+00001090: 0d00 0000 2906 7202 0000 004e 4e4e 4e4e  ....).r....NNNNN
+000010a0: 2901 722b 0000 0029 0172 2d00 0000 2901  ).r+...).r-...).
+000010b0: 4e29 0cda 116d 6174 706c 6f74 6c69 622e  N)...matplotlib.
+000010c0: 7079 706c 6f74 da06 7079 706c 6f74 7211  pyplot..pyplotr.
+000010d0: 0000 005a 116d 6174 706c 6f74 6c69 622e  ...Z.matplotlib.
+000010e0: 7469 636b 6572 7234 0000 00da 056e 756d  tickerr4.....num
+000010f0: 7079 720e 0000 0072 2500 0000 722a 0000  pyr....r%...r*..
+00001100: 0072 0900 0000 7210 0000 0072 0d00 0000  .r....r....r....
+00001110: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
+00001120: 2400 0000 da08 3c6d 6f64 756c 653e 0100  $.....<module>..
+00001130: 0000 7310 0000 000c 000c 0108 010a 0208  ..s.............
+00001140: 440a 0c0a 0e0e 05                        D......
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/bigquery.py` & `amsterdamumcdb-0.2.1/amsterdamumcdb/bigquery.py`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/dictionary/dictionary.csv` & `amsterdamumcdb-0.2.1/amsterdamumcdb/dictionary/dictionary.csv`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/fluidbalance.py` & `amsterdamumcdb-0.2.1/amsterdamumcdb/fluidbalance.py`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/plotting.py` & `amsterdamumcdb-0.2.1/amsterdamumcdb/plotting.py`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/scores.py` & `amsterdamumcdb-0.2.1/amsterdamumcdb/scores.py`

 * *Files 21% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                          (sofa_respiration['pf_ratio'] >= 300), 'sofa_respiration_score'] = 1
     sofa_respiration.loc[(sofa_respiration['pf_ratio'] < 300), 'sofa_respiration_score'] = 2
     sofa_respiration.loc[(sofa_respiration['pf_ratio'] < 200) & (sofa_respiration['pf_ratio'] >= 100) &
                          (sofa_respiration['ventilatory_support'] is True), 'sofa_respiration_score'] = 3
     sofa_respiration.loc[(sofa_respiration['pf_ratio'] < 100) &
                          (sofa_respiration['ventilatory_support'] is True), 'sofa_respiration_score'] = 4
 
-    return sofa_respiration
+    return sofa_respiration.sort_values(by=['admissionid', 'time']).reset_index(drop=True)
 
 
 def get_sofa_cardiovascular_meds(con) -> pd.DataFrame:
     """
     Returns SOFA: Cardiovascular - Hypotension, cardiovascular medication: vasopressors and / or inotropes
     Arguments:
         con -- psycopg2 connection or pandas-gbq Google BigQuery config
@@ -77,39 +77,40 @@
 
     # calculate SOFA cardiovascular score:
     sofa_cardiovascular_meds.loc[:, 'sofa_cardiovascular_score'] = 0
 
     # dopamine (itemid 7179) <= 5 or dobutamine (itemid 7178) any dose
     sofa_cardiovascular_meds.loc[(
                                          ((sofa_cardiovascular_meds['itemid'] == 7179) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] <= 5)) |
+                                                 sofa_cardiovascular_meds['max_gamma'] <= 5)) |
                                          (sofa_cardiovascular_meds['itemid'] == 7178)
                                  ), 'sofa_cardiovascular_score'] = 2
 
     # dopamine (itemid 7179) > 5, epinephrine (itemid 6818) <= 0.1, norepinephrine (itemid 7229) <= 0.1
     sofa_cardiovascular_meds.loc[(
                                          ((sofa_cardiovascular_meds['itemid'] == 7179) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] > 5) &
+                                                 sofa_cardiovascular_meds['max_gamma'] > 5) &
                                           (sofa_cardiovascular_meds['max_gamma'] < 15)) |
                                          ((sofa_cardiovascular_meds['itemid'] == 6818) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] <= 0.1)) |
+                                                 sofa_cardiovascular_meds['max_gamma'] <= 0.1)) |
                                          ((sofa_cardiovascular_meds['itemid'] == 7229) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] <= 0.1))
+                                                 sofa_cardiovascular_meds['max_gamma'] <= 0.1))
                                  ), 'sofa_cardiovascular_score'] = 3
 
     # dopamine (itemid 7179) > 15, epinephrine (itemid 6818) > 0.1, norepinephrine (itemid 7229) > 0.1
     sofa_cardiovascular_meds.loc[(
                                          ((sofa_cardiovascular_meds['itemid'] == 7179) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] > 15)) |
+                                                 sofa_cardiovascular_meds['max_gamma'] > 15)) |
                                          ((sofa_cardiovascular_meds['itemid'] == 6818) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] > 0.1)) |
+                                                 sofa_cardiovascular_meds['max_gamma'] > 0.1)) |
                                          ((sofa_cardiovascular_meds['itemid'] == 7229) & (
-                                                     sofa_cardiovascular_meds['max_gamma'] > 0.1))
+                                                 sofa_cardiovascular_meds['max_gamma'] > 0.1))
                                  ), 'sofa_cardiovascular_score'] = 4
-    return sofa_cardiovascular_meds
+    return sofa_cardiovascular_meds.sort_values(by='admissionid').reset_index(
+        drop=True)
 
 
 def get_sofa_platelets(con) -> pd.DataFrame:
     """
     Return SOFA Coagulation score.
 
     Arguments:
@@ -131,15 +132,15 @@
                        (sofa_platelets['value'] >= 100), 'sofa_coagulation_score'] = 1
     sofa_platelets.loc[(sofa_platelets['value'] < 100) &
                        (sofa_platelets['value'] >= 50), 'sofa_coagulation_score'] = 2
     sofa_platelets.loc[(sofa_platelets['value'] < 50) &
                        (sofa_platelets['value'] >= 20), 'sofa_coagulation_score'] = 3
     sofa_platelets.loc[(sofa_platelets['value'] < 20), 'sofa_coagulation_score'] = 4
 
-    return sofa_platelets
+    return sofa_platelets.sort_values(by=['admissionid', 'itemid', 'time']).reset_index(drop=True)
 
 
 def get_sofa_bilirubin(con) -> pd.DataFrame:
     """
     Returns SOFA Liver scores.
 
     Arguments:
@@ -159,15 +160,15 @@
     print('Processing SOFA Liver...')
     sofa_bilirubin.loc[:, 'sofa_liver_score'] = 0
     sofa_bilirubin.loc[(sofa_bilirubin['value'] >= 20) & (sofa_bilirubin['value'] < 33), 'sofa_liver_score'] = 1
     sofa_bilirubin.loc[(sofa_bilirubin['value'] >= 33) & (sofa_bilirubin['value'] < 102), 'sofa_liver_score'] = 2
     sofa_bilirubin.loc[(sofa_bilirubin['value'] >= 102) & (sofa_bilirubin['value'] < 204), 'sofa_liver_score'] = 3
     sofa_bilirubin.loc[(sofa_bilirubin['value'] >= 204), 'sofa_liver_score'] = 4
 
-    return sofa_bilirubin
+    return sofa_bilirubin.sort_values(by=['admissionid', 'itemid', 'time']).reset_index(drop=True)
 
 
 def get_sofa_cardiovascular_map(con):
     """
     Returns SOFA Mean arterial pressure score
     Arguments:
         con -- psycopg2 connection or pandas-gbq Google BigQuery config
@@ -191,15 +192,15 @@
     ).reset_index()
 
     # calculate SOFA cardiovascular score:
     sofa_cardiovascular_map.loc[:, 'sofa_cardiovascular_score'] = 0
     # MAP < 70
     sofa_cardiovascular_map.loc[(sofa_cardiovascular_map['lowest_mean_abp'] < 70), 'sofa_cardiovascular_score'] = 1
 
-    return sofa_cardiovascular_map
+    return sofa_cardiovascular_map.sort_values(by=['admissionid']).reset_index(drop=True)
 
 
 def get_sofa_cns(con) -> pd.DataFrame:
     """
     Return SOFA Central nervous system score
 
     Arguments:
@@ -207,29 +208,92 @@
     """
     # get Glasgow Coma Scale-score
     print('Querying SOFA Central nervous system...')
     filename = './sql/common/gcs.sql'
     sql_filename = os.path.join(dirname, filename)
     with open(sql_filename, 'r') as sql_file:
         sql_gcs = sql_file.read()
-    gcs = read_sql(sql_gcs, con)
+    sofa_cns = read_sql(sql_gcs, con)
 
     print('Processing SOFA Central nervous system...')
-    sofa_cns = gcs.groupby(['admissionid']).agg(
-        min_gcs=pd.NamedAgg(column='gcs_score', aggfunc='min')
-    ).reset_index()
-
     # calculate SOFA Central nervous system score:
+    # the SOFA score assumes that the GCS is either determined without sedation, or was known before sedation was
+    # started. Elective patients while being sedated are considered having GCS=15 with respect to the SOFA CNS score.
+    #
+    # Medical staff were trained to document an 'estimated/expected' GCS for sedated/intubated patients at least for the
+    # first 24 hours, so should be the most reliable with respect to SOFA scoring
+
+    # If scores have been performed by medical staff remove all others
+    admissionids = sofa_cns[sofa_cns['registeredby'] == 'ICV_Medisch Staflid']['admissionid']
+    sofa_cns = sofa_cns.drop(sofa_cns[
+                                 (sofa_cns['admissionid'].isin(admissionids)) &
+                                 ~(sofa_cns['registeredby'] == 'ICV_Medisch Staflid')
+                                 ].index
+                             )
+
+    admissionids = sofa_cns[sofa_cns['registeredby'] == 'ICV_Medisch']['admissionid']
+    sofa_cns = sofa_cns.drop(sofa_cns[
+                                 (sofa_cns['admissionid'].isin(admissionids)) &
+                                 ~(sofa_cns['registeredby'] == 'ICV_Medisch')
+                                 ].index
+                             )
+
+    # The most common problem for SOFA scoring is documenting GCS of 3 while patients being sedated
+    # (e.g. directly after surgery or after intubation)
+    # Drop records with gcs_score = 3 AND sedated
+    sofa_cns = sofa_cns.drop(sofa_cns[
+                                 (sofa_cns['gcs_score'] == 3) & ~(sofa_cns['sedatives_given'].isna()) &
+                                 (sofa_cns['registeredby'].isin(['ICV_IC-Verpleegkundig', 'ICV_MC-Verpleegkundig']))
+                                 ].index
+                             )
+
+    # For GCS going from e.g. E1M1V1 to E3M6V5 within 24 hours
+    sofa_cns[sofa_cns['gcs_score'] == 15][['admissionid', 'measuredat']]
+    first_gcs15 = sofa_cns[sofa_cns['gcs_score'] == 15].groupby('admissionid').agg(
+        first_gcs15_measuredat=('measuredat', 'first'))
+    sofa_cns = sofa_cns.merge(first_gcs15, on='admissionid')
+    sofa_cns = sofa_cns.drop(sofa_cns[
+                                 (sofa_cns['gcs_score'] == 3) &
+                                 (sofa_cns['measuredat'] < sofa_cns['first_gcs15_measuredat'])
+                                 ].index
+                             )
+    # the GCS verbal (V) score could be documented as 'Intubated' (v_score = 0 or -2), often considered similar
+    # to a value of 1. However, this often does not reflect the actual level of consciousness, especially if the
+    # eyes and motor score values are not '1' as well.
+    # First remove all score that do not contain at least a valid eyes and motor score
+    sofa_cns = sofa_cns.drop(sofa_cns[
+                                 (sofa_cns['eyes_score'].isna()) |
+                                 (sofa_cns['motor_score'].isna())
+                                 ].index
+                             )
+    # assume E1M1 also has V1
+    sofa_cns.loc[(sofa_cns['eyes_score'] == 1) & (sofa_cns['motor_score'] == 1), 'verbal_score'] = 1
+
+    # remove intubated scores including scores with E4M6V1 and perform back/forward fill
+    sofa_cns.loc[(sofa_cns['verbal_score'] == -2), 'verbal_score'] = np.NaN
+    sofa_cns.loc[(sofa_cns['verbal_score'] == 0), 'verbal_score'] = np.NaN
+    sofa_cns.loc[(sofa_cns['eyes_score'] == 4) & (sofa_cns['motor_score'] == 6) & (sofa_cns['verbal_score'] == 1),
+                 'verbal_score'] = np.NaN
+
+    # assume for missing verbal scores that future measurements should contain the actual value, otherwise
+    # forward fill for still missing values
+    sofa_cns['verbal_score'] = sofa_cns.groupby(['admissionid'])['verbal_score'].bfill()
+    sofa_cns['verbal_score'] = sofa_cns.groupby(['admissionid'])['verbal_score'].ffill()
+
+    # recalculate total GCS score
+    sofa_cns['gcs_score'] = sofa_cns['eyes_score'] + sofa_cns['motor_score'] + sofa_cns['verbal_score']
+
+    # calculate SOFA GCS score based on 'corrected' GCS scores:
     sofa_cns.loc[:, 'sofa_cns_score'] = 0
-    sofa_cns.loc[(sofa_cns['min_gcs'] >= 13) & (sofa_cns['min_gcs'] < 15), 'sofa_cns_score'] = 1
-    sofa_cns.loc[(sofa_cns['min_gcs'] >= 10) & (sofa_cns['min_gcs'] < 13), 'sofa_cns_score'] = 2
-    sofa_cns.loc[(sofa_cns['min_gcs'] >= 6) & (sofa_cns['min_gcs'] < 10), 'sofa_cns_score'] = 3
-    sofa_cns.loc[(sofa_cns['min_gcs'] < 6), 'sofa_cns_score'] = 4
+    sofa_cns.loc[(sofa_cns['gcs_score'] >= 13) & (sofa_cns['gcs_score'] < 15), 'sofa_cns_score'] = 1
+    sofa_cns.loc[(sofa_cns['gcs_score'] >= 10) & (sofa_cns['gcs_score'] < 13), 'sofa_cns_score'] = 2
+    sofa_cns.loc[(sofa_cns['gcs_score'] >= 6) & (sofa_cns['gcs_score'] < 10), 'sofa_cns_score'] = 3
+    sofa_cns.loc[(sofa_cns['gcs_score'] < 6), 'sofa_cns_score'] = 4
 
-    return sofa_cns
+    return sofa_cns.sort_values(by=['admissionid', 'time']).reset_index(drop=True)
 
 
 def get_sofa_renal_daily_urine_output(con) -> pd.DataFrame:
     """
     Return SOFA Urine output score
 
     Arguments:
@@ -265,15 +329,15 @@
                                            (sofa_renal_daily_urine_output['daily_urine_output'] > 200))
                                       ), 'sofa_renal_score'] = 3
 
     # urine output < 200 ml/day
     sofa_renal_daily_urine_output.loc[(
                                           ((sofa_renal_daily_urine_output['daily_urine_output'] < 200))
                                       ), 'sofa_renal_score'] = 4
-    return sofa_renal_daily_urine_output
+    return sofa_renal_daily_urine_output.sort_values(by=['admissionid']).reset_index(drop=True)
 
 
 def get_sofa_renal_creatinine(con) -> pd.DataFrame:
     print('Querying SOFA Renal: creatinine...')
     # get serum creatinine
     filename = './sql/common/creatinine_acute_kidney_injury_failure.sql'
     sql_filename = os.path.join(dirname, filename)
@@ -314,15 +378,15 @@
                               ), 'sofa_renal_score'] = 3
 
     # creatinine >440 umol/l
     sofa_renal_creatinine.loc[(
                                   ((sofa_renal_creatinine['max_creatinine'] > 440))
                               ), 'sofa_renal_score'] = 4
 
-    return sofa_renal_creatinine
+    return sofa_renal_creatinine.sort_values(by=['admissionid']).reset_index(drop=True)
 
 
 def get_sofa_admission(con) -> pd.DataFrame:
     """
     Returns a dataframe containing SOFA score in the first 24 hours of ICU admission for all patients.
     See the [SOFA](https://github.com/AmsterdamUMC/AmsterdamUMCdb/blob/master/concepts/severityscores/sofa.ipynb)
     notebook for additional information on data processing and example data and plots.
@@ -409,11 +473,13 @@
 
     # calculate total score (add al values in columns)
     total_scores = sofa.set_index('admissionid').sum(axis=1, skipna=True).to_frame('sofa_total_score')
     sofa = pd.merge(sofa, total_scores, on='admissionid', how='left')
 
     # Add location and urgency for easier selection:
     sofa = pd.merge(sofa, admissions[['admissionid', 'location', 'urgency']], on='admissionid', how='left')
-    sofa.loc[:, 'urgency'] = pd.to_numeric(sofa.loc[:, 'urgency'])
+    # To force new array with new dtype (instead of inplace setting) (FutureWarning),
+    # changed `sofa.loc[:, 'urgency'] = pd.to_numeric(sofa.loc[:, 'urgency'])` to:
+    admissions['urgency'] = pd.to_numeric(admissions.loc[:, 'urgency'])
 
     print('SOFA processing complete.')
-    return sofa
+    return sofa.sort_values(by=['admissionid']).reset_index(drop=True)
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/bilirubin.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/bilirubin.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/creatinine_acute_kidney_injury_failure.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/creatinine_acute_kidney_injury_failure.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/hematocrit.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/hematocrit.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/lactate.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/lactate.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/oxygen_device.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/oxygen_device.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 SELECT
     oxy_dev.admissionid,
     oxy_dev.valueid,
-    oxy_dev.value as O2_device,
+    oxy_dev.value as o2_device,
     oxy_dev.measuredat,
-    oxy_flow.value AS O2_flow
+    oxy_flow.value AS o2_flow
 FROM listitems oxy_dev
 LEFT JOIN admissions a ON
     oxy_dev.admissionid = a.admissionid
 LEFT JOIN numericitems oxy_flow ON
     oxy_dev.admissionid = oxy_flow.admissionid AND
     oxy_dev.measuredat = oxy_flow.measuredat AND
     oxy_flow.itemid IN (
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/pH.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/pH.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/pO2_pCO2_FiO2.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/pO2_pCO2_FiO2.sql`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 WITH oxygenation AS (
     SELECT
         pao2.admissionid,
         --pao2.itemid,
         --pao2.item,
         CASE pao2.unitid
-            WHEN 152 THEN pao2.value * 7.50061683 -- Conversion: kPa to mmHg
+            WHEN 152 THEN ROUND(pao2.value * 7.50061683, 1) -- Conversion: kPa to mmHg
             ELSE pao2.value
-        END AS "PaO2",
+        END AS pao2,
         CASE paco2.unitid
-            WHEN 152 THEN paco2.value * 7.50061683 -- Conversion: kPa to mmHg
+            WHEN 152 THEN ROUND(paco2.value * 7.50061683, 1) -- Conversion: kPa to mmHg
             ELSE paco2.value
-        END AS "PaCO2",
+        END AS paco2,
         f.value AS specimen_source,
         --pao2.registeredby,
         CASE
             WHEN pao2.registeredby NOT ILIKE '%Systeem%' THEN TRUE
             ELSE FALSE
         END AS manual_entry,
         (pao2.measuredat - a.admittedat)/(1000*60) AS time,
         --fio2.itemid,
         --fio2.item,
-        fio2.value AS "FiO2",
+        fio2.value AS fio2,
         --fio2.measuredat,
-        (fio2.measuredat - pao2.measuredat)/(60*1000) AS FiO2_time_difference,
+        (fio2.measuredat - pao2.measuredat)/(60*1000) AS fio2_time_difference,
         ROW_NUMBER() OVER(
             PARTITION BY pao2.admissionid, pao2.measuredat
             ORDER BY ABS(fio2.measuredat - pao2.measuredat)
         ) AS priority --give priority to nearest FiO2 measurement
     FROM numericitems pao2
     LEFT JOIN admissions a ON
         pao2.admissionid = a.admissionid
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/platelets.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/platelets.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/potassium.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/potassium.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/resp_rate.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/resp_rate.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/sodium.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/sodium.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/temperature.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/temperature.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/urine_output.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/urine_output.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/vasopressors_inotropes.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/vasopressors_inotropes.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/common/wbc.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/common/wbc.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/diagnosis/reason_for_admission.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/diagnosis/reason_for_admission.sql`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,22 @@
         END as diagnosis_group,
         valueid as diagnosis_group_id,
         ROW_NUMBER() OVER(PARTITION BY admissionid
         ORDER BY
             CASE --prefer NICE > APACHE IV > II > D
                 WHEN itemid = 18671 THEN 6 --NICE APACHEIV diagnosen
                 WHEN itemid = 18669 THEN 5 --NICE APACHEII diagnosen
-                WHEN itemid BETWEEN 16998 AND 17017 THEN 4 --APACHE IV diagnosis
-                WHEN itemid BETWEEN 18589 AND 18602 THEN 3 --APACHE II diagnosis
-                WHEN itemid BETWEEN 13116 AND 13145 THEN 2 --D diagnosis ICU
-                WHEN itemid BETWEEN 16642 AND 16673 THEN 1 --DMC diagnosis Medium Care
+                WHEN itemid = 16997 THEN 4 --APACHE IV Groepen
+                WHEN itemid = 18588 THEN 3 --Apache II Hoofdgroep
+                WHEN itemid = 13110 THEN 2 --D_Hoofdgroep
+                WHEN itemid = 16651 THEN 1 --DMC_Hoofdgroep, Medium Care
             END DESC,
-            updatedat DESC) AS rownum --prioritizes diagnosis with last update time
+            updatedat DESC, --prefer diagnosis_group with most recent update time
+            measuredat DESC --prefer diagnosis_group with most recent session/form time
+            ) AS rownum
     FROM listitems
     WHERE itemid IN (
         --MAIN GROUP - LEVEL 0
         13110, --D_Hoofdgroep
         16651, --DMC_Hoofdgroep, Medium Care
 
         18588, --Apache II Hoofdgroep
@@ -37,15 +39,17 @@
 ),diagnosis_subgroups AS (
     SELECT admissionid,
         item,
         value as diagnosis_subgroup,
         valueid as diagnosis_subgroup_id,
         ROW_NUMBER() OVER(PARTITION BY admissionid
         ORDER BY
-            updatedat DESC) AS rownum --prioritizes diagnosis with last update time
+            updatedat DESC, --prefer diagnosis_subgroup with most recent update time
+            measuredat DESC --prefer diagnosis_subgroup with most recent session/form time
+            ) AS rownum
     FROM listitems
     WHERE itemid IN (
         --SUB GROUP - LEVEL 1
         13111, --D_Subgroep_Thoraxchirurgie
         16669, --DMC_Subgroep_Thoraxchirurgie
         13112, --D_Subgroep_Algemene chirurgie
         16665, --DMC_Subgroep_Algemene chirurgie
@@ -145,15 +149,19 @@
                 WHEN itemid = 18671 THEN 6 --NICE APACHEIV diagnosen
                 WHEN itemid = 18669 THEN 5 --NICE APACHEII diagnosen
                 WHEN itemid BETWEEN 16998 AND 17017 THEN 4 --APACHE IV diagnosis
                 WHEN itemid BETWEEN 18589 AND 18602 THEN 3 --APACHE II diagnosis
                 WHEN itemid BETWEEN 13116 AND 13145 THEN 2 --D diagnosis ICU
                 WHEN itemid BETWEEN 16642 AND 16673 THEN 1 --DMC diagnosis Medium Care
             END DESC,
-            updatedat DESC) AS rownum --prioritizes diagnosis with last update time
+            updatedat DESC, --prefer diagnosis with most recent update time
+            measuredat DESC, --prefer diagnosis with most recent session/form time
+            valueid ASC, --force lower valued diagnoses to prevent arbitrary sorting for rare cases
+            itemid ASC --force lower valued diagnosis groups to prevent arbitrary sorting for rare cases
+            ) AS rownum
     FROM listitems
     WHERE itemid IN (
         -- Diagnosis - LEVEL 2
         --SURGICAL
         13116, --D_Thoraxchirurgie_CABG en Klepchirurgie
         16671, --DMC_Thoraxchirurgie_CABG en Klepchirurgie
         13117, --D_Thoraxchirurgie_Cardio anders
@@ -262,15 +270,16 @@
             WHEN 1 THEN 1 --'Ja'
             WHEN 2 THEN 0 --'Nee'
         END as sepsis_at_admission,
         ROW_NUMBER() OVER(
             PARTITION BY
                 admissionid
             ORDER BY
-                updatedat DESC) AS rownum --prioritizes diagnosis with last update time
+                updatedat DESC, --prefer sepsis diagnosis with most recent update time
+                measuredat DESC) AS rownum --prefer sepsis diagnosis with most recent session/form time
     FROM listitems
     WHERE
         itemid = 15808
 ), sepsis_antibiotics AS ( --non prophylactic antibiotics
     SELECT
         admissionid,
         CASE
@@ -408,13 +417,14 @@
 LEFT JOIN diagnoses on admissions.admissionid = diagnoses.admissionid
 LEFT JOIN diagnosis_subgroups on admissions.admissionid = diagnosis_subgroups.admissionid
 LEFT JOIN diagnosis_groups on admissions.admissionid = diagnosis_groups.admissionid
 LEFT JOIN sepsis on admissions.admissionid = sepsis.admissionid
 LEFT JOIN sepsis_antibiotics on admissions.admissionid = sepsis_antibiotics.admissionid
 LEFT JOIN other_antibiotics on admissions.admissionid = other_antibiotics.admissionid
 LEFT JOIN cultures on admissions.admissionid = cultures.admissionid
-WHERE --only diagnosis with last update time
+WHERE --only most recent updated diagnosis
     (diagnoses.rownum = 1 OR diagnoses.rownum IS NULL) AND
     (diagnosis_subgroups.rownum = 1 OR diagnosis_subgroups.rownum IS NULL) AND
     (diagnosis_groups.rownum = 1 OR diagnosis_groups.rownum IS NULL) AND
     (sepsis.rownum = 1 OR sepsis.rownum IS NULL)
+ORDER BY admissions.admissionid
 ;
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet_itemids.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet_itemids.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_nephrology_flowsheet_itemids.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_nephrology_flowsheet_itemids.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_CPP.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_CPP.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_itemids.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_itemids.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/flowsheets/get_respiration_flowsheet_itemids.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/flowsheets/get_respiration_flowsheet_itemids.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/functions/get_fluidbalance.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/functions/get_fluidbalance.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql` & `amsterdamumcdb-0.2.1/amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql`

 * *Files identical despite different names*

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/PKG-INFO` & `amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amsterdamumcdb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common functions for data exploration on AmsterdamUMCdb
 Home-page: https://github.com/AmsterdamUMC/AmsterdamUMCdb
 Author: Amsterdam UMC Laboratory for Critical Care Computational Intelligence
 Author-email: p.thoral@amsterdamumc.nl
 Project-URL: Bug Tracker, https://github.com/AmsterdamUMC/AmsterdamUMCdb/issues
 Keywords: AmsterdamUMCdb,Intensive Care unit,Critical Care,Medical,Patient Data
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amsterdamumcdb-0.2.0/amsterdamumcdb.egg-info/SOURCES.txt` & `amsterdamumcdb-0.2.1/amsterdamumcdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 pyproject.toml
 setup.cfg
 setup.py
 amsterdamumcdb/__init__.py
 amsterdamumcdb/amsterdamumcdb.py
 amsterdamumcdb/bigquery.py
 amsterdamumcdb/cohorts.py
+amsterdamumcdb/connections.py
 amsterdamumcdb/dictionary.py
 amsterdamumcdb/fluidbalance.py
 amsterdamumcdb/plotting.py
 amsterdamumcdb/scores.py
 amsterdamumcdb/util.py
 amsterdamumcdb.egg-info/PKG-INFO
 amsterdamumcdb.egg-info/SOURCES.txt
 amsterdamumcdb.egg-info/dependency_links.txt
 amsterdamumcdb.egg-info/requires.txt
 amsterdamumcdb.egg-info/top_level.txt
-amsterdamumcdb/__pycache__/__init__.cpython-38.pyc
-amsterdamumcdb/__pycache__/dictionary.cpython-38.pyc
-amsterdamumcdb/__pycache__/fluidbalance.cpython-38.pyc
-amsterdamumcdb/__pycache__/plotting.cpython-38.pyc
+amsterdamumcdb/__pycache__/__init__.cpython-310.pyc
+amsterdamumcdb/__pycache__/bigquery.cpython-310.pyc
+amsterdamumcdb/__pycache__/cohorts.cpython-310.pyc
+amsterdamumcdb/__pycache__/connections.cpython-310.pyc
+amsterdamumcdb/__pycache__/dictionary.cpython-310.pyc
+amsterdamumcdb/__pycache__/fluidbalance.cpython-310.pyc
+amsterdamumcdb/__pycache__/plotting.cpython-310.pyc
+amsterdamumcdb/__pycache__/scores.cpython-310.pyc
+amsterdamumcdb/__pycache__/util.cpython-310.pyc
 amsterdamumcdb/dictionary/dictionary.csv
 amsterdamumcdb/sql/common/bilirubin.sql
 amsterdamumcdb/sql/common/creatinine_acute_kidney_injury_failure.sql
 amsterdamumcdb/sql/common/gcs.sql
 amsterdamumcdb/sql/common/heart_rate.sql
 amsterdamumcdb/sql/common/hematocrit.sql
 amsterdamumcdb/sql/common/lactate.sql
@@ -46,8 +52,12 @@
 amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet.sql
 amsterdamumcdb/sql/flowsheets/get_circulation_flowsheet_itemids.sql
 amsterdamumcdb/sql/flowsheets/get_nephrology_flowsheet_itemids.sql
 amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_CPP.sql
 amsterdamumcdb/sql/flowsheets/get_neurology_flowsheet_itemids.sql
 amsterdamumcdb/sql/flowsheets/get_respiration_flowsheet_itemids.sql
 amsterdamumcdb/sql/functions/get_fluidbalance.sql
-amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql
+amsterdamumcdb/sql/lifesupport/mechanical_ventilation.sql
+tests/__init__.py
+tests/test_cohorts.py
+tests/test_scores.py
+tests/test_util.py
```

### Comparing `amsterdamumcdb-0.2.0/setup.cfg` & `amsterdamumcdb-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6d73 7465 7264 616d 756d 6364   = amsterdamumcd
 00000020: 620d 0a76 6572 7369 6f6e 203d 2030 2e32  b..version = 0.2
-00000030: 2e30 0d0a 6175 7468 6f72 203d 2041 6d73  .0..author = Ams
+00000030: 2e31 0d0a 6175 7468 6f72 203d 2041 6d73  .1..author = Ams
 00000040: 7465 7264 616d 2055 4d43 204c 6162 6f72  terdam UMC Labor
 00000050: 6174 6f72 7920 666f 7220 4372 6974 6963  atory for Critic
 00000060: 616c 2043 6172 6520 436f 6d70 7574 6174  al Care Computat
 00000070: 696f 6e61 6c20 496e 7465 6c6c 6967 656e  ional Intelligen
 00000080: 6365 0d0a 6175 7468 6f72 5f65 6d61 696c  ce..author_email
 00000090: 203d 2070 2e74 686f 7261 6c40 616d 7374   = p.thoral@amst
 000000a0: 6572 6461 6d75 6d63 2e6e 6c0d 0a64 6573  erdamumc.nl..des
```

