# Comparing `tmp/pymodaq-4.1.4.tar.gz` & `tmp/pymodaq-4.1.5.tar.gz`

## Comparing `pymodaq-4.1.4.tar` & `pymodaq-4.1.5.tar`

### file list

```diff
@@ -1,422 +1,422 @@
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/__init__.py
--rw-r--r--   0        0        0    63635 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/dashboard.py
--rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/icon.ico
--rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/splash.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/__init__.py
--rw-r--r--   0        0        0    36578 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/daq_move.py
--rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/daq_move_ui.py
--rw-r--r--   0        0        0    58421 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/daq_viewer.py
--rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/daq_viewer_ui.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/mocks.py
--rw-r--r--   0        0        0    32605 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/move_utility_classes.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/utils.py
--rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/control_modules/viewer_utility_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/__init__.py
--rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/custom_app.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/custom_viewer.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/function_plotter.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/nonlinearscanner.py
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/parameter_ex.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/preset_MockCamera.xml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
--rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
--rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
--rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
--rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
--rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/console.py
--rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/daq_logger.py
--rw-r--r--   0        0        0    54243 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/daq_scan.py
--rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/daq_scan_ui.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/h5browser.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/utils.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/pid/__init__.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/pid/daq_move_PID.py
--rw-r--r--   0        0        0    28317 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/pid/pid_controller.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/extensions/pid/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/load_and_plot.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/process_to_scalar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_analysis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/__init__.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
--rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/config_scan_template.toml
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/config_template.toml
--rw-r--r--   0        0        0    27256 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/preset_default.xml
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/setup_plugin.py
--rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/triangulation_data.npy
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
--rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
--rw-r--r--   0        0        0  8313856 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
--rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
--rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
--rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
--rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
--rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
--rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
--rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
--rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
--rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
--rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
--rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
--rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
--rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
--rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
--rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
--rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
--rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
--rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
--rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
--rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
--rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
--rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
--rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
--rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
--rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
--rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openTree.png
--rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
--rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
--rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
--rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
--rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
--rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
--rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
--rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saveTree.png
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sort_ascend.png
--rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
--rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/updateTree.png
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
--rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/array_manipulation.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/calibration_camera.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/chrono_timer.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/config.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/conftests.py
--rw-r--r--   0        0        0    30312 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/daq_utils.py
--rw-r--r--   0        0        0    86475 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/data.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/enums.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/exceptions.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/factory.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/logger.py
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/math_utils.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/messenger.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/qvariant.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/slicing.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/units.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/abstract/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/abstract/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/db/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/db/db_logger/__init__.py
--rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/db/db_logger/db_logger.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/db/db_logger/db_logger_models.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/__init__.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/custom_app.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/dock.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/file_io.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/layout.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/list_picker.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/label.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/lcd.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/push.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/qled.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/spinbox.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/table.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/tree_layout.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/tree_toml.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/__init__.py
--rw-r--r--   0        0        0    33040 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/backends.py
--rw-r--r--   0        0        0    23356 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/browsing.py
--rw-r--r--   0        0        0    34301 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/data_saving.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporter.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/h5logging.py
--rw-r--r--   0        0        0    13761 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/module_saving.py
--rw-r--r--   0        0        0    34013 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/saving.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/__init__.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/base.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/flimj.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/hyperspy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/__init__.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/action_manager.py
--rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/batchscan_manager.py
--rw-r--r--   0        0        0    20821 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/modules_manager.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/overshoot_manager.py
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/parameter_manager.py
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/preset_manager.py
--rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/preset_manager_utils.py
--rw-r--r--   0        0        0    22251 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/remote_manager.py
--rw-r--r--   0        0        0    28869 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/managers/roi_manager.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/__init__.py
--rw-r--r--   0        0        0    16887 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/ioxml.py
--rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/utils.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/gant_chart.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/image_viewer.py
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/navigator.py
--rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/scan_selector.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/widgets.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/__init__.py
--rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer.py
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
--rw-r--r--   0        0        0    23296 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
--rw-r--r--   0        0        0    42182 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
--rw-r--r--   0        0        0    38315 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewerND.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/items/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/items/axis_scaled.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/items/crosshair.py
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/items/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/axes_viewer.py
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/filter.py
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/lineout.py
--rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/plot_utils.py
--rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/signalND.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scan_config.py
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scan_factory.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanner.py
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/utils.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
--rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/__init__.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/sequential.py
--rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/tabular.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/svg/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/svg/svg_renderer.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/svg/svg_view.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/svg/svg_viewer2D.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/__init__.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/mysocket.py
--rw-r--r--   0        0        0    24932 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/serializer.py
--rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/tcp_server_client.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.1.4/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.1.4/LICENSE
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.1.4/README.rst
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymodaq-4.1.4/pyproject.toml
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 pymodaq-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/__init__.py
+-rw-r--r--   0        0        0    63635 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/dashboard.py
+-rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/icon.ico
+-rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/splash.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/__init__.py
+-rw-r--r--   0        0        0    36583 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/daq_move.py
+-rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/daq_move_ui.py
+-rw-r--r--   0        0        0    58421 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/daq_viewer.py
+-rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/daq_viewer_ui.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/mocks.py
+-rw-r--r--   0        0        0    32605 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/move_utility_classes.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/utils.py
+-rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/control_modules/viewer_utility_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/__init__.py
+-rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/custom_app.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/custom_viewer.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/function_plotter.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/nonlinearscanner.py
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/parameter_ex.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/preset_MockCamera.xml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
+-rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
+-rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
+-rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
+-rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
+-rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
+-rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/console.py
+-rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/daq_logger.py
+-rw-r--r--   0        0        0    54243 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/daq_scan.py
+-rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/daq_scan_ui.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/h5browser.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/utils.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/pid/__init__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/pid/daq_move_PID.py
+-rw-r--r--   0        0        0    28317 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/pid/pid_controller.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/extensions/pid/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/__init__.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/load_and_plot.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/process_to_scalar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/__init__.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
+-rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/config_scan_template.toml
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/config_template.toml
+-rw-r--r--   0        0        0    27256 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/preset_default.xml
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/setup_plugin.py
+-rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/triangulation_data.npy
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
+-rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
+-rw-r--r--   0        0        0  8313856 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
+-rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
+-rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
+-rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
+-rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
+-rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
+-rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
+-rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
+-rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
+-rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
+-rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
+-rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
+-rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
+-rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
+-rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
+-rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
+-rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
+-rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
+-rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
+-rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
+-rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
+-rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
+-rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
+-rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
+-rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
+-rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
+-rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openTree.png
+-rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
+-rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
+-rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
+-rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
+-rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
+-rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
+-rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
+-rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saveTree.png
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sort_ascend.png
+-rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
+-rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/updateTree.png
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
+-rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/array_manipulation.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/calibration_camera.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/chrono_timer.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/config.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/conftests.py
+-rw-r--r--   0        0        0    30357 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/daq_utils.py
+-rw-r--r--   0        0        0    86475 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/data.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/enums.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/exceptions.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/factory.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/logger.py
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/math_utils.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/messenger.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/qvariant.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/slicing.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/units.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/abstract/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/abstract/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/db/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/db/db_logger/__init__.py
+-rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/db/db_logger/db_logger.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/db/db_logger/db_logger_models.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/__init__.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/custom_app.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/dock.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/file_io.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/layout.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/list_picker.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/label.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/lcd.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/push.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/qled.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/spinbox.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/table.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/tree_layout.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/tree_toml.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/__init__.py
+-rw-r--r--   0        0        0    33040 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/backends.py
+-rw-r--r--   0        0        0    23356 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/browsing.py
+-rw-r--r--   0        0        0    34301 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/data_saving.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporter.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/h5logging.py
+-rw-r--r--   0        0        0    13761 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/module_saving.py
+-rw-r--r--   0        0        0    34013 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/saving.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/__init__.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/base.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/flimj.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/hyperspy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/__init__.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/action_manager.py
+-rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/batchscan_manager.py
+-rw-r--r--   0        0        0    20821 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/modules_manager.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/overshoot_manager.py
+-rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/parameter_manager.py
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/preset_manager.py
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/preset_manager_utils.py
+-rw-r--r--   0        0        0    22251 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/remote_manager.py
+-rw-r--r--   0        0        0    28881 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/managers/roi_manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/__init__.py
+-rw-r--r--   0        0        0    16887 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/ioxml.py
+-rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/utils.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/gant_chart.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/image_viewer.py
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/navigator.py
+-rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/scan_selector.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/widgets.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/__init__.py
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer.py
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
+-rw-r--r--   0        0        0    23296 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
+-rw-r--r--   0        0        0    42182 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
+-rw-r--r--   0        0        0    38315 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewerND.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/items/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/items/axis_scaled.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/items/crosshair.py
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/items/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/axes_viewer.py
+-rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/filter.py
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/lineout.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/plot_utils.py
+-rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/signalND.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scan_config.py
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scan_factory.py
+-rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanner.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/utils.py
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
+-rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/__init__.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/sequential.py
+-rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/tabular.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/svg/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/svg/svg_renderer.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/svg/svg_view.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/svg/svg_viewer2D.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/__init__.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/mysocket.py
+-rw-r--r--   0        0        0    24932 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/serializer.py
+-rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/tcp_server_client.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.1.5/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.1.5/LICENSE
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.1.5/README.rst
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymodaq-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 pymodaq-4.1.5/PKG-INFO
```

