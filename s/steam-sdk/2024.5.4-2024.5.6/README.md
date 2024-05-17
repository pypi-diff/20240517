# Comparing `tmp/steam-sdk-2024.5.4.tar.gz` & `tmp/steam-sdk-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-sdk-2024.5.4.tar", last modified: Tue May 14 13:15:47 2024, max compression
+gzip compressed data, was "steam-sdk-2024.5.6.tar", last modified: Fri May 17 08:33:07 2024, max compression
```

## Comparing `steam-sdk-2024.5.4.tar` & `steam-sdk-2024.5.6.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.567932 steam-sdk-2024.5.4/
--rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5837 2024-05-14 13:15:47.565931 steam-sdk-2024.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 13:15:47.567932 steam-sdk-2024.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-05-14 13:13:44.000000 steam-sdk-2024.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.141388 steam-sdk-2024.5.4/steam_sdk/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.159387 steam-sdk-2024.5.4/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEvent.py
--rw-rw-rw-   0        0        0    30954 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEventLHC.py
--rw-rw-rw-   0        0        0   135856 2024-05-14 07:53:34.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.160387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.162387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.174388 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.177388 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.185387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.188387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.196387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.199387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.223388 steam-sdk-2024.5.4/steam_sdk/builders/
--rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderAPDL_CT.py
--rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderCosim.py
--rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160548 2024-05-14 10:56:54.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    53474 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderPySIGMA.py
--rw-rw-rw-   0        0        0    66165 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderTFM.py
--rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.225387 steam-sdk-2024.5.4/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.229388 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.232388 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.236388 steam-sdk-2024.5.4/steam_sdk/cosims/
--rw-rw-rw-   0        0        0    26984 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/cosims/CoSimPyCoSim.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.293389 steam-sdk-2024.5.4/steam_sdk/data/
--rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataAPDLCTOptions.py
--rw-rw-rw-   0        0        0    13080 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DataCoSim.py
--rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    93048 2024-05-13 19:23:49.000000 steam-sdk-2024.5.4/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataFiQuSOptions.py
--rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataLEDETOptions.py
--rw-rw-rw-   0        0        0     5330 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCommon.py
--rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    12150 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCosim.py
--rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelParsimDakota.py
--rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.5.4/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0      625 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPlot.py
--rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataProteCCTOptions.py
--rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQOptions.py
--rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyCoSim.py
--rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMA.py
--rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMAOptions.py
--rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParams.py
--rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0    12733 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0     6207 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataTFM.py
--rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.312388 steam-sdk-2024.5.4/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverANSYS.py
--rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     4278 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1894 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPySIGMA.py
--rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.399387 steam-sdk-2024.5.4/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOSIM.py
--rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2614 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0     3760 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserFile.py
--rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    65086 2024-05-14 13:06:42.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyBBQ.py
--rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyCoSim.py
--rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPySIGMA.py
--rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    58167 2024-04-30 14:26:16.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCircuits.py
--rw-rw-rw-   0        0        0     9687 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCosims.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.410388 steam-sdk-2024.5.4/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.418905 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.486417 steam-sdk-2024.5.4/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0     8480 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterGriddedData.py
--rw-rw-rw-   0        0        0    20627 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.491415 steam-sdk-2024.5.4/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0    15676 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.528417 steam-sdk-2024.5.4/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/utils/MatrixOperations.py
--rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     3846 2024-05-13 21:24:50.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/utils/attribute_model.py
--rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/compare_simulations.py
--rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.5.4/steam_sdk/utils/correct_RRR_NIST.py
--rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/delete_if_existing.py
--rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.5.4/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.5.4/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.5.4/steam_sdk/utils/read_settings_file.py
--rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/reformat_figure.py
--rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.538931 steam-sdk-2024.5.4/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.540931 steam-sdk-2024.5.4/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.540931 steam-sdk-2024.5.4/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.541932 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.542930 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.545932 steam-sdk-2024.5.4/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     5837 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7694 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1781 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:07.010658 steam-sdk-2024.5.6/
+-rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5837 2024-05-17 08:33:06.992653 steam-sdk-2024.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:33:07.010658 steam-sdk-2024.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-05-17 08:32:17.000000 steam-sdk-2024.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.021652 steam-sdk-2024.5.6/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.040653 steam-sdk-2024.5.6/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisEvent.py
+-rw-rw-rw-   0        0        0    30553 2024-05-16 11:43:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisEventLHC.py
+-rw-rw-rw-   0        0        0   136171 2024-05-16 12:10:18.000000 steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.041653 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.080658 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.094653 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.096653 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.104660 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.108660 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.114652 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.122653 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.162656 steam-sdk-2024.5.6/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderAPDL_CT.py
+-rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderCosim.py
+-rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160566 2024-05-17 07:18:25.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    53553 2024-05-16 11:53:52.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderPySIGMA.py
+-rw-rw-rw-   0        0        0    66165 2024-05-13 19:22:01.000000 steam-sdk-2024.5.6/steam_sdk/builders/BuilderTFM.py
+-rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.164654 steam-sdk-2024.5.6/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.167654 steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.168654 steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.171652 steam-sdk-2024.5.6/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0    28165 2024-05-16 19:57:49.000000 steam-sdk-2024.5.6/steam_sdk/cosims/CoSimPyCoSim.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.296653 steam-sdk-2024.5.6/steam_sdk/data/
+-rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataAPDLCTOptions.py
+-rw-rw-rw-   0        0        0    13117 2024-05-16 11:43:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DataCoSim.py
+-rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    93038 2024-05-16 11:43:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataFiQuSOptions.py
+-rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataLEDETOptions.py
+-rw-rw-rw-   0        0        0     5330 2024-05-13 19:22:01.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelCommon.py
+-rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    12432 2024-05-16 13:49:56.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelCosim.py
+-rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/data/DataModelParsimDakota.py
+-rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.5.6/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0      625 2024-05-08 10:41:57.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPlot.py
+-rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataProteCCTOptions.py
+-rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPyBBQOptions.py
+-rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPyCoSim.py
+-rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPySIGMA.py
+-rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataPySIGMAOptions.py
+-rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DataRoxieParams.py
+-rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0    12733 2024-05-08 10:41:57.000000 steam-sdk-2024.5.6/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.5.6/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0     6207 2024-05-13 19:22:01.000000 steam-sdk-2024.5.6/steam_sdk/data/DataTFM.py
+-rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.360658 steam-sdk-2024.5.6/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverANSYS.py
+-rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     4251 2024-05-17 08:31:18.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     2154 2024-05-16 11:43:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverPySIGMA.py
+-rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.5.6/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.566653 steam-sdk-2024.5.6/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserCOSIM.py
+-rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2803 2024-05-16 13:49:56.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0     3783 2024-05-16 12:00:19.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserFile.py
+-rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    65086 2024-05-14 13:06:42.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserPyBBQ.py
+-rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserPyCoSim.py
+-rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserPySIGMA.py
+-rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    61395 2024-05-16 20:48:44.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.5.6/steam_sdk/parsers/utils_ParserCircuits.py
+-rw-rw-rw-   0        0        0     9688 2024-05-16 13:49:56.000000 steam-sdk-2024.5.6/steam_sdk/parsers/utils_ParserCosims.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.579652 steam-sdk-2024.5.6/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.5.6/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.5.6/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.5.6/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.582653 steam-sdk-2024.5.6/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.5.6/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.640656 steam-sdk-2024.5.6/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0     8480 2024-05-08 10:41:57.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterGriddedData.py
+-rw-rw-rw-   0        0        0    20627 2024-05-08 10:41:57.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.5.6/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.657657 steam-sdk-2024.5.6/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0    15674 2024-05-16 11:43:27.000000 steam-sdk-2024.5.6/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.832655 steam-sdk-2024.5.6/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.5.6/steam_sdk/utils/MatrixOperations.py
+-rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     3846 2024-05-13 21:24:50.000000 steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.5.6/steam_sdk/utils/attribute_model.py
+-rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/compare_simulations.py
+-rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.5.6/steam_sdk/utils/correct_RRR_NIST.py
+-rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/delete_if_existing.py
+-rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.5.6/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.5.6/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.5.6/steam_sdk/utils/read_settings_file.py
+-rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/reformat_figure.py
+-rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.881654 steam-sdk-2024.5.6/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.892654 steam-sdk-2024.5.6/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.893654 steam-sdk-2024.5.6/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.895652 steam-sdk-2024.5.6/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.895652 steam-sdk-2024.5.6/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.5.6/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:06.911652 steam-sdk-2024.5.6/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5837 2024-05-17 08:32:59.000000 steam-sdk-2024.5.6/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7694 2024-05-17 08:32:59.000000 steam-sdk-2024.5.6/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:32:59.000000 steam-sdk-2024.5.6/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1781 2024-05-17 08:32:59.000000 steam-sdk-2024.5.6/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 08:32:59.000000 steam-sdk-2024.5.6/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2024.5.4/PKG-INFO` & `steam-sdk-2024.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.4
+Version: 2024.5.6
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: SDK,STEAM,API,CERN
+Keywords: API,SDK,STEAM,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.5.4/setup.py` & `steam-sdk-2024.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 build_require = ["setuptools==69.2.0"]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="steam-sdk",
-    version="2024.5.4",
+    version="2024.5.6",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={"STEAM", "API", "SDK", "CERN"},
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEvent.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisEvent.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEventLHC.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisEventLHC.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         'output_directory_parsim_sweep_files': os.path.join(os.getcwd(), 'output', 'parsim_sweep_files'),
         'output_directory_initialization_file_viewer': os.path.join(os.getcwd(), 'output', 'initialization_files_viewer'),
         'path_postmortem_offline_data_folder': None,
         'filepath_to_temp_viewer_csv': None,
         'path_output_pdf_report': None ,
         'metrics_to_calculate':None,
         'local_library_path': None,
