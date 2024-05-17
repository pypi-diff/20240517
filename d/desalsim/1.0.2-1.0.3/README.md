# Comparing `tmp/desalsim-1.0.2.tar.gz` & `tmp/desalsim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-1.0.2.tar", last modified: Thu May 16 13:59:05 2024, max compression
+gzip compressed data, was "desalsim-1.0.3.tar", last modified: Fri May 17 12:35:45 2024, max compression
```

## Comparing `desalsim-1.0.2.tar` & `desalsim-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.838813 desalsim-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.833830 desalsim-1.0.2/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     7300 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.764013 desalsim-1.0.2/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-1.0.2/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.2/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.2/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-1.0.2/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-1.0.2/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-1.0.2/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-1.0.2/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-1.0.2/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-1.0.2/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     7300 2024-05-16 13:59:05.835820 desalsim-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6806 2024-05-16 13:48:24.000000 desalsim-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.813880 desalsim-1.0.2/example/
--rw-rw-rw-   0        0        0      786 2024-05-16 13:53:14.000000 desalsim-1.0.2/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0.2/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0.2/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.2/example/density_calc.py
--rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/economic_f.py
--rw-rw-rw-   0        0        0     8681 2024-05-16 13:54:25.000000 desalsim-1.0.2/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-1.0.2/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-1.0.2/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/example_1.py
--rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/example_2.py
--rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/ro_unit.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/example/scaleup.py
--rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-1.0.2/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-16 13:59:05.838813 desalsim-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      829 2024-05-16 13:55:11.000000 desalsim-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.830835 desalsim-1.0.2/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0.2/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0.2/tests/ed_unittest.py
--rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/med_unittest.py
--rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/tests/scaleup.py
--rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0.2/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:35:45.760438 desalsim-1.0.3/
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7072 2024-05-17 12:35:45.759441 desalsim-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6832 2024-05-17 09:52:45.000000 desalsim-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 12:35:45.722720 desalsim-1.0.3/desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-17 07:36:20.000000 desalsim-1.0.3/desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.3/desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.3/desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8836 2024-05-17 12:19:59.000000 desalsim-1.0.3/desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     3007 2024-05-17 12:20:53.000000 desalsim-1.0.3/desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11748 2024-05-17 12:20:36.000000 desalsim-1.0.3/desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    46932 2024-05-17 12:21:06.000000 desalsim-1.0.3/desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4504 2024-05-17 12:20:12.000000 desalsim-1.0.3/desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10067 2024-05-17 12:21:15.000000 desalsim-1.0.3/desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     7012 2024-05-17 07:37:50.000000 desalsim-1.0.3/desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-17 07:52:58.000000 desalsim-1.0.3/desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.3/desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8749 2024-05-17 12:20:27.000000 desalsim-1.0.3/desalsim/thermal_cryst_f.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:35:45.728910 desalsim-1.0.3/desalsim.egg-info/
+-rw-rw-rw-   0        0        0     7072 2024-05-17 12:35:45.000000 desalsim-1.0.3/desalsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2024-05-17 12:35:45.000000 desalsim-1.0.3/desalsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 12:35:45.000000 desalsim-1.0.3/desalsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2024-05-17 12:35:45.000000 desalsim-1.0.3/desalsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-17 12:35:45.000000 desalsim-1.0.3/desalsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 12:35:45.747355 desalsim-1.0.3/example/
+-rw-rw-rw-   0        0        0      786 2024-05-16 13:53:14.000000 desalsim-1.0.3/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0.3/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0.3/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.3/example/density_calc.py
+-rw-rw-rw-   0        0        0    11995 2024-05-17 12:30:07.000000 desalsim-1.0.3/example/economic_f.py
+-rw-rw-rw-   0        0        0     8681 2024-05-16 13:54:25.000000 desalsim-1.0.3/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17109 2024-05-17 12:30:44.000000 desalsim-1.0.3/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49455 2024-05-17 12:31:31.000000 desalsim-1.0.3/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33297 2024-05-17 12:32:14.000000 desalsim-1.0.3/example/example_1.py
+-rw-rw-rw-   0        0        0    21717 2024-05-17 12:32:38.000000 desalsim-1.0.3/example/example_2.py
+-rw-rw-rw-   0        0        0     8542 2024-05-17 12:32:45.000000 desalsim-1.0.3/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14939 2024-05-17 12:32:54.000000 desalsim-1.0.3/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9445 2024-05-17 12:33:02.000000 desalsim-1.0.3/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-17 12:33:18.000000 desalsim-1.0.3/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.3/example/scaleup.py
+-rw-rw-rw-   0        0        0    12280 2024-05-17 12:33:46.000000 desalsim-1.0.3/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 12:35:45.760438 desalsim-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      798 2024-05-17 11:50:27.000000 desalsim-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:35:45.758445 desalsim-1.0.3/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0.3/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0.3/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0.3/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0.3/tests/med_unittest.py
+-rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0.3/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0.3/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.3/tests/scaleup.py
+-rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0.3/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-1.0.2/DesalSim.egg-info/PKG-INFO` & `desalsim-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,34 @@
-Metadata-Version: 2.1
-Name: desalsim
-Version: 1.0.2
-Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
-Author: rodoulak
-Author-email: r.ktori@tudelft.nl
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.21.5
-Requires-Dist: pandas==1.4.4
-Requires-Dist: scipy==1.9.1
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: scikit-learn==1.0.2
-Requires-Dist: plotly>=5.9.0
-Requires-Dist: openpyxl==3.0.10
-
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
 ![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
 
 ## Table of contents
 * [Purpose](#purpose)
-* [Key features](#key-features)
 * [Installation](#installation)
+* [Key features](#key-features)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
 * [License](#license)
 
 ## Purpose 
 The purpose of this software suite is to provide researchers, engineers, and policymakers with a powerful tool for evaluating the performance and economics of desalination and brine treatment systems. By integrating technical process models with economic and environmental analyses, the suite enables users to make informed decisions about technology integration, process optimization, and resource management.
 
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalsim==1.0.2
+pip install desalsim==1.0.3
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
@@ -58,15 +41,15 @@
 - Analysis of salt concentration profiles, ion fluxes, energy consumption, and chemical usage
 - Integration of different technologies to optimize process efficiency and resource utilization
 - Economic models for technologies and integrated systems 
 - Output visualization and data export for further analysis 
 
 ### File Descriptions
 
-A brief overview of each file in the project can be found in (https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/file-description). 
+A brief overview of each file in the project can be found in [File description file](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/File_description.md). 
 
 ## Usage 
 Each simulation model serves as a standalone tool for analyzing the performance of a specific desalination or brine treatment technology. Before running the simulation, ensure that you have provided the necessary input parameters, such as feed flow rates, salinity levels, membrane properties, heat sources, and operating conditions.
 
 The simulation results, including salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs, will be generated based on the specified inputs and displayed in the console output or saved to output files for further analysis.
 
 However, simulation models of more than one technology can be combined to simulate and evaluate the performance of a treatment chain (desalination and brine treatment system). In this case, the output flow rates and stream concentrate are the input data for the next technology.
```

### Comparing `desalsim-1.0.2/DesalSim.egg-info/SOURCES.txt` & `desalsim-1.0.3/desalsim.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 LICENSE
 README.md
 setup.py
-DesalSim.egg-info/PKG-INFO
-DesalSim.egg-info/SOURCES.txt
-DesalSim.egg-info/dependency_links.txt
-DesalSim.egg-info/requires.txt
-DesalSim.egg-info/top_level.txt
-Desalsim/__init__.py
-Desalsim/constants.py
-Desalsim/density_calc.py
-Desalsim/economic_f.py
-Desalsim/ed_unit_f.py
-Desalsim/edbm_unit_f.py
-Desalsim/efc_unit_f.py
-Desalsim/med_unit_f.py
-Desalsim/mfpfr_unit_f.py
-Desalsim/nanofiltration_unit_f.py
-Desalsim/ro_unit_f.py
-Desalsim/scaleup.py
-Desalsim/thermal_cryst_f.py
+desalsim/__init__.py
+desalsim/constants.py
+desalsim/density_calc.py
+desalsim/economic_f.py
+desalsim/ed_unit_f.py
+desalsim/edbm_unit_f.py
+desalsim/efc_unit_f.py
+desalsim/med_unit_f.py
+desalsim/mfpfr_unit_f.py
+desalsim/nanofiltration_unit_f.py
+desalsim/ro_unit_f.py
+desalsim/scaleup.py
+desalsim/thermal_cryst_f.py
 desalsim.egg-info/PKG-INFO
 desalsim.egg-info/SOURCES.txt
 desalsim.egg-info/dependency_links.txt
 desalsim.egg-info/requires.txt
 desalsim.egg-info/top_level.txt
 example/__init__.py
 example/comparison.py
@@ -33,15 +28,14 @@
 example/edbm_unit_f.py
 example/efc_unit_f.py
 example/example_1.py
 example/example_2.py
 example/med_unit_f.py
 example/mfpfr_unit_f.py
 example/nanofiltration_unit_f.py
-example/ro_unit.py
 example/ro_unit_f.py
 example/scaleup.py
 example/thermal_cryst_f.py
 tests/__init__.py
 tests/economic_unittest.py
 tests/ed_unittest.py
 tests/edbm_unittest.py
```

### Comparing `desalsim-1.0.2/Desalsim/__init__.py` & `desalsim-1.0.3/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # __init__.py
 from Desalsim import density_calc
 from Desalsim import constants
+
 from Desalsim.nanofiltration_unit_f import NFMass
 from Desalsim.nanofiltration_unit_f import OsmoticPressure
 from Desalsim.nanofiltration_unit_f import NfEnergy
 
 from Desalsim.med_unit_f import MEDCalculator
 
 from Desalsim.thermal_cryst_f import thermal_calc
@@ -24,7 +25,8 @@
 
 
 
 
 
 
 
+
```

### Comparing `desalsim-1.0.2/Desalsim/constants.py` & `desalsim-1.0.3/desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/Desalsim/economic_f.py` & `desalsim-1.0.3/desalsim/economic_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #costs calculations functions 
-from Desalsim import constants 
+from desalsim import constants 
 #%%
 #symbols:
 #hr-> hours
 #lf -> lifetime 
 #el -> electricity
 #s-> steam
 #pr -> price
```

### Comparing `desalsim-1.0.2/Desalsim/ed_unit_f.py` & `desalsim-1.0.3/desalsim/ed_unit_f.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-from Desalsim import scaleup
-from Desalsim import constants 
+from desalsim import scaleup
+from desalsim import constants 
 import math
-from Desalsim.density_calc import density_calc 
+from desalsim.density_calc import density_calc 
 
 #%% Calculations 
 """
 A class used to represent Mass Balance for Electrodialysis
 
 ...
```

### Comparing `desalsim-1.0.2/Desalsim/edbm_unit_f.py` & `desalsim-1.0.3/desalsim/edbm_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math 
 import numpy as np
-from Desalsim import scaleup
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
+from desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
 
 #%%
 #Molecular weight 
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/Desalsim/efc_unit_f.py` & `desalsim-1.0.3/desalsim/efc_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 import time
 import numpy as np
 from scipy import interpolate
 import scipy.interpolate as interpolate
 from sklearn.linear_model import LinearRegression
 from collections import namedtuple
-from Desalsim import scaleup
-from Desalsim.density_calc import density_calc 
+from desalsim import scaleup
+from desalsim.density_calc import density_calc 
 # import pitzer_model_3phases_w
-from Desalsim import constants 
+from desalsim import constants 
 #Set initial time to calculate the elapsed time of the calculations
 time0=time.time()
 MW_so4=32.064+4*15.999
 
 #input data
 Qf=100 #m3/hr
 C_i_in=[20.16, 27.87, 0.50, 0.0, 0.12, 14.66]
```

### Comparing `desalsim-1.0.2/Desalsim/med_unit_f.py` & `desalsim-1.0.3/desalsim/med_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Desalsim.density_calc import density_calc 
+from desalsim.density_calc import density_calc 
 #%%calculations 
 class MEDCalculator:
     """
     A class used to represent Mass Balance for Multi-Effect Distillation 
 
     ...
```

### Comparing `desalsim-1.0.2/Desalsim/mfpfr_unit_f.py` & `desalsim-1.0.3/desalsim/mfpfr_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
-from Desalsim import scaleup
-from Desalsim.density_calc import density_calc 
+from desalsim import scaleup
+from desalsim.density_calc import density_calc 
 import math
-from Desalsim import constants 
+from desalsim import constants 
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
```

### Comparing `desalsim-1.0.2/Desalsim/nanofiltration_unit_f.py` & `desalsim-1.0.3/desalsim/nanofiltration_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import numpy as np
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
+from desalsim.density_calc import density_calc
+from desalsim import constants 
 import math
+
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
```

### Comparing `desalsim-1.0.2/Desalsim/ro_unit_f.py` & `desalsim-1.0.3/desalsim/ro_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
-from Desalsim import constants 
-from Desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim.density_calc import density_calc 
 #%%
 #%%constants
 R=8.31446261815324 #gas constant
 T=20+273.15 #K
 MW_Na=22.99
 MW_cl=35.453
 MW_so4=32.064+4*15.999
```

### Comparing `desalsim-1.0.2/Desalsim/thermal_cryst_f.py` & `desalsim-1.0.3/desalsim/thermal_cryst_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
-from Desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim import scaleup
 
 #%%
     #Molecular weight 
 MW_Na=constants.MW_Na
 MW_cl=constants.MW_cl
 MW_so4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/LICENSE` & `desalsim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/PKG-INFO` & `desalsim-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 Metadata-Version: 2.1
 Name: desalsim
-Version: 1.0.2
-Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
+Version: 1.0.3
+Home-page: https://github.com/rodoulak/desalsim.git
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy==1.21.5
-Requires-Dist: pandas==1.4.4
-Requires-Dist: scipy==1.9.1
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: scikit-learn==1.0.2
-Requires-Dist: plotly>=5.9.0
-Requires-Dist: openpyxl==3.0.10
 
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
 ![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
 
 ## Table of contents
 * [Purpose](#purpose)
-* [Key features](#key-features)
 * [Installation](#installation)
+* [Key features](#key-features)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
 * [License](#license)
 
 ## Purpose 
 The purpose of this software suite is to provide researchers, engineers, and policymakers with a powerful tool for evaluating the performance and economics of desalination and brine treatment systems. By integrating technical process models with economic and environmental analyses, the suite enables users to make informed decisions about technology integration, process optimization, and resource management.
 
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalsim==1.0.2
+pip install desalsim==1.0.3
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
@@ -58,15 +51,15 @@
 - Analysis of salt concentration profiles, ion fluxes, energy consumption, and chemical usage
 - Integration of different technologies to optimize process efficiency and resource utilization
 - Economic models for technologies and integrated systems 
 - Output visualization and data export for further analysis 
 
 ### File Descriptions
 
-A brief overview of each file in the project can be found in (https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/file-description). 
+A brief overview of each file in the project can be found in [File description file](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/File_description.md). 
 
 ## Usage 
 Each simulation model serves as a standalone tool for analyzing the performance of a specific desalination or brine treatment technology. Before running the simulation, ensure that you have provided the necessary input parameters, such as feed flow rates, salinity levels, membrane properties, heat sources, and operating conditions.
 
 The simulation results, including salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs, will be generated based on the specified inputs and displayed in the console output or saved to output files for further analysis.
 
 However, simulation models of more than one technology can be combined to simulate and evaluate the performance of a treatment chain (desalination and brine treatment system). In this case, the output flow rates and stream concentrate are the input data for the next technology.
```

### Comparing `desalsim-1.0.2/README.md` & `desalsim-1.0.3/desalsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,44 @@
+Metadata-Version: 2.1
+Name: desalsim
+Version: 1.0.3
+Home-page: https://github.com/rodoulak/desalsim.git
+Author: rodoulak
+Author-email: r.ktori@tudelft.nl
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
 
 ![system description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/assets/150446818/bb10e07d-b878-45c8-878a-0c56222546cf)
 
 ## Table of contents
 * [Purpose](#purpose)
-* [Key features](#key-features)
 * [Installation](#installation)
+* [Key features](#key-features)
 * [Usage](#usage)
 * [Contributing](#contributing)
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
 * [License](#license)
 
 ## Purpose 
 The purpose of this software suite is to provide researchers, engineers, and policymakers with a powerful tool for evaluating the performance and economics of desalination and brine treatment systems. By integrating technical process models with economic and environmental analyses, the suite enables users to make informed decisions about technology integration, process optimization, and resource management.
 
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install desalsim==1.0.2
+pip install desalsim==1.0.3
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
@@ -41,15 +51,15 @@
 - Analysis of salt concentration profiles, ion fluxes, energy consumption, and chemical usage
 - Integration of different technologies to optimize process efficiency and resource utilization
 - Economic models for technologies and integrated systems 
 - Output visualization and data export for further analysis 
 
 ### File Descriptions
 
-A brief overview of each file in the project can be found in (https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/file-description). 
+A brief overview of each file in the project can be found in [File description file](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/File_description.md). 
 
 ## Usage 
 Each simulation model serves as a standalone tool for analyzing the performance of a specific desalination or brine treatment technology. Before running the simulation, ensure that you have provided the necessary input parameters, such as feed flow rates, salinity levels, membrane properties, heat sources, and operating conditions.
 
 The simulation results, including salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs, will be generated based on the specified inputs and displayed in the console output or saved to output files for further analysis.
 
 However, simulation models of more than one technology can be combined to simulate and evaluate the performance of a treatment chain (desalination and brine treatment system). In this case, the output flow rates and stream concentrate are the input data for the next technology.
```

### Comparing `desalsim-1.0.2/example/__init__.py` & `desalsim-1.0.3/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/example/comparison.py` & `desalsim-1.0.3/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/example/constants.py` & `desalsim-1.0.3/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/example/economic_f.py` & `desalsim-1.0.3/example/economic_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #costs calculations functions 
-from Desalsim import constants 
+from desalsim import constants 
 
 #%%
 #symbols:
 #hr-> hours
 #lf -> lifetime 
 #el -> electricity
 #s-> steam
```

### Comparing `desalsim-1.0.2/example/ed_unit_f.py` & `desalsim-1.0.3/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/example/edbm_unit_f.py` & `desalsim-1.0.3/example/edbm_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math 
 import numpy as np
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
-from Desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim import scaleup
 
 #%%
 #Molecular weight 
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/example/efc_unit_f.py` & `desalsim-1.0.3/example/efc_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 import time
 import numpy as np
 from scipy import interpolate
 import scipy.interpolate as interpolate
 from sklearn.linear_model import LinearRegression
 from collections import namedtuple
-from Desalsim import scaleup
-from Desalsim.density_calc import density_calc 
+from desalsim import scaleup
+from desalsim.density_calc import density_calc 
 # import pitzer_model_3phases_w
-from Desalsim import constants 
+from desalsim import constants 
 #Set initial time to calculate the elapsed time of the calculations
 time0=time.time()
 MW_so4=32.064+4*15.999
 
 #input data
 Qf=100 #m3/hr
 C_i_in=[20.16, 27.87, 0.50, 0.0, 0.12, 14.66]
```

### Comparing `desalsim-1.0.2/example/example_1.py` & `desalsim-1.0.3/example/example_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #Import functions 
-from Desalsim.nanofiltration_unit_f import OsmoticPressure
-from Desalsim.nanofiltration_unit_f import NFMass
-from Desalsim.nanofiltration_unit_f import NfEnergy
+from desalsim import density_calc
+from desalsim import constants
+from desalsim import scaleup
 
-from Desalsim.mfpfr_unit_f import MFPFRCALC
-from Desalsim.mfpfr_unit_f import HClAddition
-from Desalsim.mfpfr_unit_f import energycons
+from desalsim.nanofiltration_unit_f import NFMass
+from desalsim.nanofiltration_unit_f import OsmoticPressure
+from desalsim.nanofiltration_unit_f import NfEnergy
 
-from Desalsim.ed_unit_f import ElectrodialysisCalc
+from desalsim.mfpfr_unit_f import MFPFRCALC
+from desalsim.mfpfr_unit_f import HClAddition
+from desalsim.mfpfr_unit_f import energycons
 
-from Desalsim.edbm_unit_f import EDBMCalc
+from desalsim.ed_unit_f import ElectrodialysisCalc
 
-from Desalsim.economic_f import revenue
-from Desalsim.economic_f import econom
+from desalsim.edbm_unit_f import EDBMCalc
+
+from desalsim.economic_f import econom
+from desalsim.economic_f import revenue
 
-from Desalsim.density_calc import density_calc
-from Desalsim import constants
-from Desalsim import scaleup
 import numpy as np
 import pandas as pd
 import math
 
 
 #%%Constants
```

### Comparing `desalsim-1.0.2/example/example_2.py` & `desalsim-1.0.3/example/example_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #Scenario 2
 ##treatment train: NF-> MED-> THERMAL CRYST                 
-from Desalsim.nanofiltration_unit_f import OsmoticPressure
-from Desalsim.nanofiltration_unit_f import NFMass
-from Desalsim.nanofiltration_unit_f import NfEnergy
+from desalsim.nanofiltration_unit_f import OsmoticPressure
+from desalsim.nanofiltration_unit_f import NFMass
+from desalsim.nanofiltration_unit_f import NfEnergy
 
-from Desalsim.med_unit_f import MEDCalculator
+from desalsim.med_unit_f import MEDCalculator
 
-from Desalsim.thermal_cryst_f import thermal_calc
-from Desalsim.thermal_cryst_f import conc_cal
-from Desalsim.thermal_cryst_f import calculate_energy
+from desalsim.thermal_cryst_f import thermal_calc
+from desalsim.thermal_cryst_f import conc_cal
+from desalsim.thermal_cryst_f import calculate_energy
 
 
-from Desalsim import constants
+from desalsim import constants
 
-from Desalsim.economic_f import revenue
-from Desalsim.economic_f import econom
+from desalsim.economic_f import revenue
+from desalsim.economic_f import econom
 
-from Desalsim import scaleup
-from Desalsim.density_calc import density_calc
+from desalsim import scaleup
+from desalsim.density_calc import density_calc
 import numpy as np
 import pandas as pd
 #%%
 #Molecular weight 
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
```

### Comparing `desalsim-1.0.2/example/med_unit_f.py` & `desalsim-1.0.3/example/med_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Desalsim.density_calc import density_calc 
+from desalsim.density_calc import density_calc 
 #%%calculations 
 class MEDCalculator:
     """
     A class used to represent Mass Balance for Multi-Effect Distillation 
 
     ...
```

### Comparing `desalsim-1.0.2/example/mfpfr_unit_f.py` & `desalsim-1.0.3/example/mfpfr_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
-from Desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim import scaleup
 import math
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/example/nanofiltration_unit_f.py` & `desalsim-1.0.3/example/nanofiltration_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import numpy as np
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
 import math
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/example/ro_unit_f.py` & `desalsim-1.0.3/example/ro_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
 #%%
 #%%constants
 R=8.31446261815324 #gas constant
 T=20+273.15 #K
 MW_Na=22.99
 MW_cl=35.453
 MW_so4=32.064+4*15.999
```

### Comparing `desalsim-1.0.2/example/thermal_cryst_f.py` & `desalsim-1.0.3/example/thermal_cryst_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
-from Desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim import scaleup
 
 #%%
     #Molecular weight 
 MW_Na=constants.MW_Na
 MW_cl=constants.MW_cl
 MW_so4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-1.0.2/setup.py` & `desalsim-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='desalsim',
-      version='1.0.2',
+      version='1.0.3',
       packages=find_packages(),
-      url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
+      url="https://github.com/rodoulak/desalsim.git",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
-          "numpy==1.21.5",
-          "pandas==1.4.4",  # Include pandas as a dependency
-          "scipy==1.9.1", # For figures 
-          "matplotlib==3.5.2", # For figures 
-          "scikit-learn==1.0.2",
-          "plotly>=5.9.0", 
-          "openpyxl==3.0.10",  #read data from excel file
+          "numpy==1.26.4",
+          "pandas==2.2.2",  # Include pandas as a dependency
+          "scipy==1.13.0", # For figures 
+          "matplotlib==3.8.4", # For figures 
+          "scikit-learn==1.4.2",
+          "plotly==5.22.0", 
+          "openpyxl==3.1.2",  #read data from excel file
       ],
       long_description= description,
       long_description_content_type="text/markdown",
       )
```

### Comparing `desalsim-1.0.2/tests/economic_unittest.py` & `desalsim-1.0.3/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/ed_unittest.py` & `desalsim-1.0.3/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/edbm_unittest.py` & `desalsim-1.0.3/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/med_unittest.py` & `desalsim-1.0.3/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/mfpfr_unittest.py` & `desalsim-1.0.3/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/nanofiltration_unittest.py` & `desalsim-1.0.3/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.2/tests/thermal_cryst_unittest.py` & `desalsim-1.0.3/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