### Comparing `pymodaq-4.1.4/src/pymodaq/__init__.py` & `pymodaq-4.1.5/src/pymodaq/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/dashboard.py` & `pymodaq-4.1.5/src/pymodaq/dashboard.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/icon.ico` & `pymodaq-4.1.5/src/pymodaq/icon.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/splash.png` & `pymodaq-4.1.5/src/pymodaq/splash.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/daq_move.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/daq_move.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from pymodaq.utils.messenger import deprecation_msg
 from pymodaq.utils.h5modules import module_saving
 from pymodaq.utils.data import DataRaw, DataToExport, DataFromPlugins, DataActuator
 from pymodaq.utils.h5modules.backends import Node
 
 
 local_path = config_mod.get_set_local_dir()
-sys.path.append(local_path)
+sys.path.append(str(local_path))
 logger = set_logger(get_module_name(__file__))
 config = config_mod.Config()
 
 DAQ_Move_Actuators = utils.get_plugins('daq_move')
 ACTUATOR_TYPES = [mov['name'] for mov in DAQ_Move_Actuators]
 if len(ACTUATOR_TYPES) == 0:
     raise ActuatorError('No installed Actuator')
```

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/daq_move_ui.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/daq_move_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/daq_viewer.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/daq_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/daq_viewer_ui.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/daq_viewer_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/mocks.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/mocks.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/move_utility_classes.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/move_utility_classes.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/utils.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/control_modules/viewer_utility_classes.py` & `pymodaq-4.1.5/src/pymodaq/control_modules/viewer_utility_classes.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/custom_app.py` & `pymodaq-4.1.5/src/pymodaq/examples/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/custom_viewer.py` & `pymodaq-4.1.5/src/pymodaq/examples/custom_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/function_plotter.py` & `pymodaq-4.1.5/src/pymodaq/examples/function_plotter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/nonlinearscanner.py` & `pymodaq-4.1.5/src/pymodaq/examples/nonlinearscanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/parameter_ex.py` & `pymodaq-4.1.5/src/pymodaq/examples/parameter_ex.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/preset_MockCamera.xml` & `pymodaq-4.1.5/src/pymodaq/examples/preset_MockCamera.xml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl` & `pymodaq-4.1.5/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/console.py` & `pymodaq-4.1.5/src/pymodaq/extensions/console.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/daq_logger.py` & `pymodaq-4.1.5/src/pymodaq/extensions/daq_logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/daq_scan.py` & `pymodaq-4.1.5/src/pymodaq/extensions/daq_scan.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/daq_scan_ui.py` & `pymodaq-4.1.5/src/pymodaq/extensions/daq_scan_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/h5browser.py` & `pymodaq-4.1.5/src/pymodaq/extensions/h5browser.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/utils.py` & `pymodaq-4.1.5/src/pymodaq/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/pid/__init__.py` & `pymodaq-4.1.5/src/pymodaq/extensions/pid/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/pid/daq_move_PID.py` & `pymodaq-4.1.5/src/pymodaq/extensions/pid/daq_move_PID.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/pid/pid_controller.py` & `pymodaq-4.1.5/src/pymodaq/extensions/pid/pid_controller.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/extensions/pid/utils.py` & `pymodaq-4.1.5/src/pymodaq/extensions/pid/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/post_treatment/load_and_plot.py` & `pymodaq-4.1.5/src/pymodaq/post_treatment/load_and_plot.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/post_treatment/process_to_scalar.py` & `pymodaq-4.1.5/src/pymodaq/post_treatment/process_to_scalar.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py` & `pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui` & `pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py` & `pymodaq-4.1.5/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/config_scan_template.toml` & `pymodaq-4.1.5/src/pymodaq/resources/config_scan_template.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/config_template.toml` & `pymodaq-4.1.5/src/pymodaq/resources/config_template.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/preset_default.xml` & `pymodaq-4.1.5/src/pymodaq/resources/preset_default.xml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/setup_plugin.py` & `pymodaq-4.1.5/src/pymodaq/resources/setup_plugin.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/triangulation_data.npy` & `pymodaq-4.1.5/src/pymodaq/resources/triangulation_data.npy`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/icons.svg` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/icons.svg`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openTree.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openTree.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saveTree.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saveTree.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sort_ascend.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sort_ascend.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/updateTree.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/updateTree.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png` & `pymodaq-4.1.5/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/array_manipulation.py` & `pymodaq-4.1.5/src/pymodaq/utils/array_manipulation.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/calibration_camera.py` & `pymodaq-4.1.5/src/pymodaq/utils/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/chrono_timer.py` & `pymodaq-4.1.5/src/pymodaq/utils/chrono_timer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/config.py` & `pymodaq-4.1.5/src/pymodaq/utils/config.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/daq_utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/daq_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,14 @@
 if version_mod.parse(platform.python_version()) >= version_mod.parse('3.9'):
     # from version 3.9 the cache decorator is available
     from functools import cache
 else:
     from functools import lru_cache as cache
 
 