+        "timeout_s": None
     }
 
     # Fill up non user specific keys of the default dictionary with keys from the settings system.yaml
     with open(settings_file_path, 'r') as yaml_file:
         yaml = ruamel.yaml.YAML(typ="safe", pure=True)
         settings_file_yaml_data = yaml.load(yaml_file)
 
@@ -94,14 +95,15 @@
         analyze_RCD_RCO_event(settings_dictionary,os.path.join(os.getcwd(), input_csv_file), flag_run_software, software, file_counter, modify_model_steps)
     else: # All other double circuits like RQs and RCBX can be run with this function as this is how it is implemented in steam_sdk:
         analyze_circuit_event(settings_dictionary,os.path.join(os.getcwd(), input_csv_file), circuit_type, flag_run_software, flag_calculate_metrics, software, file_counter, circuit_name)
 
 def analyze_circuit_event(settings_dictionary: dict, input_csv_file: str,circuit_type: str, flag_run_software: bool, flag_calculate_metrics: bool, software: str, file_counter: int, circuit_name: str):
     aSTEAM = AnalysisSTEAM()
     update_attributes_from_settings_dictionary(aSTEAM, settings_dictionary)
+    timeout_s = settings_dictionary["timeout_s"]
 
     if software == 'PSPICE':
         local_folder = settings_dictionary['local_PSPICE_folder']
         print(f"Changed local folder to {local_folder}")
     elif software == 'XYCE':
         local_folder = settings_dictionary['local_XYCE_folder']
         print(f"Changed local folder to {local_folder}")
@@ -175,15 +177,16 @@
                                                                           path_tdms_files=None,
                                                                           path_output_measurement_files=None,
                                                                           path_output=local_folder),
                                       path_postmortem_offline_data_folder=settings_dictionary['path_postmortem_offline_data_folder'],
                                       path_to_configurations_folder = settings_dictionary['directory_config_files'],
                                       filepath_to_temp_viewer_csv = settings_dictionary['filepath_to_temp_viewer_csv']
                                       ),
-        'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name="from_ParsimEvent_step", simulation_numbers=[file_counter]),
+        'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name="from_ParsimEvent_step", simulation_numbers=[file_counter],
+        timeout_s = timeout_s ),
 
         "RunViewer": RunViewer(type="RunViewer",
                                file_name_transients=settings_dictionary['filepath_to_temp_viewer_csv'],
                                flag_analyze=True,
                                verbose=True,
                                flag_save_figures=True, viewer_name="viewer_1",
                                path_output_pdf_report=settings_dictionary['path_output_pdf_report']),
@@ -208,20 +211,14 @@
     if flag_run_software == True: AnalysisStepSequence.append('run_simulation')
 
     # If the flag for running a simulation is set, the run_simulation step will be appended to the analysis step sequence
     if flag_calculate_metrics== True: AnalysisStepSequence.extend(["RunViewer", "CalculateMetrics"])
 
     aSTEAM.data_analysis.AnalysisStepSequence = AnalysisStepSequence
 
-    # If th dictionary modify model steps is defined than we add these steps to the definition and the sequence --> Old piece of code that was needed for Dakota
-    # index_of_runParsimEvent = aSTEAM.data_analysis.AnalysisStepSequence.index('runParsimEvent')
-    # if modify_model_steps:
-    #     aSTEAM.data_analysis.AnalysisStepDefinition.update(modify_model_steps)
-    #     aSTEAM.data_analysis.AnalysisStepSequence[index_of_runParsimEvent:index_of_runParsimEvent] = list(modify_model_steps.keys())
-
     if software == 'PSPICE':
         list_output_file = [os.path.join(aSTEAM.settings.local_PSPICE_folder, f'{circuit_type}', f'{file_counter}',
                                      f'{circuit_type}.cir')]
     elif software == 'XYCE':
         list_output_file = [os.path.join(aSTEAM.settings.local_XYCE_folder, f'{circuit_type}', f'{file_counter}',
                                      f'{circuit_type}.cir')]
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,21 +298,20 @@
         # Change the value of the selected variable
         for v, value in enumerate(step.variable_value):
             BM: Union[BuilderModel, BuilderCosim] = self.list_models[
                 step.model_name]  # original BuilderModel or BuilderCosim object
             case_model = BM.case_model  # model case (magnet, conductor, circuit, cosim)
 
             if 'Conductors[' in step.variable_to_change:  # Special case when the variable to change is the Conductors key
