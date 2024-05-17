# Comparing `tmp/pynxtools-0.2.1.tar.gz` & `tmp/pynxtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools-0.2.1.tar", last modified: Tue Apr 16 10:03:35 2024, max compression
+gzip compressed data, was "pynxtools-0.3.0.tar", last modified: Fri May 17 11:26:58 2024, max compression
```

## Comparing `pynxtools-0.2.1.tar` & `pynxtools-0.3.0.tar`

### file list

```diff
@@ -1,447 +1,449 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.598617 pynxtools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 10:02:28.000000 pynxtools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22176 2024-04-16 10:03:35.594617 pynxtools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-16 10:02:28.000000 pynxtools-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-16 10:02:28.000000 pynxtools-0.2.1/TROUBLESHOOTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-16 10:02:28.000000 pynxtools-0.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.526617 pynxtools-0.2.1/pynxtools/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/_build_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/file_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/hdfdict.py
--rw-r--r--   0 runner    (1001) docker     (127)    30525 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/base/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/ellips/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/ellips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/ellips/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/ellips/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/example/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_map/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_yml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/json_yml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/readers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/dataconverter/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.530617 pynxtools-0.2.1/pynxtools/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/NXDL_VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.534617 pynxtools-0.2.1/pynxtools/definitions/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXarchive.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXarpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50852 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXcanSAS.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXdirecttof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXfluo.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXindirecttof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXiqproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXlauetof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXmonopd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50338 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXmx.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXrefscan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXreftof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXsas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXsastof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXscan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXspe.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXsqom.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXstxm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtofnpd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtofraw.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtofsingle.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtomo.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtomophase.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXtomoproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxasproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxbase.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxeuler.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxkappa.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxlaue.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxnb.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/applications/NXxrot.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.546617 pynxtools-0.2.1/pynxtools/definitions/base_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXaperture.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbeam.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcite.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcollection.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdata.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    40505 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXentry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfilter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXflipper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXgrating.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXguide.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXlog.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmirror.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXnote.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXobject.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXorientation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXparameters.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpdb.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXprocess.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXreflections.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXroot.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsample.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsensor.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXshape.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXslit.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsource.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXuser.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.582617 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63361 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20415 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16475 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    61348 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    74694 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50568 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    24509 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28514 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44194 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    30052 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35831 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44639 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53837 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27543 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.582617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/dir_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/impatient_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/manual_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/nxclass_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/anchor_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27419 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/nxdl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/xsd_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/ext/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/ext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/ext/contrib_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.586617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/nxdl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/impatient-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/impatient-guide/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.522617 pynxtools-0.2.1/pynxtools/definitions/manual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5388 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/epics/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2538 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1706 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.526617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1827 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1979 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1490 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2816 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)      738 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.590617 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/simple3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/verysimple.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51563 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/nxdl.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/nxdlTypes.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.594617 pynxtools-0.2.1/pynxtools/definitions/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10003 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/utils/create_release_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/utils/dev_create_release_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-04-16 10:03:29.000000 pynxtools-0.2.1/pynxtools/definitions/utils/update_copyright_date.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.594617 pynxtools-0.2.1/pynxtools/eln_mapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)      654 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/eln_mapper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5626 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/eln_mapper/eln.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/eln_mapper/eln_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/eln_mapper/scheme_eln.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.594617 pynxtools-0.2.1/pynxtools/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pynxtools/nexus/nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 10:03:35.000000 pynxtools-0.2.1/pynxtools/nexus-version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:03:35.594617 pynxtools-0.2.1/pynxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25580 2024-04-16 10:03:35.000000 pynxtools-0.2.1/pynxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-16 10:02:28.000000 pynxtools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:03:35.598617 pynxtools-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.181162 pynxtools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 11:25:24.000000 pynxtools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20654 2024-05-17 11:26:58.181162 pynxtools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-17 11:25:24.000000 pynxtools-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-17 11:25:24.000000 pynxtools-0.3.0/TROUBLESHOOTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-17 11:25:24.000000 pynxtools-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.101161 pynxtools-0.3.0/pynxtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/_build_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/file_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/hdfdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32762 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/nexus_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/readers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/base/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/readers/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/example/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_map/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_yml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/json_yml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/readers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/dataconverter/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.105161 pynxtools-0.3.0/pynxtools/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/NXDL_VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.113161 pynxtools-0.3.0/pynxtools/definitions/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXarchive.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXarpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50852 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXcanSAS.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXdirecttof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXfluo.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXindirecttof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXiqproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXlauetof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXmonopd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50338 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXmx.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXrefscan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXreftof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXsas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXsastof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXscan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXspe.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXsqom.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXstxm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtofnpd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtofraw.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtofsingle.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtomo.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtomophase.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXtomoproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxasproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxbase.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxeuler.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxkappa.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxlaue.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxnb.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/applications/NXxrot.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.125161 pynxtools-0.3.0/pynxtools/definitions/base_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXaperture.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbeam.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcite.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcollection.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdata.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    40526 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXentry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfilter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXflipper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXgrating.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXguide.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXlog.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmirror.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXnote.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXobject.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXorientation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXparameters.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpdb.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXprocess.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXreflections.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXroot.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsample.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsensor.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXshape.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXslit.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsource.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXuser.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63644 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17894 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20415 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62967 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50568 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    24509 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28514 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44594 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    30066 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16465 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35845 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    59085 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    55436 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27543 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/dir_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/impatient_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/manual_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/nxclass_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/anchor_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27419 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/nxdl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/xsd_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/ext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/ext/contrib_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.169162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/nxdl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/impatient-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/impatient-guide/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.097161 pynxtools-0.3.0/pynxtools/definitions/manual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5388 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/epics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2538 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1706 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.101161 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1827 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.173162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1979 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1490 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2816 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      738 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/simple3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/verysimple.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51563 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/nxdl.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/nxdlTypes.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/definitions/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10003 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/utils/create_release_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/utils/dev_create_release_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-05-17 11:26:52.000000 pynxtools-0.3.0/pynxtools/definitions/utils/update_copyright_date.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/eln_mapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      654 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/eln_mapper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5626 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/eln_mapper/eln.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/eln_mapper/eln_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/eln_mapper/scheme_eln.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30703 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pynxtools/nexus/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 11:26:57.000000 pynxtools-0.3.0/pynxtools/nexus-version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:26:58.177162 pynxtools-0.3.0/pynxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-17 11:26:58.000000 pynxtools-0.3.0/pynxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-17 11:25:24.000000 pynxtools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:26:58.181162 pynxtools-0.3.0/setup.cfg
```

### Comparing `pynxtools-0.2.1/LICENSE` & `pynxtools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/PKG-INFO` & `pynxtools-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Extend NeXus for experiments and characterization in Materials Science and Materials Engineering and serve as a NOMAD parser implementation for NeXus.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -225,14 +225,16 @@
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: numpy>=1.21.2
 Requires-Dist: pandas>=1.3.2
 Requires-Dist: ase>=3.19.0
 Requires-Dist: mergedeep
 Requires-Dist: importlib-metadata
 Requires-Dist: lxml>=4.9.1
+Requires-Dist: anytree
+Requires-Dist: pydantic
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocs-material-extensions; extra == "docs"
 Requires-Dist: mkdocs-macros-plugin; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
@@ -243,27 +245,29 @@
 Requires-Dist: structlog; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: convert
-Requires-Dist: pynxtools[apm,em,mpes,stm,xps,xrd]; extra == "convert"
+Requires-Dist: pynxtools[apm,ellips,em,mpes,stm,xps,xrd]; extra == "convert"
 Provides-Extra: apm
 Requires-Dist: pynxtools-apm; extra == "apm"
 Provides-Extra: em
 Requires-Dist: pynxtools-em; extra == "em"
 Provides-Extra: mpes
 Requires-Dist: pynxtools-mpes; extra == "mpes"
 Provides-Extra: xps
 Requires-Dist: pynxtools-xps; extra == "xps"
 Provides-Extra: stm
 Requires-Dist: pynxtools-stm; extra == "stm"
 Provides-Extra: xrd
 Requires-Dist: pynxtools-xrd; extra == "xrd"