-if version_mod.parse(platform.python_version()) >= version_mod.parse('3.9'):
-    # from version 3.9 the cache decorator is available
-    from functools import cache
-else:
-    from functools import lru_cache as cache
-
 logger = logger_module.set_logger(logger_module.get_module_name(__file__))
 
 plot_colors = [(255, 255, 255), (255, 0, 0), (0, 255, 0), (0, 0, 255), (14, 207, 189), (207, 14, 166), (207, 204, 14)]
 config = Config()
 
 
 def __getattr__(name):
@@ -607,27 +601,31 @@
                 movemodule = importlib.import_module(f'{entrypoint.value}.daq_move_plugins', entrypoint.value)
                 plugin_list.extend([{'name': mod[len('daq_move') + 1:],
                                      'module': movemodule,
                                      'parent_module': importlib.import_module(entrypoint.value),
                                      'type': 'daq_move'}
                                     for mod in [mod[1] for mod in pkgutil.iter_modules([str(movemodule.path.parent)])]
                                     if 'daq_move' in mod])
+                if len(plugin_list) > 0:
+                    logger.info(f"Found Move Instrument: {plugin_list[-1]['name']}")
             except ModuleNotFoundError:
                 pass
             viewer_modules = {}
             for vtype in viewer_types:
                 try:
                     viewer_modules[vtype] = importlib.import_module(f'{entrypoint.value}.daq_viewer_plugins.plugins_{vtype}',
                                                     entrypoint.value)
                     plugin_list.extend([{'name': mod[len(f'daq_{vtype}viewer') + 1:],
                                      'module': viewer_modules[vtype],
                                      'parent_module': importlib.import_module(entrypoint.value),
                                      'type': f'daq_{vtype}viewer'}
                                     for mod in [mod[1] for mod in pkgutil.iter_modules([str(viewer_modules[vtype].path.parent)])]
                                     if f'daq_{vtype}viewer' in mod])