+                idx_conductor = int(step.variable_to_change.split('Conductors[')[1].split(']')[0])
+                conductor_variable_to_change = step.variable_to_change.split('].')[1]
+                old_value = get_attribute_model(case_model, BM, conductor_variable_to_change, idx_conductor)
                 if verbose:
-                    idx_conductor = int(step.variable_to_change.split('Conductors[')[1].split(']')[0])
-                    conductor_variable_to_change = step.variable_to_change.split('].')[1]
                     print(f'Variable {step.variable_to_change} is treated as a Conductors key. Conductor index: #{idx_conductor}. '
                           f'Conductor variable to change: {conductor_variable_to_change}.')
-
-                    old_value = get_attribute_model(case_model, BM, conductor_variable_to_change, idx_conductor)
                     print(f'Variable {conductor_variable_to_change} changed from {old_value} to {value}.')
 
                 if len_new_model_name > 0:  # Make a new copy of the BuilderModel object, and change it
                     self.list_models[step.new_model_name[v]] = deepcopy(BM)
                     BM = self.list_models[step.new_model_name[v]]
 
                     if case_model == 'conductor':
@@ -392,14 +391,15 @@
 
     def step_run_simulation(self, step, verbose: bool = None):
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         software = step.software
         simulation_name = step.simulation_name
         simFileType = step.simFileType
         sim_numbers = step.simulation_numbers
+        timeout_s = step.timeout_s
         if simulation_name == 'from_last_parametric_list':
             sim_numbers = list(self.input_parsim_sweep_df.simulation_number.to_numpy())
             sim_names = list(self.input_parsim_sweep_df.simulation_name.to_numpy())
         elif simulation_name == 'from_SetUpFolder_step':  # todo: this name should probably be changed
             sim_numbers = list(self.input_parsim_sweep_df.simulation_number.to_numpy())
             for step_data in self.data_analysis.AnalysisStepDefinition.values():
                 if step_data.type == 'MakeModel':
@@ -418,15 +418,15 @@
         if len(sim_numbers) != len(set(sim_numbers)):
             raise Exception('Simulation numbers must be unique!')
 
         for sim_name, sim_number in zip(sim_names, sim_numbers):
             if verbose:
                 print('Running simulation of model {} #{} using {}.'.format(simulation_name, sim_number, software))
             # Run simulation