+Provides-Extra: ellips
+Requires-Dist: pynxtools-ellips; extra == "ellips"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/pylint.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/pynxtools)
 ![](https://img.shields.io/pypi/l/pynxtools)
@@ -311,36 +315,14 @@
 - [**dataconverter**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/dataconverter/README.md): Creates compliant instances of NeXus/HDF5 files to [NeXus schemas](https://nexusformat.org).
 - [**read_nexus**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/nexus/README.md): Outputs a debug log for a given NeXus file.
 - [**generate_eln**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/eln_mapper/README.md): Outputs ELN files that can be used to add metadata to the dataconverter routine.
 
 # Documentation
 Documentation for the different tools can be found [here](https://fairmat-nfdi.github.io/pynxtools/).
 
-# Plugins
-There are a number of plugins available for pynxtools. These are extensions of pynxtools used for reading data of specialized experimental techniques.
-- [**pynxtools-mpes**](https://github.com/FAIRmat-NFDI/pynxtools-mpes): A reader for multi-dimensional photoelectron spectroscopy data.
-- [**pynxtools-stm**](https://github.com/FAIRmat-NFDI/pynxtools-stm): A reader for scanning tunneling microscopy (SPM) and spectroscopy (STS) data.
-- [**pynxtools-xps**](https://github.com/FAIRmat-NFDI/pynxtools-xps): A reader for X-ray photoelectron spectroscopy (XPS) data.
-
-Respective readers for the research fields of electron microscopy and atom probe are currently refactored into pynxtools plugins.
-Until this refactoring will have become completed, users are advised to use the apm and em readers via pynxtools<=0.1.1.
-- [**pynxtools-apm**](https://github.com/FAIRmat-NFDI/pynxtools-apm): A reader for atom probe as well as related field ion microscopy data.
-- [**pynxtools-em**](https://github.com/FAIRmat-NFDI/pynxtools-em): A reader for electron microscopy data.
-
-You can install each of the plugins together with `pynxtools` by passing the name of the plugin as an extra to the pip install call. For example, for the `pynxtools-mpes` plugin:
-```shell
-pip install pynxtools[mpes]
-```
-
-In addition, you can also install all of the `pynxtools` reader plugins which are maintained by FAIRmat by passing the `[convert]` extra to the pip install call:
-```shell
-pip install pynxtools[convert]
-```
-There is also a [cookiecutter template](https://github.com/FAIRmat-NFDI/pynxtools-plugin-template) available for creating your own pynxtools plugin.
-
 # Contributing
 
 ## Development install
 
 Install the package with its dependencies:
 
 ```shell
```

### Comparing `pynxtools-0.2.1/README.md` & `pynxtools-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -48,36 +48,14 @@
 - [**dataconverter**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/dataconverter/README.md): Creates compliant instances of NeXus/HDF5 files to [NeXus schemas](https://nexusformat.org).
 - [**read_nexus**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/nexus/README.md): Outputs a debug log for a given NeXus file.
 - [**generate_eln**](https://github.com/FAIRmat-NFDI/pynxtools/blob/master/pynxtools/eln_mapper/README.md): Outputs ELN files that can be used to add metadata to the dataconverter routine.
 
 # Documentation
 Documentation for the different tools can be found [here](https://fairmat-nfdi.github.io/pynxtools/).
 
-# Plugins
-There are a number of plugins available for pynxtools. These are extensions of pynxtools used for reading data of specialized experimental techniques.
-- [**pynxtools-mpes**](https://github.com/FAIRmat-NFDI/pynxtools-mpes): A reader for multi-dimensional photoelectron spectroscopy data.
-- [**pynxtools-stm**](https://github.com/FAIRmat-NFDI/pynxtools-stm): A reader for scanning tunneling microscopy (SPM) and spectroscopy (STS) data.
-- [**pynxtools-xps**](https://github.com/FAIRmat-NFDI/pynxtools-xps): A reader for X-ray photoelectron spectroscopy (XPS) data.
-
-Respective readers for the research fields of electron microscopy and atom probe are currently refactored into pynxtools plugins.
-Until this refactoring will have become completed, users are advised to use the apm and em readers via pynxtools<=0.1.1.
-- [**pynxtools-apm**](https://github.com/FAIRmat-NFDI/pynxtools-apm): A reader for atom probe as well as related field ion microscopy data.
-- [**pynxtools-em**](https://github.com/FAIRmat-NFDI/pynxtools-em): A reader for electron microscopy data.
-
-You can install each of the plugins together with `pynxtools` by passing the name of the plugin as an extra to the pip install call. For example, for the `pynxtools-mpes` plugin:
-```shell
-pip install pynxtools[mpes]
-```
-
-In addition, you can also install all of the `pynxtools` reader plugins which are maintained by FAIRmat by passing the `[convert]` extra to the pip install call:
-```shell
-pip install pynxtools[convert]
-```
-There is also a [cookiecutter template](https://github.com/FAIRmat-NFDI/pynxtools-plugin-template) available for creating your own pynxtools plugin.
-
 # Contributing
 
 ## Development install
 
 Install the package with its dependencies:
 
 ```shell
```

### Comparing `pynxtools-0.2.1/TROUBLESHOOTING.md` & `pynxtools-0.3.0/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/dev-requirements.txt` & `pynxtools-0.3.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/__init__.py` & `pynxtools-0.3.0/pynxtools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import re
 from datetime import datetime
-from glob import glob
-from typing import Union
 
 from pynxtools._build_wrapper import get_vcs_version
 from pynxtools.definitions.dev_tools.globals.nxdl import get_nxdl_version
 
 MAIN_BRANCH_NAME = "fairmat"
```

### Comparing `pynxtools-0.2.1/pynxtools/_build_wrapper.py` & `pynxtools-0.3.0/pynxtools/_build_wrapper.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/convert.py` & `pynxtools-0.3.0/pynxtools/dataconverter/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,26 +20,28 @@
 import glob
 import importlib.machinery
 import importlib.util
 import json
 import logging
 import os
 import sys
-import xml.etree.ElementTree as ET
 from gettext import gettext
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Literal, Optional, Tuple
 
 import click
+import lxml.etree as ET
 import yaml
 from click_default_group import DefaultGroup
 
 from pynxtools.dataconverter import helpers
+from pynxtools.dataconverter.nexus_tree import generate_tree_from
 from pynxtools.dataconverter.readers.base.reader import BaseReader
 from pynxtools.dataconverter.template import Template
+from pynxtools.dataconverter.validation import validate_dict_against
 from pynxtools.dataconverter.writer import Writer
 from pynxtools.nexus import nexus
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler())
 
@@ -95,69 +97,19 @@
             all_readers.append(
                 file[index_of_readers_folder_name:index_of_last_path_sep]
             )
     plugins = list(map(lambda ep: ep.name, entry_points(group="pynxtools.reader")))
     return sorted(all_readers + plugins)
 
 
-def get_nxdl_root_and_path(nxdl: str):
-    """Get xml root element and file path from nxdl name e.g. NXapm.
-
-    Parameters
-    ----------
-    nxdl: str
-        Name of nxdl file e.g. NXapm from NXapm.nxdl.xml.
-
-    Returns
-    -------
-    ET.root
-        Root element of nxdl file.
-    str
-        Path of nxdl file.
-
-    Raises
-    ------
-    FileNotFoundError
-        Error if no file with the given nxdl name is found.
-    """
-    # Reading in the NXDL and generating a template
-    definitions_path = nexus.get_nexus_definitions_path()
-    if nxdl == "NXtest":
-        nxdl_f_path = os.path.join(
-            f"{os.path.abspath(os.path.dirname(__file__))}/../../",
-            "tests",
-            "data",
-            "dataconverter",
-            "NXtest.nxdl.xml",
-        )
-    elif nxdl == "NXroot":
-        nxdl_f_path = os.path.join(definitions_path, "base_classes", "NXroot.nxdl.xml")
-    else:
-        nxdl_f_path = os.path.join(
-            definitions_path, "contributed_definitions", f"{nxdl}.nxdl.xml"
-        )
-        if not os.path.exists(nxdl_f_path):
-            nxdl_f_path = os.path.join(
-                definitions_path, "applications", f"{nxdl}.nxdl.xml"
-            )
-        if not os.path.exists(nxdl_f_path):
-            nxdl_f_path = os.path.join(
-                definitions_path, "base_classes", f"{nxdl}.nxdl.xml"
-            )
-        if not os.path.exists(nxdl_f_path):
-            raise FileNotFoundError(f"The nxdl file, {nxdl}, was not found.")
-
-    return ET.parse(nxdl_f_path).getroot(), nxdl_f_path
-
-
 def transfer_data_into_template(
     input_file,
     reader,
     nxdl_name,
-    nxdl_root: Optional[ET.Element] = None,
+    nxdl_root: Optional[ET._Element] = None,
     skip_verify: bool = False,
     **kwargs,
 ):
     """Transfer parse and merged data from input experimental file, config file and eln.
 
     Experimental and eln files will be parsed and finally will be merged into template.
     Before returning the template validate the template data.
@@ -178,15 +130,15 @@
     Returns
     -------
     Template
         Template filled with data from raw file and eln file.
 
     """
     if nxdl_root is None:
-        nxdl_root, _ = get_nxdl_root_and_path(nxdl=nxdl_name)
+        nxdl_root, _ = helpers.get_nxdl_root_and_path(nxdl=nxdl_name)
 
     template = Template()
     helpers.generate_template_from_nxdl(nxdl_root, template)
 
     if isinstance(input_file, str):
         input_file = (input_file,)
 
@@ -200,19 +152,32 @@
     if not (
         nxdl_name in data_reader.supported_nxdls or "*" in data_reader.supported_nxdls
     ):
         raise NotImplementedError(
             "The chosen NXDL isn't supported by the selected reader."
         )
 
+    if "ignore_undocumented" in kwargs:
+        ignore_undocumented = kwargs["ignore_undocumented"]
+        del kwargs["ignore_undocumented"]
+    else:
+        ignore_undocumented = False
+
     data = data_reader().read(  # type: ignore[operator]
         template=Template(template), file_paths=input_file, **kwargs
     )
+    entry_names = data.get_all_entry_names()
+    for entry_name in entry_names:
+        helpers.write_nexus_def_to_entry(data, entry_name, nxdl_name)
     if not skip_verify:
-        helpers.validate_data_dict(template, data, nxdl_root)
+        validate_dict_against(
+            nxdl_name,
+            data,
+            ignore_undocumented=ignore_undocumented,
+        )
     return data
 
 
 # pylint: disable=too-many-arguments,too-many-locals,W1203
 def convert(
     input_file: Tuple[str, ...],
     reader: str,
@@ -247,15 +212,15 @@
         Skips verification routine if set to True
 
     Returns
     -------
     None.
     """
 
-    nxdl_root, nxdl_f_path = get_nxdl_root_and_path(nxdl)
+    nxdl_root, nxdl_f_path = helpers.get_nxdl_root_and_path(nxdl)
 
     data = transfer_data_into_template(
         input_file=input_file,
         reader=reader,
         nxdl_name=nxdl,
         nxdl_root=nxdl_root,
         skip_verify=skip_verify,
@@ -360,14 +325,20 @@
 @click.option(
     "--undocumented",
     is_flag=True,
     default=False,
     help="Shows a log output for all undocumented fields",
 )
 @click.option(
+    "--ignore-undocumented",
+    is_flag=True,
+    default=False,
+    help="Ignore all undocumented fields during validation.",
+)
+@click.option(
     "--skip-verify",
     is_flag=True,
     default=False,
     help="Skips the verification routine during conversion.",
 )
 @click.option(
     "--mapping",
@@ -379,14 +350,15 @@
     files: Tuple[str, ...],
     input_file: Tuple[str, ...],
     reader: str,
     nxdl: str,
     output: str,
     fair: bool,
     params_file: str,
+    ignore_undocumented: bool,
     undocumented: bool,
     skip_verify: bool,
     mapping: str,
 ):
     """This command allows you to use the converter functionality of the dataconverter."""
     if params_file:
         try:
@@ -419,23 +391,29 @@
         file_list.append(file)
 
     if input_file:
         logger.warning(
             "The --input-file option is deprecated. Please use the positional arguments instead."
         )
 
-    convert(
-        tuple(file_list) + input_file,
-        reader,
-        nxdl,
-        output,
-        fair,
-        undocumented,
-        skip_verify,
-    )
+    try:
+        convert(
+            tuple(file_list) + input_file,
+            reader,
+            nxdl,
+            output,
+            fair,
+            undocumented,
+            skip_verify,
+            ignore_undocumented=ignore_undocumented,
+        )
+    except FileNotFoundError as exc:
+        raise click.BadParameter(
+            f"{nxdl} is not a valid application definition", param_hint="--nxdl"
+        ) from exc
 
 
 @main_cli.command()
 @click.option(
     "--nxdl",
     default=None,
     help=("The name of the NXDL file to use without extension. For example: NXmpes"),
@@ -460,27 +438,30 @@
     "Generates and prints a template to use for your nxdl."
 
     def write_to_file(text):
         f = open(output, "w")
         f.write(text)
         f.close()
 
-    print_or_write = lambda txt: write_to_file(txt) if output else print(txt)
+    tree = generate_tree_from(nxdl)
 
-    nxdl_root, nxdl_f_path = get_nxdl_root_and_path(nxdl)
-    template = Template()
-    helpers.generate_template_from_nxdl(nxdl_root, template)
+    print_or_write = lambda txt: write_to_file(txt) if output else print(txt)
 
+    level: Literal["required", "recommended", "optional"] = "optional"
     if required:
-        template = Template(template.get_optionality("required"))
+        level = "required"
+    reqs = tree.required_fields_and_attrs_names(level=level)
+    template = {
+        helpers.convert_nxdl_path_dict_to_data_converter_dict(req): None for req in reqs
+    }
 
     if pythonic:
         print_or_write(str(template))
         return
     print_or_write(
         json.dumps(
-            template.get_accumulated_dict(),
+            template,
             indent=4,
             sort_keys=True,
             ensure_ascii=False,
         )
     )
```

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/exceptions.py` & `pynxtools-0.3.0/pynxtools/dataconverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/file_hashing.py` & `pynxtools-0.3.0/pynxtools/dataconverter/file_hashing.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/hdfdict.py` & `pynxtools-0.3.0/pynxtools/dataconverter/hdfdict.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/helpers.py` & `pynxtools-0.3.0/pynxtools/dataconverter/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,31 +15,165 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Helper functions commonly used by the convert routine."""
 
 import json
 import logging
+import os
 import re
 from datetime import datetime, timezone
+from enum import Enum
+from functools import lru_cache
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import h5py
 import lxml.etree as ET
 import numpy as np
 from ase.data import chemical_symbols
 
 from pynxtools import get_nexus_version, get_nexus_version_hash
 from pynxtools.nexus import nexus
-from pynxtools.nexus.nexus import NxdlAttributeNotFoundError
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
+class ValidationProblem(Enum):
+    UnitWithoutDocumentation = 1
+    InvalidEnum = 2
+    MissingRequiredGroup = 3
+    MissingRequiredField = 4
+    MissingRequiredAttribute = 5
+    InvalidType = 6
+    InvalidDatetime = 7
+    IsNotPosInt = 8
+    ExpectedGroup = 9
+    MissingDocumentation = 10
+    MissingUnit = 11
+    ChoiceValidationError = 12
+    UnitWithoutField = 13
+    AttributeForNonExistingField = 14
+    BrokenLink = 15
+    FailedNamefitting = 16
+    NXdataMissingSignalData = 17
+    NXdataMissingAxisData = 18
+    NXdataAxisMismatch = 19
+
+
+class Collector:
+    """A class to collect data and return it in a dictionary format."""
+
+    def __init__(self):
+        self.data = set()
+        self.logging = True
+
+    def _log(self, path: str, log_type: ValidationProblem, value: Optional[Any], *args):
+        if value is None:
+            value = "<unknown>"
+
+        if log_type == ValidationProblem.UnitWithoutDocumentation:
+            logger.warning(
+                f"The unit, {path} = {value}, "
+                "is being written but has no documentation"
+            )
+        elif log_type == ValidationProblem.InvalidEnum:
+            logger.warning(
+                f"The value at {path} should be on of the "
+                f"following strings: {value}"
+            )
+        elif log_type == ValidationProblem.MissingRequiredGroup:
+            logger.warning(f"The required group, {path}, hasn't been supplied.")
+        elif log_type == ValidationProblem.MissingRequiredField:
+            logger.warning(
+                f"The data entry corresponding to {path} is required "
+                "and hasn't been supplied by the reader.",
+            )
+        elif log_type == ValidationProblem.InvalidType:
+            logger.warning(
+                f"The value at {path} should be one of: {value}"
+                f", as defined in the NXDL as {args[0] if args else '<unknown>'}."
+            )
+        elif log_type == ValidationProblem.InvalidDatetime:
+            logger.warning(
+                f"The value at {path} = {value} should be a timezone aware ISO8601 "
+                "formatted str. For example, 2022-01-22T12:14:12.05018Z"
+                " or 2022-01-22T12:14:12.05018+00:00."
+            )
+        elif log_type == ValidationProblem.IsNotPosInt:
+            logger.warning(
+                f"The value at {path} should be a positive int, but is {value}."
+            )
+        elif log_type == ValidationProblem.ExpectedGroup:
+            logger.warning(
+                f"Expected a group at {path} but found a field or attribute."
+            )
+        elif log_type == ValidationProblem.MissingDocumentation:
+            logger.warning(f"Field {path} written without documentation.")
+        elif log_type == ValidationProblem.MissingUnit:
+            logger.warning(
+                f"Field {path} requires a unit in the unit category {value}."
+            )
+        elif log_type == ValidationProblem.MissingRequiredAttribute:
+            logger.warning(f'Missing attribute: "{path}"')
+        elif log_type == ValidationProblem.UnitWithoutField:
+            logger.warning(f"Unit {path} in dataset without its field {value}")
+        elif log_type == ValidationProblem.AttributeForNonExistingField:
+            logger.warning(
+                f"There were attributes set for the field {path}, "
+                "but the field does not exist."
+            )
+        elif log_type == ValidationProblem.BrokenLink:
+            logger.warning(f"Broken link at {path} to {value}")
+        elif log_type == ValidationProblem.FailedNamefitting:
+            logger.warning(f"Found no namefit of {path} in {value}.")
+        elif log_type == ValidationProblem.NXdataMissingSignalData:
+            logger.warning(f"Missing data for signal in {path}.")
+        elif log_type == ValidationProblem.NXdataMissingAxisData:
+            logger.warning(f"Missing data for @axes in {path}.")
+        elif log_type == ValidationProblem.NXdataAxisMismatch:
+            logger.warning(
+                f"Length of axis {path} does not match to {value} in dimension {args[0]}"
+            )
+
+    def collect_and_log(
+        self,
+        path: str,
+        log_type: ValidationProblem,
+        value: Optional[Any],
+        *args,
+        **kwargs,
+    ):
+        """Inserts a path into the data dictionary and logs the action."""
+        if log_type == ValidationProblem.MissingUnit and value in (
+            "NX_UNITLESS",
+            "NX_DIMENSIONLESS",
+            "NX_ANY",
+        ):
+            return
+        if self.logging:
+            self._log(path, log_type, value, *args, **kwargs)
+        self.data.add(path)
+
+    def has_validation_problems(self):
+        """Returns True if there were any validation problems."""
+        return len(self.data) > 0
+
+    def get(self):
+        """Returns the set of problematic paths."""
+        return self.data
+
+    def clear(self):
+        """Clears the collected data."""
+        self.data = set()
+
+
+collector = Collector()
+
+
 def is_a_lone_group(xml_element) -> bool:
     """Checks whether a given group XML element has no field or attributes mentioned"""
     if xml_element.get("type") == "NXentry":
         return False
     for child in xml_element.findall(".//"):
         if remove_namespace_from_tag(child.tag) in ("field", "attribute"):
             return False
@@ -55,14 +189,64 @@
         name_to_add = (
             f"{convert_nexus_to_caps(xml_element.attrib['type'])}"
             f"[{convert_nexus_to_suggested_name(xml_element.attrib['type'])}]"
         )
     return name_to_add
 
 
+def get_nxdl_root_and_path(nxdl: str):
+    """Get xml root element and file path from nxdl name e.g. NXapm.
+
+    Parameters
+    ----------
+    nxdl: str
+        Name of nxdl file e.g. NXapm from NXapm.nxdl.xml.
+
+    Returns
+    -------
+    ET.root
+        Root element of nxdl file.
+    str
+        Path of nxdl file.
+
+    Raises
+    ------
+    FileNotFoundError
+        Error if no file with the given nxdl name is found.
+    """
+    # Reading in the NXDL and generating a template
+    definitions_path = nexus.get_nexus_definitions_path()
+    if nxdl == "NXtest":
+        nxdl_f_path = os.path.join(
+            f"{os.path.abspath(os.path.dirname(__file__))}/../../",
+            "tests",
+            "data",
+            "dataconverter",
+            "NXtest.nxdl.xml",
+        )
+    elif nxdl == "NXroot":
+        nxdl_f_path = os.path.join(definitions_path, "base_classes", "NXroot.nxdl.xml")
+    else:
+        nxdl_f_path = os.path.join(
+            definitions_path, "contributed_definitions", f"{nxdl}.nxdl.xml"
+        )
+        if not os.path.exists(nxdl_f_path):
+            nxdl_f_path = os.path.join(
+                definitions_path, "applications", f"{nxdl}.nxdl.xml"
+            )
+        if not os.path.exists(nxdl_f_path):
+            nxdl_f_path = os.path.join(
+                definitions_path, "base_classes", f"{nxdl}.nxdl.xml"
+            )
+        if not os.path.exists(nxdl_f_path):
+            raise FileNotFoundError(f"The nxdl file, {nxdl}, was not found.")
+
+    return ET.parse(nxdl_f_path).getroot(), nxdl_f_path
+
+
 def get_all_defined_required_children_for_elem(xml_element):
     """Gets all possible inherited required children for a given NXDL element"""
     list_of_children_to_add = set()
     for child in xml_element:
         tag = remove_namespace_from_tag(child.tag)
         if tag not in ("group", "field", "attribute"):
             continue
@@ -136,20 +320,25 @@
 
     tag = remove_namespace_from_tag(root.tag)
 
     if tag == "doc":
         return
 
     suffix = ""
-    if "name" in root.attrib:
+    if "name" in root.attrib and not contains_uppercase(root.attrib["name"]):
         suffix = root.attrib["name"]
     elif "type" in root.attrib:
         nexus_class = convert_nexus_to_caps(root.attrib["type"])
-        hdf5name = f"[{convert_nexus_to_suggested_name(root.attrib['type'])}]"
-        suffix = f"{nexus_class}{hdf5name}"
+        name = root.attrib.get("name")
+        hdf_name = root.attrib.get("type")[2:]  # .removeprefix("NX") (python > 3.8)
+        suffix = (
+            f"{name}[{name.lower()}]"
+            if name is not None
+            else f"{nexus_class}[{hdf_name}]"
+        )
 
     path = path + "/" + (f"@{suffix}" if tag == "attribute" else suffix)
 
     # Only add fields or attributes to the dictionary
     if tag in ("field", "attribute"):
         optionality = get_required_string(root)
         if optionality == "required":
@@ -206,29 +395,62 @@
 
 
 def convert_nexus_to_caps(nexus_name):
     """Helper function to convert a NeXus class from <NxClass> to <CLASS>."""
     return nexus_name[2:].upper()
 
 
+def contains_uppercase(field_name: Optional[str]) -> bool:
+    """Helper function to check if a field name contains uppercase characters."""
+    if field_name is None:
+        return False
+    return any(char.isupper() for char in field_name)
+
+
 def convert_nexus_to_suggested_name(nexus_name):
     """Helper function to suggest a name for a group from its NeXus class."""
+    if contains_uppercase(nexus_name):
+        return nexus_name
     return nexus_name[2:]
 
 
 def convert_data_converter_entry_to_nxdl_path_entry(entry) -> Union[str, None]:
     """
     Helper function to convert data converter style entry to NXDL style entry:
     ENTRY[entry] -> ENTRY
     """
     regex = re.compile(r"(.*?)(?=\[)")
     results = regex.search(entry)
     return entry if results is None else results.group(1)
 
 
+def convert_nxdl_path_entry_to_data_converter_entry(entry) -> str:
+    """
+    Helper function to convert NXDL style entry to data converter style entry:
+    ENTRY -> ENTRY[entry]
+    """
+    return f"{entry}[{entry.lower()}]"
+
+
+def convert_nxdl_path_dict_to_data_converter_dict(path) -> str:
+    """
+    Helper function to convert NXDL style path to data converter style path:
+    /ENTRY/entry -> /ENTRY[entry]/entry
+    """
+    data_converter_path = ""
+    for entry in path.split("/")[1:]:
+        if not contains_uppercase(entry):
+            data_converter_path += f"/{entry}"
+            continue
+        data_converter_path += "/" + convert_nxdl_path_entry_to_data_converter_entry(
+            entry
+        )
+    return data_converter_path
+
+
 def convert_data_converter_dict_to_nxdl_path(path) -> str:
     """
     Helper function to convert data converter style path to NXDL style path:
     /ENTRY[entry]/sample -> /ENTRY/sample
     """
     nxdl_path = ""
     for entry in path.split("/")[1:]:
@@ -237,16 +459,20 @@
 
 
 def get_name_from_data_dict_entry(entry: str) -> str:
     """Helper function to get entry name from data converter style entry
 
     ENTRY[entry] -> entry
     """
-    regex = re.compile(r"(?<=\[)(.*?)(?=\])")
-    results = regex.search(entry)
+
+    @lru_cache(maxsize=None)
+    def get_regex():
+        return re.compile(r"(?<=\[)(.*?)(?=\])")
+
+    results = get_regex().search(entry)
     if results is None:
         return entry
     if entry[0] == "@":
         return "@" + results.group(1)
     return results.group(1)
 
 
@@ -257,22 +483,20 @@
     """
     hdf5path = ""
     for entry in path.split("/")[1:]:
         hdf5path += "/" + get_name_from_data_dict_entry(entry)
     return hdf5path
 
 
-def is_value_valid_element_of_enum(value, elem) -> Tuple[bool, list]:
+def is_value_valid_element_of_enum(value, elist) -> Tuple[bool, list]:
     """Checks whether a value has to be specific from the NXDL enumeration and returns options."""
-    if elem is not None:
-        has_enums, enums = nexus.get_enums(elem)
-        if has_enums and (
-            isinstance(value, list) or value not in enums[0:-1] or value == ""
-        ):
-            return False, enums
+    for elem in elist:
+        enums = nexus.get_enums(elem)
+        if enums is not None:
+            return value in enums, enums
     return True, []
 
 
 NUMPY_FLOAT_TYPES = (np.half, np.float16, np.single, np.double, np.longdouble)
 NUMPY_INT_TYPES = (np.short, np.intc, np.int_)
 NUMPY_UINT_TYPES = (np.ushort, np.uintc, np.uint)
 
@@ -341,15 +565,15 @@
     if value.lower() == "true":
         return True
     if value.lower() == "false":
         return False
     return None
 
 
-def is_valid_data_field(value, nxdl_type, path):
+def is_valid_data_field(value, nxdl_type, path) -> bool:
     """Checks whether a given value is valid according to what is defined in the NXDL.
 
     This function will also try to convert typical types, for example int to float,
     and return the successful conversion.
 
     If it fails to convert, it raises an Exception.
 
@@ -360,57 +584,45 @@
     if not isinstance(value, dict) and not is_valid_data_type(value, accepted_types):
         try:
             if accepted_types[0] is bool and isinstance(value, str):
                 value = convert_str_to_bool_safe(value)
                 if value is None:
                     raise ValueError
             return accepted_types[0](value)
-        except ValueError as exc:
-            raise ValueError(
-                f"The value at {path} should be of Python type: {accepted_types}"
-                f", as defined in the NXDL as {nxdl_type}."
-            ) from exc
+        except ValueError:
+            collector.collect_and_log(
+                path, ValidationProblem.InvalidType, accepted_types, nxdl_type
+            )
 
     if nxdl_type == "NX_POSINT" and not is_positive_int(value):
-        raise ValueError(f"The value at {path} should be a positive int.")
+        collector.collect_and_log(path, ValidationProblem.IsNotPosInt, value)
 
     if nxdl_type in ("ISO8601", "NX_DATE_TIME"):
         iso8601 = re.compile(
             r"^(\d{4})-(\d{2})-(\d{2})T(\d{2}):(\d{2}):(\d{2}(?:"
             r"\.\d*)?)(((?!-00:00)(\+|-)(\d{2}):(\d{2})|Z){1})$"
         )
         results = iso8601.search(value)
         if results is None:
-            raise ValueError(
-                f"The date at {path} should be a timezone aware ISO8601 "
-                f"formatted str. For example, 2022-01-22T12:14:12.05018Z"
-                f" or 2022-01-22T12:14:12.05018+00:00."
-            )
+            collector.collect_and_log(path, ValidationProblem.InvalidDatetime, value)
 
-    return value
+    return True
 
 
-def path_in_data_dict(nxdl_path: str, hdf_path: str, data: dict) -> Tuple[bool, str]:
+@lru_cache(maxsize=None)
+def path_in_data_dict(nxdl_path: str, data_keys: Tuple[str, ...]) -> List[str]:
     """Checks if there is an accepted variation of path in the dictionary & returns the path."""
-    accepted_unfilled_key = None
-    for key in data.keys():
-        if (
-            nxdl_path == convert_data_converter_dict_to_nxdl_path(key)
-            or convert_data_dict_path_to_hdf5_path(key) == hdf_path
-        ):
-            if data[key] is None:
-                accepted_unfilled_key = key
-                continue
-            return True, key
-    if accepted_unfilled_key:
-        return True, accepted_unfilled_key
-    return False, None
+    found_keys = []
+    for key in data_keys:
+        if nxdl_path == convert_data_converter_dict_to_nxdl_path(key):
+            found_keys.append(key)
+    return found_keys
 
 
-def check_for_optional_parent(path: str, nxdl_root: ET.Element) -> str:
+def check_for_optional_parent(path: str, nxdl_root: ET._Element) -> str:
     """Finds a parent in the branch that is optional and returns it's path or s<<NOT_FOUND>>."""
     parent_path = path.rsplit("/", 1)[0]
 
     if parent_path == "":
         return "<<NOT_FOUND>>"
 
     parent_nxdl_path = convert_data_converter_dict_to_nxdl_path(parent_path)
@@ -433,30 +645,25 @@
         )
     node = nexus.get_node_at_nxdl_path(nxdl_key, elem=nxdl_root, exc=False)
     return nexus.get_required_string(node) == "<<REQUIRED>>"
 
 
 def all_required_children_are_set(optional_parent_path, data, nxdl_root):
     """Walks over optional parent's children and makes sure all required ones are set"""
-    optional_parent_path = convert_data_converter_dict_to_nxdl_path(
-        optional_parent_path
-    )
     for key in data:
         if key in data["lone_groups"]:
             continue
         nxdl_key = convert_data_converter_dict_to_nxdl_path(key)
+        name = nxdl_key[nxdl_key.rfind("/") + 1 :]
+        renamed_path = f"{optional_parent_path}/{name}"
         if (
-            nxdl_key[0 : nxdl_key.rfind("/")] == optional_parent_path
+            nxdl_key[: nxdl_key.rfind("/")]
+            == convert_data_converter_dict_to_nxdl_path(optional_parent_path)
             and is_node_required(nxdl_key, nxdl_root)
-            and data[
-                path_in_data_dict(
-                    nxdl_key, convert_data_dict_path_to_hdf5_path(key), data
-                )[1]
-            ]
-            is None
+            and (renamed_path not in data or data[renamed_path] is None)
         ):
             return False
 
     return True
 
 
 def is_nxdl_path_a_child(nxdl_path: str, parent: str):
@@ -464,29 +671,14 @@
     while nxdl_path.rfind("/") != -1:
         nxdl_path = nxdl_path[0 : nxdl_path.rfind("/")]
         if parent == nxdl_path:
             return True
     return False
 
 
-def check_optionality_based_on_parent_group(path, nxdl_path, nxdl_root, data, template):
-    """Checks whether field is part of an optional parent and then confirms its optionality"""
-    for optional_parent in template["optional_parents"]:
-        optional_parent_nxdl = convert_data_converter_dict_to_nxdl_path(optional_parent)
-        if is_nxdl_path_a_child(
-            nxdl_path, optional_parent_nxdl
-        ) and not all_required_children_are_set(optional_parent, data, nxdl_root):
-            raise LookupError(
-                f"The data entry, {path}, has an optional parent, "
-                f"{optional_parent}, with required children set. Either"
-                f" provide no children for {optional_parent} or provide"
-                f" all required ones."
-            )
-
-
 def is_group_part_of_path(path_to_group: str, path_of_entry: str) -> bool:
     """Returns true if a group is contained in a path"""
 
     tokens_group = path_to_group.split("/")
     tokens_entry = convert_data_converter_dict_to_nxdl_path(path_of_entry).split("/")
 
     if len(tokens_entry) < len(tokens_group):
@@ -504,141 +696,22 @@
     path_to_group = convert_data_converter_dict_to_nxdl_path(path_to_group)
     for path in data:
         if is_group_part_of_path(path_to_group, path) and data[path] is not None:
             return True
     return False
 
 
-# pylint: disable=W1203
-def ensure_all_required_fields_exist(template, data, nxdl_root):
-    """Checks whether all the required fields are in the returned data object."""
-    for path in template["required"]:
-        entry_name = get_name_from_data_dict_entry(path[path.rindex("/") + 1 :])
-        if entry_name == "@units":
-            continue
-        nxdl_path = convert_data_converter_dict_to_nxdl_path(path)
-        is_path_in_data_dict, renamed_path = path_in_data_dict(
-            nxdl_path, convert_data_dict_path_to_hdf5_path(path), data
-        )
-
-        renamed_path = path if renamed_path is None else renamed_path
-        if path in template["lone_groups"]:
-            opt_parent = check_for_optional_parent(path, nxdl_root)
-            if opt_parent != "<<NOT_FOUND>>":
-                if does_group_exist(opt_parent, data) and not does_group_exist(
-                    renamed_path, data
-                ):
-                    logger.warning(
-                        f"The required group, {path}, hasn't been supplied"
-                        f" while its optional parent, {opt_parent}, is supplied."
-                    )
-                continue
-            if not does_group_exist(renamed_path, data):
-                logger.warning(f"The required group, {path}, hasn't been supplied.")
-                continue
-            continue
-        if not is_path_in_data_dict or data[renamed_path] is None:
-            logger.warning(
-                f"The data entry corresponding to {path} is required "
-                f"and hasn't been supplied by the reader.",
-            )
-
-
-def try_undocumented(data, nxdl_root: ET.Element):
-    """Tries to move entries used that are from base classes but not in AppDef"""
-    for path in list(data.undocumented):
-        entry_name = get_name_from_data_dict_entry(path[path.rindex("/") + 1 :])
-
-        nxdl_path = convert_data_converter_dict_to_nxdl_path(path)
-
-        if entry_name == "@units":
-            field_path = path.rsplit("/", 1)[0]
-            if field_path in data.get_documented() and path in data.undocumented:
-                field_requiredness = get_required_string(
-                    nexus.get_node_at_nxdl_path(
-                        nxdl_path=convert_data_converter_dict_to_nxdl_path(field_path),
-                        elem=nxdl_root,
-                    )
-                )
-                data[field_requiredness][path] = data.undocumented[path]
-                del data.undocumented[path]
-            continue
-
-        if entry_name[0] == "@" and "@" in nxdl_path:
-            index_of_at = nxdl_path.rindex("@")
-            nxdl_path = nxdl_path[0:index_of_at] + nxdl_path[index_of_at + 1 :]
-
-        try:
-            elem = nexus.get_node_at_nxdl_path(nxdl_path=nxdl_path, elem=nxdl_root)
-            data[get_required_string(elem)][path] = data.undocumented[path]
-            del data.undocumented[path]
-            units = f"{path}/@units"
-            if units in data.undocumented:
-                data[get_required_string(elem)][units] = data.undocumented[units]
-                del data.undocumented[units]
-        except NxdlAttributeNotFoundError:
-            pass
-
-
-def validate_data_dict(template, data, nxdl_root: ET.Element):
-    """Checks whether all the required paths from the template are returned in data dict."""
-    assert nxdl_root is not None, "The NXDL file hasn't been loaded."
-
-    # nxdl_path_set helps to skip validation check on the same type of nxdl signiture
-    # This reduces huge amount of runing time
-    nxdl_path_to_elm: dict = {}
-
-    # Make sure all required fields exist.
-    ensure_all_required_fields_exist(template, data, nxdl_root)
-    try_undocumented(data, nxdl_root)
-
-    for path in data.get_documented().keys():
-        if data[path] is not None:
-            entry_name = get_name_from_data_dict_entry(path[path.rindex("/") + 1 :])
-            nxdl_path = convert_data_converter_dict_to_nxdl_path(path)
-
-            if entry_name == "@units":
-                continue
-
-            if entry_name[0] == "@" and "@" in nxdl_path:
-                index_of_at = nxdl_path.rindex("@")
-                nxdl_path = nxdl_path[0:index_of_at] + nxdl_path[index_of_at + 1 :]
-
-            if nxdl_path in nxdl_path_to_elm:
-                elem = nxdl_path_to_elm[nxdl_path]
-            else:
-                elem = nexus.get_node_at_nxdl_path(nxdl_path=nxdl_path, elem=nxdl_root)
-                nxdl_path_to_elm[nxdl_path] = elem
-
-            # Only check for validation in the NXDL if we did find the entry
-            # otherwise we just pass it along
-            if (
-                elem is not None
-                and elem.attrib.get("name") == entry_name
-                and remove_namespace_from_tag(elem.tag) in ("field", "attribute")
-            ):
-                check_optionality_based_on_parent_group(
-                    path, nxdl_path, nxdl_root, data, template
-                )
-
-                attrib = elem.attrib
-                nxdl_type = (
-                    attrib["type"]
-                    if "type" in attrib.keys()
-                    else "NXDL_TYPE_UNAVAILABLE"
-                )
-                data[path] = is_valid_data_field(data[path], nxdl_type, path)
-                is_valid_enum, enums = is_value_valid_element_of_enum(data[path], elem)
-                if not is_valid_enum:
-                    raise ValueError(
-                        f"The value at {path} should be on of the "
-                        f"following strings: {enums}"
-                    )
-
-    return True
+def get_concept_basepath(path: str) -> str:
+    """Get the concept path from the path"""
+    path_list = path.split("/")
+    concept_path = []
+    for p in path_list:
+        if re.search(r"[A-Z]", p):
+            concept_path.append(p)
+    return "/" + "/".join(concept_path)
 
 
 def remove_namespace_from_tag(tag):
     """Helper function to remove the namespace from an XML tag."""
 
     if not isinstance(tag, str):
         return ""
@@ -691,15 +764,15 @@
     """
     Takes a dict/Template and adds NXroot fields/attributes that are inherently available
     """
 
     def update_and_warn(key: str, value: str):
         if key in data and data[key] != value:
             logger.warning(
-                f"The NXroot entry '{key}' (value: {data[key]}) should not be populated by "
+                f"The NXroot entry '{key}' (value: {data[key]}) should not be changed by "
                 f"the reader. This is overwritten by the actually used value '{value}'"
             )
         data[key] = value
 
     update_and_warn("/@NX_class", "NXroot")
     update_and_warn("/@file_name", filename)
     update_and_warn("/@file_time", str(datetime.now(timezone.utc).astimezone()))
@@ -710,14 +783,42 @@
         f"blob/{get_nexus_version_hash()}",
     )
     update_and_warn("/@NeXus_version", get_nexus_version())
     update_and_warn("/@HDF5_version", ".".join(map(str, h5py.h5.get_libversion())))
     update_and_warn("/@h5py_version", h5py.__version__)
 
 
+def write_nexus_def_to_entry(data, entry_name: str, nxdl_def: str):
+    """
+    Writes the used nexus definition and version to /ENTRY/definition
+    """
+
+    def update_and_warn(key: str, value: str, overwrite=False):
+        if key in data and data[key] is not None and data[key] != value:
+            report = (
+                f"This is overwritten by the actually used value '{value}'"
+                if overwrite
+                else f"The provided version '{value}' is kept. We assume you know what you are doing."
+            )
+            logger.log(
+                logging.WARNING if overwrite else logging.INFO,
+                f"The entry '{key}' (value: {data[key]}) should not be changed by "
+                f"the reader. {report}",
+            )
+        if overwrite or data.get(key) is None:
+            data[key] = value
+
+    update_and_warn(f"/ENTRY[{entry_name}]/definition", nxdl_def, overwrite=True)
+    update_and_warn(
+        f"/ENTRY[{entry_name}]/definition/@version",
+        get_nexus_version(),
+        overwrite=False,
+    )
+
+
 def extract_atom_types(formula, mode="hill"):
     """Extract atom types form chemical formula."""
     atom_types: set = set()
     element: str = ""
 
     for char in formula:
         if char.isalpha():
```

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/readers/base/reader.py` & `pynxtools-0.3.0/pynxtools/dataconverter/readers/base/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/readers/example/reader.py` & `pynxtools-0.3.0/pynxtools/dataconverter/readers/example/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,40 +55,38 @@
 
         for k in template.keys():
             # The entries in the template dict should correspond with what the dataconverter
             # outputs with --generate-template for a provided NXDL file
             if (
                 k.startswith("/ENTRY[entry]/required_group")
                 or k == "/ENTRY[entry]/optional_parent/req_group_in_opt_group"
+                or k.startswith("/ENTRY[entry]/OPTIONAL_group")
             ):
                 continue
 
             field_name = k[k.rfind("/") + 1 :]
             if field_name != "@units":
                 template[k] = data[field_name]
-                if (
-                    f"{field_name}_units" in data.keys()
-                    and f"{k}/@units" in template.keys()
-                ):
+                if f"{field_name}_units" in data.keys():
                     template[f"{k}/@units"] = data[f"{field_name}_units"]
 
         template["required"]["/ENTRY[entry]/optional_parent/required_child"] = 1
         template["optional"][
-            ("/ENTRY[entry]/optional_parent/" "req_group_in_opt_group/DATA[data]")
+            "/ENTRY[entry]/optional_parent/req_group_in_opt_group/DATA[data]"
         ] = [0, 1]
 
         # Add non template key
         template["/ENTRY[entry]/does/not/exist"] = "None"
         template["/ENTRY[entry]/required_group/description"] = "A test description"
         template["/ENTRY[entry]/required_group2/description"] = "A test description"
         template["/ENTRY[entry]/program_name"] = "None"
 
         # internal links
         template["/ENTRY[entry]/test_link/internal_link"] = {
-            "link": "/entry/NXODD_name/posint_value"
+            "link": "/entry/nxodd_name/posint_value"
         }
 
         # external links
         template[("/ENTRY[entry]/test_link/external_link")] = {
             "link": f"{os.path.dirname(__file__)}/../../../../tests/"
             "data/nexus/xarray_saved_small_calibration.h5:/axes/ax3"
         }
```

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/readers/json_map/reader.py` & `pynxtools-0.3.0/pynxtools/dataconverter/readers/json_map/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/readers/json_yml/reader.py` & `pynxtools-0.3.0/pynxtools/dataconverter/readers/json_yml/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/readers/utils.py` & `pynxtools-0.3.0/pynxtools/dataconverter/readers/utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/template.py` & `pynxtools-0.3.0/pynxtools/dataconverter/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """A Template object to control and separate template paths according to optionality"""
 
 import copy
 import json
+import re
+from typing import Set
 
 from pynxtools.dataconverter import helpers
 
 
 class Template(dict):
     """A Template object to control and separate template paths according to optionality"""
 
@@ -145,24 +147,21 @@
 
     def __getitem__(self, k):
         """Handles how values are accessed from the Template object."""
         # Try setting item in all else throw error. Does not append to default.
         if k in ("optional_parents", "lone_groups"):
             return getattr(self, k)
         if k.startswith("/"):
-            try:
+            if k in self.optional:
                 return self.optional[k]
-            except KeyError:
-                try:
-                    return self.recommended[k]
-                except KeyError:
-                    try:
-                        return self.required[k]
-                    except KeyError:
-                        return self.undocumented[k]
+            if k in self.recommended:
+                return self.recommended[k]
+            if k in self.required:
+                return self.required[k]
+            return self.undocumented.get(k)
         if k in ("required", "optional", "recommended", "undocumented"):
             return self.get_optionality(k)
         raise KeyError(
             "Only paths starting with '/' or one of [optional_parents, "
             "lone_groups, required, optional, recommended, undocumented] can be used."
         )
 
@@ -193,14 +192,28 @@
                     key.index(entry_search_term) + len(entry_search_term) :
                 ]
                 if entry_name == old_name:
                     value = internal_dict[key] if deepcopy else None
                     internal_dict[f"/ENTRY[{new_name}]{rest_of_path}"] = value
                     del internal_dict[key]
 
+    def get_all_entry_names(self) -> Set[str]:
+        """
+        Get all entry names in the template.
+
+        Returns:
+            Set[str]: A set of entry names.
+        """
+        entry_names = set()
+        for key in self:
+            entry_name_match = re.search(r"\/ENTRY\[([a-zA-Z0-9_\.]+)\]", key)
+            if entry_name_match is not None:
+                entry_names.add(entry_name_match.group(1))
+        return entry_names
+
     def update(self, template):
         """Merges second template to original
         or updates values from a dictionary if the type of :code:`template` is dict"""
         if isinstance(template, Template):
             for optionality in ("optional", "recommended", "required", "undocumented"):
                 self.get_optionality(optionality).update(
                     template.get_optionality(optionality)
```

### Comparing `pynxtools-0.2.1/pynxtools/dataconverter/writer.py` & `pynxtools-0.3.0/pynxtools/dataconverter/writer.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXarchive.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXarchive.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXarpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXarpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXcanSAS.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXcanSAS.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXdirecttof.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXdirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXfluo.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXfluo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXindirecttof.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXindirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXiqproc.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXiqproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXlauetof.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXlauetof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXmonopd.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXmonopd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXmx.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXmx.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXrefscan.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXrefscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXreftof.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXreftof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXsas.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXsas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXsastof.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXsastof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXscan.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXspe.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXspe.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXsqom.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXsqom.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXstxm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXstxm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtas.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtofnpd.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtofnpd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtofraw.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtofraw.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtofsingle.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtofsingle.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtomo.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtomo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtomophase.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtomophase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXtomoproc.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXtomoproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxas.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxasproc.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxasproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxbase.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxbase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxeuler.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxeuler.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxkappa.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxkappa.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxlaue.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxlaue.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxnb.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxnb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/applications/NXxrot.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/applications/NXxrot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXaperture.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXaperture.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbeam.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbeam.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcite.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcite.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcollection.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcollection.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdata.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector.nxdl.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -465,14 +465,15 @@
     <enumeration>
       <item value="gated"/>
       <item value="triggered"/>
       <item value="summed"/>
       <item value="event"/>
       <item value="histogrammed"/>
       <item value="decimated"/>
+      <item value="pulse counting"/>
     </enumeration>
   </field>
   <field name="angular_calibration_applied" type="NX_BOOLEAN">
     <doc>True when the angular calibration has been applied in the
              electronics, false otherwise.</doc>
   </field>
   <field name="angular_calibration" type="NX_FLOAT">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXentry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml`

 * *Files 4% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml`

```diff
@@ -65,8 +65,19 @@
     <doc>Any actuator used to control the environment. This can be linked to an actuator
              defined in an NXinstrument instance.</doc>
   </group>
   <group type="NXsensor">
     <doc>Any sensor used to monitor the environment. This can be linked to a sensor
              defined in an NXinstrument instance.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfilter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfilter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXflipper.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXflipper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXgrating.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXgrating.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXguide.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXguide.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXlog.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXlog.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmirror.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmirror.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXnote.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXnote.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXobject.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXobject.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXorientation.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXorientation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXparameters.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXparameters.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpdb.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpdb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXprocess.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXprocess.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXreflections.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXreflections.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXroot.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXroot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsample.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsample.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsensor.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsensor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXshape.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXshape.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXslit.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXslit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsource.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsource.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXuser.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXuser.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml`

 * *Files 8% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml`

```diff
@@ -78,9 +78,20 @@
   </field>
   <group type="NXtransformations">
     <doc>This is the group recommended for holding the chain of translation
              and rotation operations necessary to position the actuator within
              the instrument. The dependency chain may however traverse similar groups in
              other component groups.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
   <group type="NXfabrication"/>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml`

```diff
@@ -283,15 +283,15 @@
                          challenged by these differences as at.-% and wt.-% are both
                          fractional quantities.</doc>
           <enumeration>
             <item value="atom_percent"/>
             <item value="weight_percent"/>
           </enumeration>
         </field>
-        <group type="NXion" minOccurs="1" maxOccurs="118">
+        <group name="ionID" type="NXion" minOccurs="1" maxOccurs="118">
           <field name="chemical_symbol" type="NX_CHAR">
             <doc>Human-readable name of the element (e.g. Fe).
                              Name has to be a symbol of an element from the periodic table.
                              All symbols in the set of NXion instances inside the group
                              chemical_composition need to be disjoint.</doc>
           </field>
           <field name="composition" type="NX_FLOAT" units="NX_DIMENSIONLESS">
@@ -694,15 +694,15 @@
         </group>
         <field name="evaporation_identifier_offset" type="NX_INT" units="NX_UNITLESS">
           <doc>Integer used to name the first pulse to know if there is an
                          offset of the evaporation_identifier to zero.
                          
                          Identifiers can be defined either implicitly or explicitly.
                          For implicit indexing identifiers are defined on the interval
-                         :math:`[identifier_offset, identifier_offset + c - 1]`.
+                         :math:`[identifier\_offset, identifier\_offset + c - 1]`.
                          
                          Therefore, implicit identifier are completely defined by the value of
                          identifier_offset and cardinality. For example if identifier run from
                          -2 to 3 the value for identifier_offset is -2.
                          
                          For explicit indexing the field identifier has to be used.
                          Fortran-/Matlab- and C-/Python-style indexing have specific implicit
@@ -819,15 +819,15 @@
         <field name="reconstructed_positions" type="NX_FLOAT">
           <dimensions rank="2">
             <dim index="1" value="n"/>
             <dim index="2" value="3"/>
           </dimensions>
         </field>
         <group name="naive_discretization" type="NXprocess">
-          <group type="NXprogram" minOccurs="1" maxOccurs="unbounded">
+          <group name="programID" type="NXprogram" minOccurs="1" maxOccurs="unbounded">
             <field name="program" type="NX_CHAR">
               <attribute name="version" type="NX_CHAR"/>
             </field>
           </group>
           <!--config/input
 results-->
           <group type="NXdata">
@@ -942,23 +942,23 @@
           </group>
           <group name="peakID" type="NXpeak" minOccurs="0" maxOccurs="unbounded">
             <field name="label" type="NX_CHAR" recommended="true"/>
             <field name="description" type="NX_CHAR"/>
             <field name="category" type="NX_CHAR" recommended="true">
               <doc>Category for the peak offering a qualitative statement of the location of the peak
                                  in light of limited mass-resolving power that is relevant for
-                                 composition quantification. See `D. Larson et al. &lt;https://doi.org/10.1007/978-1-4614-8721-0&gt;`_ 
+                                 composition quantification. See `D. Larson et al. (p172) &lt;https://doi.org/10.1007/978-1-4614-8721-0&gt;`_ 
                                  for examples of each category:
                                  
-                                 * 0, well-separated, 10^B +, 28^Si ++
-                                 * 1, close, but typically sufficiently separated with LEAP system, 14^N +, 28^Si ++
-                                 * 2, closely overlapping, demands better than LEAP4000X MRP, 14^N +, 28^Si ++
-                                 * 3, overlapped, multi-charge state, 16^O 16^O ++, 16^O +
-                                 * 4, overlapped, same charge state, not discriminatable with a LEAP4000X, 14^N 14^N + 28^Si +
-                                 * 5, overlapped, same charge state, any expectation of resolvability, 54^Cr ++, 54^Fe ++</doc>
+                                 * 0, well-separated, :math:`^{10}B^{+}`, :math:`^{28}Si^{2+}`
+                                 * 1, close, but can be sufficiently separated for quantification in a LEAP system, :math:`^{94}Mo^{3+}`, :math:`^{63}Cu^{2+}`
+                                 * 2, closely overlapping, demands better than LEAP4000X MRP can provide :math:`^{14}N^{+}`, :math:`^{28}Si^{2+}` at different charge states
+                                 * 3, overlapped exactly due to multi-charge molecular species, :math:`^{16}{O_{2}}^{2+}`, :math:`^{16}O^{+}`
+                                 * 4, overlapped, same charge state, cannot as of 2013 be discriminated with a LEAP4000X, :math:`^{14}{N_{2}}^{+}`, :math:`^{28}Si^{+}`
+                                 * 5, overlapped, same charge state, any expectation of resolvability, :math:`^{54}Cr^{2+}`, :math:`^{54}Fe^{2+}`</doc>
               <enumeration>
                 <item value="0"/>
                 <item value="1"/>
                 <item value="2"/>
                 <item value="3"/>
                 <item value="4"/>
                 <item value="5"/>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml`

```diff
@@ -54,18 +54,18 @@
   <field name="nuclides" type="NX_UINT" units="NX_UNITLESS">
     <doc>Input constraint, list of nuclide_hash for typically elements used for the
              ranging definition of the ion whose charge state the analyses covered.
              The list contains each hash as many times as its multiplicity.
              Nuclides are encoded using the hashing rule that is defined in :ref:`NXion`.
              
              As an example, a ranging definition H:2 O:1 is configured by setting nuclides to
-             a list with entries :math:`1 + 256 * 0`, :math:`1 + 256 * 0`, :math:`8 + 256 * 0`.
+             a list with entries :math:`1 + 0 \cdot 256`, :math:`1 + 0 \cdot 256`, :math:`8 + 0 \cdot 256`.
              An empty list does not release the constraint. Instead, a list with all elements
              in the periodic table (encoded as nuclide_hash values) should be used, i.e.
-             :math:`1 + 256 * 0`, :math:`2 + 256 * 0`, and so on and so forth.
+             :math:`1 + 0 \cdot 256`, :math:`2 + 0 \cdot 256`, and so on and so forth.
              
              Keep in mind that with a weakly constrained parameter space the combinatorial
              analysis may become very time consuming!</doc>
     <dimensions rank="1">
       <dim index="1" value="i"/>
     </dimensions>
   </field>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml`

```diff
@@ -41,15 +41,15 @@
     <group name="v_v_spatial_correlationID" type="NXapm_paraprobe_tool_config" minOccurs="1" maxOccurs="unbounded">
       <doc>Tracking volume_volume_spatial_correlations (v_v) is the process of building logical
                  relations between objects, their proximity and eventual volumetric intersections.
                  Here, objects are assumed to be represented as a set of triangulated surface meshes.
                  
                  Volumetric overlap and proximity of volumetric features is identified for members of
                  sets of features to members of other sets of volumetric features. Specifically, for each time
-                 step :math:`$k$` pairs of sets are compared:
+                 step :math:`k` pairs of sets are compared:
                  Members of a so-called current_set to members of a so-called next_set.
                  Members can be different types of volumetric features.</doc>
       <!--config-->
       <field name="intersection_detection_method" type="NX_CHAR">
         <doc>Specifies the method whereby to decide if two objects intersect volumetrically.
                      For reasons which are detailed in the supplementary material of `M. Kühbach et al. &lt;https://arxiv.org/abs/2205.13510&gt;`_,
                      it is assumed by default that two objects intersect if they share at least one ion with the same evaporation ID (shared_ion).
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml`

```diff
@@ -640,28 +640,43 @@
                      those for the second DCOM iteration and so on and so forth.</doc>
         <dimensions rank="1">
           <dim index="1" value="n_fct_iterations"/>
         </dimensions>
       </field>
     </group>
     <group name="oned_profile" type="NXapm_paraprobe_tool_config" minOccurs="0" maxOccurs="1">
-      <doc>Analysis of one-dimensional profiles in ROIs placed in the dataset. Such analyses are useful for quantifying
-                 interfacial excess or classical composition analyses. The tool will test for each ROIs if it is completely embedded
-                 in the dataset. Specifically, in each such test the tool evaluates if the ROI cuts at least one triangle of the triangulated surface mesh refered to by surface. If this is the case the ROI is close to the surface and not analyzed further.
-                 Otherwise, the ROI is processed further.
+      <doc>Analysis of one-dimensional profiles in ROIs placed in the dataset.
+                 Such analyses are useful for quantifying interfacial excess or for
+                 performing classical composition analyses.
                  
-                 Users should be aware that the latter intersection analysis is not a volumetric intersection analysis as such one
-                 is much more computationally involved because the edge model can be a closed non-convex polyhedron
-                 in which case one would have to test robustly if the cylinder pierces or is laying completely inside the polyhedron.
-                 For this the polyhedron has to be tessellated first into convex polyhedra, as test for volumetric intersection using
-                 the Gilbert-Johnson-Keerthi algorithm (GJK) are applicable only to convex polyhedra.
+                 The tool will test for each ROIs if it is completely embedded in the dataset.
+                 Specifically, each such test evaluates if the ROI cuts at least one triangle
+                 of the triangulated surface mesh that is referred to by surface.
+                 If this is the case the ROI is marked as one close to the surface
+                 and not analyzed further. Otherwise, the ROI is marked as one far
+                 from the surface and processed further.
                  
-                 For each ROI the tool computes atomically decomposed profiles. This means, molecular ions are split into
-                 nuclides with respective multiplicity. For each processed ROI a set of a sorted list of signed distance values
-                 is returned to enable classical Krakauer/Seidman-style interfacial excess analyses.</doc>
+                 For each ROI the tool computes atomically decomposed profiles.
+                 This means, molecular ions are splitted into nuclides as many times as
+                 their respective multiplicity. For each processed ROI the tool stores
+                 a sorted list of signed distance values to enable post-processing with
+                 other software like e.g. reporter to perform classical
+                 Krakauer/Seidman-style interfacial excess analyses.
+                 
+                 Users should be aware that the latter intersection analysis is not
+                 a volumetric intersection analysis. Given that the triangulated mesh
+                 referred to in surface is not required to mesh neither a watertight
+                 nor convex polyhedron a rigorous testing of volumetric intersection
+                 is much more involved. If the mesh is watertight one could use split
+                 the task in first tessellating the mesh into convex polyhedra (e.g.
+                 tetrahedra and apply a volumetric intersection method like the
+                 Gilbert-Johnson-Keerthi algorithm (GJK). In cases when the mesh is not
+                 even watertight distance-based segmentation in combination with again
+                 intersection of triangles and convex polyhedra is a robust but currently
+                 not implemented method to quantify intersections.</doc>
       <group type="NXidentifier" optional="true"/>
       <field name="analysis_identifier" type="NX_UINT" recommended="true"/>
       <group name="reconstruction" type="NXserialized">
         <field name="type" type="NX_CHAR"/>
         <field name="path" type="NX_CHAR"/>
         <field name="checksum" type="NX_CHAR"/>
         <field name="algorithm" type="NX_CHAR"/>
@@ -700,17 +715,19 @@
         <field name="algorithm" type="NX_CHAR"/>
         <field name="distance" type="NX_CHAR">
           <doc>Absolute path in the (HDF5) file that points to the distance values.
                          The tool assumes that the values are stored in the same order as
                          points (ions).</doc>
         </field>
       </group>
-      <group name="feature" type="NXserialized">
+      <group name="feature" type="NXserialized" optional="true">
         <doc>A precomputed triangulated mesh of the feature representing a model of the
-                     interface at which to place ROIs to profile.</doc>
+                     interface at which to place ROIs to profile. This can be the mesh of an
+                     interface as returned e.g. by a previous interface_meshing task or the
+                     mesh of an iso-surface from a previous delocalization task.</doc>
         <field name="type" type="NX_CHAR"/>
         <field name="path" type="NX_CHAR"/>
         <field name="checksum" type="NX_CHAR"/>
         <field name="algorithm" type="NX_CHAR"/>
         <field name="vertices" type="NX_CHAR">
           <doc>Absolute HDF5 path to the dataset that specifies the array of vertex positions.</doc>
         </field>
@@ -732,15 +749,18 @@
         <group name="patch_filter" type="NXmatch_filter" optional="true">
           <doc>If interface_model is isosurface this filter can be used to restrict the analysis to specific
                          patches of an iso-surface.</doc>
           <field name="method" type="NX_CHAR"/>
           <field name="match" type="NX_NUMBER"/>
         </group>
       </group>
-      <group name="feature_distance" type="NXserialized" recommended="true">
+      <group name="feature_distance" type="NXserialized" optional="true">
+        <doc>To enable an additional filtration of specific parts of the feature
+                     mesh it is recommended to feed precomputed distances of each ion to
+                     the triangles of the feature mesh.</doc>
         <field name="type" type="NX_CHAR"/>
         <field name="path" type="NX_CHAR"/>
         <field name="checksum" type="NX_CHAR"/>
         <field name="algorithm" type="NX_CHAR"/>
         <field name="distance" type="NX_CHAR">
           <doc>Absolute path in the (HDF5) file that points to the distance values.
                          The tool assumes that the values are stored in the same order as
@@ -792,56 +812,66 @@
         <field name="match" type="NX_NUMBER"/>
       </group>
       <group name="hit_multiplicity_filter" type="NXmatch_filter" optional="true">
         <field name="method" type="NX_CHAR"/>
         <field name="match" type="NX_NUMBER"/>
       </group>
       <!--config-->
+      <group name="user_defined_roi" type="NXobject" optional="true">
+        <doc>As an alternative mode the tool can be instructed to place ROIs
+                     at specific locations into the dataset. This is the programmatic
+                     equivalent to the classical approach in atom probe to place ROIs
+                     for composition analyses via positioning and rotating them via
+                     a graphical user interface (such as in IVAS / AP Suite).</doc>
+        <group name="cylinder_set" type="NXcg_cylinder_set">
+          <!--dimensionality(NX_POSINT):
+cardinality(NX_POSINT):-->
+          <field name="identifier_offset" type="NX_INT"/>
+          <field name="center" type="NX_NUMBER">
+            <dimensions rank="2">
+              <dim index="1" value="n_rois"/>
+              <dim index="2" value="3"/>
+            </dimensions>
+          </field>
+          <field name="height" type="NX_NUMBER">
+            <dimensions rank="2">
+              <dim index="1" value="n_rois"/>
+              <dim index="2" value="3"/>
+            </dimensions>
+          </field>
+          <field name="radii" type="NX_NUMBER">
+            <dimensions rank="1">
+              <dim index="1" value="n_rois"/>
+            </dimensions>
+          </field>
+        </group>
+      </group>
+      <!--could add other shapes in the future if necessary
+but cylinders are most frequently used-->
       <field name="distancing_model" type="NX_CHAR">
         <doc>Which type of distance should be reported for the profile.</doc>
         <enumeration>
           <item value="project_to_triangle_plane"/>
         </enumeration>
       </field>
       <field name="roi_orientation" type="NX_CHAR">
-        <doc>In which directions should the tool probe for each ROI.</doc>
+        <doc>For each ROI, along which direction should the cylindrical ROI
+                     be oriented if ROIs are placed at triangles of the feature mesh.</doc>
         <enumeration>
           <item value="triangle_outer_unit_normal"/>
         </enumeration>
       </field>
-      <field name="roi_cylinder_center" type="NX_FLOAT" units="NX_LENGTH">
-        <doc>Explicit x, y, z coordinates (in the paraprobe coordinate system) where ROIs
-                     should be placed if feature is absent.</doc>
-        <dimensions rank="2">
-          <dim index="1" value="n_rois"/>
-          <dim index="2" value="3"/>
-        </dimensions>
-      </field>
-      <field name="roi_cylinder_orientation" type="NX_FLOAT" units="NX_LENGTH">
-        <doc>Explicit outer unit normal which explains into which direction each cylinder ROI
-                     is oriented.</doc>
-        <dimensions rank="2">
-          <dim index="1" value="n_rois"/>
-          <dim index="2" value="3"/>
-        </dimensions>
-      </field>
-      <!--
-not yet implemented the case to have ROIs of different size for each triangle of
-the feature mesh
--->
       <field name="roi_cylinder_height" type="NX_FLOAT" units="NX_LENGTH">
-        <doc>For each ROI, how high (projected on the cylinder axis) should the cylindrical ROI be.
-                     
-                     If roi_cylinder_center and roi_cylinder_orientation have been defined, roi_cylinder_height
-                     and roi_cylinder_radius can be defined as arrays of size (n_rois,) to instruct the tool to
-                     place a collection of ROIs with different size.
-                     Otherwise, roi_cylinder_height and roi_cylinder_radius have to be a scalars.</doc>
+        <doc>For each ROI, how high (projected onto the cylinder axis) should
+                     the cylindrical ROI be if ROIs are placed at triangles
+                     of the feature mesh.</doc>
       </field>
       <field name="roi_cylinder_radius" type="NX_FLOAT" units="NX_LENGTH">
-        <doc>For each ROI, how wide (radius) should the cylindrical ROI be.</doc>
+        <doc>For each ROI, how wide (in radius) should the cylindrical ROI
+                     be if ROIs are placed at triangles of the feature mesh.</doc>
       </field>
     </group>
     <group name="common" type="NXapm_paraprobe_tool_common">
       <field name="status" type="NX_CHAR"/>
       <group name="programID" type="NXprogram" minOccurs="1" maxOccurs="unbounded">
         <field name="program" type="NX_CHAR">
           <attribute name="version" type="NX_CHAR"/>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml`

 * *Files 5% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml`

```diff
@@ -52,14 +52,17 @@
     </symbol>
     <symbol name="n_v_feat">
       <doc>The total number of volumetric features.</doc>
     </symbol>
     <symbol name="n_speci">
       <doc>The total number of member distinguished when reporting composition.</doc>
     </symbol>
+    <symbol name="n_rois">
+      <doc>The total number of ROIs placed in an oned_profile task.</doc>
+    </symbol>
   </symbols>
   <doc>Application definition for results files of the paraprobe-nanochem tool.
          
          This tool is part of the paraprobe-toolbox. Inspect the base class :ref:`NXapm_paraprobe_tool_results`.</doc>
   <group type="NXentry" minOccurs="1" maxOccurs="1">
     <field name="definition" type="NX_CHAR">
       <attribute name="version" type="NX_CHAR"/>
@@ -134,15 +137,15 @@
             <dim index="1" value="d"/>
           </dimensions>
         </field>
         <!--coordinate_system implicit-->
         <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
           <doc>Integer which specifies the first index to be used for distinguishing identifiers for cells.
                          Identifiers are defined either implicitly or explicitly. For implicit indexing the identifiers are
-                         defined on the interval [identifier_offset, identifier_offset+c-1].
+                         defined on the interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.
                          For explicit indexing the identifier array has to be defined.</doc>
         </field>
         <field name="kernel_size" type="NX_POSINT" units="NX_DIMENSIONLESS">
           <doc>Halfwidth of the kernel about the central voxel.
                          The shape of the kernel is that of a cuboid
                          of extent 2*kernel_extent[i] + 1 in each dimension i.</doc>
           <dimensions rank="1">
@@ -174,30 +177,30 @@
           <field name="is_axis_aligned" type="NX_BOOLEAN">
             <doc>For atom probe should be set to true.</doc>
           </field>
           <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
             <doc>Integer which specifies the first index to be used for distinguishing
                              hexahedra. Identifiers are defined either implicitly or explicitly.
                              For implicit indexing the identifiers are defined on the interval
-                             [identifier_offset, identifier_offset+c-1].
+                             :math:`[identifier\_offset, identifier\_offset + c - 1]`.
                              For explicit indexing the identifier array has to be defined.</doc>
           </field>
           <group name="hexahedron" type="NXcg_face_list_data_structure">
             <field name="vertex_identifier_offset" type="NX_INT" units="NX_UNITLESS">
               <doc>Integer which specifies the first index to be used for distinguishing
                                  identifiers for vertices. Identifiers are defined either implicitly or explicitly.
                                  For implicit indexing the identifiers are defined on the interval 
-                                 [identifier_offset, identifier_offset+c-1]. For explicit indexing the identifier array
+                                 :math:`[identifier\_offset, identifier\_offset + c - 1]`. For explicit indexing the identifier array
                                  has to be defined.</doc>
             </field>
             <field name="face_identifier_offset" type="NX_INT" units="NX_UNITLESS">
               <doc>Integer which specifies the first index to be used for distinguishing
                                  identifiers for faces. Identifiers are defined either implicitly or explicitly.
                                  For implicit indexing the identifiers are defined on the interval
-                                 [identifier_offset, identifier_offset+c-1]. For explicit indexing the identifier array
+                                 :math:`[identifier\_offset, identifier\_offset + c - 1]`. For explicit indexing the identifier array
                                  has to be defined.</doc>
             </field>
             <field name="vertices" type="NX_NUMBER" units="NX_LENGTH">
               <doc>Positions of the vertices.
                                  Users are encouraged to reduce the vertices to unique set of positions
                                  and vertices as this supports a more efficient storage of the geometry data.
                                  It is also possible though to store the vertex positions naively in which
@@ -417,15 +420,15 @@
           <group name="triangle_soup" type="NXcg_triangle_set" optional="true">
             <doc>The resulting triangle soup computed via marching cubes.</doc>
             <field name="dimensionality" type="NX_POSINT" units="NX_UNITLESS"/>
             <field name="cardinality" type="NX_POSINT" units="NX_UNITLESS"/>
             <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
               <doc>Integer which specifies the first index to be used for distinguishing triangles.
                                  Identifiers are defined either implicitly or explicitly. For implicit indexing the
-                                 identifiers are defined on the interval [identifier_offset, identifier_offset+c-1].</doc>
+                                 identifiers are defined on the interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.</doc>
             </field>
             <group name="triangles" type="NXcg_face_list_data_structure">
               <field name="number_of_vertices" type="NX_POSINT"/>
               <field name="number_of_faces" type="NX_POSINT"/>
               <field name="vertex_identifier_offset" type="NX_INT"/>
               <field name="face_identifier_offset" type="NX_INT"/>
               <field name="vertices" type="NX_NUMBER" units="NX_LENGTH">
@@ -911,15 +914,15 @@
             <dim index="1" value="c"/>
             <dim index="2" value="4"/>
           </dimensions>
         </field>
       </group>
     </group>
     <group name="oned_profile" type="NXapm_paraprobe_tool_results" minOccurs="0" maxOccurs="1">
-      <group name="window" type="NXcs_filter_boolean_mask">
+      <group name="window" type="NXcs_filter_boolean_mask" optional="true">
         <field name="number_of_ions" type="NX_UINT"/>
         <field name="bitdepth" type="NX_UINT"/>
         <field name="mask" type="NX_UINT"/>
       </group>
       <!--results-->
       <group name="xdmf_cylinder" type="NXcg_polyhedron_set">
         <doc>The ROIs are defined as cylinders for the computations. To visualize these we discretize
@@ -932,58 +935,68 @@
           <doc>Position of the geometric center, which often is but not
                          necessarily has to be the center_of_mass of the polyhedra.</doc>
           <dimensions rank="2">
             <dim index="1" value="i"/>
             <dim index="2" value="3"/>
           </dimensions>
         </field>
-        <field name="roi_identifier" type="NX_UINT" units="NX_UNITLESS">
-          <doc>Integer which specifies the first index to be used for distinguishing
-                         ROI cylinder explicitly.</doc>
-          <dimensions rank="1">
+        <field name="orientation" type="NX_FLOAT" units="NX_LENGTH">
+          <doc>The orientation of the ROI defined via a vector which points along
+                         the cylinder axis and whose length is the height of the cylinder.</doc>
+          <dimensions rank="2">
             <dim index="1" value="i"/>
+            <dim index="2" value="3"/>
           </dimensions>
         </field>
-        <group name="polyhedra" type="NXcg_face_list_data_structure" minOccurs="0" maxOccurs="1">
-          <field name="edge_contact" type="NX_UINT" optional="true" units="NX_UNITLESS">
-            <dimensions rank="1">
-              <dim index="1" value="i"/>
-            </dimensions>
-          </field>
-          <field name="number_of_atoms" type="NX_UINT" optional="true" units="NX_UNITLESS">
-            <doc>The number of atoms in each ROI.</doc>
-            <dimensions rank="1">
-              <dim index="1" value="i"/>
-            </dimensions>
-          </field>
-          <field name="number_of_ions" type="NX_UINT" optional="true" units="NX_UNITLESS">
-            <doc>The number of ions in each ROI.</doc>
-            <dimensions rank="1">
-              <dim index="1" value="i"/>
-            </dimensions>
-          </field>
-          <field name="orientation" type="NX_FLOAT" optional="true" units="NX_LENGTH">
-            <doc>The orientation of the ROI defined via a vector which points along
-                             the cylinder axis and whose length is the height of the cylinder.</doc>
-            <dimensions rank="2">
-              <dim index="1" value="i"/>
-              <dim index="2" value="3"/>
-            </dimensions>
-          </field>
+        <!--XDMF support-->
+        <field name="identifier" type="NX_UINT" optional="true" units="NX_UNITLESS">
+          <doc>XDMF support to enable colouring each ROI by its identifier.</doc>
+          <dimensions rank="1">
+            <dim index="1" value="j"/>
+          </dimensions>
+        </field>
+        <field name="edge_contact" type="NX_UINT" optional="true" units="NX_UNITLESS">
+          <doc>XDMF support to enable colouring each ROI whether it has edge contact or not.</doc>
+          <dimensions rank="1">
+            <dim index="1" value="j"/>
+          </dimensions>
+        </field>
+        <field name="number_of_atoms" type="NX_UINT" optional="true" units="NX_UNITLESS">
+          <doc>XDMF support to enable colouring each ROI by its number of atoms.</doc>
+          <dimensions rank="1">
+            <dim index="1" value="j"/>
+          </dimensions>
+        </field>
+        <field name="number_of_ions" type="NX_UINT" optional="true" units="NX_UNITLESS">
+          <doc>XDMF support to enable colouring each ROI by its number of ions.</doc>
+          <dimensions rank="1">
+            <dim index="1" value="j"/>
+          </dimensions>
+        </field>
+        <group name="rois_far_from_edge" type="NXprocess">
+          <doc>Distance and iontype-specific processed data for each ROI.
+                         Arrays signed_distance and nuclide_hash are sorted by increasing
+                         distance.
+                         Array nuclide_hash reports one hash for each atom of each isotope.
+                         Effectively, this can yield to groups of values on signed_distance
+                         with the same distance value as molecular ions are reported decomposed
+                         into their atoms.
+                         Therefore, the XDMF support fields number_of_atoms and number_of_ions
+                         are only expected to display pairwise the same values respectively,
+                         if all ions are built from a single atom only.</doc>
           <group name="roiID" type="NXobject" minOccurs="0" maxOccurs="unbounded">
-            <doc>EXPLAIN HOW FIELDS SIGNED_DISTANCE AND NUCLIDE
-                             ARE COMPUTED/CONSTRUCTED.</doc>
             <field name="signed_distance" type="NX_FLOAT" units="NX_LENGTH">
-              <doc>In the direction of the ROI.</doc>
+              <doc>Sorted in increasing order projected along the positive direction
+                                 of the ROI as defined by orientation in the parent group.</doc>
               <dimensions rank="1">
                 <dim index="1" value="k"/>
               </dimensions>
             </field>
-            <field name="nuclide" type="NX_UINT" units="NX_UNITLESS">
-              <doc>Hashvalue using the following hashing rule :math:`H = Z + 256 * N`.</doc>
+            <field name="nuclide_hash" type="NX_UINT" units="NX_UNITLESS">
+              <doc>Hashvalue as defined in :ref:`NXion`.</doc>
               <dimensions rank="1">
                 <dim index="1" value="k"/>
               </dimensions>
             </field>
           </group>
         </group>
       </group>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml`

 * *Files 5% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml`

```diff
@@ -148,8 +148,19 @@
                  Should be a valid NeXus path name, e.g., /entry/data/energy.</doc>
     </attribute>
   </field>
   <group type="NXdata">
     <doc>Any data acquired/used during the calibration that does not fit the `NX_FLOAT` fields above.
              NXdata groups can be used for multidimensional data which are relevant to the calibration</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml`

```diff
@@ -75,15 +75,15 @@
   </field>
   <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer offset whereby the identifier of the first member
              of the set differs from zero.
              
              Identifiers can be defined either implicitly or explicitly.
              For implicit indexing identifiers are defined on the interval
-             :math:`[identifier_offset, identifier_offset + c - 1]`.
+             :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              
              Therefore, implicit identifier are completely defined by the value of
              identifier_offset and cardinality. For example if identifier run from
              -2 to 3 the value for identifier_offset is -2.
              
              For explicit indexing the field identifier has to be used.
              Fortran-/Matlab- and C-/Python-style indexing have specific implicit
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml`

 * *Files 5% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml`

```diff
@@ -71,14 +71,25 @@
              NXtransformations base class are used. In principle, the McStas coordinate
              system is used. The first transformation has to point either to another
              component of the system or . (for pointing to the reference frame) to relate it
              relative to the experimental setup. Typically, the components of a system should
              all be related relative to each other and only one component should relate to
              the reference coordinate system.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
   <group type="NXaperture">
     <doc>The size and position of an aperture inserted in the column, e.g. field aperture
              or contrast aperture</doc>
   </group>
   <group type="NXdeflector">
     <doc>Deflectors in the collection column section</doc>
   </group>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml`

```diff
@@ -147,17 +147,17 @@
   <field name="atom_identifier" type="NX_CHAR">
     <doc>Label for each atom position.</doc>
     <dimensions rank="1">
       <dim index="1" value="n_pos"/>
     </dimensions>
   </field>
   <field name="atom_type" type="NX_UINT" units="NX_UNITLESS">
-    <doc>The hash value :math:`H` is :math:`H = Z + N*256` with :math:`Z`
+    <doc>The hash value :math:`H` is :math:`H = Z + N \cdot 256` with :math:`Z`
              the number of protons and :math:`N` the number of neutrons
-             of each isotope respectively. Z and N have to be 8-bit unsigned integers.
+             of each isotope respectively. :math:`Z` and :math:`N` have to be 8-bit unsigned integers.
              For the rationale behind this `M. Kühbach et al. (2021) &lt;https://doi.org/10.1017/S1431927621012241&gt;`_</doc>
     <dimensions rank="1">
       <dim index="1" value="n_pos"/>
     </dimensions>
   </field>
   <!--atom_position(NXcg_point_set):-->
   <field name="atom_position" type="NX_NUMBER" units="NX_ANY">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml`

```diff
@@ -87,17 +87,17 @@
     <field name="method" type="NX_CHAR">
       <enumeration>
         <item value="whitelist"/>
       </enumeration>
     </field>
     <field name="match" type="NX_UINT" units="NX_UNITLESS">
       <doc>A list of nuclides based on which to evaluate the weight. Nuclides need to exist in the nuclide table.
-                 Values are nuclide (isotope) hash values using the following hashing rule :math:`$H = Z + 256 * N$`
-                 with :math:`$Z$` the number of protons and :math:`$N$` the number of neutrons of the nuclide.
-                 For elements set :math:`$N$` to zero.</doc>
+                 Values are nuclide (isotope) hash values using the following hashing rule :math:`H = Z + N \cdot 256`
+                 with :math:`Z` the number of protons and :math:`N` the number of neutrons of the nuclide.
+                 For elements set :math:`N` to zero.</doc>
       <dimensions rank="1">
         <dim index="1" value="n_nuclides"/>
       </dimensions>
     </field>
     <field name="mark" type="NX_NUMBER" units="NX_UNITLESS">
       <doc>Attribute data for each member of the point cloud. For APM these are the
                  iontypes generated via ranging. The number of mark data per point is 1
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml`

 * *Files 4% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml`

```diff
@@ -59,21 +59,16 @@
       </enumeration>
     </field>
     <field name="emitter_type" type="NX_CHAR">
       <doc>Emitter type used to create the beam.
                  
                  If the emitter type is other, give further details
                  in the description field.</doc>
-      <enumeration>
-        <item value="filament"/>
-        <item value="schottky"/>
-        <item value="cold_cathode_field_emitter"/>
-        <item value="other"/>
-      </enumeration>
     </field>
+    <!--enumeration: [filament, schottky, cold_cathode_field_emitter, other]-->
     <field name="emitter_material" type="NX_CHAR">
       <doc>Material of which the emitter is build, e.g. the filament material.</doc>
     </field>
     <!--MK could be made an instance of NXsample-->
     <field name="description" type="NX_CHAR">
       <doc>Ideally, a (globally) unique persistent identifier, link,
                  or text to a resource which gives further details.</doc>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml`

 * *Files 5% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml`

```diff
@@ -208,14 +208,25 @@
              from the NXtransformations base class are used. In principle, the McStas
              coordinate system is used. The first transformation has to point either to
              another component of the system or &quot;.&quot; (for pointing to the reference frame) to
              relate it relative to the experimental setup. Typically, the components of a
              system should all be related relative to each other and only one component
              should relate to the reference coordinate system.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
   <group type="NXcollectioncolumn">
     <doc>Describes the electron collection (spatial and momentum imaging) column</doc>
   </group>
   <group type="NXenergydispersion">
     <doc>Describes the energy dispersion section</doc>
   </group>
   <group type="NXspindispersion">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml`

 * *Files 14% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -17,70 +17,46 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<!--06/2022
-A draft version of a NeXus application definition for ellipsometry.-->
-<!--The document has the following main elements:
-- Instrument used and is characteristics
-- Sample: Properties of the sample
-- Data: measured data, data errors
-- Derived parameters: e.g. extra parameters derived in the measurement software-->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="application" name="NXellipsometry" extends="NXopt" type="group" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
-  <!--symbols:
-  doc: "Variables used throughout the document, e.g. dimensions and important parameters"
-  N_wavelength: "Size of the energy or wavelength vector used, the length of
-    NXinstrument/spectrometer/wavelength array"
-  N_variables: "How many variables are saved in a measurement. e.g. 2 for Psi
-    and Delta, 16 for Mueller matrix elements, 15 for normalized
-    Mueller matrix, 3 for NCS, the length of NXsample/column_names"
-  N_angles: "Number of incident angles used, the length of
-    NXinstrument/angle_of_incidence array"-->
-  <!--  N_p1:
-    "Number of sample parameters scanned, if you varied any of the parameters
-    such as temperature, pressure, or pH, the maximal length of the arrays
-    specified by NXsample/environment_conditions/SENSOR/value if it exists."
-  N_time: "Number of time points measured, the length of NXsample/time_points"-->
+<!--
+04/2024
+A rework of the draft version(06/2022) of a NeXus application definition for ellipsometry.-->
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="application" type="group" name="NXellipsometry" extends="NXopt" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
   <symbols>
     <doc>Variables used throughout the document, e.g. dimensions or parameters.</doc>
     <symbol name="N_spectrum">
       <doc>Length of the spectrum array (e.g. wavelength or energy) of the measured
                  data.</doc>
     </symbol>
-    <symbol name="N_sensors">
-      <doc>Number of sensors used to measure parameters that influence the sample,
-                 such as temperature or pressure.</doc>
-    </symbol>
     <symbol name="N_measurements">
       <doc>Number of measurements (1st dimension of measured_data array). This is
                  equal to the number of parameters scanned. For example, if the experiment
                  was performed at three different temperatures and two different pressures
                  N_measurements = 2*3 = 6.</doc>
     </symbol>
     <symbol name="N_detection_angles">
       <doc>Number of detection angles of the beam reflected or scattered off the
                  sample.</doc>
     </symbol>
     <symbol name="N_incident_angles">
       <doc>Number of angles of incidence of the incident beam.</doc>
     </symbol>
-    <symbol name="N_observables">
-      <doc>Number of observables that are saved in a measurement. e.g. one for
-                 intensity, reflectivity or transmittance, two for Psi and Delta etc. This
-                 is equal to the second dimension of the data array 'measured_data' and the
-                 number of column names.</doc>
-    </symbol>
-    <symbol name="N_time">
-      <doc>Number of time points measured, the length of NXsample/time_points</doc>
-    </symbol>
   </symbols>
-  <doc>Ellipsometry, complex systems, up to variable angle spectroscopy.
+  <doc>This is the application definition describing ellipsometry experiments.
+         
+         Such experiments may be as simple as identifying how a reflected
+         beam of light with a single wavelength changes its polarization state,
+         to a variable angle spectroscopic ellipsometry experiment.
+         
+         The application definition specifies optical spectroscopy (NXopt), by extending
+         the terms and setting specific requirements.
          
          Information on ellipsometry is provided, e.g. in:
          
          * H. Fujiwara, Spectroscopic ellipsometry: principles and applications,
            John Wiley &amp; Sons, 2007.
          * R. M. A. Azzam and N. M. Bashara, Ellipsometry and Polarized Light,
            North-Holland Publishing Company, 1977.
@@ -107,77 +83,54 @@
          * E. A. Irene, &quot;Applications of spectroscopic ellipsometry to microelectronics&quot;,
            Thin Solid Films 233, 96-111 (1993),
            https://doi.org/10.1016/0040-6090(93)90069-2
          * S. Zollner et al., &quot;Spectroscopic ellipsometry from 10 to 700 K&quot;,
            Adv. Opt. Techn., (2022),
            https://doi.org/10.1515/aot-2022-0016</doc>
   <group type="NXentry">
-    <doc>This is the application definition describing ellipsometry experiments.
-             
-             Such experiments may be as simple as identifying how a reflected
-             beam of light with a single wavelength changes its polarization state,
-             to a variable angle spectroscopic ellipsometry experiment.
-             
-             The application definition defines:
-             
-             * elements of the experimental instrument
-             * calibration information if available
-             * parameters used to tune the state of the sample
-             * sample description</doc>
     <field name="definition">
       <doc>An application definition for ellipsometry.</doc>
       <attribute name="version">
         <doc>Version number to identify which definition of this application
                      definition was used for this entry/data.</doc>
       </attribute>
       <attribute name="url">
         <doc>URL where to find further material (documentation, examples) relevant
                      to the application definition.</doc>
       </attribute>
       <enumeration>
         <item value="NXellipsometry"/>
       </enumeration>
     </field>
-    <field name="experiment_description">
-      <doc>An optional free-text description of the experiment.
+    <field name="title"/>
+    <field name="experiment_type">
+      <doc>Specify the type of the optical experiment.
                  
-                 However, details of the experiment should be defined in the specific
-                 fields of this application definition rather than in this experiment
-                 description.</doc>
+                 You may specify fundamental characteristics or properties in the experimental sub-type.</doc>
+      <enumeration>
+        <item value="ellipsometry"/>
+      </enumeration>
     </field>
-    <field name="experiment_type">
+    <field name="ellipsometry_experiment_type">
       <doc>Specify the type of ellipsometry.</doc>
       <enumeration>
         <item value="in situ spectroscopic ellipsometry"/>
         <item value="THz spectroscopic ellipsometry"/>
         <item value="infrared spectroscopic ellipsometry"/>
         <item value="ultraviolet spectroscopic ellipsometry"/>
         <item value="uv-vis spectroscopic ellipsometry"/>
         <item value="NIR-Vis-UV spectroscopic ellipsometry"/>
-        <item value="imaging ellipsometry"/>
+        <item value="other"/>
       </enumeration>
     </field>
+    <field name="ellipsometry_experiment_type_other" optional="true">
+      <doc>If the ellipsometry_experiment_type is `other`, a name should be specified here.</doc>
+    </field>
     <group type="NXinstrument">
       <doc>Properties of the ellipsometry equipment.</doc>
-      <field name="company" optional="true">
-        <doc>Name of the company which build the instrument.</doc>
-      </field>
-      <field name="construction_year" type="NX_DATE_TIME" optional="true">
-        <doc>ISO8601 date when the instrument was constructed.
-                     UTC offset should be specified.</doc>
-      </field>
-      <group name="software" type="NXprocess">
-        <field name="program">
-          <doc>Commercial or otherwise defined given name of the program that was
-                         used to generate the result file(s) with measured data and metadata.
-                         This program converts the measured signals to ellipsometry data. If
-                         home written, one can provide the actual steps in the NOTE subfield
-                         here.</doc>
-        </field>
-      </group>
       <field name="ellipsometer_type">
         <doc>What type of ellipsometry was used? See Fujiwara Table 4.2.</doc>
         <enumeration>
           <item value="rotating analyzer"/>
           <item value="rotating analyzer with analyzer compensator"/>
           <item value="rotating analyzer with polarizer compensator"/>
           <item value="rotating polarizer"/>
@@ -196,96 +149,170 @@
         <enumeration>
           <item value="polarizer (source side)"/>
           <item value="analyzer (detector side)"/>
           <item value="compensator (source side)"/>
           <item value="compensator (detector side)"/>
         </enumeration>
       </field>
-      <group type="NXbeam_path">
-        <group name="light_source" type="NXsource">
-          <doc>Specify the used light source. Multiple selection possible.</doc>
-          <field name="source_type">
-            <enumeration>
-              <item value="arc lamp"/>
-              <item value="halogen lamp"/>
-              <item value="LED"/>
-              <item value="other"/>
-            </enumeration>
-          </field>
-        </group>
-        <group name="focussing_probes" type="NXlens_opt" optional="true">
-          <doc>If focussing probes (lenses) were used, please state if the data
-                         were corrected for the window effects.</doc>
-          <field name="data_correction" type="NX_BOOLEAN">
-            <doc>Were the recorded data corrected by the window effects of the
-                             focussing probes (lenses)?</doc>
-          </field>
-          <field name="angular_spread" type="NX_NUMBER" recommended="true" units="NX_ANGLE">
-            <doc>Specify the angular spread caused by the focussing probes.</doc>
-          </field>
-        </group>
-        <group type="NXdetector">
-          <doc>Properties of the detector used. Integration time is the count time
-                         field, or the real time field. See their definition.</doc>
-        </group>
-        <group name="rotating_element" type="NXwaveplate" optional="true">
-          <doc>Properties of the rotating element defined in
-                         'instrument/rotating_element_type'.</doc>
-          <field name="revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
-            <doc>Define how many revolutions of the rotating element were averaged
-                             for each measurement. If the number of revolutions was fixed to a
-                             certain value use the field 'fixed_revolutions' instead.</doc>
-          </field>
-          <field name="fixed_revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
-            <doc>Define how many revolutions of the rotating element were taken
-                             into account for each measurement (if number of revolutions was
-                             fixed to a certain value, i.e. not averaged).</doc>
-          </field>
-          <field name="max_revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
-            <doc>Specify the maximum value of revolutions of the rotating element
-                             for each measurement.</doc>
-          </field>
-        </group>
-        <group name="spectrometer" type="NXmonochromator" optional="true">
-          <doc>The spectroscope element of the ellipsometer before the detector,
-                         but often integrated to form one closed unit. Information on the
-                         dispersive element can be specified in the subfield GRATING. Note
-                         that different gratings might be used for different wavelength
-                         ranges. The dispersion of the grating for each wavelength range can
-                         be stored in grating_dispersion.</doc>
-        </group>
+      <group name="focussing_probes" type="NXlens_opt" optional="true">
+        <doc>If focussing probes (lenses) were used, please state if the data
+                     were corrected for the window effects.</doc>
+        <!--This as well can be stated in window/aperture-->
+        <field name="data_correction" type="NX_BOOLEAN">
+          <doc>Were the recorded data corrected by the window effects of the
+                         focussing probes (lenses)?</doc>
+        </field>
+        <field name="angular_spread" type="NX_NUMBER" recommended="true" units="NX_ANGLE">
+          <doc>Specify the angular spread caused by the focussing probes.</doc>
+        </field>
+      </group>
+      <group name="rotating_element" type="NXwaveplate" optional="true">
+        <doc>Properties of the rotating element defined in
+                     'instrument/rotating_element_type'.</doc>
+        <field name="revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
+          <doc>Define how many revolutions of the rotating element were averaged
+                         for each measurement. If the number of revolutions was fixed to a
+                         certain value use the field 'fixed_revolutions' instead.</doc>
+        </field>
+        <field name="fixed_revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
+          <doc>Define how many revolutions of the rotating element were taken
+                         into account for each measurement (if number of revolutions was
+                         fixed to a certain value, i.e. not averaged).</doc>
+        </field>
+        <field name="max_revolutions" type="NX_NUMBER" optional="true" units="NX_COUNT">
+          <doc>Specify the maximum value of revolutions of the rotating element
+                         for each measurement.</doc>
+        </field>
       </group>
     </group>
     <group type="NXsample">
-      <field name="backside_roughness" type="NX_BOOLEAN">
+      <field name="backside_roughness" type="NX_BOOLEAN" optional="true">
         <doc>Was the backside of the sample roughened? Relevant for infrared
                      ellipsometry.</doc>
       </field>
     </group>
-    <group name="data_collection" type="NXprocess">
+    <!--The following NXdata setction called data_collection, is specialization
+from the old (NXopt and NXellipsometry) for the new NXellipometry.
+The generic description of the data collection will in future be
+included in the generic NXopt, but is now keept limited to
+NXellipsometry.-->
+    <group name="data_collection" type="NXdata">
+      <doc>Measured data, data errors, and varied parameters. This may be used to describe
+                 indirectly derived data or data transformed between different descriptions,
+                 such as:
+                 Raw Data --&gt; Psi
+                 Delta Psi, Delta --&gt; N,C,S
+                 Mueller matrix --&gt; N,C,S
+                 Mueller matrix --&gt; Psi, Delta
+                 etc.
+                 
+                 Other types of data, such as temperature or sample location, may be saved
+                 in a generic (NXdata) concept from NXopt, or better directly in the
+                 location of the sample positioner or temperature sensor.</doc>
+      <field name="data_identifier" type="NX_NUMBER">
+        <doc>An identifier to correlate data to the experimental conditions,
+                     if several were used in this measurement; typically an index of 0-N.</doc>
+      </field>
       <field name="data_type">
-        <doc>Select which type of data was recorded, for example Psi and Delta
-                     (see: https://en.wikipedia.org/wiki/Ellipsometry#Data_acquisition).
-                     It is possible to have multiple selections. Data types may also be
-                     converted to each other, e.g. a Mueller matrix contains N,C,S data
-                     as well. This selection defines how many columns (N_observables) are
-                     stored in the data array.</doc>
+        <doc>Select which type of data was recorded, for example intensity,
+                     reflectivity, transmittance, Psi and Delta etc.
+                     It is possible to have multiple selections. The enumeration list
+                     depends on the type of experiment and may differ for different
+                     application definitions.</doc>
         <enumeration>
+          <item value="intensity"/>
+          <item value="reflectivity"/>
+          <item value="transmittance"/>
           <item value="Psi/Delta"/>
           <item value="tan(Psi)/cos(Delta)"/>
           <item value="Mueller matrix"/>
           <item value="Jones matrix"/>
           <item value="N/C/S"/>
           <item value="raw data"/>
         </enumeration>
       </field>
+      <field name="NAME_spectrum" type="NX_FLOAT" optional="true" units="NX_ANY">
+        <doc>Spectral values (e.g. wavelength or energy) used for the measurement.
+                     An array of 1 or more elements. Length defines N_spectrum. Replace
+                     'SPECTRUM' by the physical quantity that is used, e.g. wavelength.</doc>
+        <dimensions rank="1">
+          <dim index="1" value="N_spectrum"/>
+        </dimensions>
+        <attribute name="units" optional="true">
+          <doc>If applicable, change 'unit: NX_ANY' to the appropriate NXDL unit.
+                         If the unit of the measured data is not covered by NXDL units state
+                         here which unit was used.</doc>
+        </attribute>
+      </field>
+      <field name="measured_data" type="NX_FLOAT" units="NX_ANY">
+        <doc>Resulting data from the measurement, described by 'data_type'.
+                     
+                     The first dimension is defined by the number of measurements taken,
+                     (N_measurements). The instructions on how to order the values
+                     contained in the parameter vectors given in the doc string of
+                     INSTRUMENT/sample_stage/environment_conditions/PARAMETER/values,
+                     define the N_measurements parameter sets. For example, if the
+                     experiment was performed at three different temperatures
+                     (T1, T2, T3), two different pressures (p1, p2) and two different
+                     angles of incidence (a1, a2), the first measurement was taken at the
+                     parameters {a1,p1,T1}, the second measurement at {a1,p1,T2} etc.</doc>
+        <dimensions rank="3">
+          <dim index="1" value="N_measurements"/>
+          <dim index="2" value="N_observables"/>
+          <dim index="3" value="N_spectrum"/>
+        </dimensions>
+        <attribute name="units" optional="true">
+          <doc>If applicable, change 'unit: NX_ANY' to the appropriate NXDL unit.
+                         If the unit of the measured data is not covered by NXDL units state
+                         here which unit was used.</doc>
+        </attribute>
+      </field>
+      <field name="measured_data_errors" type="NX_FLOAT" optional="true" units="NX_ANY">
+        <doc>Specified uncertainties (errors) of the data described by 'data_type'
+                     and provided in 'measured_data'.</doc>
+        <dimensions rank="3">
+          <dim index="1" value="N_measurements"/>
+          <dim index="2" value="N_observables"/>
+          <dim index="3" value="N_spectrum"/>
+        </dimensions>
+        <attribute name="units" optional="true">
+          <doc>If applicable, change 'unit: NX_ANY' to the appropriate NXDL unit.
+                         If the unit of the measured data is not covered by NXDL units state
+                         here which unit was used.</doc>
+        </attribute>
+      </field>
+      <field name="varied_parameter_link" optional="true">
+        <doc>List of links to the values of the sensors. Add a link for each
+                     varied parameter (i.e. for each sensor).</doc>
+        <dimensions rank="1">
+          <dim index="1" value="N_sensors"/>
+        </dimensions>
+      </field>
+      <field name="reference_data_link" optional="true">
+        <doc>Link to the NeXus file which describes the reference data if a
+                     reference measurement was performed. Ideally, the reference
+                     measurement was performed using the same conditions as the actual
+                     measurement and should be as close in time to the actual measurement
+                     as possible.</doc>
+      </field>
+      <group name="data_software" type="NXprogram" optional="true">
+        <field name="program">
+          <doc>Commercial or otherwise defined given name of the program that was
+                         used to generate the result file(s) with measured data and/or
+                         metadata (in most cases, this is the same as INSTRUMENT/software).
+                         If home written, one can provide the actual steps in the NOTE
+                         subfield here.</doc>
+        </field>
+        <field name="version">
+          <doc>Either version with build number, commit hash, or description of a
+                         (online) repository where the source code of the program and build
+                         instructions can be found so that the program can be configured in
+                         such a way that result files can be created ideally in a
+                         deterministic manner.</doc>
+        </field>
+        <attribute name="url" optional="true">
+          <doc>Website of the software.</doc>
+        </attribute>
+      </group>
     </group>
   </group>
-  <!--column_names:
-  doc: |
-    Please list in this array the column names used in your actual data.
-    That is ['Psi', 'Delta'] or ['MM1', 'MM2', 'MM3', ..., 'MM16] for
-    a full Mueller matrix, etc.
-  dimensions:
-    rank: 1
-    dim: [[1, N_observables]]-->
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml`

```diff
@@ -140,8 +140,19 @@
              Conventions from the NXtransformations base class are used. In principle,
              the McStas coordinate system is used. The first transformation has to point
              either to another  component of the system or . (for pointing to the reference frame)
              to relate it relative to the experimental setup. Typically, the components of a system
              should all be related relative to each other and only one component should relate to
              the reference coordinate system.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml`

```diff
@@ -94,15 +94,15 @@
   </field>
   <field name="pulse_identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer used to name the first pulse to know if there is an
              offset of the identifiers to zero.
              
              Identifiers can be defined either implicitly or explicitly.
              For implicit indexing identifiers are defined on the interval
-             :math:`[identifier_offset, identifier_offset + c - 1]`.
+             :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              
              Therefore, implicit identifier are completely defined by the value of
              identifier_offset and cardinality. For example if identifier run from
              -2 to 3 the value for identifier_offset is -2.
              
              For explicit indexing the field identifier has to be used.
              Fortran-/Matlab- and C-/Python-style indexing have specific implicit
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml`

 * *Files 19% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml`

```diff
@@ -17,24 +17,35 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXfabrication" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
-  <doc>Details about a component as it is defined by its manufacturer.</doc>
-  <field name="vendor" type="NX_CHAR">
-    <doc>Company name of the manufacturer.</doc>
-  </field>
-  <field name="model" type="NX_CHAR">
-    <doc>Version or model of the component named by the manufacturer.</doc>
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXidentifier" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+  <doc>An identifier for a (persistent) resource, e.g., a DOI or orcid.</doc>
+  <field name="service" type="NX_CHAR">
+    <doc>The service by which the resouce can be resolved.
+             If the service is not in the list a simple `url` may be used.
+             The `url` can either be a resolving service for the `identifier`
+             or a fully qualified identification in itself.</doc>
+    <enumeration>
+      <item value="doi"/>
+      <item value="urn"/>
+      <item value="hdl"/>
+      <item value="purl"/>
+      <item value="orcid"/>
+      <item value="iso"/>
+      <item value="url"/>
+    </enumeration>
   </field>
   <field name="identifier" type="NX_CHAR">
-    <doc>Ideally, (globally) unique persistent identifier, i.e.
-             a serial number or hash identifier of the component.</doc>
+    <doc>The unique code, IRI or hash to resolve this reference.
+             Typically, this is stated by the service which is considered a complete
+             identifier, e.g., for a DOI it's something of the form `10.1107/S1600576714027575`
+             or `https://doi.org/10.1107/S1600576714027575`, which are both resolvable.</doc>
   </field>
-  <field name="capability" type="NX_CHAR">
-    <doc>Free-text list with eventually multiple terms of
-             functionalities which the component offers.</doc>
+  <field name="is_persistent" type="NX_BOOLEAN">
+    <doc>True if the identifier is persistent (i.e., unique and available indefinetely),
+             False otherwise.</doc>
   </field>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml`

```diff
@@ -41,15 +41,15 @@
     <doc>Total number of edges, counting eventual bidirectional edges only once.</doc>
   </field>
   <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer which specifies the first index to be used for distinguishing
              edges. Identifiers are defined either implicitly or explicitly.
              
              For implicit indexing the identifiers are defined on the interval
-             :math:`[identifier_offset, identifier_offset + c - 1]`.
+             :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              
              For explicit indexing use the field identifier. For implicit indexing,
              consult :ref:`NXcg_primitive_set` to get guidance how to set identifier_offset.</doc>
   </field>
   <field name="identifier" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer used to distinguish edges for explicit indexing.</doc>
     <dimensions rank="1">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml`

```diff
@@ -60,15 +60,15 @@
     <doc>Number of nodes of the graph.</doc>
   </field>
   <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer which specifies the first index to be used for distinguishing
              nodes. Identifiers are defined either implicitly or explicitly.
              
              For implicit indexing the identifiers are defined on the interval
-             :math:`[identifier_offset, identifier_offset + c - 1]`.
+             :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              
              For explicit indexing use the field identifier. For implicit indexing,
              consult :ref:`NXcg_primitive_set` to get guidance how to set identifier_offset.</doc>
   </field>
   <field name="identifier" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer used to distinguish nodes for explicit indexing.</doc>
     <dimensions rank="1">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml`

 * *Files 4% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml`

```diff
@@ -40,14 +40,19 @@
     <doc>Any physical process that was performed on the physical entity prior or during the
              experiment.</doc>
   </group>
   <group type="NXchemical_process">
     <doc>Any chemical process that was performed on the physical entity prior or during the
              experiment.</doc>
   </group>
+  <group type="NXidentifier">
+    <doc>An ID or reference to the location or a unique (globally
+             persistent) identifier of e.g. another file which gives
+             as many as possible details of the history event.</doc>
+  </group>
   <!--There should be more activities here, like measurement.-->
   <group name="notes" type="NXnote">
     <doc>A descriptor to keep track of the treatment of the physical entity before or during the
              experiment (NXnote allows to add pictures, audio, movies). Alternatively, a
              reference to the location or a unique identifier or other metadata file. In the
              case these are not available, free-text description.
              This should only be used in case that there is no rigorous description
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml`

 * *Files 18% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml`

```diff
@@ -17,35 +17,23 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXidentifier" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
-  <doc>An identifier for a (persistent) resource, e.g., a DOI or orcid.</doc>
-  <field name="service" type="NX_CHAR">
-    <doc>The service by which the resouce can be resolved.
-             If the service is not in the list a simple `url` may be used.
-             The `url` can either be a resolving service for the `identifier`
-             or a fully qualified identification in itself.</doc>
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXpump" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+  <doc>Device to reduce an atmosphere (real or simulated) to a controlled pressure.</doc>
+  <group type="NXfabrication"/>
+  <field name="design" type="NX_CHAR">
+    <doc>Principle type of the pump.</doc>
     <enumeration>
-      <item value="doi"/>
-      <item value="urn"/>
-      <item value="hdl"/>
-      <item value="purl"/>
-      <item value="orcid"/>
-      <item value="iso"/>
-      <item value="url"/>
+      <item value="membrane"/>
+      <item value="rotary_vane"/>
+      <item value="roots"/>
+      <item value="turbo_molecular"/>
     </enumeration>
   </field>
-  <field name="identifier" type="NX_CHAR">
-    <doc>The unique code, IRI or hash to resolve this reference.
-             Typically, this is stated by the service which is considered a complete
-             identifier, e.g., for a DOI it's something of the form `10.1107/S1600576714027575`
-             or `https://doi.org/10.1107/S1600576714027575`, which are both resolvable.</doc>
-  </field>
-  <field name="is_persistent" type="NX_BOOLEAN">
-    <doc>True if the identifier is persistent (i.e., unique and available indefinetely),
-             False otherwise.</doc>
-  </field>
+  <!--NEW ISSUE: take community input and work further to store what is relevant to report about pumps
+NEW ISSUE: see e.g. https://www.youtube.com/watch?v=Nsr_AdTiIIA for a discussion about
+NEW ISSUE: the role, pros and cons of pump used for atom probe microscopy-->
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml`

```diff
@@ -46,15 +46,15 @@
     <doc>Ion type (ion species) identifier.
              
              The identifier zero is reserved for the special unknown ion type.</doc>
   </field>
   <field name="nuclide_hash" type="NX_UINT" units="NX_UNITLESS">
     <doc>Vector of nuclide hash values.
              
-             Individual hash values :math:`H` is :math:`H = Z + N*256` with :math:`Z`
+             Individual hash values :math:`H` is :math:`H = Z + N \cdot 256` with :math:`Z`
              encode the number of protons :math:`Z` and the number of neutrons :math:`N`
              of each nuclide respectively. :math:`Z` and :math:`N` have to be 8-bit unsigned integers.
              
              The array is sorted in decreasing order. For the rationale behind this see `M. Kühbach et al. (2021) &lt;https://doi.org/10.1017/S1431927621012241&gt;`_</doc>
     <dimensions rank="1">
       <dim index="1" value="n_ivec_max"/>
     </dimensions>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml`

```diff
@@ -70,26 +70,26 @@
   <field name="current" type="NX_NUMBER" units="NX_CURRENT">
     <doc>Excitation current of the lens.
              
              For dipoles it is a single number.
              For higher order multipoles, it is an array.</doc>
   </field>
   <field name="value" type="NX_NUMBER" units="NX_ANY">
-    <doc>This field should be used when the exact voltage or current of the lens
-             is not directly controllable as the control software of the microscope
-             does not enable or was not configured to display these values.
+    <doc>This field should be used when the exact voltage or current of the lens is not
+             directly controllable as the control software of the microscope  does not enable
+             or was not configured to display these values (for end users).
              
              In this case this value field should be used and the value
              from the control software stored as is.
              
              Although this value does not document the exact physical voltage or
              excitation, it can still give useful context to reproduce the lens setting,
-             which, provided a properly working instrument and software sets the lens
-             into a similar state to the technical level possible when no more information
-             is available physically or accessible legally.</doc>
+             provided a properly working instrument and software sets the lens
+             into a similar state to the technical level possible when no more 
+             information is available physically or accessible legally.</doc>
   </field>
   <field name="mode" type="NX_CHAR">
     <doc>This field should be used when the exact operation mode of the lens
              is not directly controllable as the control software of the microscope
              does not enable or was not configured to display these values.
              
              Like value the mode can only be interpreted for a specific microscope
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml`

 * *Files 3% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -17,15 +17,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" name="NXlockin" extends="NXobject" type="group" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXlockin" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
   <doc>Base classes definition for lock in devices.</doc>
   <group name="hardware" type="NXfabrication">
     <doc>Hardware manufacturers and type of lockin amplifier.</doc>
   </group>
   <group type="NXamplifier">
     <doc>By mixing the input signal (STS signal) with the modulated signal (such as Bias)
              and comparing it with the reference signal, they are enhanced and the effects of
@@ -49,16 +49,16 @@
     <doc>Sets the amplitude (in physical units of the modulated signal) of the sine
              modulation.</doc>
   </field>
   <field name="modulation_frequency" type="NX_NUMBER" units="NX_FREQUENCY">
     <doc>Sets the frequency of the sine modulation added to the signal to modulate.</doc>
   </field>
   <field name="demodulated_signal">
-    <doc>The input signal (STS signal) will be demodulated, in order to determine the amplitude 
-             and phase at the frequency set in the Frequency field or harmonics, such as current, 
+    <doc>The input signal (STS signal) will be demodulated, in order to determine the amplitude
+             and phase at the frequency set in the Frequency field or harmonics, such as current,
              bias, et.al.</doc>
   </field>
   <!--output (demodulated signal) characterisation (foreach channel, like demodulation, a separate sensor output, e.g. X,Y)-->
   <field name="number_of_demodulator_channels" type="NX_NUMBER">
     <doc>The number of signals which will be demodulated.</doc>
   </field>
   <field name="low_pass" type="NX_NUMBER" units="NX_FREQUENCY">
@@ -88,15 +88,15 @@
              signal, which would lead to a component at modulation frequency in the
              demodulated signals.</doc>
   </field>
   <field name="sync" type="NX_BOOLEAN">
     <doc>Switch on/off the Sync filter on the demodulated signals (X,Y) on or off.
              (foreach DemodulatorChannels)</doc>
   </field>
-  <field name="ref_phase_N" type="NX_NUMBER" units="NX_FREQUENCY">
+  <field name="ref_phase_N" type="NX_NUMBER" units="NX_ANGLE">
     <doc>Reference phase for the sine on the demodulated signal with respect to the
              modulation signal. (foreach DemodulatorChannels)</doc>
   </field>
   <field name="integration_time" type="NX_NUMBER" units="NX_TIME">
     <doc>Time during which the data are acquired and averaged. (for the input filter)</doc>
   </field>
   <field name="harmonic_order_N" type="NX_NUMBER">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml`

```diff
@@ -178,9 +178,20 @@
              the NXtransformations base class are used. In principle, the McStas coordinate
              system is used. The first transformation has to point either to another
              component of the system or . (for pointing to the reference frame) to relate it
              relative to the experimental setup. Typically, the components of a system should
              all be related relative to each other and only one component should relate to
              the reference coordinate system.</doc>
   </group>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
   <group type="NXfabrication"/>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml`

```diff
@@ -423,15 +423,15 @@
           <group type="NXpid" recommended="true">
             <field name="setpoint" type="NX_FLOAT" recommended="true"/>
           </group>
         </group>
         <group name="device_information" type="NXfabrication" recommended="true">
           <field name="vendor" recommended="true"/>
           <field name="model" recommended="true"/>
-          <field name="identifier"/>
+          <field name="identifier" recommended="true"/>
         </group>
       </group>
       <group name="pressure_gauge" type="NXsensor" recommended="true">
         <doc>Device to measure the gas pressure around the sample.</doc>
         <field name="name" recommended="true"/>
         <field name="measurement">
           <enumeration>
@@ -502,17 +502,17 @@
       </group>
       <group name="ellipticity_calibration" type="NXcalibration" optional="true">
         <field name="calibrated_axis" type="NX_FLOAT" recommended="true"/>
       </group>
       <group name="energy_referencing" type="NXcalibration" optional="true">
         <group name="level" type="NXelectron_level" recommended="true"/>
         <field name="reference_peak"/>
-        <field name="binding_energy" type="NX_FLOAT" recommended="true"/>
-        <field name="offset" type="NX_FLOAT" recommended="true"/>
-        <field name="calibrated_axis" type="NX_FLOAT" recommended="true"/>
+        <field name="binding_energy" type="NX_FLOAT" units="NX_ENERGY" recommended="true"/>
+        <field name="offset" type="NX_FLOAT" units="NX_ENERGY" recommended="true"/>
+        <field name="calibrated_axis" type="NX_FLOAT" units="NX_ENERGY" recommended="true"/>
       </group>
       <group name="transmission_correction" type="NXcalibration" optional="true">
         <group name="transmission_function" type="NXdata" recommended="true">
           <attribute name="signal"/>
           <attribute name="axes"/>
           <field name="kinetic_energy" type="NX_FLOAT" units="NX_ENERGY">
             <doc>Kinetic energy values</doc>
@@ -663,15 +663,20 @@
       </attribute>
       <field name="data" type="NX_NUMBER" units="NX_ANY">
         <doc>Represents a measure of one- or more-dimensional photoemission counts, where the
                      varied axis may be for example energy, momentum, spatial coordinate, pump-probe
                      delay, spin index, temperature, etc. The axes traces should be linked to the
                      actual encoder position in NXinstrument or calibrated axes in NXprocess.</doc>
       </field>
-      <field name="energy" type="NX_NUMBER" recommended="true">
+      <field name="energy" type="NX_NUMBER" units="NX_ENERGY" recommended="true">
+        <doc>Calibrated energy axis.
+                     
+                     This could be a link to either
+                     /entry/process/energy_calibration/calibrated_axis or
+                     /entry/process/energy_correction/calibrated_axis.</doc>
         <attribute name="type" recommended="true"/>
       </field>
       <attribute name="energy_depends" type="NX_CHAR" optional="true">
         <doc>The energy can be dispersed according to different strategies. ``energy_depends`` points to
                      the path of a field defining the calibrated axis on which the energy axis depends.
                      
                      For example:
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml`

```diff
@@ -270,15 +270,15 @@
       </group>
       <group name="snapshot_set" type="NXms_snapshot_set">
         <doc>Collection of microstructural data observed/simulated.</doc>
         <field name="identifier_offset" type="NX_UINT" units="NX_UNITLESS">
           <doc>Integer which specifies the first index to be used for distinguishing
                          snapshots. Identifiers are defined either implicitly or explicitly.
                          For implicit indexing the identifiers are defined on the
-                         interval [identifier_offset, identifier_offset+c-1].
+                         interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.
                          For explicit indexing the identifier array has to be defined.
                          
                          The identifier_offset field can for example be used to communicate
                          if the identifiers are expected to start from 1 (referred to as
                          Fortran-/Matlab-) or from 0 (referred to as C-, Python-style index
                          notation) respectively.</doc>
         </field>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml`

```diff
@@ -142,15 +142,15 @@
 the key problem is that at least for an implementation in HDF5 we are not allowed to have two groups named geometry even if their attributes are different because
 HDF5 implements no conceptual understanding of the relations between elements in the underlying graph which holds the data, these elements are either attributes, fields, groups, all of which
 end up as links-->
   <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer which specifies the first index to be used for distinguishing
              features. Identifiers are defined either implicitly
              or explicitly. For implicit indexing the identifiers are defined on the
-             interval [identifier_offset, identifier_offset+c-1].
+             interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              For explicit indexing the identifier array has to be defined.
              
              The identifier_offset field can for example be used to communicate if the
              identifiers are expected to start from 1 (referred to as Fortran-/Matlab-)
              or from 0 (referred to as C-, Python-style index notation) respectively.</doc>
   </field>
   <field name="identifier" type="NX_INT" units="NX_UNITLESS">
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml`

 * *Files 1% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml`

```diff
@@ -149,15 +149,15 @@
     </field>
     <field name="crystal_identifier_offset" type="NX_INT" units="NX_UNITLESS">
       <doc>Integer offset whereby the identifier of the first member
                  of the set differs from zero.
                  
                  Identifiers can be defined either implicitly or explicitly.
                  For implicit indexing identifiers are defined on the interval
-                 :math:`[identifier_offset, identifier_offset + c - 1]`.</doc>
+                 :math:`[identifier\_offset, identifier\_offset + c - 1]`.</doc>
     </field>
     <field name="crystal_identifier" type="NX_INT" units="NX_UNITLESS">
       <doc>Identifier used for crystals for explicit indexing.</doc>
       <dimensions rank="1">
         <dim index="1" value="n_c_two"/>
       </dimensions>
     </field>
@@ -264,15 +264,15 @@
     </field>
     <field name="interface_identifier_offset" type="NX_INT" units="NX_UNITLESS">
       <doc>Integer offset whereby the identifier of the first member
                  of the set differs from zero.
                  
                  Identifiers can be defined either implicitly or explicitly.
                  For implicit indexing identifiers are defined on the interval
-                 :math:`[identifier_offset, identifier_offset + c - 1]`.</doc>
+                 :math:`[identifier\_offset, identifier\_offset + c - 1]`.</doc>
     </field>
     <field name="interface_identifier" type="NX_INT" units="NX_UNITLESS">
       <doc>Identifier for each interface using explicit indexing.</doc>
       <dimensions rank="1">
         <dim index="1" value="n_i_two"/>
       </dimensions>
     </field>
@@ -307,15 +307,15 @@
     </field>
     <field name="triple_point_identifier_offset" type="NX_INT" units="NX_UNITLESS">
       <doc>Integer offset whereby the identifier of the first member
                  of the set differs from zero.
                  
                  Identifiers can be defined either implicitly or explicitly.
                  For implicit indexing identifiers are defined on the interval
-                 :math:`[identifier_offset, identifier_offset + c - 1]`.</doc>
+                 :math:`[identifier\_offset, identifier\_offset + c - 1]`.</doc>
     </field>
     <field name="triple_point_identifier" type="NX_INT" units="NX_UNITLESS">
       <doc>Identifier for each triple point using explicit indexing.</doc>
       <dimensions rank="1">
         <dim index="1" value="n_t_two"/>
       </dimensions>
     </field>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml`

```diff
@@ -287,15 +287,15 @@
       </group>
       <group name="snapshot_set" type="NXms_snapshot_set">
         <doc>Collection of microstructural data observed/simulated.</doc>
         <field name="identifier_offset" type="NX_UINT" units="NX_UNITLESS">
           <doc>Integer which specifies the first index to be used for distinguishing
                          snapshots. Identifiers are defined either implicitly or explicitly.
                          For implicit indexing the identifiers are defined on the
-                         interval [identifier_offset, identifier_offset+c-1].
+                         interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.
                          For explicit indexing the identifier array has to be defined.
                          
                          The identifier_offset field can for example be used to communicate
                          if the identifiers are expected to start from 1 (referred to as
                          Fortran-/Matlab-) or from 0 (referred to as C-, Python-style index
                          notation) respectively.</doc>
         </field>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml`

 * *Files 4% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -17,15 +17,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" name="NXms_snapshot_set" extends="NXobject" type="group" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXms_snapshot_set" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
   <symbols>
     <doc>The symbols used in the schema to specify e.g. dimensions of arrays.</doc>
   </symbols>
   <doc>A collection of spatiotemporal microstructure data.</doc>
   <field name="comment">
     <doc>Is this set describing a measurement or a simulation?</doc>
     <enumeration>
@@ -33,15 +33,15 @@
       <item value="simulation"/>
     </enumeration>
   </field>
   <field name="identifier_offset" type="NX_INT" units="NX_UNITLESS">
     <doc>Integer which specifies the first index to be used for distinguishing
              snapshots. Identifiers are defined either implicitly
              or explicitly. For implicit indexing the identifiers are defined on the
-             interval [identifier_offset, identifier_offset+c-1].
+             interval :math:`[identifier\_offset, identifier\_offset + c - 1]`.
              For explicit indexing the identifier array has to be defined.
              
              The identifier_offset field can for example be used to communicate if the
              identifiers are expected to start from 1 (referred to as Fortran-/Matlab-)
              or from 0 (referred to as C-, Python-style index notation) respectively.</doc>
   </field>
   <!--should we rather name snapshots explicitly always snapshot_1, snapshot_2
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml`

```diff
@@ -35,15 +35,15 @@
              not the physical size, of an object.</doc>
   </field>
   <field name="defocus" type="NX_NUMBER" units="NX_LENGTH">
     <doc>The defocus aberration constant (oftentimes referred to as C_1_0).
              See respective details in :ref:`NXaberration` class instances.</doc>
   </field>
   <field name="semi_convergence_angle" type="NX_NUMBER" units="NX_ANGLE">
-    <doc>Citing the JEOL TEM glosssary this is the value *when a cone shaped,
+    <doc>Citing the JEOL TEM glossary this is the value *when a cone shaped,
              convergent electron beam illuminates a specimen, the semi-angle of the cone
              is termed convergence angle.*</doc>
   </field>
   <field name="field_of_view" type="NX_NUMBER" units="NX_LENGTH">
     <doc>The extent of the observable parts of the specimen given the current
              magnification and other settings of the instrument.</doc>
   </field>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml`

 * *Files 8% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml`

```diff
@@ -71,8 +71,19 @@
   </field>
   <field name="K_t_const" type="NX_NUMBER" units="NX_TIME">
     <doc>The Type switches controller parameters between P/I (proportional gain/integral
              gain) and P/T (proportional gain/time constant). The formula for the controller
              in the frequency domain is G(s) = P + I/s = P(1 + 1/(Ts)). The integral gain and
              time constant are related as follows I = P/T.</doc>
   </field>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml`

```diff
@@ -162,23 +162,23 @@
       <doc>Electronic core or valence level that was used for the calibration.</doc>
     </group>
     <field name="reference_peak">
       <doc>Reference peak that was used for the calibration.
                  
                  For example: adventitious carbon | C-C | metallic Au | elemental Si | Fermi edge | vacuum level</doc>
     </field>
-    <field name="binding_energy" type="NX_FLOAT">
+    <field name="binding_energy" type="NX_FLOAT" units="NX_ENERGY">
       <doc>The binding energy (in units of eV) that the specified emission line appeared at,
                  after adjusting the binding energy scale.
                  
                  This concept is related to term `12.16`_ of the ISO 18115-1:2023 standard.
                  
                  .. _12.16: https://www.iso.org/obp/ui/en/#iso:std:iso:18115:-1:ed-3:v1:en:term:12.16</doc>
     </field>
-    <field name="offset" type="NX_FLOAT">
+    <field name="offset" type="NX_FLOAT" units="NX_ENERGY">
       <doc>Offset between measured binding energy and calibrated binding energy of the
                  emission line.</doc>
     </field>
     <field name="calibrated_axis" type="NX_FLOAT" units="NX_ENERGY">
       <doc>This is the calibrated energy axis to be used for data plotting.
                  
                  This should link to /entry/data/energy.</doc>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml`

 * *Files 24% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml`

```diff
@@ -17,23 +17,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXpump" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
-  <doc>Device to reduce an atmosphere (real or simulated) to a controlled pressure.</doc>
-  <group type="NXfabrication"/>
-  <field name="design" type="NX_CHAR">
-    <doc>Principle type of the pump.</doc>
-    <enumeration>
-      <item value="membrane"/>
-      <item value="rotary_vane"/>
-      <item value="roots"/>
-      <item value="turbo_molecular"/>
-    </enumeration>
+<!--
+symbols:-->
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="base" type="group" name="NXsubsampling_filter" extends="NXobject" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+  <doc>Base class of a filter to sample members in a set based on their identifier.</doc>
+  <field name="min_incr_max" type="NX_INT" units="NX_UNITLESS">
+    <doc>Triplet of the minimum, the increment, and the maximum identifier to
+             include of a sequence :math:`[i_0, i_0 + 1, i_0 + 2, \ldots, i_0 + \mathcal{N}] with i_0 \in \mathcal{Z}`
+             of identifier. The increment controls which n-th identifier (value) to take.
+             
+             Take as an example a dataset with 100 identifier (aka entries). Assume that
+             the identifier start at zero, i.e. identifier_offset is 0). Assume further
+             that min_incr_max is set to [0, 1, 99]. In this case the filter will
+             yield all identifier. Setting min_incr_max to [0, 2, 99] will take each
+             second identifier. Setting min_incr_max to [90, 3, 99] will take each
+             third identifier beginning from identifier 90 up to 99.</doc>
+    <dimensions rank="1">
+      <dim index="1" value="3"/>
+    </dimensions>
   </field>
-  <!--NEW ISSUE: take community input and work further to store what is relevant to report about pumps
-NEW ISSUE: see e.g. https://www.youtube.com/watch?v=Nsr_AdTiIIA for a discussion about
-NEW ISSUE: the role, pros and cons of pump used for atom probe microscopy-->
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml`

 * *Files 6% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml`

```diff
@@ -74,11 +74,22 @@
              definition, i.e., of the form /entry/instrument/my_part/my_field.</doc>
   </field>
   <field name="resolution_formula" type="NX_CHAR">
     <doc>A resolution formula to determine the resolution from a set of symbols as
              entered by the `formula_...` fields.
              The output unit should match the provided unit of this field.</doc>
   </field>
+  <attribute name="default">
+    <doc>.. index:: plotting
+             
+             Declares which child group contains a path leading
+             to a :ref:`NXdata` group.
+             
+             It is recommended (as of NIAC2014) to use this attribute
+             to help define the path to the default dataset to be plotted.
+             See https://www.nexusformat.org/2014_How_to_find_default_data.html
+             for a summary of the discussion.</doc>
+  </attribute>
   <group type="NXcalibration">
     <doc>For storing details and data of a calibration to derive a resolution from data.</doc>
   </group>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml`

 * *Files 4% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -17,30 +17,39 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 # For further information, see http://www.nexusformat.org
 -->
-<!--2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
-<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="application" name="NXsts" extends="NXsensor_scan" type="group" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
+<!--
+2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
+<!--
+2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
+<!--
+2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
+<!--
+2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
+<!--
+2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the-->
+<definition xmlns="http://definition.nexusformat.org/nxdl/3.1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" category="application" type="group" name="NXsts" extends="NXsensor_scan" xsi:schemaLocation="http://definition.nexusformat.org/nxdl/3.1 ../nxdl.xsd">
   <doc>Application definition for temperature-dependent IV curve measurements
-         #2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the 
+         #2023.19.7 This Nexus file is currently only for STS data, it will be updated to handle the
          STM image mode in the future with a focus on bias spectroscopy in Scanning Tunneling Microscopy.
          
          In this application definition, times should be specified always together with a UTC offset.
          
          This is the application definition describing temperature (T) dependent current voltage (IV) curve
          measurements. For this, a temperature is set. After reaching the temperature, a voltage sweep
          is performed. For each voltage, a current is measured.
          Then, the next desired temperature is set and an IV measurement is performed.
-         The data can be visualized in a tensor with:  
+         The data can be visualized in a tensor with:
          I (NXsensor_C, NXsoftware_Read_offset, NXcircuit)
-         parameters: 
-         V has (NXsource+offset, NXsoftware_Scan_offset, NXsensor_V, NXcircuit)  
+         parameters:
+         V has (NXsource+offset, NXsoftware_Scan_offset, NXsensor_V, NXcircuit)
          T has (NXsource, NXsoftware_Scan_offset, NXsensor_T)
          x has (NXsoftware_Scan_offset)
          y has (NXsoftware_Scan_offset)
          z has (NXsoftware_Scan_offset)</doc>
   <group type="NXentry">
     <field name="definition">
       <enumeration>
@@ -51,15 +60,15 @@
       <doc>Name of the experiment where the application is applicable.</doc>
       <enumeration>
         <item value="sts"/>
         <item value="stm"/>
       </enumeration>
     </field>
     <field name="type">
-      <doc>The equipments and techniques as well as the parameter settings and reference signals 
+      <doc>The equipments and techniques as well as the parameter settings and reference signals
                  are used during the experiments used in Scanning Tunneling Microscopy (STM).</doc>
       <!--NOTE_: What does the enum refer, scan could be forward or backward. (not in data file)
 What is about [constant current mode, constant height mode]-->
       <enumeration>
         <item value="background"/>
         <item value="reference"/>
         <item value="sample"/>
@@ -70,117 +79,115 @@
                  221122_Au_5K00014)</doc>
     </field>
     <field name="collection_identifier">
       <doc>The name of the series output file, which represents only the public part of the
                  output file. (e.g. 221122_Au_5K)</doc>
     </field>
     <field name="experiment_identifier" optional="true">
-      <doc>Path to storage of output files. 
+      <doc>Path to storage of output files.
                  (e.g. Path C:\Users\SPM-PEEM\Desktop\DATA_Nanonis\20220711_CreaTec_Service_Benchmarks_LHe\Nanonis-Session-PMD100-HVHU_CreaTec_Service_PalmaLabBerlin220711)</doc>
     </field>
     <field name="experiment_description" optional="true">
-      <doc>Descriptive comments for this experiment, added by the experimenter, coming from the 
-                 output file. (e.g. Comment01 SYNC &amp; Filter LP 8order WITHDRAW 600 steps, locked Au(111), 
+      <doc>Descriptive comments for this experiment, added by the experimenter, coming from the
+                 output file. (e.g. Comment01 SYNC &amp; Filter LP 8order WITHDRAW 600 steps, locked Au(111),
                  50pA, 100 mV set point, 1mV DCA, 973Hz,138 1st H, -84 2nd H)</doc>
     </field>
     <group type="NXinstrument">
       <group name="hardware" type="NXfabrication" optional="true">
         <doc>Hardware type used in SPM experiment, includes hardware manufacturers and type.
                      (e.g. Nanonis BP5e)</doc>
       </group>
       <!--hardware: Current amplifier> hardware: CreaTec GmbH
 any or specifique 'harware' and 'software'?-->
       <group name="software" type="NXfabrication" optional="true">
         <doc>Type of software used in SPM experiments, such as software version serial number, UI and
                      RT probe release method. (e.g. SW Version Generic 5e -- RT Release 10771)</doc>
-        <field name="version" optional="false">
-          <doc>Version of the software.</doc>
-        </field>
       </group>
       <!--amplification: Current amplifier> factor (V/V): 1E-10
 crosstalk_compensation: Current amplifier> Capacitive cross-talk compensation: Yes/No-->
       <group name="current_amplifier" type="NXamplifier" optional="true">
-        <doc>The Amplifier description that improves or helps to determine tunnel current (current 
+        <doc>The Amplifier description that improves or helps to determine tunnel current (current
                      between tip and bias).</doc>
       </group>
       <group name="lock_in" type="NXlockin" optional="true">
         <field name="status" optional="true">
           <!--status: Lock-in>Lock-in status ON # ON/OFF of Lock-in amplifier-->
           <doc>Status of Lock-in device whether while performing the experiment</doc>
         </field>
+        <field name="run" optional="true">
+          <doc>Select whether to set the Lock-In to run during the measurement. When using this
+                         feature, make sure the Lock-In is configured correctly and settling times are
+                         set to twice the Lock-In period at least. This option is ignored when Lock-In is
+                         already running. This option is disabled if the Sweep Mode is MLS and the flag
+                         to configure the Lock-In per segment in the Multiline segment editor is set.</doc>
+        </field>
         <!--amplifier_status: -> amplifier/active_channels
 Lock-in Amplifier>Yes/No
- doc:  Lock-in Amplifier>Yes/No # If a lock-in amplifier employed to filter or obtain
-       the electronic derivatives dI/dV of the signal
+doc:  Lock-in Amplifier>Yes/No # If a lock-in amplifier employed to filter or obtain
+the electronic derivatives dI/dV of the signal
 hardware:     Lock-in Amplifier>Hardware: Nanonis-->
         <field name="modulation_signal" optional="true" units="NX_VOLTAGE">
           <doc>This is the signal on which the modulation (sine) will be added.</doc>
         </field>
         <!--modulate_signal: Lock-in>Modulated signal Bias (V)-->
         <field name="modulation_frequency" type="NX_NUMBER" units="NX_FREQUENCY">
           <!--Lock-in>Frequency (Hz) 973E+0-->
-          <doc>The signal is modulated by adding the frequency of the sine modulation. The 
-                         modulation frequency spans can be from 10 mHz to 40 kHz, corresponding to the output filter 
-                         cut-off range. When dealing with harmonics, it's essential to ensure that the 
-                         harmonic frequencies remain below ~100 kHz, which aligns with the input filter cut-off. 
-                         Be mindful that hardware filters might impact the amplitude as the signal approaches 
+          <doc>The signal is modulated by adding the frequency of the sine modulation. The
+                         modulation frequency spans can be from 10 mHz to 40 kHz, corresponding to the output filter
+                         cut-off range. When dealing with harmonics, it's essential to ensure that the
+                         harmonic frequencies remain below ~100 kHz, which aligns with the input filter cut-off.
+                         Be mindful that hardware filters might impact the amplitude as the signal approaches
                          their cut-off frequencies.&quot; (e.g. 973E+0)</doc>
         </field>
         <field name="modulation_amplitude" type="NX_NUMBER">
           <!--amplitude: Lock-in>Amplitude 2E-3-->
           <doc>The amplitude (in physical units of modulated signal) of the sine modulation.</doc>
         </field>
         <field name="demodulated_signal" optional="true">
           <!--Lock-in>Demodulated signal Current (A) # This is the signal which
 will be demodulated, in order to determine the amplitude and phase at the frequency
 set in the Frequency field (“4”) or harmonics.-->
-          <doc>The input signal (STS signal) will be demodulated, in order to determine the amplitude 
-                         and phase at the frequency set in the Frequency field or harmonics, such as current, 
+          <doc>The input signal (STS signal) will be demodulated, in order to determine the amplitude
+                         and phase at the frequency set in the Frequency field or harmonics, such as current,
                          bias, et.al.</doc>
         </field>
         <field name="harmonic_order_N" type="NX_NUMBER">
-          <!--  Lock-in>Harmonic D1 1
-  Lock-in>Harmonic D2 2 # See below.-->
+          <!--Lock-in>Harmonic D1 1
+Lock-in>Harmonic D2 2 # See below.-->
           <doc>N denotes 1 or 2. The order of the harmonic oscillation to be detected in the demodulated
-                         signal should be considered relative to the modulation frequency. When dealing with 
+                         signal should be considered relative to the modulation frequency. When dealing with
                          higher harmonics, it's essential to ensure that their frequencies do not surpass
                          the analogue signal bandwidth (e.g. harmonic_order_1).</doc>
         </field>
         <field name="ref_phase_N" type="NX_NUMBER" optional="true">
-          <!--  Lock-in>Reference phase D1 (deg) 137.597E+0
-  Lock-in>Reference phase D2 (deg) -83.6562E+0 # See below.-->
+          <!--Lock-in>Reference phase D1 (deg) 137.597E+0
+Lock-in>Reference phase D2 (deg) -83.6562E+0 # See below.-->
           <doc>Reference phase for the sine on the demodulated signal with respect to the
                          modulation signal. The determined phase is displayed with respect to the
                          reference phase.</doc>
         </field>
         <field name="lock_in_data_flip_number" type="NX_NUMBER"/>
       </group>
       <!--items below should go to bias/spectroscopy/...!!!
 recorded_channels:
- doc: Select the channels to record. (e.g. Current (A);LI Demod 2 X (A);LI Demod 2 Y (A);
-    LI Demod 1 X (A);LI Demod 1 Y (A) # Select the channels to record.)
+doc: Select the channels to record. (e.g. Current (A);LI Demod 2 X (A);LI Demod 2 Y (A);
+LI Demod 1 X (A);LI Demod 1 Y (A) # Select the channels to record.)
 bias_reset:
- doc: When selected, the Bias voltage returns to the initial value (before starting the
-    sweep) at the end of the spectroscopy measurement (default). When not selected, Bias
-    remains at the last value of the sweep. This is useful e.g. when combining several
-    sweep segments. Example for an automated measurement (using Programming Interface):
-    switch off Z-Controller, start spectroscopy sweep segments (only fwd sweep, no reset
-    bias), set bias back to initial value, switch on Z-Controller.  (e.g. TRUE)
+doc: When selected, the Bias voltage returns to the initial value (before starting the
+sweep) at the end of the spectroscopy measurement (default). When not selected, Bias
+remains at the last value of the sweep. This is useful e.g. when combining several
+sweep segments. Example for an automated measurement (using Programming Interface):
+switch off Z-Controller, start spectroscopy sweep segments (only fwd sweep, no reset
+bias), set bias back to initial value, switch on Z-Controller.  (e.g. TRUE)
 record_final_z:
- doc: Select whether to record the Z position during Z averaging time at the end of the
-    sweep (after Z control time) and store the average value in the header of the file
-    when saving. Using this option increases the sweep time by Z averaging time. (e.g. FALSE)
-run:
- doc: Bias Spectroscopy>Lock-In run FALSE # Select whether to set the Lock-In to run
-    during the measurement. When using this feature, make sure the Lock-In is configured
-    correctly and settling times are set to twice the Lock-In period at least. This
-    option is ignored when Lock-In is already running. This option is disabled if the
-    Sweep Mode is MLS and the flag to configure the Lock-In per segment in the Multiline
-    segment editor is set.-->
+doc: Select whether to record the Z position during Z averaging time at the end of the
+sweep (after Z control time) and store the average value in the header of the file
+when saving. Using this option increases the sweep time by Z averaging time. (e.g. FALSE)-->
       <group name="sample_bias" type="NXiv_bias">
+        <doc>Bias voltage applied to the sample.</doc>
         <field name="bias" type="NX_NUMBER" units="NX_VOLTAGE">
           <doc>Applied a voltage between tip and sample.</doc>
         </field>
         <field name="bias_calibration" type="NX_NUMBER"/>
         <field name="bias_offset" type="NX_NUMBER" units="NX_VOLTAGE"/>
       </group>
       <!--sample_bias(NXbias):
@@ -191,91 +198,90 @@
 unit: NX_VOLTAGE
 doc: Same directional representation as bias. (e.g. 1E-3)-->
       <field name="stm_head_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
         <doc>Temperature of STM head. Note: At least one field from stm_head_temperature,
                      cryo_bottom_temp and cryo_sheild_temp must be provided.</doc>
       </field>
       <field name="cryo_bottom_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
-        <doc>Temperature of liquid helium cryostat. Note: At least one field from 
+        <doc>Temperature of liquid helium cryostat. Note: At least one field from
                      stm_head_temperature, cryo_bottom_temp and cryo_sheild_temp must be provided.</doc>
       </field>
       <field name="cryo_shield_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
-        <doc>Temperature of liquid nitrogen shield. Temperature 3 (K) (e.g 78.00000E+0). Note: At 
+        <doc>Temperature of liquid nitrogen shield. Temperature 3 (K) (e.g 78.00000E+0). Note: At
                      least one field from stm_head_temperature, cryo_bottom_temp and cryo_sheild_temp
                      must be provided.</doc>
       </field>
       <group name="output_cabling" type="NXcircuit" optional="true"/>
       <!--Cabling & Config
 output_mode:
 doc: Number of output channels. (e.g. User Output)
 output_value(NX_NUMBER):
 doc: The user output in each monitor mode. (e.g. 0E+0)
 output_name:
 doc: User outputs whose name can be modified in the corresponding module. (e.g. Input 24 (V))
 output_slew_rate(NX_NUMBER):
 doc: The rate at which the one of the signal changes when ramping to the starting point. (V/s) (e.g. Inf)-->
       <group name="piezo_config" type="NXcollection" optional="true">
-        <doc>Configuration for piezoelectric scanner used to move tip along X and Y direction. The 
-                     material of the Piezoelectric scanner composed of polycrystalline solids and sensitive to 
+        <doc>Configuration for piezoelectric scanner used to move tip along X and Y direction. The
+                     material of the Piezoelectric scanner composed of polycrystalline solids and sensitive to
                      applied voltage.</doc>
         <field name="active_calib">
           <doc>The name of calibration type. (e.g. LHe)</doc>
         </field>
         <field name="calib_N" type="NX_NUMBER" optional="true">
-          <doc>N denotes X or Y or Z. There are three parameters in the X, Y, and Z directions, 
-                         along with three available controls: Calibration (m/V), Range (m), and HV gain. Only 
-                         two of these parameters are required to define the calibration. Consequently, when any 
+          <doc>N denotes X or Y or Z. There are three parameters in the X, Y, and Z directions,
+                         along with three available controls: Calibration (m/V), Range (m), and HV gain. Only
+                         two of these parameters are required to define the calibration. Consequently, when any
                          value is changed, one of the other values will be automatically updated. (e.g. calib_X = 3.8E-9)</doc>
         </field>
         <field name="hv_gain_N" type="NX_NUMBER" optional="true">
           <doc>N denotes X or Y or Z. In some systems, there is an HV gain readout feature. For
                          these systems, the HV gain should be automatically adjusted whenever the gain is
                          changed at the high voltage amplifier. (e.g. 14.5)</doc>
         </field>
         <!--(e.g. 0.318343)-->
         <field name="tilt_N" type="NX_NUMBER" optional="true" units="NX_ANGLE">
-          <doc>N denotes X or Y. There are 2 parameters in X and Y directions, and tilt needs to be 
+          <doc>N denotes X or Y. There are 2 parameters in X and Y directions, and tilt needs to be
                          adjusted according to the actual surface. (in degrees, first order correction).</doc>
         </field>
         <!--Inf-->
         <field name="curvature_radius_N" type="NX_NUMBER" optional="true" units="NX_LENGTH">
           <doc>N denotes X or Y. There are 2 parameters in X and Y directions. (can be set
                          approximately to the length of the piezotube).</doc>
         </field>
         <field name="2nd_order_corr_N" type="NX_NUMBER" optional="true">
-          <doc>N denotes X or Y. There are 2 parameters in X and Y directions. If you know them, 
-                         you can enter the 2nd order piezo characteristics to compensate for it. The 
-                         following equation shows the interpretation of the 2nd order correction parameter: 
-                         For the X-piezo: &quot;Ux = 1/cx · X + cxx · X2&quot; with units: 
+          <doc>N denotes X or Y. There are 2 parameters in X and Y directions. If you know them,
+                         you can enter the 2nd order piezo characteristics to compensate for it. The
+                         following equation shows the interpretation of the 2nd order correction parameter:
+                         For the X-piezo: &quot;Ux = 1/cx · X + cxx · X2&quot; with units:
                          [V] = [V/m] · [m] + [V/m2] · [m2] where cx is the calibration of the piezo X and cxx
                          is the 2nd order correction. (V/m^2). (e.g. 0E+0)</doc>
         </field>
         <field name="drift_N" type="NX_NUMBER" optional="true">
-          <doc>N denotes X, Y or Z. There are 3 parameters in X, Y and Z directions. Define the 
+          <doc>N denotes X, Y or Z. There are 3 parameters in X, Y and Z directions. Define the
                          drift speed for all three axes. When the compensation is on, the piezos will start to
                          move at that speed. (e.g. 0E+0)</doc>
         </field>
         <field name="drift_correction_status" type="NX_BOOLEAN">
           <doc>Use the button to enable or disable the drift compensation. (e.g. FALSE)</doc>
         </field>
       </group>
-      <group type="NXenvironment" optional="false">
-        <doc>Describes an environment setup for a temperature-dependent IV measurement experiment.
-                     The temperature and voltage must be present as independently scanned controllers and
-                     the current sensor must also be present with its readings.</doc>
+      <group type="NXenvironment">
+        <doc>An environmental setup to measure the tunneling current due to different tip-
+                     sample biases.</doc>
         <group name="current_sensor" type="NXsensor" optional="true">
           <field name="current" type="NX_NUMBER" units="NX_CURRENT">
-            <doc>This is set-point of tip current (in the constant current mode should be equal to set-point, 
+            <doc>This is set-point of tip current (in the constant current mode should be equal to set-point,
                              in the constant height mode means the real tunnelling current between tip and sample).</doc>
           </field>
-          <field name="current_calibration" type="NX_NUMBER" units="NX_CURRENT">
+          <field name="current_calibration" type="NX_NUMBER" units="NX_ANY">
             <doc>Value of calibration that comes as A/V.</doc>
           </field>
           <field name="current_offset" type="NX_NUMBER" units="NX_CURRENT"/>
-          <field name="current_gain" units="NX_UNITLESS"/>
+          <field name="current_gain" type="NX_NUMBER" units="NX_UNITLESS" optional="true"/>
           <field name="calibration_time" type="NX_DATE_TIME" optional="true"/>
           <field name="value" type="NX_NUMBER" optional="true"/>
         </group>
         <group name="position" type="NXpositioner_sts">
           <doc>Clarify the frame laboratory frame.</doc>
           <field name="x" type="NX_NUMBER" optional="true" units="NX_LENGTH">
             <doc>The scanning area in x position in the frame. (e.g. -890.53E-12)</doc>
@@ -284,15 +290,15 @@
             <doc>The scanning area in y position in the frame. (e.g. 29.6968E-9)</doc>
           </field>
           <field name="z" type="NX_NUMBER" optional="true" units="NX_LENGTH">
             <doc>The scanning area in z position in the frame. (e.g. 130.5E-9)</doc>
           </field>
           <group name="z_controller" type="NXcollection">
             <field name="z" type="NX_NUMBER" units="NX_LENGTH">
-              <doc>Indicate the relative tip position z between tip and sample. The tip position can also 
+              <doc>Indicate the relative tip position z between tip and sample. The tip position can also
                                  be varied when the z_controller is not running. (e.g. 130.5E-9)</doc>
             </field>
           </group>
         </group>
         <!--TODO: Is if this are uncomment than getting error.
 voltage_controller(NXsensor):
 temperature_controller(NXsensor):
@@ -312,29 +318,29 @@
               <doc>The end bias values of the sweep. (e.g. 300E-3)</doc>
             </field>
             <field name="num_pixel" type="NX_NUMBER">
               <doc>The sweep number of points is defined as the maximum spectrum resolution, which
                                  is equal to the bias sweep window divided by the number of pixels. (e.g. 4096)</doc>
             </field>
             <field name="z_avg_time" type="NX_NUMBER" units="NX_TIME">
-              <doc>The Z position is recorded and averaged for a certain duration both before and 
-                                 after the sweep. After the initial Z averaging time, if &quot;Z-Controller to Hold&quot; 
+              <doc>The Z position is recorded and averaged for a certain duration both before and
+                                 after the sweep. After the initial Z averaging time, if &quot;Z-Controller to Hold&quot;
                                  is selected, the Z-Controller is set to hold mode, and the tip is positioned at
                                  the previously averaged Z position (adjusted by the Z offset). (e.g. 100E-3)</doc>
             </field>
           </group>
           <group name="circuit" type="NXcollection" optional="true">
             <field name="rt_frequency" type="NX_NUMBER" units="NX_FREQUENCY">
-              <doc>The bandwidth of the Hardware and/or Software is instrument specific. 
+              <doc>The bandwidth of the Hardware and/or Software is instrument specific.
                                  For example, Nanonis Generic 5 has 'RT Frequency' (e.g. 20E+3).</doc>
             </field>
             <field name="signals_oversampling" type="NX_NUMBER">
-              <doc>The Signals Period represents the rate at which signals are transferred to 
-                                 the host computer, which operates the control software. This rate may 
-                                 be 10 times lower than the sampling rate, as the real-time engine internally 
+              <doc>The Signals Period represents the rate at which signals are transferred to
+                                 the host computer, which operates the control software. This rate may
+                                 be 10 times lower than the sampling rate, as the real-time engine internally
                                  oversamples the signal. If desired, you may have the option to reduce the oversampling
                                  to 1, enabling higher frequency resolution in the Spectrum Analyzer. (e.g. 10)</doc>
             </field>
             <field name="acquisition_period" type="NX_NUMBER" units="NX_TIME" optional="true">
               <doc>The update rate is utilized in various processes, including the History Graph,
                                  Auto-Approach, and multiple Programming Interface functions. It may be
                                  configured to a 20 ms interval. Any additional timings must strictly be integer
@@ -366,21 +372,21 @@
                                  within this module, as the sweep modules automatically set this value according
                                  to the sweep timings. (e.g. 500E-3)</doc>
             </field>
           </group>
         </group>
         <!--parameters how to change the location from measurement to measurement during the scan-->
         <group name="scan_control" type="NXcollection" optional="true">
-          <group name="roi" type="NXtransformations">
+          <group name="roi" type="NXtransformations" optional="true">
             <field name="frame">
-              <doc>Also clarify the frame for the ROI of the scan in lab frame, the middle of the lab 
+              <doc>Also clarify the frame for the ROI of the scan in lab frame, the middle of the lab
                                  frame is (0, 0), and positive in x means right and in y means up.</doc>
             </field>
           </group>
-          <group name="circuit" type="NXcollection">
+          <group name="circuit" type="NXcollection" optional="true">
             <field name="channels_current">
               <doc>The scan channels are selected by users. (e.g. (A);Bias (V);Z (m);LI Demod 2 X
                                  (A);LI Demod 2 Y (A);LI Demod 1 X (A);LI Demod 1 Y (A))</doc>
             </field>
           </group>
           <group name="positioner" type="NXcollection">
             <field name="scanfield" type="NX_NUMBER">
@@ -406,263 +412,295 @@
     <!--RESOLUTION (calculation input)
 TODO: After fix resolution_indicators back to required
 As all of the bellow are linked
 should be NXcollection not NXprocess-->
     <group name="resolution_indicators" type="NXprocess" optional="true">
       <!--Temperature 1>link to INSTR/STM/head Temperature 1 (K) (e.g. 4.92997E+0) # Temperature of STM head.-->
       <field name="stm_head_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
-        <doc>Link to target:/NXentry/NXinstrument/stm_head_temp</doc>
+        <doc>Link to target: /NXentry/NXinstrument/stm_head_temp</doc>
       </field>
       <!--Temperature 2>link to Temperature 2 (K) - # Temperature of bottom of LHe helium cryostat.-->
       <field name="cryo_bottom_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
-        <doc>Link to target:/NXentry/NXinstrument/cryo_bottom_temp</doc>
+        <doc>Link to target: /NXentry/NXinstrument/cryo_bottom_temp</doc>
       </field>
       <!--Temperature 3>link to Temperature 3 (K) - # Temperature of LN2 nitrogen shield.-->
       <field name="cryo_shield_temp" type="NX_NUMBER" optional="true" units="NX_TEMPERATURE">
-        <doc>Link to target:/NXentry/NXinstrument/temp_cryo_shield</doc>
+        <doc>Link to target: /NXentry/NXinstrument/temp_cryo_shield</doc>
       </field>
       <!--Lock-in>link to Modulated signal Bias (V) (e.g. 1E-3) # Applied modulation to the bias voltage.-->
       <field name="modulation_signal" optional="true" units="NX_VOLTAGE">
-        <doc>Link to target:/NXentry/NXinstrument/NXlock_in/modulation_signal</doc>
+        <doc>Link to target: /NXentry/NXinstrument/NXlock_in/modulation_signal</doc>
       </field>
       <!--link to Integration time (s) (e.g. 150E-6)
 Time during which the spectroscopy data are acquired and averaged.-->
       <field name="integration_time" type="NX_NUMBER" units="NX_TIME">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/NXintegration_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/NXintegration_time</doc>
       </field>
       <!--link to Bias Spectroscopy>Number of sweeps (e.g. 100) Number of sweeps to measure and average.-->
       <field name="number_of_sweeps" type="NX_NUMBER" units="NX_UNITLESS" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/number_of_sweeps</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/number_of_sweeps</doc>
       </field>
       <!--link to Bias Spectroscopy>Sweep Start (V) (e.g. -300E-3) # The first bias values of the sweep.-->
       <field name="sweep_start" type="NX_NUMBER" units="NX_VOLTAGE">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/sweep_start</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/sweep_start</doc>
       </field>
       <!--link to Bias Spectroscopy>Sweep End (V) (e.g. 300E-3) # The last bias values of the sweep.-->
       <field name="sweep_end" type="NX_NUMBER" units="NX_VOLTAGE">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/sweep_end</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/sweep_end</doc>
       </field>
       <!--link to Bias Spectroscopy>Num Pixel (e.g. 4096) # Define the sweep number of points, that is, the maximum spectrum resolution eq. Bias window divide by Num Pixel.-->
       <field name="num_pixel" type="NX_NUMBER">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/num_pixel</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/num_pixel</doc>
       </field>
       <!--link to Bias Spectroscopy>Z Avg time (s) (e.g. 100E-3) # Duration over which the Z
 position is recorded and averaged before and after the sweep (the latter only if Record
 final Z position is selected in the Advanced section). After the initial Z averaging
 time, if Z-Controller to Hold is selected in the Advanced section, the Z-Controller is
 set to hold and the tip is placed at the previously averaged Z position (plus Z offset).-->
       <field name="z_avg_time" type="NX_NUMBER" units="NX_TIME">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_avg_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_avg_time</doc>
       </field>
       <!--link to SoftwareMain>RT Frequency (Hz) (e.g. 20E+3) # The bandwitdh of the
 Hardware and/or Software-->
       <field name="rt_frequency" type="NX_NUMBER" units="NX_FREQUENCY">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/rt_frequency</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/rt_frequency</doc>
       </field>
       <!--link to SoftwareMain>Signals Oversampling (e.g. 10) # (Signals Periods)
 The Signals Period is the rate at which the signals are transferred to the host computer
 running the control software. This is usually lower by a factor of 10 than the sampling
 rate, because an internal oversampling of the signal is done on the real time engine.
 You can reduce the oversampling down to 1 in order to resolve higher frequencies in the
 Spectrum Analyzer.-->
       <field name="signals_oversampling" type="NX_NUMBER">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/signals_oversampling</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/signals_oversampling</doc>
       </field>
       <!--link to SoftwareMain>Acquisition Period (s) (e.g. 20E-3) # Update rate for several
 processes like History Graph, Auto-Approach, and for many Programming Interface functions.
 This is usually set to 20 ms. All additional timings (7-9) can only be integer multiples
 of this value. They can be set to different values, but the actual timing value will be
 coerced to a multiple of the Acquisition Period.-->
       <field name="acquisition_period" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/acquisition_period</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/acquisition_period</doc>
       </field>
       <!--link to SoftwareMain>Animations Period (s) (e.g. 20E-3) # Update rate of animated
 graphical indicators. These are e.g. some graphs & sliders. A reasonable value is
 40 ms (25 updates per second). Increase this period to reduce the processor load
 for the graphical user interface, especially on slow computers. This value is purely a
 user interface update rate and does not affect measurements in any way.-->
       <field name="animations_period" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/animations_period</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/animations_period</doc>
       </field>
       <!--link to SoftwareMain>Indicators Period (s) (e.g. 300E-3) # Update rate of digital
 indicators, e.g. the numbers displayed besides each slider. Here, 3 updates per
 second, or 300 ms is enough. This value is purely a user interface update rate and
 does not affect measurements in any way.-->
       <field name="indicators_period" type="NX_NUMBER" units="NX_TIME">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/indicators_period</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/indicators_period</doc>
       </field>
       <!--link to SoftwareMain>Measurements Period (s) (e.g. 500E-3) # The Measurements
 period is the integration time for precise measurements (averaging over specified period),
 mostly used in sweep modules. Examples are recording of a force-distance curve or a
 resonance of a cantilever. For fast measurements with small steps, a value of 40 ms may be
 reasonable. For normal use, 300-500 ms is a good value, but for recording a resonance of a
 high-Q cantilever, values of several seconds might be necessary. Usually this parameter doesn’t need to be set from this module; the sweep modules will set this value according to the sweep timings.-->
       <field name="measurements_period" type="NX_NUMBER" optional="true" units="NX_TIME">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/measurements_period</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXcircuit/measurements_period</doc>
       </field>
     </group>
     <!--TODO: Later fix REPRODUCIBILITY_indicator
 as all of the bellow are linked-->
     <group name="reproducibility_indicators" type="NXprocess" optional="true">
       <!--Bias>Bias(NXBias) (V) (e.g. 100E-3) # Applied bias voltage.-->
       <field name="bias" type="NX_NUMBER" units="NX_VOLTAGE">
-        <doc>Link to target:/NXentry/NXinstrument/NXsample_bias/bias</doc>
+        <doc>Link to target: /NXentry/NXinstrument/NXsample_bias/bias</doc>
       </field>
       <!--Current>Current(NXcircuit) (A) (e.g. -5.3429E-15) # The tunneling current is displayed here.-->
       <field name="current" type="NX_NUMBER" units="NX_CURRENT">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current</doc>
+        <doc>Link to target: /NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current</doc>
       </field>
       <!--Bias>Calibration(NXbias) (V/V) (e.g. 1E+0) Calibration of the Bias output. If you have
 a Range switch the calibration is stored per range setting.-->
       <field name="bias_calibration" type="NX_NUMBER" units="NX_UNITLESS">
-        <doc>Link to target:/NXentry/NXnstrument/NXsample_bias/bias_calibration</doc>
+        <doc>Link to target: /NXentry/NXnstrument/NXsample_bias/bias_calibration</doc>
       </field>
       <field name="bias_offset" type="NX_NUMBER" units="NX_VOLTAGE">
-        <doc>Link to target:/NXentry/NXinstrument/NXsample_bias/bias_offset</doc>
+        <doc>Link to target: /NXentry/NXinstrument/NXsample_bias/bias_offset</doc>
       </field>
       <!--Current>Calibration(NXcircuit) (A/V) (e.g. 100E-12)
 The signals voltages are converted to real world physical values according to the calibration & offset parameters:
 Physical signal = (Voltage * calibration) + offset.-->
       <field name="current_calibration" type="NX_NUMBER" units="NX_CURRENT">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_calibration</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_calibration</doc>
       </field>
       <!--Current>Offset(NXcircuit) (A) (e.g. 16.2897E-15) # The same as "Current>Calibration (A/V)" tag-->
       <field name="current_offset" type="NX_NUMBER" units="NX_CURRENT">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_offset</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_offset</doc>
       </field>
       <!--Current>Gain(NXcircuit) (e.g. Not switchable) # None-->
       <field name="current_gain" type="NX_NUMBER" units="NX_UNITLESS">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_gain</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXcurrent_sensor/current_gain</doc>
       </field>
       <!--Z offset(NXpositioner_sts) (m) (e.g. 0E+0) # Offset added to the initial averaged position
 Zaver before starting to sweep. This parameter is disabled when Z-Controller to Hold is
 deselected in the Advanced section. The LED “Alt” next to the Z offset indicates if an
 alternate Z-controller setpoint is enabled.-->
       <!--Settling time(NXbias) (s) (e.g. 2.1E-3) Time to wait after changing the bias to the next
 level and before starting to acquire data. Adjust this parameter to avoid transient
 effect induced by the bias change. Integration time: time during which the data are
 acquired and averaged.-->
       <field name="z_offset" type="NX_NUMBER" units="NX_LENGTH">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_offset</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_offset</doc>
       </field>
       <field name="settling_time" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/settling_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/settling_time</doc>
       </field>
       <!--Z-Ctrl hold(NXpositioner_sts) (e.g. TRUE) # When selected, the Z-Controller is set to hold
 during the pulse. This means that the controller doesn't control the Z position during the pulse.-->
       <field name="z_control_hold" type="NX_BOOLEAN" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_ccontroller_hold</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_ccontroller_hold</doc>
       </field>
       <!--Final Z(NXpositioner_sts) (m) (e.g. N/A)-->
       <field name="final_z" type="NX_NUMBER" units="NX_LENGTH" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/record_final_z</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/record_final_z</doc>
       </field>
       <!--Start time(NXlog) (e.g.23.11.2022 18:55:16) # Timestamp of the moment
 when the acquisition starts by pressing the Start button.
 TODO: no available concept is found for the  below link
 start_time(link):
-  exists: optional
+exists: optional
 Link to t target: none
 Bias Spectroscopy>1st Settling time(NXbias) (s) (e.g.2.1E-3) # See the "Settling time (s)" below.-->
       <field name="first_settling_time" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/first_settling_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/first_settling_time</doc>
       </field>
       <!--Bias Spectroscopy>Integration time(NXbias) (s) (e.g.150E-6) # Time during which the data
 are acquired and averaged.
 integration_time(link):
 Link to ttarget: /ENTRY[entry]/INSTRUMENT[instrument]/ENVIRONMENT[environment]/sweep_control/bias_spectroscopy/integration_time
 Bias Spectroscopy>End Settling time(NXbias) (s) (e.g.4E-3) # Time to wait after the sweep has finished and the bias is ramped to the initial value.-->
       <field name="end_settling_time" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/end_settling_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/end_settling_time</doc>
       </field>
       <!--Bias Spectroscopy>Z control time(NXbias) (s) (e.g.200E-3) # Time during which the
 Z-Controller is enabled once a sweep has finished. When averaging multiple sweeps
 (i.e. Sweeps>1), the Z-Controller is enabled for this duration between each sweep.
 After the last sweep, it will wait the specified time before continuing a running scan.
 This ensures each sweep reliably starts from the same position. This parameter is
 disabled when Z-Controller to Hold is deselected in the Advanced section.-->
       <field name="z_control_time" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_control_time</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/z_control_time</doc>
       </field>
       <!--Bias Spectroscopy>Max Slew rate(NXbias) (V/s) (e.g.1E+0) # Maximum rate at which
 the bias changes (before, during and after sweeping).-->
       <field name="max_slew_rate" type="NX_NUMBER" units="NX_ANY" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/max_slew_rate</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/max_slew_rate</doc>
       </field>
       <!--Bias Spectroscopy>backward sweep(NXbias) (e.g.TRUE) # Select whether to measure
 the backward (return) sweep or the forward only.-->
       <field name="backward_sweep" type="NX_NUMBER" units="NX_ANY" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/backward_sweep</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXsweep_control/NXbias_spectroscopy/backward_sweep</doc>
       </field>
       <!--Z-Controller>Controller name(NXpositioner_sts) (e.g.log Current) # Controller name.
 This name which will be displayed at places where you can select a controller.-->
       <field name="z_controller_name" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/controller_name</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/controller_name</doc>
       </field>
       <!--Z-Controller>Controller status(NXpositioner_sts) (e.g.OFF) # ON/OFF-->
       <field name="z_controller_status" type="NX_BOOLEAN" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/controller_status</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/controller_status</doc>
       </field>
       <!--Z-Controller>Setpoint(NXpositioner_sts) (e.g.50E-12) # Set Point is the desired value
 of the control signal. It can be set by editing the number or using the slider bar.
 Click the "Set" button above the input field to use the actual value as Set Point. The slider shows the Set Point as well as the current value.
 Z-Controller>Setpoint unit(NXpositioner_sts) (e.g.A) # Angstrom-->
       <field name="z_controller_setpoint" type="NX_NUMBER" units="NX_CURRENT" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/set_point</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/set_point</doc>
       </field>
       <!--Z-Controller>P gain(NXpid) (e.g.6E-12) # The Type switches controller parameters
 between P/I (proportional gain/integral gain) and P/T (proportional gain/time constant).
 The formula for the controller in the frequency domain is: G(s) = P + I/s = P(1 + 1/(Ts)).
 The integral gain and time constant are related as follows: I = P/T.-->
       <field name="y_control_p_gain" type="NX_NUMBER" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/p_gain</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/p_gain</doc>
       </field>
       <!--Z-Controller>I gain(NXpid) (e.g.39.8241E-9) # See "Z-Controller>P gain" below.-->
       <field name="z_control_i_gain" type="NX_NUMBER" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/i_gain</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/i_gain</doc>
       </field>
       <!--Z-Controller>Time const(NXpid) (s) (e.g.150.662E-6) # See "Z-Controller>P gain" below.-->
-      <field name="z_control_time_const" units="NX_TIME" type="NX_NUMBER" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/time_const</doc>
+      <field name="z_control_time_const" type="NX_NUMBER" units="NX_TIME" optional="true">
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/time_const</doc>
       </field>
       <!--Z-Controller>TipLift(NXpositioner_sts) (m) (e.g.0E+0) # Lifts the tip by the specified
 amount when then controller is switched off. This can be a positive or a negative number,
 i.e. the tip can also be moved towards the sample. Be careful with sign and value when
 using this feature.-->
       <field name="z_control_tip_lift" type="NX_NUMBER" units="NX_LENGTH" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/tip_lift</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/tip_lift</doc>
       </field>
       <!--Z-Controller>Switch off delay(NXpositioner_sts) (s) (e.g.0E+0) # Use this parameter for
 a reproducible position when switching off the Z-controller. When >0 and the Z-controller
 is switched off, it doesn't switch off immediately but continues to run for the specified time and averages the Z position.-->
       <field name="z_control_switchoff_delay" type="NX_NUMBER" units="NX_TIME" optional="true">
-        <doc>Link to target:/NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/switchoff_delay</doc>
+        <doc>Link to target:
+                     /NXentry/NXinstrument/NXenvironment/NXposition/NXz_controller/switchoff_delay</doc>
       </field>
     </group>
     <group name="sample" type="NXsample" optional="true">
-      <doc>To describe sample and other constaints that applied on sample before scanning.</doc>
-      <field name="sample_prep_descripton">
-        <doc>At this moment no base class available that can track entire sample preparation.</doc>
+      <doc>To describe the sample and other constraints that are applied to that sample
+                 before scanning.</doc>
+      <field name="sample_prep_descripton" optional="true">
+        <doc>At this moment no base class is available that can track entire sample
+                     preparation.</doc>
       </field>
     </group>
     <!--TODO: discuss convertion data to DATA-->
     <group type="NXdata">
       <doc>This NXdata should contain separate fields for the current values at different temperature setpoints, for example current_at_100C.
                  There should also be two more fields called temperature and voltage containing the setpoint values.
                  There should also be a field with an array of rank equal to the number of different temperature setpoints and each child's dimension
                  equal to the number of voltage setpoints.
                  axes: bias_calc
                  signals:
                  li_demod_[1;2]_[X/Y]_[-;bwd;filt;bwd_filt]
                  current_[-;bwd;filt;bwd_filt]
-                 temperature
-                 x
-                 y
-                 z</doc>
-      <!--DATA # multi dimensional array: multi I-V array per scan point;
+                 temperature</doc>
+    </group>
+    <!--DATA # multi dimensional array: multi I-V array per scan point;
 doc: The format of the data here is similar to a column matrix.
 Bias calc (V) #scanning parameter
 Current (A) # current during forward direction scanning of bias - original NXsensor
 LI Demod 2 X (A) lockin (NXsensor+lockin)
 LI Demod 2 Y (A) lockin
 LI Demod 1 X (A) lockin
 LI Demod 1 Y (A) lockin
@@ -682,17 +720,25 @@
 LI Demod 1 X (A) [bwd] [filt] lockin
 LI Demod 1 Y (A) [bwd] [filt] lockin
 Temperature
 x
 y
 z
 single point default plot # current(I) vs bias(V)-->
-      <group name="single_point" type="NXdata" optional="true"/>
-      <!--line scan default plot # multi I vs. V curves-->
-      <group name="line_scan" type="NXdata" optional="true"/>
-      <!--alternative plot # current(I) curve in the 2D space of (position(x), bias(V))-->
-      <group name="alternative_plot" type="NXdata" optional="true"/>
-      <!--mesh scan default plot # 2D slices of the above alternative plot-->
-      <group name="mesh_scan" type="NXdata" optional="true"/>
+    <group name="single_point" type="NXdata" optional="true">
+      <doc>Plot for a single point (x,y) with I vs. V curve.</doc>
+    </group>
+    <!--line scan default plot # multi I vs. V curves-->
+    <group name="line_scan" type="NXdata" optional="true">
+      <doc>Line scan with multiple I vs. V curves for different single (x,y) co-ordinates.</doc>
+    </group>
+    <!--alternative plot # current(I) curve in the 2D space of (position(x), bias(V))-->
+    <group name="alternative_plot" type="NXdata" optional="true">
+      <doc>Plot for current(I) curve in the 2D space of (position(x), bias(V)) which can be
+                 derived from the `line_scan` plot.</doc>
+    </group>
+    <!--mesh scan default plot # 2D slices of the above alternative plot-->
+    <group name="mesh_scan" type="NXdata" optional="true">
+      <doc>Mesh scan with 2D slices of the above alternative plot for other y co-ordinates.</doc>
     </group>
   </group>
 </definition>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml`

 * *Files 2% similar despite different names*

#### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-stylesheet type="text/xsl" href="nxdlformat.xsl"?>
 <!--
 # NeXus - Neutron and X-ray Common Data Format
-# 
-# Copyright (C) 2014-2022 NeXus International Advisory Committee (NIAC)
-# 
+#
+# Copyright (C) 2014-2024 NeXus International Advisory Committee (NIAC)
+#
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -47,29 +47,29 @@
       <item value="tetragonal"/>
       <item value="rhombohedral"/>
       <item value="hexagonal"/>
       <item value="cubic"/>
     </enumeration>
   </field>
   <field name="space_group">
-    <doc>Crystallographic space group. 
+    <doc>Crystallographic space group.
              A space group is the symmetry group of a repeating pattern in space.
              For further information, see International Table for Crystallography (https://it.iucr.org/).</doc>
   </field>
   <field name="point_group">
     <doc>Crystallographic point group.
-             A crystallographic point group is a set of symmetry operations, corresponding to one of the point groups in three dimensions, 
+             A crystallographic point group is a set of symmetry operations, corresponding to one of the point groups in three dimensions,
              such that each operation (perhaps followed by a translation) would leave the structure of a crystal unchanged.
              This field should use Schoenflies notation (see Schoenflies, A., Krystallsysteme und Krystallstructur, 1891).
              For further information, see https://dictionary.iucr.org/Point_group.</doc>
   </field>
   <field name="laue_group">
     <doc>Laue group (also called Laue class).
              The Laue classes are eleven geometric crystal classes containing centrosymmetric crystallographic types of point groups and their subgroups.
-             When absorption is negligible and Friedel's law applies, it is impossible to distinguish by diffraction between a centrosymmetric point group 
+             When absorption is negligible and Friedel's law applies, it is impossible to distinguish by diffraction between a centrosymmetric point group
              and one of its non-centrosymmetric subgroups; only point groups belonging to different Laue classes can then be distinguished.
              For further information, see https://dictionary.iucr.org/Laue_class.</doc>
   </field>
   <!--defined using which convention?-->
   <field name="a_b_c" type="NX_FLOAT" units="NX_LENGTH">
     <doc>Crystallography unit cell parameters a, b, and c</doc>
     <dimensions rank="1">
@@ -136,17 +136,17 @@
   <field name="atom_identifier">
     <doc>Labels for each atom position</doc>
     <dimensions rank="1">
       <dim index="1" value="n_pos"/>
     </dimensions>
   </field>
   <field name="atom" type="NX_UINT" units="NX_UNITLESS">
-    <doc>The hash value :math:`H` is :math:`H = Z + N*256` with :math:`Z`
+    <doc>The hash value :math:`H` is :math:`H = Z + N \cdot 256` with :math:`Z`
              the number of protons and :math:`N` the number of neutrons
-             of each isotope respectively. Z and N have to be 8-bit unsigned integers.
+             of each isotope respectively. :math:`Z` and :math:`N` have to be 8-bit unsigned integers.
              For the rationale behind this `M. Kühbach et al. (2021) &lt;https://doi.org/10.1017/S1431927621012241&gt;`_</doc>
     <dimensions rank="1">
       <dim index="1" value="n_pos"/>
     </dimensions>
   </field>
   <field name="atom_positions" type="NX_FLOAT" units="NX_LENGTH">
     <doc>Atom positions x, y, z.</doc>
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml` & `pynxtools-0.3.0/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/__main__.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/dir_app.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/dir_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/manual_app.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/manual_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/apps/nxclass_app.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/apps/nxclass_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/anchor_list.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/anchor_list.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/nxdl.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/nxdl_index.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/nxdl_index.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/xsd.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/xsd.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/docs/xsd_units.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/docs/xsd_units.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/ext/contrib_ext.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/ext/contrib_ext.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/directories.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/directories.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/globals/nxdl.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/globals/nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/discover.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/discover.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/nxdl/syntax.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/nxdl/syntax.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_docs.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_nxdl.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""This is a code that performs several tests on nexus tool
-
-"""
+"""This is a code that performs several tests on nexus tool"""
 
 #
 # Copyright The NOMAD Authors.
 #
 # This file is part of NOMAD. See https://nomad-lab.eu for further info.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -19,14 +17,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 
 import lxml.etree as ET
+import pytest
 
 from ..utils import nxdl_utils as nexus
 
 
 def test_get_nexus_classes_units_attributes():
     """Check the correct parsing of a separate list for:
     Nexus classes (base_classes)
@@ -132,7 +131,64 @@
     assert len(elist) == 4
 
     (_, _, elist) = nexus.get_inherited_nodes(
         nxdl_path="/ENTRY/INSTRUMENT/ENVIRONMENT/voltage_controller",
         nx_name="NXiv_temp",
     )
     assert len(elist) == 4
+
+
+@pytest.mark.parametrize(
+    "hdf_name,concept_name,should_fit",
+    [
+        ("source_pump", "sourceType", False),
+        ("source_pump", "sourceTYPE", True),
+        ("source pump", "sourceTYPE", False),
+        ("source", "sourceTYPE", False),
+        ("source123", "SOURCE", True),
+        ("1source", "SOURCE", True),
+        ("_source", "SOURCE", True),
+        ("same_name", "same_name", True),
+        ("angular_energy_resolution", "angularNresolution", True),
+        ("angularresolution", "angularNresolution", False),
+        ("Name with some whitespaces in it", "ENTRY", False),
+        ("simple_name", "TEST", True),
+        (".test", "TEST", False),
+    ],
+)
+def test_namefitting(hdf_name, concept_name, should_fit):
+    """Test namefitting of nexus concept names"""
+    if should_fit:
+        assert nexus.get_nx_namefit(hdf_name, concept_name) > -1
+    else:
+        assert nexus.get_nx_namefit(hdf_name, concept_name) == -1
+
+
+@pytest.mark.parametrize(
+    "hdf_name,concept_name, score",
+    [
+        ("test_name", "TEST_name", 9),
+        ("te_name", "TEST_name", 7),
+        ("my_other_name", "TEST_name", 5),
+        ("test_name", "test_name", 18),
+        ("test_other", "test_name", -1),
+        ("my_fancy_yet_long_name", "my_SOME_name", 8),
+    ],
+)
+def test_namefitting_scores(hdf_name, concept_name, score):
+    """Test namefitting of nexus concept names"""
+    assert nexus.get_nx_namefit(hdf_name, concept_name) == score
+
+
+@pytest.mark.parametrize(
+    "better_fit,better_ref,worse_fit,worse_ref",
+    [
+        ("sourcetype", "sourceTYPE", "source_pump", "sourceTYPE"),
+        ("source_pump", "sourceTYPE", "source_pump", "TEST"),
+    ],
+)
+def test_namefitting_precedence(better_fit, better_ref, worse_fit, worse_ref):
+    """Test if namefitting follows proper precedence rules"""
+
+    assert nexus.get_nx_namefit(better_fit, better_ref) > nexus.get_nx_namefit(
+        worse_fit, worse_ref
+    )
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/copy.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/copy.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/diff.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/diff.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/github.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/github.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/dev_tools/utils/nxdl_utils.py` & `pynxtools-0.3.0/pynxtools/definitions/dev_tools/utils/nxdl_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # pylint: disable=too-many-lines
-"""Parse NeXus definition files
-"""
+"""Parse NeXus definition files"""
 
 import os
 import re
 import textwrap
 from functools import lru_cache
 from glob import glob
 from pathlib import Path
+from typing import List
+from typing import Optional
 
 import lxml.etree as ET
 from lxml.etree import ParseError as xmlER
 
 
 def remove_namespace_from_tag(tag):
     """Helper function to remove the namespace from an XML tag."""
@@ -40,16 +41,16 @@
 
 def get_app_defs_names():
     """Returns all the AppDef names without their extension: .nxdl.xml"""
     app_def_path_glob = nexus_def_path / "applications" / "*.nxdl*"
 
     contrib_def_path_glob = Path(nexus_def_path) / "contributed_definitions" / "*.nxdl*"
 
-    files = sorted(glob(app_def_path_glob))
-    for nexus_file in sorted(contrib_def_path_glob):
+    files = sorted(glob(str(app_def_path_glob)))
+    for nexus_file in sorted(glob(str(contrib_def_path_glob))):
         root = get_xml_root(nexus_file)
         if root.attrib["category"] == "application":
             files.append(nexus_file)
 
     return [Path(file).name[:-9] for file in files] + ["NXroot"]
 
 
@@ -104,50 +105,77 @@
 def get_nx_class(nxdl_elem):
     """Get the nexus class for a NXDL node"""
     if "category" in nxdl_elem.attrib.keys():
         return ""
     return nxdl_elem.attrib.get("type", "NX_CHAR")
 
 
-def get_nx_namefit(hdf_name, name, name_any=False):
+def get_nx_namefit(hdf_name: str, name: str, name_any: bool = False) -> int:
     """
     Checks if an HDF5 node name corresponds to a child of the NXDL element.
-    A group of uppercase letters anywhere can be replaced by an arbitrary name.
+    A group of uppercase letters anywhere in the name is treated as freely choosable
+    part of this name.
+    If a match is found this function returns twice the length for an exact match,
+    otherwise the number of matching characters (case insensitive) or zero, if
+    `name_any` is set to True, is returned.
+    All uppercase groups are considered independently.
+    Lowercase matches are independent of uppercase group lengths, e.g.,
+    an hdf_name `get_nx_namefit("my_fancy_yet_long_name", "my_SOME_name")` would
+    return a score of 8 for the lowercase matches `my_..._name`.
+    All characters in `[a-zA-Z0-9_.]` are considered for matching to an uppercase letter.
+    If you use any other letter in the name, it will not match and return -1.
+    Periods at the beginning or end of the hdf_name are not allowed, only exact
+    matches will be considered.
+
+    Examples:
+
+        * `get_nx_namefit("test_name", "TEST_name")` returns 9
+        * `get_nx_namefit("te_name", "TEST_name")` returns 7
+        * `get_nx_namefit("my_other_name", "TEST_name")` returns 5
+        * `get_nx_namefit("test_name", "test_name")` returns 18
+        * `get_nx_namefit("test_other", "test_name")` returns -1
 
     Args:
-        hdf_name (str): The hdf_name, containing uppercase parts.
-        name (str): The string to match against hdf_name.
+        hdf_name (str): The hdf_name, containing the name of the HDF5 node.
+        name (str): The concept name to match against.
         name_any (bool, optional):
-            Accept any name and just return the matching characters.
+            Accept any name and return either 0 (match) or -1 (no match).
             Defaults to False.
 
     Returns:
-        int:
-            -1 if no match is found or the number of matching
-            characters (case insensitive) between for all uppercase groups.
+        int: -1 if no match is found or the number of matching
+             characters (case insensitive).
     """
+    path_regex = r"([a-zA-Z0-9_.]+)"
+
     if name == hdf_name:
         return len(name) * 2
+    if hdf_name.startswith(".") or hdf_name.endswith("."):
+        # Don't match anything with a dot at the beginning or end
+        return -1
 
-    uppercase_parts = re.findall("[A-Z]+(?:_[A-Z]+)*", name)
+    uppercase_parts = re.findall(r"[A-Z]+(?:_[A-Z]+)*", name)
 
+    regex_name = name
+    uppercase_count = 0
     for up in uppercase_parts:
-        name = name.replace(up, r"([a-zA-Z0-9_]+)")
+        uppercase_count += len(up)
+        regex_name = regex_name.replace(up, path_regex)
 
-    name_match = re.search(rf"^{name}$", hdf_name)
+    name_match = re.search(rf"^{regex_name}$", hdf_name)
     if name_match is None:
         return 0 if name_any else -1
 
-    fit = 0
-    for up, low in zip(uppercase_parts, name_match.groups()):
-        for i in range(min(len(up), len(low))):
-            if up[i].lower() == low[i]:
-                fit += 1
+    match_count = 0
+    for uppercase, match in zip(uppercase_parts, name_match.groups()):
+        for s1, s2 in zip(uppercase.upper(), match.upper()):
+            if s1 == s2:
+                match_count += 1
 
-    return fit
+    return len(name) + match_count - uppercase_count
 
 
 def get_nx_classes():
     """Read base classes from the NeXus definition folder.
     Check each file in base_classes, applications, contributed_definitions.
     If its category attribute is 'base', then it is added to the list."""
     nexus_definition_path = nexus_def_path
@@ -313,26 +341,14 @@
     """Checks if an NXDL child node fits to the specific name (either nxdl or hdf)
     name       - nxdl name
     class_type - nxdl type or hdf classname (for groups, it is obligatory)
     hdf_name   - hdf name"""
     for child in nxdl_elem:
         if not isinstance(child.tag, str):
             continue
-        if child.attrib.get("name") == name:
-            return set_nxdlpath(child, nxdl_elem)
-    for child in nxdl_elem:
-        if not isinstance(child.tag, str):
-            continue
-        if child.attrib.get("name") == name:
-            child.set("nxdlbase", nxdl_elem.get("nxdlbase"))
-            return child
-
-    for child in nxdl_elem:
-        if not isinstance(child.tag, str):
-            continue
         result = get_own_nxdl_child_reserved_elements(child, name, nxdl_elem)
         if result is not False:
             return result
         if nexus_type and get_local_name_from_xml(child) != nexus_type:
             continue
         result = get_own_nxdl_child_base_types(
             child, class_type, nxdl_elem, name, hdf_name
@@ -411,15 +427,15 @@
     return "<<REQUIRED>>"
 
 
 # below there are some functions used in get_nxdl_doc function:
 def write_doc_string(logger, doc, attr):
     """Simple function that prints a line in the logger if doc exists"""
     if doc:
-        logger.debug("@%s [NX_CHAR]", attr)
+        logger.debug(f"@{attr} [NX_CHAR]")
     return logger, doc, attr
 
 
 def try_find_units(logger, elem, nxdl_path, doc, attr):
     """Try to find if units is defined inside the field in the NXDL element,
     otherwise try to find if units is defined as a child of the NXDL element."""
     try:  # try to find if units is defined inside the field in the NXDL element
@@ -563,21 +579,23 @@
     )
     if not ntype:
         anchor = anchor[:-1]
     doc = ""  # RST documentation from the field 'doc'
     doc_field = node.find("doc")
     if doc_field is not None:
         doc = doc_field.text
-    (index, enums) = get_enums(node)  # enums
-    if index:
+    enums = get_enums(node)  # enums
+    if enums is not None:
         enum_str = (
             "\n "
-            + ("Possible values:" if enums.count(",") else "Obligatory value:")
+            + ("Possible values:" if len(enums) > 1 else "Obligatory value:")
             + "\n   "
-            + enums
+            + "["
+            + ",".join(enums)
+            + "]"
             + "\n"
         )
     else:
         enum_str = ""
     return anchor, doc + enum_str
 
 
@@ -599,28 +617,34 @@
 
 
 def get_namespace(element):
     """Extracts the namespace for elements in the NXDL"""
     return element.tag[element.tag.index("{") : element.tag.rindex("}") + 1]
 
 
-def get_enums(node):
-    """Makes list of enumerations, if node contains any.
-    Returns comma separated STRING of enumeration values, if there are enum tag,
-    otherwise empty string."""
-    # collect item values from enumeration tag, if any
+def get_enums(node: ET._Element) -> Optional[List[str]]:
+    """
+    Makes list of enumerations, if node contains any.
+
+    Args:
+        node (ET._Element): The node to check for enumerations.
+
+    Returns:
+        Optional[List[str]]:
+            Returns a list of the enumeration values if an enumeration was found.
+            If no enumeration was found it returns None.
+    """
     namespace = get_namespace(node)
     enums = []
     for enumeration in node.findall(f"{namespace}enumeration"):
         for item in enumeration.findall(f"{namespace}item"):
             enums.append(item.attrib["value"])
-        enums = ",".join(enums)
-        if enums != "":
-            return (True, "[" + enums + "]")
-    return (False, "")  # if there is no enumeration tag, returns empty string
+        if enums:
+            return enums
+    return None
 
 
 def add_base_classes(elist, nx_name=None, elem: ET.Element = None):
     """
     Add the base classes corresponding to the last element in elist to the list. Note that if
     elist is empty, a nxdl file with the name of nx_name or a placeholder elem is used if provided
     """
```

### Comparing `pynxtools-0.2.1/pynxtools/definitions/impatient-guide/conf.py` & `pynxtools-0.3.0/pynxtools/definitions/impatient-guide/conf.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/conf.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/conf.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/simple3D.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/simple3D.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/manual/source/examples/verysimple.py` & `pynxtools-0.3.0/pynxtools/definitions/manual/source/examples/verysimple.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/nxdl.xsd` & `pynxtools-0.3.0/pynxtools/definitions/nxdl.xsd`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/nxdlTypes.xsd` & `pynxtools-0.3.0/pynxtools/definitions/nxdlTypes.xsd`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/utils/create_release_notes.py` & `pynxtools-0.3.0/pynxtools/definitions/utils/create_release_notes.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/definitions/utils/update_copyright_date.py` & `pynxtools-0.3.0/pynxtools/definitions/utils/update_copyright_date.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/eln_mapper/__init__.py` & `pynxtools-0.3.0/pynxtools/eln_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/eln_mapper/eln.py` & `pynxtools-0.3.0/pynxtools/eln_mapper/eln.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/eln_mapper/eln_mapper.py` & `pynxtools-0.3.0/pynxtools/eln_mapper/eln_mapper.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/eln_mapper/scheme_eln.py` & `pynxtools-0.3.0/pynxtools/eln_mapper/scheme_eln.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from typing import Dict, Any
-import xml.etree.ElementTree as ET
+from typing import Any, Dict
+
+import lxml.etree as ET
 import yaml
-from pynxtools.eln_mapper.eln import retrieve_nxdl_file
-from pynxtools.dataconverter.helpers import remove_namespace_from_tag
 
+from pynxtools.dataconverter.helpers import remove_namespace_from_tag
+from pynxtools.eln_mapper.eln import retrieve_nxdl_file
 
 NEXUS_TYPE_TO_NUMPY_TYPE = {
     "NX_CHAR": {
         "convert_typ": "str",
         "component_nm": "StringEditQuantity",
         "default_unit_display": "<No Default unit>",
     },
@@ -104,38 +105,38 @@
     }
     fld_dict.update(m_annotation)
 
     # handle description
     construct_decription(fld_elem, fld_dict)
 
 
-def construct_decription(elm: ET.Element, concept_dict: Dict) -> None:
+def construct_decription(elm: ET._Element, concept_dict: Dict) -> None:
     """Collect doc from concept doc."""
     desc_text = ""
     for child_elm in elm:
         tag = remove_namespace_from_tag(child_elm.tag)
         if tag == "doc":
             desc_text = child_elm.text
             desc_text = " ".join([x.strip() for x in desc_text.split("\n")])
             break
 
     concept_dict["description"] = desc_text
 
 
-def construct_group_structure(grp_elm: ET.Element, subsections: Dict) -> None:
+def construct_group_structure(grp_elm: ET._Element, subsections: Dict) -> None:
     """To construct group structure as follows:
     <group_name>:
         section:
             m_annotations:
                 eln:
                     overview: true
 
     Parameters
     ----------
-    elm : ET.Element
+    elm : ET._Element
         Group element
     subsections : Dict
         Dict to include group recursively
     """
 
     default_m_annot = {"m_annotations": {"eln": {"overview": True}}}
 
@@ -154,43 +155,43 @@
     section = grp_dict["section"]
     section.update(default_m_annot)
 
     # pass the grp elment for recursive search
     scan_xml_element_recursively(grp_elm, section)
 
 
-def _should_skip_iteration(elm: ET.Element) -> bool:
+def _should_skip_iteration(elm: ET._Element) -> bool:
     """Define some elements here that should be skipped.
 
     Parameters
     ----------
-    elm : ET.Element
+    elm : ET._Element
         The element to investigate to skip
     """
     attr = elm.attrib
     elm_type = ""
     if "type" in attr:
         elm_type = attr["type"]
         if elm_type in ["NXentry"]:
             return True
     return False
 
 
 def scan_xml_element_recursively(
-    nxdl_element: ET.Element,
+    nxdl_element: ET._Element,
     recursive_dict: Dict,
     root_name: str = "",
     reader_name: str = "<READER_NAME>",
     is_root: bool = False,
 ) -> None:
     """Scan xml elements, and pass the element to the type of element handaler.
 
     Parameters
     ----------
-    nxdl_element : ET.Element
+    nxdl_element : ET._Element
         This xml element that will be scanned through the descendants.
     recursive_dict : Dict
         A dict that store hierarchical structure of scheme eln.
     root_name : str, optional
         Name of root that user want to see to name their application, e.g. MPES,
         by default 'ROOT_NAME'
     reader_name : Prefered name of the reader.
```

### Comparing `pynxtools-0.2.1/pynxtools/nexus/__init__.py` & `pynxtools-0.3.0/pynxtools/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.2.1/pynxtools/nexus/nexus.py` & `pynxtools-0.3.0/pynxtools/nexus/nexus.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     nx_name: str = None,
     elem: ET._Element = None,
     hdf_node=None,
     hdf_path=None,
     hdf_root=None,
     attr=False,
 ):
-    """Returns a list of ET.Element for the given path."""
+    """Returns a list of ET._Element for the given path."""
     # let us start with the given definition file
     if hdf_node is None:
         raise ValueError("hdf_node must not be None")
     elist = []  # type: ignore[var-annotated]
     add_base_classes(elist, nx_name, elem)
     nxdl_elem_path = [elist[0]]
```

### Comparing `pynxtools-0.2.1/pynxtools.egg-info/SOURCES.txt` & `pynxtools-0.3.0/pynxtools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 pynxtools/nexus-version.txt
 pynxtools/dataconverter/__init__.py
 pynxtools/dataconverter/convert.py
 pynxtools/dataconverter/exceptions.py
 pynxtools/dataconverter/file_hashing.py
 pynxtools/dataconverter/hdfdict.py
 pynxtools/dataconverter/helpers.py
+pynxtools/dataconverter/nexus_tree.py
 pynxtools/dataconverter/template.py
+pynxtools/dataconverter/validation.py
 pynxtools/dataconverter/writer.py
 pynxtools/dataconverter/readers/__init__.py
 pynxtools/dataconverter/readers/utils.py
 pynxtools/dataconverter/readers/base/__init__.py
 pynxtools/dataconverter/readers/base/reader.py
-pynxtools/dataconverter/readers/ellips/__init__.py
-pynxtools/dataconverter/readers/ellips/mock.py
-pynxtools/dataconverter/readers/ellips/reader.py
 pynxtools/dataconverter/readers/example/__init__.py
 pynxtools/dataconverter/readers/example/reader.py
 pynxtools/dataconverter/readers/json_map/__init__.py
 pynxtools/dataconverter/readers/json_map/reader.py
 pynxtools/dataconverter/readers/json_yml/__init__.py
 pynxtools/dataconverter/readers/json_yml/reader.py
 pynxtools/definitions/NXDL_VERSION
@@ -129,14 +128,16 @@
 pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml
+pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml
+pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml
@@ -289,26 +290,28 @@
 pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml
+pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
+pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml
 pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml
```

### Comparing `pynxtools-0.2.1/pyproject.toml` & `pynxtools-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     "xarray>=0.20.2",
     "PyYAML>=6.0",
     "numpy>=1.21.2",
     "pandas>=1.3.2",
     "ase>=3.19.0",
     "mergedeep",
     "importlib-metadata",
-    "lxml>=4.9.1", 
+    "lxml>=4.9.1",
+    "anytree",
+    "pydantic",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FAIRmat-NFDI/pynxtools"
 "Bug Tracker" = "https://github.com/FAIRmat-NFDI/pynxtools/issues"
 
 [project.optional-dependencies]
@@ -57,15 +59,15 @@
     "types-pyyaml",
     "types-pytz",
     "types-requests",
     "pip-tools",
     "pre-commit",
 ]
 convert = [
-    "pynxtools[apm,em,mpes,xps,stm,xrd]",
+    "pynxtools[apm,em,mpes,xps,stm,xrd,ellips]",
 ]
 apm = [
     "pynxtools-apm",
 ]
 em = [
     "pynxtools-em",
 ]
@@ -77,14 +79,17 @@
 ]
 stm = [
     "pynxtools-stm",
 ]
 xrd = [
     "pynxtools-xrd",
 ]
+ellips = [
+    "pynxtools-ellips",
+]
 
 [project.scripts]
 read_nexus = "pynxtools.nexus.nexus:main"
 dataconverter = "pynxtools.dataconverter.convert:main_cli"
 generate_eln = "pynxtools.eln_mapper.eln_mapper:get_eln"
 
 [tool.setuptools.package-data]
```