+                    if len(plugin_list) > 0:
+                        logger.info(f"Found Viewer Instrument: {plugin_list[-1]['name']}")
                 except ModuleNotFoundError:
                     pass
 
             # check if modules are importable
             for mod in plugin_list:
                 try:
                     plugin_type = mod['type']
```

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/data.py` & `pymodaq-4.1.5/src/pymodaq/utils/data.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/enums.py` & `pymodaq-4.1.5/src/pymodaq/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/exceptions.py` & `pymodaq-4.1.5/src/pymodaq/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/factory.py` & `pymodaq-4.1.5/src/pymodaq/utils/factory.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/logger.py` & `pymodaq-4.1.5/src/pymodaq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/math_utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/messenger.py` & `pymodaq-4.1.5/src/pymodaq/utils/messenger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/slicing.py` & `pymodaq-4.1.5/src/pymodaq/utils/slicing.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/units.py` & `pymodaq-4.1.5/src/pymodaq/utils/units.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/abstract/__init__.py` & `pymodaq-4.1.5/src/pymodaq/utils/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/abstract/logger.py` & `pymodaq-4.1.5/src/pymodaq/utils/abstract/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/db/db_logger/db_logger.py` & `pymodaq-4.1.5/src/pymodaq/utils/db/db_logger/db_logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/db/db_logger/db_logger_models.py` & `pymodaq-4.1.5/src/pymodaq/utils/db/db_logger/db_logger_models.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/custom_app.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/dock.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/dock.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/file_io.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/file_io.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,16 +66,17 @@
     ----------
     start_path: str or Path
         The strating point in the file/folder system to open the popup from
     save: bool
         if True, ask you to enter a filename (with or without extension)
     ext: str
         the extension string, e.g. xml, h5, png ...
-    filter: list of string
-        list of possible extensions, mostly valid for loading
+    filter: string
+        list of possible extensions, if you need several you can separate them by ;;
+        for example: "Images (*.png *.xpm *.jpg);;Text files (*.txt);;XML files (*.xml)"
     force_save_extension: bool
         if True force the extension of the saved file to be set to ext
 
     Returns
     -------
     Path: the Path object of the file to save or load
     """
```

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/layout.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/layout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/list_picker.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/list_picker.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/label.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/label.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/lcd.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/lcd.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/push.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/push.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/qled.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/qled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/spinbox.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/table.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/tree_layout.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/tree_layout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/gui_utils/widgets/tree_toml.py` & `pymodaq-4.1.5/src/pymodaq/utils/gui_utils/widgets/tree_toml.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/backends.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/backends.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/browsing.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/browsing.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/data_saving.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/data_saving.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporter.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/h5logging.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/h5logging.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/module_saving.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/module_saving.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/saving.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/saving.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/base.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/base.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/flimj.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/flimj.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/h5modules/exporters/hyperspy.py` & `pymodaq-4.1.5/src/pymodaq/utils/h5modules/exporters/hyperspy.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/action_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/action_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/batchscan_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/batchscan_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/modules_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/modules_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/overshoot_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/overshoot_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/parameter_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/parameter_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/preset_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/preset_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/preset_manager_utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/preset_manager_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/remote_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/remote_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/managers/roi_manager.py` & `pymodaq-4.1.5/src/pymodaq/utils/managers/roi_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,15 +558,15 @@
             self.settings.child(*('ROIs', self.roi_format(index))).remove()
             # self.settings.sigTreeStateChanged.connect(self.roi_tree_changed)
 
     def load_ROI(self, path=None, params=None):
         try:
             if params is None:
                 if path is None:
