# Comparing `tmp/sage_lib-0.1.5.1.tar.gz` & `tmp/sage_lib-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.1.tar", last modified: Sat May 11 07:21:27 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.2.tar", last modified: Fri May 17 08:26:29 2024, max compression
```

## Comparing `sage_lib-0.1.5.1.tar` & `sage_lib-0.1.5.2.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976934 sage_lib-0.1.5.1/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-11 07:21:27.976754 sage_lib-0.1.5.1/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.1/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.955518 sage_lib-0.1.5.1/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.959659 sage_lib-0.1.5.1/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.1/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.1/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.1/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.1/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.1/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.1/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.1/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-10 17:27:54.000000 sage_lib-0.1.5.1/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.1/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.1/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.1/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.961056 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.963962 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    23500 2024-05-10 17:27:44.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.966535 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5298 2024-05-10 17:25:34.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.1/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.967413 sage_lib-0.1.5.1/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.1/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.1/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.968091 sage_lib-0.1.5.1/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.1/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.1/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60962 2024-05-10 13:07:36.000000 sage_lib-0.1.5.1/sage_lib/main.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.969190 sage_lib-0.1.5.1/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56677 2024-04-03 13:00:04.000000 sage_lib-0.1.5.1/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.5.1/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.970142 sage_lib-0.1.5.1/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.970960 sage_lib-0.1.5.1/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.1/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    27088 2024-05-10 17:27:44.000000 sage_lib-0.1.5.1/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.975300 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976400 sage_lib-0.1.5.1/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.1/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976560 sage_lib-0.1.5.1/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3657 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-11 07:21:27.976972 sage_lib-0.1.5.1/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-11 07:21:06.000000 sage_lib-0.1.5.1/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.179460 sage_lib-0.1.5.2/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-17 08:26:29.179257 sage_lib-0.1.5.2/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.2/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.157737 sage_lib-0.1.5.2/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.161800 sage_lib-0.1.5.2/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.2/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.2/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.2/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.2/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.2/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.2/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.2/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.2/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.2/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.2/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.2/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.163128 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.165962 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5381 2024-05-16 15:28:23.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24115 2024-05-16 15:36:29.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.168505 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     9849 2024-05-16 15:55:52.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.2/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.169386 sage_lib-0.1.5.2/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.2/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.2/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.170185 sage_lib-0.1.5.2/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.2/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.2/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60970 2024-05-16 15:27:57.000000 sage_lib-0.1.5.2/sage_lib/main.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.171139 sage_lib-0.1.5.2/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.2/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.2/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.172075 sage_lib-0.1.5.2/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.2/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.172951 sage_lib-0.1.5.2/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.2/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-16 15:06:54.000000 sage_lib-0.1.5.2/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.177692 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.178854 sage_lib-0.1.5.2/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.2/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.2/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.2/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-17 08:26:29.179033 sage_lib-0.1.5.2/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3726 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-17 08:26:29.000000 sage_lib-0.1.5.2/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-17 08:26:29.179506 sage_lib-0.1.5.2/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-17 07:20:53.000000 sage_lib-0.1.5.2/setup.py
```

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.2/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/OutFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,22 @@
 try:
     from sage_lib.IO.structure_handling_tools.structural_file_readers.GEN import GEN
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.GEN: {str(e)}\n")
     del sys
 
-class AtomPositionLoader(CIF, POSCAR, XYZ, SI, PDB, ASE, AIMS, GEN):
+try:
+    from sage_lib.IO.structure_handling_tools.structural_file_readers.DUMP import DUMP
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing sage_lib.IO.structure_handling_tools.structural_file_readers.GEN: {str(e)}\n")
+    del sys
+
+class AtomPositionLoader(CIF, POSCAR, XYZ, SI, PDB, ASE, AIMS, GEN, DUMP):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         CIF.__init__(self, name=name, file_location=file_location)
         POSCAR.__init__(self, name=name, file_location=file_location)
         XYZ.__init__(self, name=name, file_location=file_location)
         SI.__init__(self, name=name, file_location=file_location)
         PDB.__init__(self, name=name, file_location=file_location)
         ASE.__init__(self, name=name, file_location=file_location)
@@ -80,25 +87,27 @@
                             'POSCAR': 'export_as_POSCAR',
                             'XYZ': 'export_as_XYZ',
                             'SI': 'export_as_SI',
                             'PDB': 'export_as_PDB',
                             'ASE': 'export_as_ASE',
                             'AIMS': 'export_as_AIMS',
                             'GEN': 'export_as_GEN',
+                            'DUMP': 'export_as_DUMP',
                             }
 
         self.import_dict = {
                             'CIF': 'read_AIMS',
                             'POSCAR': 'read_POSCAR',
                             'XYZ': 'read_XYZ',
                             'SI': 'read_SI',
                             'PDB': 'read_PDB',
                             'ASE': 'read_ASE',
                             'AIMS': 'read_AIMS',
                             'GEN': 'read_GEN',
+                            'DUMP': 'read_DUMP',
                             }
 
                             
     def read(self, source:str='VASP', file_location:str=None):
         metodo = getattr(self, self.import_dict[source.upper()], None)
         if callable(metodo):
             metodo(file_location)
```

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         Type: list of str or None
         Example: ["Fe", "N",  "N", "N", "N", "N", "C", "C", "C"] (for a structure with these atoms in sequence)
         Size: Length equal to the total number of atoms.
         Additional Information: Provides a straightforward way to identify each atom's type.
         self._fullAtomLabelString:
         '''
         self._time = None
+        self._timestep = None 
 
         self._fullAtomLabelString = None  # Concatenated string of all atom labels. Type: str or None. Example: "FeFeFeNNNNNNNCCCCCCCCCCCCCCCHHHHHHHHHHHHHHHH"
         self._atomPositions_tolerance = 1e-2  # Tolerance for position comparison. Type: float
         self._distance_matrix = None  # Distance matrix between atoms. Type: np.array or None
         self._kdtree = None
 
         # == == Molecular / atomistic representations == == #
@@ -176,16 +177,19 @@
         self._magnetization = None  # Magnetization. Type: float or None
         self._total_force = None  # Total force. Type: np.array or None
         self._force = None  # Total force. Type: np.array or None
 
         self._E = None  # Total energy. Type: float or None
         self._Edisp = None  # Dispersion energy. Type: float or None
 
-        self._IR_position = None  # IR positions for a finite diference avaluation. Type: FxNx3
-        self._IR_displacement = None  # IR displacement. Type: np.array or None
+        self._dynamical_eigenvalues = None  # array Type: N
+        self._dynamical_eigenvector = None  # array Type: Nx3
+        self._dynamical_eigenvalues_fractional = None  # array Type: Nx3
+        self._dynamical_eigenvector_diff = None  # array Type: Nx3
+        self._dynamical_eigenvector_diff_fractional = None  # array Type: Nx3
 
         self._mass = None # 
         self._mass_list = None # 
 
         self.info_system = {}
         self.info_atoms = {}
         
@@ -415,14 +419,36 @@
         if self._mass_list is list:
             return np.array(self._mass_list)
         else:
             self._mass_list = np.array([ float(self.atomic_mass[atom_label]) for atom_label in self.atomLabelsList], np.float64)
             return self._mass_list
 
     @property
+    def time(self):
+        """
+
+        """
+        if self.is_number(self._time):
+            return self._time
+        else:
+            self._time = 0
+            return self._time
+
+    @property
+    def timestep(self):
+        """
+
+        """
+        if self.is_number(self._timestep):
+            return self._timestep
+        else:
+            self._timestep = 0
+            return self._timestep
+
+    @property
     def mass(self):
         """
 
         """
         if self._mass is float:
             return self._mass
         else:
```

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     del sys
 
 class POSCAR(FileManager, AtomicProperties):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         FileManager.__init__(self, name=name, file_location=file_location)
         AtomicProperties.__init__(self)
 
-    def export_as_POSCAR(self, file_location:str=None, dimer:int=False, v:bool=False) -> bool:
+    def export_as_POSCAR(self, file_location:str=None, v:bool=False) -> bool:
         file_location  = file_location  if not file_location  is None else self.file_location+'POSCAR' if self.file_location is str else self.file_location
 
         self.group_elements_and_positions()
 
         with open(file_location, 'w') as file:
             # Comentario inicial
             file.write(f'POSCAR : JML code \n')
@@ -62,19 +62,18 @@
             for i, atom in enumerate(self.atomPositions if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else self.atomPositions_fractional):
                 coords = '\t'.join(['{:>18.15f}'.format(n) for n in atom])
                 constr = '\t'.join(['T' if n else 'F' for n in self.atomicConstraints[i]]) if self.selectiveDynamics else ''
                 file.write(f'\t{coords}\t{constr}\n')
 
             # Comentario final (    opcional)
             file.write('Comment_line\n')
-            if not self.dynamical_eigenvector_diff is None: 
+            if hasattr(self, 'dynamical_eigenvector_diff') and not self.dynamical_eigenvector_diff is None: 
                 for i, atom in enumerate(self.dynamical_eigenvector_diff if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else self.dynamical_eigenvector_diff_fractional):
                     coords = '\t'.join(['{:>18.15f}'.format(n) for n in atom])
                     file.write(f'\t{coords}\n')
-
                 
     def read_POSCAR(self, file_location:str=None):
         file_location = file_location if type(file_location) == str else self.file_location
         lines = [n for n in self.read_file(file_location) ]
         
         self._comment = lines[0].strip()
         self._scaleFactor = list(map(float, lines[1].strip().split()))
```

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.2/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/__init__.py` & `sage_lib-0.1.5.2/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.2/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.2/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.2/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.2/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/main.py` & `sage_lib-0.1.5.2/sage_lib/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
     PT.handleBLENDER( values={f'{plot}':values}  )
 
 def add_arguments(parser):
     """
     Adds common arguments to the given subparser. This includes arguments for file paths, 
     verbosity, and other common settings used across various sub-commands.
     """
-    structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB']
+    structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB', 'DUMP']
     parser.add_argument('--path', type=str, default='.', help='Path to the files directory')
     parser.add_argument('--source', type=str, choices=structure_list, help='Source of calculation from which the files originate: VASP, molecular_dynamics, or force_field (default: VASP)')
     
     parser.add_argument('--forces-tag', type=str, default='forces', help='')
     parser.add_argument('--energy-tag', type=str, default='E', help='')
 
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
```

### Comparing `sage_lib-0.1.5.1/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.2/sage_lib/master/AtomicProperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,15 @@
                 'H': 1, 'He': 2, 'Li': 3, 'Be': 4, 'B': 5, 'C': 6, 'N': 7, 'O': 8, 'F': 9, 'Ne': 10, 'Na': 11, 'Mg': 12, 'Al': 13, 'Si': 14, 'P': 15,
                 'S': 16, 'Cl': 17, 'Ar': 18, 'K': 19, 'Ca': 20, 'Sc': 21, 'Ti': 22, 'V': 23, 'Cr': 24, 'Mn': 25, 'Fe': 26, 'Co': 27, 'Ni': 28, 'Cu': 29,
                 'Zn': 30, 'Ga': 31, 'Ge': 32, 'As': 33, 'Se': 34, 'Br': 35, 'Kr': 36, 'Rb': 37, 'Sr': 38, 'Y': 39, 'Zr': 40, 'Nb': 41, 'Mo': 42, 'Tc': 43,
                 'Ru': 44, 'Rh': 45, 'Pd': 46, 'Ag': 47, 'Cd': 48, 'In': 49, 'Sn': 50, 'Sb': 51, 'Te': 52, 'I': 53, 'Xe': 54, 'Cs': 55, 'Ba': 56, 'Lu': 71,
                 'Hf': 72, 'Ta': 73, 'W': 74, 'Re': 75, 'Os': 76, 'Ir': 77, 'Pt': 78, 'Au': 79, 'Hg': 80, 'Tl': 81, 'Pb': 82, 'Bi': 83, 'Po': 84, 'At': 85,
                 'Rn': 86, 'Fr': 87, 'Ra': 88, 'Ac': 89, 'Th': 90, 'U': 92, 'Np': 93, 'Pu': 94, 'X': 99
                                 }
+        self._atomic_name = {value: key for key, value in self._atomic_numbers.items()}
         
         self._Z = self._atomic_numbers
 
         self._element_names = {
             'H': 'hydrogen', 'He': 'helium', 'Li': 'lithium', 'Be': 'beryllium', 'B': 'boron', 'C': 'carbon', 'N': 'nitrogen', 'O': 'oxygen',
             'F': 'fluorine', 'Ne': 'neon', 'Na': 'sodium', 'Mg': 'magnesium', 'Al': 'aluminium', 'Si': 'silicon', 'P': 'phosphorus', 'S': 'sulfur',
             'Cl': 'chlorine', 'Ar': 'argon', 'K': 'potassium', 'Ca': 'calcium', 'Sc': 'scandium', 'Ti': 'titanium', 'V': 'vanadium', 'Cr': 'chromium',
@@ -160,15 +161,17 @@
             'Dy': 162.5, 'Ho': 164.93033, 'Er': 167.259, 'Tm': 168.93422, 'Yb': 173.04, 'Lu': 174.9668, 'Hf': 178.49, 'Ta': 180.94788,
             'W': 183.84, 'Re': 186.207, 'Os': 190.23, 'Ir': 192.217, 'Pt': 195.084, 'Au': 196.966569, 'Hg': 200.592, 'Tl': 204.38,
             'Pb': 207.2, 'Bi': 208.98040, 'Th': 232.03805, 'Pa': 231.03588, 'U': 238.05078, 'Np': 237.0, 'Pu': 244.0, 'Am': 243.0,
             'Cm': 247.0, 'Bk': 247.0, 'Cf': 251.0, 'Es': 252.0, 'Fm': 257.0, 'Md': 258.0, 'No': 259.0, 'Lr': 262.0, 'Rf': 267.0,
             'Db': 270.0, 'Sg': 271.0, 'Bh': 270.0, 'Hs': 277.0, 'Mt': 276.0, 'Ds': 281.0, 'Rg': 280.0, 'Cn': 285.0, 'Nh': 284.0,
             'Fl': 289.0, 'Mc': 288.0, 'Lv': 293.0, 'Ts': 294.0, 'Og': 294.0
                                 }
-        
+
+        self._atomic_mass_list = [ self._atomic_mass.get(self._atomic_name.get(N, None), None) for N in range(1,100) ]
+  
         self._covalent_radii = {
             'H' :  .31, 'He':  .28, 'Li': 1.28, 'Be':  .96, 'B' :  .84, 'C' :  .76, 'N' :  .71, 'O' :  .66, 'F': .57,
             'Ne':  .58, 'Na': 1.66, 'Mg': 1.41, 'Al': 1.21, 'Si': 1.11, 'P' : 1.07, 'S' : 1.05, 'Cl': 1.02,
             'Ar': 1.06, 'K' : 1.03, 'Ca': 1.76, 'Sc': 1.70, 'Ti': 1.60, 'V' : 1.53, 'Cr': 1.39, 'Mn': 1.39,
             'Fe': 1.32, 'Co': 1.26, 'Ni': 1.24, 'Cu': 1.32, 'Zn': 1.22, 'Ga': 1.22, 'Ge': 1.20, 'As': 1.19,
             'Se': 1.20, 'Br': 1.20, 'Kr': 1.16, 'Rb': 2.20, 'Sr': 1.95, 'Y' : 1.90, 'Zr': 1.75, 'Nb': 1.64,
             'Mo': 1.54, 'Tc': 1.47, 'Ru': 1.46, 'Rh': 1.42, 'Pd': 1.39, 'Ag': 1.45, 'Cd': 1.44, 'In': 1.42,
```

### Comparing `sage_lib-0.1.5.1/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.2/sage_lib/master/FileManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,18 +94,20 @@
     @file_location.deleter
     def file_location(self):
         print("Deleting file_location")
         del self._file_location
 
     @staticmethod
     def is_number(s):
+        if s is None:
+            return False
         try:
             float(s)
             return True
-        except ValueError:
+        except (ValueError, TypeError):
             return False
         
     def is_numpy_array_Nx3(self, variable):
         if variable is not False:  # Asegúrate de que la variable no es False
             variable = np.array(variable)  # Convierte la variable a un array de NumPy si aún no lo es
             if variable.ndim == 2 and variable.shape[1] == 3:  # Verifica que sea 2D y de tamaño Nx3
                 return True
```

### Comparing `sage_lib-0.1.5.1/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.2/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.2/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.2/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.2/sage_lib/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.2/sage_lib/partition/PartitionManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,23 +280,24 @@
 
         Returns:
         None
         """
         source = self._identify_file_type(file_location) if source is None else source
 
         if subfolders:
-            self.read_subfolder(file_location=file_location, source=source, verbose=verbose)
+            self.readSubFolder(file_location=file_location, source=source, verbose=verbose)
             return
 
         # Define a strategy for each source format to simplify the conditional structure
         source_strategy = {
             'VASP': self.read_vasp_folder,
             'TRAJ': self.read_traj,
             'XYZ': self.read_XYZ,
-            'OUTCAR': self.read_OUTCAR
+            'OUTCAR': self.read_OUTCAR,
+            'DUMP': self.read_dump,
         }
 
         try:
             # Attempt to read using a specific strategy for the source format
             if source.upper() in source_strategy:
                 source_strategy[source.upper()](file_location=file_location, add_container=True,
                                                 verbose=verbose, energy_tag=energy_tag, forces_tag=forces_tag)
@@ -352,16 +353,43 @@
             If available, time information is also stored.
         """
         file_location = file_location if type(file_location) == str else self.file_location
         SR = SingleRun(file_location)
         SR.read_structure(file_location=file_location, source=source) 
         self.add_container(container=SR)
 
+    def read_dump(self, file_location:str=None, add_container:bool=True, verbose=False, **kargs):
+        '''
+        '''
+        file_location = file_location if type(file_location) == str else self.file_location
+
+        lines =list(self.read_file(file_location,strip=False))
+        container = []
+
+        for i, line in enumerate(lines):
+            if line.startswith("ITEM: TIMESTEP"):
+                SR = SingleRun(file_location)
+                SR.AtomPositionManager = AtomPosition()
+                SR.AtomPositionManager.read_DUMP(lines=lines[i:])
+
+                container.append(SR)
+
+                if add_container and SR.AtomPositionManager is not None: 
+                        self.add_container(container=SR)
+
+                if verbose: 
+                    try: 
+                        print(f' >> READ dump :: frame {len(container)} - atoms {num_atoms}')
+                    except Exception as e:
+                        print(f'Verbose output failed due to an error: {e}')
+                        print('Skipping line due to the above error.')
+                            
+        return container
 
-    def read_traj(self, file_location:str=None, add_container:bool=True, verbose=False):
+    def read_traj(self, file_location:str=None, add_container:bool=True, verbose=False, *args):
         """
         Reads a trajectory file and stores each frame along with its time information.
 
         Args:
             file_location (str, optional): The file path of the trajectory file.
             verbose (bool, optional): If True, enables verbose output.
 
@@ -418,15 +446,15 @@
 
     def read_OUTCAR(self, file_location:str=None, add_container:bool=True, verbose=False, **kwargs):
         '''
         '''
         OF = OutFileManager(file_location)
         OF.readOUTCAR()
 
-        if not type(OF.dynamical_eigenvector) is None: 
+        if not OF.dynamical_eigenvector is None: 
 
             for dynamical_eigenvalues, dynamical_eigenvector, dynamical_eigenvector_diff in zip(OF.dynamical_eigenvalues, OF.dynamical_eigenvector, OF.dynamical_eigenvector_diff):
                 SR = SingleRun(file_location)   
                 SR._AtomPositionManager = OF.AtomPositionManager[0]
                 SR._AtomPositionManager._atomPositions = dynamical_eigenvector
                 SR._AtomPositionManager._dynamical_eigenvector = dynamical_eigenvector
                 SR._AtomPositionManager._dynamical_eigenvalues = dynamical_eigenvalues
```

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.2/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.2/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.2/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.2/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.2/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.1/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.2/sage_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
 sage_lib/IO/structure_handling_tools/PeriodicSystem.py
 sage_lib/IO/structure_handling_tools/__init__.py
 sage_lib/IO/structure_handling_tools/plot.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
 sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
 sage_lib/descriptor/MBTR.py
```