-            self.run_sim(software, sim_name, sim_number, simFileType, verbose)
+            self.run_sim(software, sim_name, sim_number, simFileType, timeout_s, verbose)
 
     def step_postprocess_compare(self, step, verbose: bool = None):
         """
         The postprocessing method is for comparing results between two solutions: e.g., map2d files between FiQuS and SIGMA
         Supported physical quantities: magnetic_flux_density,
         :param step:
         :param verbose:
@@ -468,18 +468,20 @@
             elif self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool'].lower() == 'fiqus':
                 parser_obj.create_map2d_file_from_FiQuS(
                     results_path=Path(os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr), step.simulation_name + ".map2d")),
                     new_file_name=new_file_names[results_name])
             else:
                 raise ValueError("Source tool not yet supported for post-process comparison.")
 
-        if isinstance(step.simulation_numbers, int) and step.physical_quantity != 'magnetic_flux_density':
+        compare_to_reference = isinstance(step.simulation_numbers, int) or isinstance(step.simulation_numbers, str)
+
+        if compare_to_reference and step.physical_quantity != 'magnetic_flux_density':
             raise ValueError("Comparison with ROXIE is only supported for the magnetic flux density.")
 
-        elif isinstance(step.simulation_numbers, int) and step.physical_quantity == 'magnetic_flux_density':
+        elif compare_to_reference and step.physical_quantity == 'magnetic_flux_density':
             source_sim_nbr = step.simulation_numbers
             results_name = f"{self.simulation_numbers_source_tools_and_models[source_sim_nbr]['tool']}_{source_sim_nbr}"
             new_file_names[results_name] = f"{results_name}_b.map2d"
             create_map2d_files()
 
             # Copy ROXIE reference file
             shutil.copy(ref_map2d, step.path_to_saved_files)
@@ -1194,15 +1196,15 @@
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
 
     def run_sim(self, software: str, simulation_name: str, sim_number: int, simFileType: str = None,
-                verbose: bool = False):
+                timeout_s: int =None ,verbose: bool = False):
         """
         Run selected simulation.
         The function applies a different logic for each simulation software.
         """
         if software == 'FiQuS':
             #local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
             #local_analysis_folder = simulation_name + '_' + str(sim_number)
@@ -1214,15 +1216,15 @@
         elif software == 'LEDET':
             #local_LEDET_folder = self._get_local_folder('local_LEDET_folder')
             dLEDET = DriverLEDET(path_exe=self.settings.LEDET_path, path_folder_LEDET=self.settings.local_LEDET_folder, verbose=verbose)
             self.summary = dLEDET.run_LEDET(simulation_name, str(sim_number), simFileType=simFileType)
         elif software == 'PSPICE':
             #local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
             local_model_folder = Path(os.path.join(self.settings.local_PSPICE_folder, simulation_name, str(sim_number))).resolve()
-            dPSPICE = DriverPSPICE(path_exe=self.settings.PSPICE_path, path_folder_PSPICE=local_model_folder, verbose=verbose)
+            dPSPICE = DriverPSPICE(path_exe=self.settings.PSPICE_path, path_folder_PSPICE=local_model_folder, timeout_s = timeout_s, verbose = verbose)
             dPSPICE.run_PSPICE(simulation_name, suffix='')
         elif software == 'PyBBQ':
             #local_PyBBQ_folder = self._get_local_folder('local_PyBBQ_folder')
             local_model_folder_input = os.path.join(self.settings.local_PyBBQ_folder, simulation_name, str(sim_number))
             relative_folder_output = os.path.join(simulation_name, str(sim_number))
             dPyBBQ = DriverPyBBQ(path_exe=self.settings.PyBBQ_path, path_folder_PyBBQ=self.settings.local_PyBBQ_folder,
                                  path_folder_PyBBQ_input=local_model_folder_input, verbose=verbose)
@@ -1379,15 +1381,18 @@
             else:
                 raise Exception(f'Software {software} not supported for the ParsimEvent step.')
 
             # Read input file and run the ParsimEvent analysis
             pec = ParsimEventCircuit(ref_model=self.list_models[model_name], library_path=self.settings.local_library_path, verbose=verbose)
             pec.read_from_input(path_input_file=input_file, flag_append=False)
             if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"]:
-                simulation_numbers = [0 + simulation_numbers[-1], 1 + simulation_numbers[-1]]
+                try:
+                    simulation_numbers = [0 + simulation_numbers[-1], 1 + simulation_numbers[-1]]
+                except:
+                    raise Exception(f'Simulation numbers {simulation_numbers} must be integers.')
                 self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers = simulation_numbers
             pec.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
                                  path_outputfile_event_csv=path_output_event_csv)
 
             quenching_magnet_list = []  # required for families where multiple magnets can quench like RB
             quenching_magnet_time = []
             quenching_current_list = []
@@ -1797,19 +1802,20 @@
                 model_name = row['simulation_name']
                 if verbose: print(f'row {i + 1}: Using model {model_name} as specified in the input file {input_sweep_file}.')
             else:
                 model_name = default_model_name
                 if verbose: print(f'row {i + 1}: Using default model {default_model_name} as initial model.')
 
             # check if simulation number is provided and extract it from file
-            try:
-                # number has to be present & has to be an int (or be parsable into one) for the rest of the code to work
+            if isinstance(row['simulation_number'], str) and not row['simulation_number'].isdigit():
+                print(f'Warning: simulation number at row {i + 1} is not an integer.')
+                simulation_number = row['simulation_number']
+            else:
                 simulation_number = int(row['simulation_number'])
-            except:
-                raise Exception(f'ERROR: no simulation_number provided in csv file {input_sweep_file}.')
+
             if verbose: print(f'changing these fields row # {i + 1}: {row}')
 
             dict_variables_to_change = dict()
 
             # unpack model_data
             if case_model == 'magnet':
                 model_data = self.list_models[model_name].model_data
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2024.5.6/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderAPDL_CT.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderAPDL_CT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderCosim.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderLEDET.py`

 * *Files 0% similar despite different names*

```diff
@@ -1376,23 +1376,23 @@
             elif magnet_type in ['CCT_straight']:
                 # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
                 #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
                 # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows = 1, header = None)
                 # self.Auxiliary.overwrite_inductance_coil_sections = float(df.to_numpy().sum())  # [:-1] to remove last nan
                 HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten for CCT_straight by method self.assignCCTValuesWindings()
             elif magnet_type in ['CWS']:
-                selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
-                                                               f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
-                self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
-                fL_I_fL_L_file = Path.joinpath(self.path_input_file,
-                                               f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
-                self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
-                self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
+                # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
+                #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
+                # self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
+                # fL_I_fL_L_file = Path.joinpath(self.path_input_file,
+                #                                f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                # df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
+                # self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
+                # self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
                 HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten
             else:
                 raise Exception(f'Magnet type not recognized: {magnet_type}.')
 
         # Self-mutual inductances between coil sections, per unit length [H/m]
         self.setAttribute(self.Inputs, 'M_m', self.Auxiliary.overwrite_inductance_coil_sections)
         self.setAttribute(self.Inputs, 'HalfTurnToInductanceBlock', HalfTurnToInductanceBlock)
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             :param sim_number: Simulation number or string that will be used to write the output file
             :param output_path: Output folder
             :param flag_plot_all: Display figures
             :param verbose: If True, display logging information
         :return:
         '''
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
-        sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number
+        sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number  # TODO consider instead: sim_suffix = f'_{sim_number}' if sim_number else ''
 
         # Load model data from the input ROXIE files
         if self.model_data.GeneralParameters.magnet_type in ['multipole']:
             self.loadRoxieData()
         else:
             raise Exception(f'Selected magnet type {sim_name} is not supported for APDL_CT.')
 
@@ -415,15 +415,15 @@
         # Load model data from the input ROXIE files
         if self.model_data.GeneralParameters.magnet_type in ['multipole', 'busbar']:
             self.loadRoxieData()
         # Calculate half-turn electrical order
         self.calc_electrical_order(flag_plot=flag_plot_all, verbose=verbose)
 
         #if library_path != None:
-        if self.model_data.GeneralParameters.magnet_type =='multipole':
+        if self.model_data.GeneralParameters.magnet_type == 'multipole':
             make_folder_if_not_existing(output_path)  # somehow sometimes the output folder does not exist so making sure it is created
             shutil.copyfile(self.path_bh, os.path.join(output_path, 'roxie.bhdata'))
             shutil.copyfile(self.path_map2d, os.path.join(output_path, f"{sim_name}{sim_suffix}_ROXIE_REFERENCE.map2d"))
         else:
             pass # for CCT and Pancake3D no bhdata is needed
         builder_FiQuS = BuilderFiQuS(model_data=self.model_data, roxie_data=self.roxie_data, flag_build=True, verbose=verbose)
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderPySIGMA.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/BuilderTFM.py` & `steam-sdk-2024.5.6/steam_sdk/builders/BuilderTFM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2024.5.6/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/Solenoids.py` & `steam-sdk-2024.5.6/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2024.5.6/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2024.5.6/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/cosims/CoSimPyCoSim.py` & `steam-sdk-2024.5.6/steam_sdk/cosims/CoSimPyCoSim.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,17 +96,27 @@
 
         # Initialize the dictionary that will be used to pass variable values from an output file to a model data object
         self._reset_variables_to_pass()
 
         # Initialize the dictionary that will be used to check convergence at each time window
         self.dict_convergence_variables = {key: {} for key in self.cosim_data.Simulations}  # Assign empty list to all models
 
+        # Check that the variables variables_to_modify_cosim_for_each_time_window have all the same length, if their flag_run_cosim is True
+        dict_check_lengths = {}
+        for model in self.cosim_data.Simulations.values():
+            if model.flag_run_cosim:
+                dict_check_lengths[model.name] = len(model.variables_to_modify_cosim_for_each_time_window)
+                self.n_time_windows = len(model.variables_to_modify_cosim_for_each_time_window)
+        if len(set(list(dict_check_lengths.values()))) > 1:
+            raise Exception(f'The variable variables_to_modify_cosim_for_each_time_window must have the same length in all models that have flag_run_cosim=True. {dict_check_lengths}')
+
         if verbose:
             print(f'PyCoSim initialized with input file {file_model_data}.')
             print(f'Local PyCoSim folder is {self.local_PyCoSim_folder}')
+            print(f'Number of windows: {self.n_time_windows}')
 
     def run(self):
         """
         This runs co-sim
         """
         # Read initial
         # A1 Make the folder structure
@@ -139,39 +149,43 @@
                 self._run_sim(model=model)
                 # TODO add some basic check that the simulation run without errors
                 self._copy_files(model=model)
                 self._copy_variables(model=model, verbose=self.verbose)
 
         # Co-simulation
         # Loop through time windows
-        for tw, time_wind in enumerate(self.cosim_data.Settings.Time_Windows):
+        for tw in range(self.n_time_windows):
             # Reset convergence variables
             flag_converge, list_flag_converge, current_iteration = False, [], 0
             # Reset the dictionary that is used to pass variable values from an output file to a model data object TODO how to pass info from one time window to the next?
             self._reset_variables_to_pass()
             # Loop until convergence is found
             while flag_converge == False:
                 for model_set, model in enumerate(self.cosim_data.Simulations.values()):
                     self.nsti.update(self.sim_number, model_set, tw + 1, current_iteration)
                     # Make model
                     if model.flag_run_cosim:
                         if self.verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}. Iteration {self.nsti.i}.')
+                        extra_variables_to_change: ParametersToModify() = ParametersToModify(
+                            **self.variables_to_pass[model.name]['variables_to_modify_cosim'].dict() |  # Variables to modify at every time windows
+                            model.variables_to_modify_cosim_for_each_time_window[tw].dict())  # Variables to modify at this specific time windows
+
                         write_model_input_files(cosim_data=self.cosim_data, model=model,
                                                 cosim_software='PyCoSim', data_settings=self.data_settings,
-                                                extra_variables_to_change=self.variables_to_pass[model.name]['variables_to_modify_cosim'],
+                                                extra_variables_to_change=extra_variables_to_change,
                                                 nsti=self.nsti, verbose=self.verbose)
                         self._run_sim(model=model)
                         # TODO add some basic check that the simulation run without errors
                         self._copy_files(model=model)
                         self._copy_variables(model=model, verbose=self.verbose)
 
                         # Check convergence
                         list_flag_converge.append(self._check_convergence(model=model))
 
-                flag_converge = all(list_flag_converge)
+                flag_converge = any(list_flag_converge)
                 if not flag_converge:
                     current_iteration = current_iteration + 1
 
         # Post-cosim
         # TODO how to pass info from the last time window to the post-cosim?
         for model_set, model in enumerate(self.cosim_data.Simulations.values()):
             self.nsti.update(self.sim_number, model_set, len(self.cosim_data.Settings.Time_Windows.t_0) + 1, 0)
@@ -393,15 +407,15 @@
         # either relative_tolerance or absolute_tolerance must be fulfilled to pass convergence check
 
         :return:
         :rtype:
         """
 
         #TODO allow checking convergence on a scalar variable, not just on a vector