-                    path = select_file(start_path=Path.home(), save=False, ext='xml', filter=['xml'])
+                    path = select_file(start_path=Path.home(), save=False, ext='xml', filter='XML files (*.xml)')
                     if path != '':
                         params = Parameter.create(title='Settings', name='settings', type='group',
                                                   children=ioxml.XML_file_to_parameter(path))
 
             if params is not None:
                 self.clear_ROI()
                 QtWidgets.QApplication.processEvents()
```

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/ioxml.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/ioxml.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py` & `pymodaq-4.1.5/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/gant_chart.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/gant_chart.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/image_viewer.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/navigator.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/navigator.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/scan_selector.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/scan_selector.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/widgets.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer0D.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer0D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer1D.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer1D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer2D.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/data_viewers/viewerND.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/data_viewers/viewerND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/items/axis_scaled.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/items/axis_scaled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/items/crosshair.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/items/crosshair.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/items/image.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/items/image.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/axes_viewer.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/axes_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/filter.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/lineout.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/lineout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/plot_utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/plotting/utils/signalND.py` & `pymodaq-4.1.5/src/pymodaq/utils/plotting/utils/signalND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scan_config.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scan_config.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scan_factory.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scan_factory.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scanner.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/utils.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/_1d_scanners.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/_1d_scanners.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/_2d_scanners.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/_2d_scanners.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/sequential.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/sequential.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/scanner/scanners/tabular.py` & `pymodaq-4.1.5/src/pymodaq/utils/scanner/scanners/tabular.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/svg/svg_view.py` & `pymodaq-4.1.5/src/pymodaq/utils/svg/svg_view.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/svg/svg_viewer2D.py` & `pymodaq-4.1.5/src/pymodaq/utils/svg/svg_viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/mysocket.py` & `pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/mysocket.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/serializer.py` & `pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/serializer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/src/pymodaq/utils/tcp_ip/tcp_server_client.py` & `pymodaq-4.1.5/src/pymodaq/utils/tcp_ip/tcp_server_client.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/.gitignore` & `pymodaq-4.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/LICENSE` & `pymodaq-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/README.rst` & `pymodaq-4.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/pyproject.toml` & `pymodaq-4.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.1.4/PKG-INFO` & `pymodaq-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pymodaq
-Version: 4.1.4
+Version: 4.1.5
 Summary: Modular Data Acquisition with Python
 Project-URL: Homepage, http://pymodaq.cnrs.fr
 Project-URL: Source, https://github.com/PyMoDAQ/PyMoDAQ
 Project-URL: Tracker, https://github.com/PyMoDAQ/PyMoDAQ/issues
 Author-email: Sébastien Weber <sebastien.weber@cemes.fr>
 License: The MIT License (MIT)
```