-        #TODO allow checking convergence on max/min/aveg values rather than on a vector
+        #TODO allow checking convergence on max/min/avg values rather than on a vector
 
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         # Define local folder
         local_folder = self.__find_local_source_folder(model=model)
         if not self.nsti.t in self.dict_convergence_variables[model.name]:
             self.dict_convergence_variables[model.name][self.nsti.t] = {}
@@ -410,40 +424,40 @@
         for check_to_perform in model.convergence_checks_cosim:
             if verbose: print(f'Performing convergence check for model {model.name} on variable {check_to_perform.var_name}.')
 
             # Check whether to add an NSTI suffix between the base name and the extension of the old file name. NSTI: N=simulation number. S=simulation set. T=time window. I=Iteration number
             file_name_relative_path = self._add_nsti_to_file_name(check_to_perform.file_name_relative_path, nsti=self.nsti) if check_to_perform.flag_add_nsti_to_file_name else check_to_perform.file_name_relative_path
             # Get variable value from the source file. Supported formats: .csd, .csv, .mat
             original_file = Path(Path(local_folder), file_name_relative_path).resolve()
-            var_value = get_signals_from_file(full_name_file=original_file, list_signals=check_to_perform.var_name, dict_variable_types={})
+            var_value = get_signals_from_file(full_name_file=original_file, list_signals=check_to_perform.var_name, dict_variable_types={})[check_to_perform.var_name.strip()]
 
             # Add convergence variable values to self.self.dict_convergence_variables
-            self.self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i][check_to_perform.var_name] = var_value
+            self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i][check_to_perform.var_name] = var_value
             if check_to_perform.time_var_name:
                 # Add time vector of the convergence variable values to self.self.dict_convergence_variables
-                time_var_value = get_signals_from_file(full_name_file=original_file, list_signals=check_to_perform.time_var_name, dict_variable_types={})
-                self.self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i][check_to_perform.time_var_name] = time_var_value
+                time_var_value = get_signals_from_file(full_name_file=original_file, list_signals=check_to_perform.time_var_name, dict_variable_types={})[check_to_perform.time_var_name.strip()]
+                self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i][check_to_perform.time_var_name] = time_var_value
 
             # At the first iteration, always return False (no convergence reached yet)
             if self.nsti.i == 0:
                 if verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}.')
                 return False
             else:
-                old_var_value = self.self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i-1][check_to_perform.var_name]
+                old_var_value = self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i-1][check_to_perform.var_name]
                 if check_to_perform.time_var_name:
                     # Interpolate the variable over the time vector (use the time vector of the previous iteration)
-                    old_time_var_value = self.self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i-1][check_to_perform.time_var_name]
+                    old_time_var_value = self.dict_convergence_variables[model.name][self.nsti.t][self.nsti.i-1][check_to_perform.time_var_name]
                     new_var_value_interpolated = interp1d(time_var_value, var_value)(old_time_var_value)
                     var_value = new_var_value_interpolated  # Use the interpolated values
 
                 # Perform relative-tolerance check
                 rel_error = abs(var_value - old_var_value) / abs(old_var_value)
                 # Perform absolute-tolerance check
                 abs_error = abs(var_value - old_var_value)
                 # Check whether converge criteria are met
-                if rel_error < check_to_perform.relative_tolerance or abs_error <= check_to_perform.absolute_tolerance:
+                if np.all(rel_error < check_to_perform.relative_tolerance) or np.all(abs_error <= check_to_perform.absolute_tolerance):
                     flag_converged = True
                     print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}. Convergence reached at iteration {self.nsti.i}. Absolute tolerance: {abs_error} <= {check_to_perform.absolute_tolerance}. Relative tolerance: {rel_error} <= {check_to_perform.relative_tolerance}.')
                 else:
                     flag_converged = False
                     print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}. Convergence not yet reached at iteration {self.nsti.i}. Absolute tolerance: {abs_error}. Relative tolerance: {rel_error}.')
                 return flag_converged
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataAPDLCTOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataAPDLCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         Level 2: Analysis step to run a simulation file
     """
     type: Literal['RunSimulation']
     software: Optional[str] = None
     simulation_name: Optional[str] = None
     simulation_numbers: List[Union[int, str]] = []
     simFileType: Optional[str] = None
+    timeout_s: Optional[int] = None
 
 
 class PostProcessCompare(BaseModel):
     """
         Level 2: Analysis step to run a simulation file
     """
     type: Literal['PostProcessCompare']
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataConductor.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataFiQuS.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,23 +902,15 @@
 class MultipoleSolveGaussianPoints(BaseModel):
     """
     Level 4: Class for FiQuS Multipole
     """
 
     conducting_elements: int = 4
     insulation: int = 3
-
-
-class MultipoleSolveThinShellApproximationParameters(BaseModel):
-    """
-        Level 4: Class for FiQuS Multipole
-    """
-    integration_points: Optional[int] = None  # needs to be reasonably large to properly integrate non-linearity (>= 2)
-    global_size: Optional[float] = None
-    minimum_discretizations: int = 1
+    TSA: int = 2
 
 
 class MultipoleSolveInsulationBlockToBlock(BaseModel):
     """
         Level 4: Class for FiQuS Multipole
     """
     material: Optional[str] = None
@@ -966,18 +958,15 @@
 
 class MultipoleSolveThermal(BaseModel):
     """
         Level 3: Class for FiQuS Multipole
     """
     solved: Optional[str] = None
     gaussian_points: MultipoleSolveGaussianPoints = MultipoleSolveGaussianPoints()
-    TSA: MultipoleSolveThinShellApproximationParameters = MultipoleSolveThinShellApproximationParameters()
     basis_order: MultipoleSolveBasisOrder = MultipoleSolveBasisOrder()
-    isothermal_conductors: bool = False
-    isothermal_wedges: bool = False
     initial_temperature: Optional[float] = None
     enforce_initial_temperature_as_minimum: bool = False
     He_cooling: MultipoleSolveHeCooling = MultipoleSolveHeCooling()
     boundary_conditions: MultipoleSolveBoundaryConditionsThermal = MultipoleSolveBoundaryConditionsThermal()
     non_linear_solver: MultipoleSolveNonLinearSolver = MultipoleSolveNonLinearSolver()
     transient: MultipoleSolveTransientThermal = MultipoleSolveTransientThermal()
 
@@ -988,14 +977,22 @@
     """
     SizeMin: Optional[float] = None
     SizeMax: Optional[float] = None
     DistMin: Optional[float] = None
     DistMax: Optional[float] = None
 
 
+class MultipoleMeshThinShellApproximationParameters(BaseModel):
+    """
+        Level 4: Class for FiQuS Multipole
+    """
+    global_size: Optional[float] = None
+    minimum_discretizations: int = 1
+
+
 class MultipoleMeshTargetSize(BaseModel):
     """
         Level 3: Class for FiQuS Multipole
     """
     height: Optional[float] = None
     width: Optional[float] = None
 
@@ -1008,16 +1005,18 @@
     wedges: bool = False
 
 
 class MultipoleGeometry(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
+    geom_file_path: Optional[str] = None
     with_iron_yoke: Optional[bool] = None
     with_wedges: Optional[bool] = None
+    use_TSA: Optional[bool] = None
     symmetry: Optional[str] = None
 
 
 class MultipoleMesh(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
@@ -1026,14 +1025,19 @@
     wedge_target_sizes: MultipoleMeshTargetSize = MultipoleMeshTargetSize()
     coil_and_wedges: MultipoleMeshThreshold = MultipoleMeshThreshold()
     iron: MultipoleMeshThreshold = MultipoleMeshThreshold()
     bore: MultipoleMeshThreshold = MultipoleMeshThreshold()
     Algorithm: Optional[int] = None  # sets gmsh Mesh.Algorithm
     ElementOrder: Optional[int] = None  # sets gmsh Mesh.ElementOrder
     Optimize: Optional[int] = None  # sets gmsh Mesh.Optimize
+    isothermal_conductors: bool = False
+    isothermal_wedges: bool = False
+    TSA: MultipoleMeshThinShellApproximationParameters = (
+        MultipoleMeshThinShellApproximationParameters()
+    )
 
 
 class MultipoleSolve(BaseModel):
     """
         Level 2: Class for FiQuS Multipole
     """
     insulation_TSA: MultipoleSolveInsulationTSA = MultipoleSolveInsulationTSA()
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataFiQuSOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataFiQuSOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataLEDETOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataLEDETOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelCommon.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelCommon.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelCosim.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelCosim.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     modelCase: Optional[str] = None
     flag_run_pre_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (false) pre-cosim solution")
     flag_run_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (false) cosim solution")
     flag_run_post_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (False) post-cosim solution")
     convergence_checks_cosim: List[ConvergenceChecks] = Field(default=[], description="List of convergence checks to perform during each time window (all variable checks must be fulfilled to pass the convergence check)")
     variables_to_modify_pre_cosim: ParametersToModify = ParametersToModify()
     variables_to_modify_cosim: ParametersToModify = ParametersToModify()
+    variables_to_modify_cosim_for_each_time_window: List[ParametersToModify] = Field(default=[], description="List of ParametersToModify objects, each defining a list of parameters to change at one time window. This list must have as many elements as the number of time windows.")
     variables_to_modify_post_cosim: ParametersToModify = ParametersToModify()
     files_to_copy_after: FilesToCopy = FilesToCopy()
     variables_to_copy_after: VariablesToCopy = VariablesToCopy()
 
 class sim_FiQuS(sim_Generic): # TODO add/edit keys
     """
         Level 1: Class of FiQuS simulation configuration
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataModelParsimDakota.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataModelParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPlot.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPlot.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataProteCCTOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataProteCCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPyBBQOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPyCoSim.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMA.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMAOptions.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataPySIGMAOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataSettings.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataSignal.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DataTFM.py` & `steam-sdk-2024.5.6/steam_sdk/data/DataTFM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2024.5.6/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverANSYS.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverANSYS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverFiQuS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from operator import call
 import os
 import sys
 import subprocess
 import json
 
 
 class DriverFiQuS:
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverPySIGMA.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2024.5.6/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOSIM.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserCOSIM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserFiQuS.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,18 @@
         :param verbose: boolean if set to true more information is printed to the screen
         """
 
         self.builder_FiQuS = builder_FiQuS
         self.verbose = verbose
 
         if self.builder_FiQuS.data_FiQuS.magnet.type == 'multipole':
-            self.attributes = ['data_FiQuS', 'data_FiQuS_geo', 'data_FiQuS_set']
-            self.file_exts = ['yaml', 'geom', 'set']
+            if self.builder_FiQuS.data_FiQuS.magnet.geometry.geom_file_path:
+                self.attributes, self.file_exts = ['data_FiQuS', 'data_FiQuS_set'], ['yaml', 'set']
+            else:
+                self.attributes, self.file_exts = ['data_FiQuS', 'data_FiQuS_geo', 'data_FiQuS_set'], ['yaml', 'geom', 'set']
         elif self.builder_FiQuS.data_FiQuS.magnet.type == 'CCT_straight':
             self.attributes = ['data_FiQuS']
             self.file_exts = ['yaml']
         elif self.builder_FiQuS.data_FiQuS.magnet.type == 'CWS':
             self.attributes = ['data_FiQuS']
             self.file_exts = ['yaml']
         elif self.builder_FiQuS.data_FiQuS.magnet.type == 'Pancake3D':
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserFile.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # Read the signals as a dataframe
         df_signals = get_signals_from_csd(full_name_file, list_signals)
         # Assign them to a dict where each key is an array represented as a column vector
         dict_signals = {}
         for column in df_signals.columns:
             dict_signals[column] = df_signals[column].values
         return dict_signals
-    elif file_type == '.csv':
+    elif file_type == '.csv' or file_type == '.txt':
         # Check whether the file should be read column by column or as a single variable
         with open(full_name_file, 'r') as file:
             if ',' in file.readline():
                 flag_column_file = True
             else:
                 flag_column_file = False
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyBBQ.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyCoSim.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPySIGMA.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserXYCE.py`

 * *Files 4% similar despite different names*

```diff
@@ -360,14 +360,108 @@
         self.flag_read_parametrized_component = False
         self.flag_read_options = False
         self.flag_read_autoconverge = False
         self.flag_read_time_schedule = False
         self.flag_read_probe = False
         self.name_last_component = None  # this is used to have the name of the latest added component (used to read the parameters of parametrized component over multiple rows)
 
+    def writeNetlist(self, Netlist: dict, output_path: str = '',  verbose: bool = True):
+        # Prepare netlist
+        rows_netlist = []
+        rows_netlist.append(add_comment('**** Netlist ****'))  # Add header of this section
+        for s, name in enumerate(Netlist.keys()):
+            # Read keys
+            type = getattr(Netlist[name], 'type')
+            nodes = getattr(Netlist[name], 'nodes')
+            value = getattr(Netlist[name], 'value')
+            parameters = getattr(Netlist[name], 'parameters')
+            # name, nodes, value, parameters, type = component.name, component.nodes, component.value, component.parameters, component.type
+
+            # Check inputs
+            if not type:
+                raise Exception('At least one netlist entry of known type must be added. Supported component types:\n' +
+                                '- comment\n' +
+                                '- standard component\n'
+                                '- stimulus-controlled component\n'
+                                '- controlled-source component\n'
+                                '- pulsed-source component\n'
+                                '- parametrized component\n'
+                                '- transient-source component\n'
+                                'Netlist cannot be generated.')
+
+            # Add the relevant row depending on the component type
+            if type == 'comment':
+                if verbose: print('Netlist entry {} in position #{} is treated as a comment.'.format(name, s + 1))
+                rows_netlist.append(add_comment(value))
+            elif type == 'standard component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a standard component.'.format(name, s + 1))
+                rows_netlist.append(add_standard_component(name, nodes, value))
+            elif type == 'stimulus-controlled component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a stimulus-controlled component.'.format(name,
+                                                                                                             s + 1))
+                rows_netlist.append(add_stimulus_controlled_component(name, nodes, value, output_path=output_path))
+            elif type == 'pulsed-source component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a pulsed-source component.'.format(name, s + 1))
+                rows_netlist.append(add_pulsed_source_component(name, nodes, value))
+            elif type == 'controlled-source component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a controlled-source component.'.format(name, s + 1))
+                rows_netlist.append(add_controlled_source_component(name, nodes, value))
+            elif type == 'nonlinear-dependent-source component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a controlled-source component.'.format(name, s + 1))
+                rows_netlist.append(add_nonlinear_source_component(name, nodes, value))
+            elif type == 'transient-source component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a transient-source component.'.format(name, s + 1))
+                rows_netlist.append(add_transient_source_component(name, nodes, value))
+            elif type == 'parametrized component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a parametrized component.'.format(name, s + 1))
+                rows_netlist.append(add_parametrized_component(name, nodes, value, parameters))
+            elif type == 'behavioral-current component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a behavioral-current component.'.format(name,
+                                                                                                            s + 1))
+                rows_netlist.append(add_behavioral_current_component(name, nodes, value))
+            elif type == 'behavioral-voltage component':
+                if name == None or nodes == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(
+                            s + 1, type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a behavioral-voltage component.'.format(name,
+                                                                                                            s + 1))
+                rows_netlist.append(add_behavioral_voltage_component(name, nodes, value))
+            elif type == 'function':
+                if name == None or value == None:
+                    raise Exception('Netlist component in position #{} is of type {} and requires name, and value.'.format(s + 1,
+                                                                                                               type))
+                if verbose: print('Netlist entry {} in position #{} is treated as a function.'.format(name, s + 1))
+                rows_netlist.append(add_function(name, nodes[0], value))
+            else:
+                raise Exception('Netlist entry {} in position #{} has an unknown type: {}.'.format(name, s + 1, type))
+        return rows_netlist
+
     def write2XYCE(self, full_path_file_name: str,
                    flag_copy_additional_files: bool = False,
                    flag_resolve_library_paths: bool = False,
                    verbose: bool = False):
         '''
         ** Writes a XYCE netlist file **
 
@@ -434,77 +528,15 @@
             for name, value in self.circuit_data.InitialConditions.initial_conditions.items():
                 if name[0].casefold()=='i':
                     if verbose: print('Initial condition for currents not supported in XYCE. Will be ignored.')
                     continue
                 rows_initial_conditions.append(add_initial_condition(name, value))
 
         # Prepare netlist
-        rows_netlist = []
-        rows_netlist.append(add_comment('**** Netlist ****'))  # Add header of this section
-        for s, name in enumerate(self.circuit_data.Netlist.keys()):
-            # Read keys
-            type = getattr(self.circuit_data.Netlist[name], 'type')
-            nodes = getattr(self.circuit_data.Netlist[name], 'nodes')
-            value = getattr(self.circuit_data.Netlist[name], 'value')
-            parameters = getattr(self.circuit_data.Netlist[name], 'parameters')
-            # name, nodes, value, parameters, type = component.name, component.nodes, component.value, component.parameters, component.type
-
-            # Check inputs
-            if not type:
-                raise Exception('At least one netlist entry of known type must be added. Supported component types:\n' +
-                                '- comment\n' +
-                                '- standard component\n'
-                                '- stimulus-controlled component\n'
-                                '- controlled-source component\n'
-                                '- pulsed-source component\n'
-                                '- parametrized component\n'
-                                '- transient-source component\n'
-                                'Netlist cannot be generated.')
-
-            # Add the relevant row depending on the component type
-            if type == 'comment':
-                if verbose: print('Netlist entry {} in position #{} is treated as a comment.'.format(name, s + 1))
-                rows_netlist.append(add_comment(value))
-            elif type == 'standard component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a standard component.'.format(name, s + 1))
-                rows_netlist.append(add_standard_component(name, nodes, value))
-            elif type == 'stimulus-controlled component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a stimulus-controlled component.'.format(name, s + 1))
-                rows_netlist.append(add_stimulus_controlled_component(name, nodes, value, output_path=output_path))
-            elif type == 'pulsed-source component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a pulsed-source component.'.format(name, s + 1))
-                rows_netlist.append(add_pulsed_source_component(name, nodes, value))
-            elif type == 'controlled-source component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a controlled-source component.'.format(name, s + 1))
-                rows_netlist.append(add_controlled_source_component(name, nodes, value))
-            elif type == 'nonlinear-dependent-source component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a controlled-source component.'.format(name, s + 1))
-                rows_netlist.append(add_nonlinear_source_component(name, nodes, value))
-            elif type == 'transient-source component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a transient-source component.'.format(name, s + 1))
-                rows_netlist.append(add_transient_source_component(name, nodes, value))
-            elif type == 'parametrized component':
-                if name == None or nodes == None or value == None:
-                    raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
-                if verbose: print('Netlist entry {} in position #{} is treated as a parametrized component.'.format(name, s + 1))
-                rows_netlist.append(add_parametrized_component(name, nodes, value, parameters))
-            else:
-                raise Exception ('Netlist entry {} in position #{} has an unknown type: {}.'.format(name, s+1, type))
+        rows_netlist = self.writeNetlist(self.circuit_data.Netlist, output_path = output_path, verbose = verbose)
 
         # Prepare options - Simulation options
         rows_options = []
         options = self.circuit_data.Options.options_simulation
 
         keywords_timeInt = ['method', 'reltol', 'abstol', 'restartstepscale', 'nlnearconv'] # Not complete list, but most used
         keywords_NonLinSolv = ['nlstrategy', 'searchmethod', 'continuation', 'reltol', 'abstol', 'deltaxtol', 'rhstol']
@@ -790,19 +822,40 @@
     ''' Format stimulus-controlled component netlist row '''
     nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'PULSE ' + value
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
     return formatted_text
 
+def add_behavioral_current_component(name: str, nodes: list, value: str):
+    ''' Format stimulus-controlled component netlist row '''
+    nodes = [str(x) for x in nodes]
+    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_value = 'I={' + value + '}'
+    formatted_text = name + ' ' + str_nodes + ' ' + str_value
+    return formatted_text
+
+def add_behavioral_voltage_component(name: str, nodes: list, value: str):
+    ''' Format stimulus-controlled component netlist row '''
+    nodes = [str(x) for x in nodes]
+    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_value = 'V={' + value + '}'
+    formatted_text = name + ' ' + str_nodes + ' ' + str_value
+    return formatted_text
+
 def add_option(name: str, value: str):
     ''' Format option row '''
     formatted_text = '+ ' + name + '=' + str(value)
     return formatted_text
 
+def add_function(name: str, argument:str, value: str):
+    ''' Format option row '''
+    formatted_text = '.FUNC ' + name + '(' + argument + ')'+ '{'+ str(value)+'}'
+    return formatted_text
+
 
 def add_transient_source_component(name: str, nodes: list, value: str):
     ''' Format controlled-source component netlist row '''
     nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'AC ' + '{' + value + '}'
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCircuits.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/utils_ParserCircuits.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCosims.py` & `steam-sdk-2024.5.6/steam_sdk/parsers/utils_ParserCosims.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model.name)
         if software == 'XYCE':
             local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model.name)
     elif cosim_software == 'PyCoSim':
         local_cosim_folder = data_settings.local_PyCoSim_folder
         local_folder_prefix = os.path.join(local_cosim_folder, cosim_name, software)
         if software == 'FiQuS':
-            local_folder = os.path.join(local_folder_prefix, model.modelName) # use model set in the input folder name
+            local_folder = os.path.join(local_folder_prefix, model.modelName)  # use model set in the input folder name
         elif software == 'LEDET':
             local_folder = os.path.join(local_folder_prefix, str(nsti.n))
         elif software in ['PSPICE', 'XYCE']:
             local_folder = os.path.join(local_folder_prefix, str(nsti.n))  #TODO double check
     else:
          raise Exception(f'Co-simulation software {cosim_software} not supported.')
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2024.5.6/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2024.5.6/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2024.5.6/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2024.5.6/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2024.5.6/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2024.5.6/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterGriddedData.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterGriddedData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2024.5.6/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2024.5.6/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def run_metrics(self):
         """
             Function to initiate interpolation, start the different metrics and append the result to the output
         """
         # variables which need to be interpolated
         list_metrics_that_need_interpolation = ['maximum_abs_error', 'RMSE', 'RELATIVE_RMSE', 'RMSE_ratio',
-                                                'RELATIVE_RMSE_AFTER_t_PC_off','_RELATIVE_RMSE_IN_INTERVAL_0_100',
+                                                'RELATIVE_RMSE_AFTER_t_PC_off','RELATIVE_RMSE_IN_INTERVAL_0_100',
                                                 'MARE','MARE_1S', 'MARE_AFTER_t_PC_off']
          # For metrics that need interpolation of both simulation data and reference data:
         if any(n in self.metrics_to_do for n in set(list_metrics_that_need_interpolation)):
 
             # Clean arrays
             var_to_interpolate_cleaned, time_vector_cleaned = self.clean_array_touple(
                 self.var_to_interpolate,
@@ -78,15 +78,15 @@
                 result = self._maximum_abs_error(var_of_interest,var_ref )
             elif metric == 'RMSE':
                 result = self._RMSE(var_of_interest, var_ref)
             elif metric == 'RELATIVE_RMSE':
                 result = self._RELATIVE_RMSE(var_of_interest, var_ref)
             elif metric == 'RELATIVE_RMSE_AFTER_t_PC_off':
                 result = self._RELATIVE_RMSE_AFTER_t_PC_off(var_of_interest, var_ref,time_stamps_overlap)
-            elif metric == '_RELATIVE_RMSE_IN_INTERVAL_0_100':
+            elif metric == 'RELATIVE_RMSE_IN_INTERVAL_0_100':
                 result = self._RELATIVE_RMSE_IN_INTERVAL_0_100(var_of_interest, var_ref,time_stamps_overlap)
             elif metric == 'RMSE_ratio':
                 result = self._RMSE_ratio(var_of_interest, var_ref)
             elif metric == 'MARE':
                 result = self._MARE(var_of_interest, var_ref) # Calculate Mean Absolute Relative Error (MARE)
             elif metric == 'MARE_AFTER_t_PC_off':
                 result = self._MARE_AFTER_t_PC_off(var_of_interest, var_ref,time_stamps_overlap)
```

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2024.5.6/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2024.5.6/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2024.5.6/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/attribute_model.py` & `steam-sdk-2024.5.6/steam_sdk/utils/attribute_model.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2024.5.6/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/compare_simulations.py` & `steam-sdk-2024.5.6/steam_sdk/utils/compare_simulations.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2024.5.6/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/correct_RRR_NIST.py` & `steam-sdk-2024.5.6/steam_sdk/utils/correct_RRR_NIST.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2024.5.6/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/make_folder_if_not_existing.py` & `steam-sdk-2024.5.6/steam_sdk/utils/make_folder_if_not_existing.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/misc.py` & `steam-sdk-2024.5.6/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2024.5.6/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/read_settings_file.py` & `steam-sdk-2024.5.6/steam_sdk/utils/read_settings_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/reformat_figure.py` & `steam-sdk-2024.5.6/steam_sdk/utils/reformat_figure.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/tic_toc.py` & `steam-sdk-2024.5.6/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/utils/utils_PC.py` & `steam-sdk-2024.5.6/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/viewers/Viewer.py` & `steam-sdk-2024.5.6/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2024.5.6/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2024.5.6/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.4
+Version: 2024.5.6
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: SDK,STEAM,API,CERN
+Keywords: API,SDK,STEAM,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
```

### Comparing `steam-sdk-2024.5.4/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2024.5.6/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.4/steam_sdk.egg-info/requires.txt` & `steam-sdk-2024.5.6/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

