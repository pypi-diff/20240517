# Comparing `tmp/meteva-1.8.2.tar.gz` & `tmp/meteva-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteva-1.8.2.tar", last modified: Thu Apr  4 16:14:42 2024, max compression
+gzip compressed data, was "meteva-1.8.3.tar", last modified: Fri May 17 09:15:22 2024, max compression
```

## Comparing `meteva-1.8.2.tar` & `meteva-1.8.3.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.062904 meteva-1.8.2/
--rw-rw-rw-   0        0        0      940 2024-04-04 16:14:42.061968 meteva-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2024-02-23 15:27:40.000000 meteva-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.851526 meteva-1.8.2/meteva/
--rw-rw-rw-   0        0        0      254 2024-04-04 16:14:04.000000 meteva-1.8.2/meteva/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.863528 meteva-1.8.2/meteva/base/
--rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.8.2/meteva/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.947085 meteva-1.8.2/meteva/base/basicdata/
--rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.8.2/meteva/base/basicdata/__init__.py
--rw-rw-rw-   0        0        0     1266 2023-11-13 02:13:55.000000 meteva-1.8.2/meteva/base/basicdata/const.py
--rw-rw-rw-   0        0        0     7386 2023-07-03 13:42:46.000000 meteva-1.8.2/meteva/base/basicdata/ctl.py
--rw-rw-rw-   0        0        0    19260 2023-04-21 03:19:11.000000 meteva-1.8.2/meteva/base/basicdata/dicts.py
--rw-rw-rw-   0        0        0    11165 2022-12-20 01:27:25.000000 meteva-1.8.2/meteva/base/basicdata/grid.py
--rw-rw-rw-   0        0        0    32686 2024-03-05 12:30:49.000000 meteva-1.8.2/meteva/base/basicdata/grid_data.py
--rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.8.2/meteva/base/basicdata/keys.py
--rw-rw-rw-   0        0        0     7163 2022-09-17 14:18:55.000000 meteva-1.8.2/meteva/base/basicdata/sta_data.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.214771 meteva-1.8.2/meteva/base/fun/
--rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.8.2/meteva/base/fun/__init__.py
--rw-rw-rw-   0        0        0    30617 2024-02-12 23:48:02.000000 meteva-1.8.2/meteva/base/fun/combining.py
--rw-rw-rw-   0        0        0    28007 2024-01-07 04:30:26.000000 meteva-1.8.2/meteva/base/fun/computing.py
--rw-rw-rw-   0        0        0    18705 2024-03-04 12:58:48.000000 meteva-1.8.2/meteva/base/fun/diagnosing.py
--rw-rw-rw-   0        0        0    35296 2024-02-21 15:22:08.000000 meteva-1.8.2/meteva/base/fun/grouping.py
--rw-rw-rw-   0        0        0    34810 2024-02-28 06:31:06.000000 meteva-1.8.2/meteva/base/fun/interpolating.py
--rw-rw-rw-   0        0        0    14417 2023-04-23 14:30:42.000000 meteva-1.8.2/meteva/base/fun/nearing.py
--rw-rw-rw-   0        0        0    56419 2024-04-03 00:23:48.000000 meteva-1.8.2/meteva/base/fun/selecting.py
--rw-rw-rw-   0        0        0    36232 2023-08-31 06:14:58.000000 meteva-1.8.2/meteva/base/fun/statisticing.py
--rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.8.2/meteva/base/fun/timing.py
--rw-rw-rw-   0        0        0     7042 2023-04-23 13:10:39.000000 meteva-1.8.2/meteva/base/fun/transformating.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.600834 meteva-1.8.2/meteva/base/io/
--rw-rw-rw-   0        0        0    21310 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/io/CMADaasAccess.py
--rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.8.2/meteva/base/io/DataBlock_pb2.py
--rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.8.2/meteva/base/io/GDS_data_service.py
--rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.8.2/meteva/base/io/SignGenUtil.py
--rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.8.2/meteva/base/io/__init__.py
--rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.8.2/meteva/base/io/clienthandler.py
--rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.8.2/meteva/base/io/encoding.py
--rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/ftpconn.py
--rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.8.2/meteva/base/io/httpclient.py
--rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/httpconn.py
--rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/loglib.py
--rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.8.2/meteva/base/io/print_grib_info.py
--rw-rw-rw-   0        0        0    21031 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/io/read_graphydata.py
--rw-rw-rw-   0        0        0    81459 2024-04-02 06:05:14.000000 meteva-1.8.2/meteva/base/io/read_griddata.py
--rw-rw-rw-   0        0        0    91613 2024-02-29 15:27:44.000000 meteva-1.8.2/meteva/base/io/read_stadata.py
--rw-rw-rw-   0        0        0     4670 2023-03-02 08:36:03.000000 meteva-1.8.2/meteva/base/io/write_array.py
--rw-rw-rw-   0        0        0    10893 2024-02-23 08:01:29.000000 meteva-1.8.2/meteva/base/io/write_griddata.py
--rw-rw-rw-   0        0        0    12830 2023-10-10 05:58:04.000000 meteva-1.8.2/meteva/base/io/write_stadata.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.841901 meteva-1.8.2/meteva/base/tool/
--rw-rw-rw-   0        0        0     1216 2023-03-01 02:53:13.000000 meteva-1.8.2/meteva/base/tool/__init__.py
--rw-rw-rw-   0        0        0    54048 2024-02-23 03:35:58.000000 meteva-1.8.2/meteva/base/tool/color_tools.py
--rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.8.2/meteva/base/tool/copy_tools.py
--rw-rw-rw-   0        0        0     1248 2023-04-04 14:53:16.000000 meteva-1.8.2/meteva/base/tool/frprmn2.py
--rw-rw-rw-   0        0        0     4695 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/tool/grib_tools.py
--rw-rw-rw-   0        0        0     8797 2023-07-04 02:34:53.000000 meteva-1.8.2/meteva/base/tool/maskout.py
--rw-rw-rw-   0        0        0    11675 2023-06-20 14:47:49.000000 meteva-1.8.2/meteva/base/tool/math_tools.py
--rw-rw-rw-   0        0        0    12484 2024-01-18 07:10:32.000000 meteva-1.8.2/meteva/base/tool/path_tools.py
--rw-rw-rw-   0        0        0   180509 2024-02-23 05:27:55.000000 meteva-1.8.2/meteva/base/tool/plot_tools.py
--rw-rw-rw-   0        0        0    35597 2024-02-23 03:38:22.000000 meteva-1.8.2/meteva/base/tool/plot_tools_adv.py
--rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.8.2/meteva/base/tool/process_tools.py
--rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.8.2/meteva/base/tool/station_tools.py
--rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.8.2/meteva/base/tool/time_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.851898 meteva-1.8.2/meteva/method/
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.426875 meteva-1.8.2/meteva/method/Vector/
--rw-rw-rw-   0        0        0      624 2024-02-22 04:04:47.000000 meteva-1.8.2/meteva/method/Vector/__init__.py
--rw-rw-rw-   0        0        0    33207 2024-02-22 07:27:38.000000 meteva-1.8.2/meteva/method/Vector/plot.py
--rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.8.2/meteva/method/Vector/score.py
--rw-rw-rw-   0        0        0      387 2023-09-22 07:51:37.000000 meteva-1.8.2/meteva/method/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.998948 meteva-1.8.2/meteva/method/continuous/
--rw-rw-rw-   0        0        0     1128 2024-01-27 14:08:41.000000 meteva-1.8.2/meteva/method/continuous/__init__.py
--rw-rw-rw-   0        0        0    40762 2024-02-23 01:50:41.000000 meteva-1.8.2/meteva/method/continuous/plot.py
--rw-rw-rw-   0        0        0    54412 2024-02-22 03:32:35.000000 meteva-1.8.2/meteva/method/continuous/score.py
--rw-rw-rw-   0        0        0     1248 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/method/continuous/skill.py
--rw-rw-rw-   0        0        0     5417 2023-12-26 02:41:16.000000 meteva-1.8.2/meteva/method/continuous/table.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.025974 meteva-1.8.2/meteva/method/ensemble/
--rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.8.2/meteva/method/ensemble/__init__.py
--rw-rw-rw-   0        0        0     4412 2022-02-26 23:44:42.000000 meteva-1.8.2/meteva/method/ensemble/plot.py
--rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/ensemble/score.py
--rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.8.2/meteva/method/ensemble/table.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.060950 meteva-1.8.2/meteva/method/multi_category/
--rw-rw-rw-   0        0        0      602 2024-04-04 15:25:22.000000 meteva-1.8.2/meteva/method/multi_category/__init__.py
--rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.8.2/meteva/method/multi_category/plot.py
--rw-rw-rw-   0        0        0    27982 2024-04-04 16:02:06.000000 meteva-1.8.2/meteva/method/multi_category/score.py
--rw-rw-rw-   0        0        0     7803 2022-12-28 08:27:35.000000 meteva-1.8.2/meteva/method/multi_category/table.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.114949 meteva-1.8.2/meteva/method/probability/
--rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.8.2/meteva/method/probability/__init__.py
--rw-rw-rw-   0        0        0    21703 2022-10-23 06:25:47.000000 meteva-1.8.2/meteva/method/probability/plot.py
--rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/probability/score.py
--rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/probability/table.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.160003 meteva-1.8.2/meteva/method/space/
--rw-rw-rw-   0        0        0      802 2024-02-21 07:49:52.000000 meteva-1.8.2/meteva/method/space/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.189005 meteva-1.8.2/meteva/method/space/acc/
--rw-rw-rw-   0        0        0       82 2023-10-04 03:56:47.000000 meteva-1.8.2/meteva/method/space/acc/__init__.py
--rw-rw-rw-   0        0        0    10168 2024-03-26 08:45:02.000000 meteva-1.8.2/meteva/method/space/acc/acc.py
--rw-rw-rw-   0        0        0      747 2023-09-15 14:42:11.000000 meteva-1.8.2/meteva/method/space/acc/acc_climate_pre.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.211004 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/
--rw-rw-rw-   0        0        0      134 2023-10-01 08:10:28.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.294002 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/
--rw-rw-rw-   0        0        0      244 2023-10-01 08:15:28.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py
--rw-rw-rw-   0        0        0      774 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0     1560 2024-02-18 07:34:44.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py
--rw-rw-rw-   0        0        0     4594 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py
--rw-rw-rw-   0        0        0     2530 2023-08-21 23:56:50.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0     3977 2024-02-18 07:34:44.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py
--rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      625 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py
--rw-rw-rw-   0        0        0     1978 2023-08-22 00:02:02.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py
--rw-rw-rw-   0        0        0      278 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_prep.py
--rw-rw-rw-   0        0        0     5528 2023-08-22 00:02:02.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.307023 meteva-1.8.2/meteva/method/space/cra/
--rw-rw-rw-   0        0        0       62 2024-02-21 07:47:43.000000 meteva-1.8.2/meteva/method/space/cra/__init__.py
--rw-rw-rw-   0        0        0     5824 2024-02-21 13:13:05.000000 meteva-1.8.2/meteva/method/space/cra/cra.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.329005 meteva-1.8.2/meteva/method/space/fqi/
--rw-rw-rw-   0        0        0       65 2023-10-01 08:00:00.000000 meteva-1.8.2/meteva/method/space/fqi/__init__.py
--rw-rw-rw-   0        0        0     5179 2023-09-23 11:58:12.000000 meteva-1.8.2/meteva/method/space/fqi/fqi.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.388005 meteva-1.8.2/meteva/method/space/fqi/lib/
--rw-rw-rw-   0        0        0      366 2023-10-01 08:03:25.000000 meteva-1.8.2/meteva/method/space/fqi/lib/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-08-22 02:14:25.000000 meteva-1.8.2/meteva/method/space/fqi/lib/aaft2d.py
--rw-rw-rw-   0        0        0      658 2023-01-29 06:47:11.000000 meteva-1.8.2/meteva/method/space/fqi/lib/ampstats.py
--rw-rw-rw-   0        0        0       93 2023-01-24 09:38:13.000000 meteva-1.8.2/meteva/method/space/fqi/lib/cbind.py
--rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.2/meteva/method/space/fqi/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      947 2023-04-02 10:16:53.000000 meteva-1.8.2/meteva/method/space/fqi/lib/distfun.py
--rw-rw-rw-   0        0        0      947 2023-03-26 09:44:16.000000 meteva-1.8.2/meteva/method/space/fqi/lib/fft2d.py
--rw-rw-rw-   0        0        0     2531 2023-08-22 02:11:26.000000 meteva-1.8.2/meteva/method/space/fqi/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/fqi/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0      278 2021-06-01 19:24:10.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locmeasures2d_prep.py
--rw-rw-rw-   0        0        0     4102 2024-02-18 12:48:31.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locperf.py
--rw-rw-rw-   0        0        0      262 2023-03-25 10:39:31.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locperfer.py
--rw-rw-rw-   0        0        0      158 2023-01-28 04:35:01.000000 meteva-1.8.2/meteva/method/space/fqi/lib/mae.py
--rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.2/meteva/method/space/fqi/lib/solutionset.py
--rw-rw-rw-   0        0        0     2398 2023-08-22 02:14:05.000000 meteva-1.8.2/meteva/method/space/fqi/lib/surrogater2d.py
--rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.2/meteva/method/space/fqi/lib/util.py
--rw-rw-rw-   0        0        0      274 2023-01-26 07:28:17.000000 meteva-1.8.2/meteva/method/space/fqi/lib/zapsmall.py
--rw-rw-rw-   0        0        0     1008 2023-08-22 02:11:50.000000 meteva-1.8.2/meteva/method/space/fqi/uiqi.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.395002 meteva-1.8.2/meteva/method/space/fss/
--rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.8.2/meteva/method/space/fss/__init__.py
--rw-rw-rw-   0        0        0     8387 2023-04-22 14:53:18.000000 meteva-1.8.2/meteva/method/space/fss/fss.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.484058 meteva-1.8.2/meteva/method/space/fuzzy_logic/
--rw-rw-rw-   0        0        0      194 2023-10-01 07:24:57.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-08-21 03:43:04.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/fss.py
--rw-rw-rw-   0        0        0     2273 2023-09-06 03:36:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/fuzzy.py
--rw-rw-rw-   0        0        0     1806 2023-09-04 07:58:00.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/joint.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.677592 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/
--rw-rw-rw-   0        0        0      492 2023-10-01 08:15:28.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/__init__.py
--rw-rw-rw-   0        0        0      783 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      860 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fss2dfun.py
--rw-rw-rw-   0        0        0     1908 2023-08-20 08:53:21.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py
--rw-rw-rw-   0        0        0     7349 2023-09-06 09:36:29.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2d.py
--rw-rw-rw-   0        0        0     1016 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py
--rw-rw-rw-   0        0        0     1243 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py
--rw-rw-rw-   0        0        0     1266 2023-09-04 08:38:48.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py
--rw-rw-rw-   0        0        0     6283 2023-08-22 01:44:20.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     3456 2023-09-25 03:11:25.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py
--rw-rw-rw-   0        0        0     7289 2023-08-20 13:30:27.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      188 2023-08-20 12:21:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/mincvg2dfun.py
--rw-rw-rw-   0        0        0      183 2023-08-21 03:05:37.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/multicon2dfun.py
--rw-rw-rw-   0        0        0      536 2023-09-06 03:46:36.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py
--rw-rw-rw-   0        0        0      715 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder.py
--rw-rw-rw-   0        0        0      811 2023-08-21 03:06:59.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py
--rw-rw-rw-   0        0        0     4704 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/vxstats.py
--rw-rw-rw-   0        0        0      275 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/zapsmall.py
--rw-rw-rw-   0        0        0     2255 2023-09-07 06:37:55.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/minimum_coverage.py
--rw-rw-rw-   0        0        0     2233 2023-09-06 09:01:35.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/multi_event.py
--rw-rw-rw-   0        0        0     2218 2023-09-06 03:36:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/pragmatic.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.695594 meteva-1.8.2/meteva/method/space/geo_box_plot/
--rw-rw-rw-   0        0        0     2496 2023-09-25 04:29:49.000000 meteva-1.8.2/meteva/method/space/geo_box_plot/GeoBoxPlot.py
--rw-rw-rw-   0        0        0       24 2023-10-02 02:14:48.000000 meteva-1.8.2/meteva/method/space/geo_box_plot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.744592 meteva-1.8.2/meteva/method/space/geometric_characterizations/
--rw-rw-rw-   0        0        0       86 2023-10-01 08:16:08.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/__init__.py
--rw-rw-rw-   0        0        0     5187 2024-02-18 08:43:27.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/aindex.py
--rw-rw-rw-   0        0        0     2664 2023-09-24 12:12:06.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/cindex.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.756595 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/
--rw-rw-rw-   0        0        0       55 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/__init__.py
--rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/util.py
--rw-rw-rw-   0        0        0     2934 2023-09-24 11:40:50.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/sindex.py
--rw-rw-rw-   0        0        0     1859 2023-08-22 00:10:29.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/spatial_index.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.758594 meteva-1.8.2/meteva/method/space/hausdorff_metric/
--rw-rw-rw-   0        0        0       43 2023-10-01 08:17:18.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.770594 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/
--rw-rw-rw-   0        0        0      150 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-05-23 18:14:16.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/as_unitname.py
--rw-rw-rw-   0        0        0      947 2023-04-02 10:14:50.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distfun.py
--rw-rw-rw-   0        0        0     4731 2023-04-02 10:09:41.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distmap.py
--rw-rw-rw-   0        0        0     2518 2023-08-22 00:16:03.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-05-23 18:14:16.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/solutionset.py
--rw-rw-rw-   0        0        0     5361 2024-02-18 09:02:26.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/locperf.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.163305 meteva-1.8.2/meteva/method/space/mode/
--rw-rw-rw-   0        0        0     1960 2023-08-24 01:06:15.000000 meteva-1.8.2/meteva/method/space/mode/__init__.py
--rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/angles_psp.py
--rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/as_psp.py
--rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.8.2/meteva/method/space/mode/bearing.py
--rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/censqdelta.py
--rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.8.2/meteva/method/space/mode/centmatch.py
--rw-rw-rw-   0        0        0    13874 2023-12-22 00:57:57.000000 meteva-1.8.2/meteva/method/space/mode/consistent.py
--rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/data_pre.py
--rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.8.2/meteva/method/space/mode/deltametric.py
--rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltamm.py
--rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltammSqCen.py
--rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltamm_bak.py
--rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/distmap.py
--rw-rw-rw-   0        0        0     6070 2024-02-22 03:58:40.000000 meteva-1.8.2/meteva/method/space/mode/feature_axis.py
--rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.8.2/meteva/method/space/mode/feature_comps.py
--rw-rw-rw-   0        0        0    32379 2023-08-22 14:03:20.000000 meteva-1.8.2/meteva/method/space/mode/feature_finder.py
--rw-rw-rw-   0        0        0    10157 2023-02-07 02:37:08.000000 meteva-1.8.2/meteva/method/space/mode/feature_match_analyzer.py
--rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.8.2/meteva/method/space/mode/feature_props.py
--rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.8.2/meteva/method/space/mode/feature_table.py
--rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.8.2/meteva/method/space/mode/interester.py
--rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/intersect.py
--rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/lengths_psp.py
--rw-rw-rw-   0        0        0     1358 2023-04-23 02:57:31.000000 meteva-1.8.2/meteva/method/space/mode/load.py
--rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/loc_list_setup.py
--rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.8.2/meteva/method/space/mode/locperf.py
--rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/make_SpatialVx_bak.py
--rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/make_spatialVx.py
--rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.8.2/meteva/method/space/mode/merge_force.py
--rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/midpoints_psp.py
--rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/minboundmatch.py
--rw-rw-rw-   0        0        0     5727 2023-02-07 02:37:07.000000 meteva-1.8.2/meteva/method/space/mode/operater.py
--rw-rw-rw-   0        0        0    32345 2023-08-01 13:36:13.000000 meteva-1.8.2/meteva/method/space/mode/plot.py
--rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.8.2/meteva/method/space/mode/regress2.py
--rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.8.2/meteva/method/space/mode/sma.py
--rw-rw-rw-   0        0        0    10465 2023-07-27 07:47:11.000000 meteva-1.8.2/meteva/method/space/mode/tran_to_dataframe.py
--rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/utils.py
--rw-rw-rw-   0        0        0     4595 2023-03-20 12:31:25.000000 meteva-1.8.2/meteva/method/space/point_to_area.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.184306 meteva-1.8.2/meteva/method/space/pphindcast/
--rw-rw-rw-   0        0        0      134 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/pphindcast/__init__.py
--rw-rw-rw-   0        0        0     6295 2023-05-12 01:24:44.000000 meteva-1.8.2/meteva/method/space/pphindcast/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     2976 2023-08-22 02:29:43.000000 meteva-1.8.2/meteva/method/space/pphindcast/kernel2dsmooth.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.201306 meteva-1.8.2/meteva/method/space/pphindcast/lib/
--rw-rw-rw-   0        0        0      272 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/as_unitname.py
--rw-rw-rw-   0        0        0       86 2021-09-05 14:49:53.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/datagrabber.py
--rw-rw-rw-   0        0        0     1081 2021-10-24 16:33:14.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/hoods2dPrep.py
--rw-rw-rw-   0        0        0     2512 2023-08-22 00:21:36.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/im.py
--rw-rw-rw-   0        0        0     6295 2023-05-11 14:59:50.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     2963 2023-08-22 00:21:36.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dsmooth.py
--rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      719 2023-01-11 13:49:43.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/thresholder.py
--rw-rw-rw-   0        0        0     4704 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/vxstats.py
--rw-rw-rw-   0        0        0     6087 2023-09-24 15:02:06.000000 meteva-1.8.2/meteva/method/space/pphindcast/pphindcast2d.py
--rw-rw-rw-   0        0        0      275 2023-05-12 01:24:46.000000 meteva-1.8.2/meteva/method/space/pphindcast/zapsmall.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.266307 meteva-1.8.2/meteva/method/space/rigider/
--rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.8.2/meteva/method/space/rigider/__init__.py
--rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.8.2/meteva/method/space/rigider/fint2d.py
--rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.8.2/meteva/method/space/rigider/fint2d_old.py
--rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.8.2/meteva/method/space/rigider/imomenter.py
--rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/mij.py
--rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/q_loss_rigid.py
--rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.8.2/meteva/method/space/rigider/rigid_transform.py
--rw-rw-rw-   0        0        0    14406 2024-02-21 13:04:04.000000 meteva-1.8.2/meteva/method/space/rigider/rigider.py
--rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/zapsmall.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.283307 meteva-1.8.2/meteva/method/space/s1/
--rw-rw-rw-   0        0        0     2234 2023-09-25 04:01:56.000000 meteva-1.8.2/meteva/method/space/s1/S1.py
--rw-rw-rw-   0        0        0       16 2023-10-01 09:00:39.000000 meteva-1.8.2/meteva/method/space/s1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.299306 meteva-1.8.2/meteva/method/space/saller/
--rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.8.2/meteva/method/space/saller/__init__.py
--rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.8.2/meteva/method/space/saller/saller.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.362821 meteva-1.8.2/meteva/method/space/significance/
--rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.8.2/meteva/method/space/significance/LocSig.py
--rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.8.2/meteva/method/space/significance/__init__.py
--rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.8.2/meteva/method/space/significance/bootstrap.py
--rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.8.2/meteva/method/space/significance/bootstrap_ci.py
--rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.8.2/meteva/method/space/significance/is_sig.py
--rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.8.2/meteva/method/space/significance/sig_coverage.py
--rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.8.2/meteva/method/space/significance/significance.py
--rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.8.2/meteva/method/space/significance/spatbiasFS.py
--rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.8.2/meteva/method/space/significance/tsboot.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.365824 meteva-1.8.2/meteva/method/space/uqi/
--rw-rw-rw-   0        0        0       20 2023-09-22 07:51:37.000000 meteva-1.8.2/meteva/method/space/uqi/__init__.py
--rw-rw-rw-   0        0        0      989 2023-09-22 08:31:14.000000 meteva-1.8.2/meteva/method/space/uqi/uqi.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.422875 meteva-1.8.2/meteva/method/space/vgm/
--rw-rw-rw-   0        0        0      167 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/method/space/vgm/__init__.py
--rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/rdist.py
--rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/structurogram.py
--rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/structurogram_matrix.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.453941 meteva-1.8.2/meteva/method/weather_system/
--rw-rw-rw-   0        0        0       25 2024-02-22 12:26:37.000000 meteva-1.8.2/meteva/method/weather_system/__init__.py
--rw-rw-rw-   0        0        0    15316 2024-02-11 03:37:27.000000 meteva-1.8.2/meteva/method/weather_system/identify.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.544874 meteva-1.8.2/meteva/method/yes_or_no/
--rw-rw-rw-   0        0        0      850 2023-10-02 14:10:45.000000 meteva-1.8.2/meteva/method/yes_or_no/__init__.py
--rw-rw-rw-   0        0        0    11060 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/yes_or_no/plot.py
--rw-rw-rw-   0        0        0    36054 2023-10-29 14:33:23.000000 meteva-1.8.2/meteva/method/yes_or_no/score.py
--rw-rw-rw-   0        0        0     2995 2023-03-03 07:52:23.000000 meteva-1.8.2/meteva/method/yes_or_no/skill.py
--rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/yes_or_no/table.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.635591 meteva-1.8.2/meteva/perspact/
--rw-rw-rw-   0        0        0      167 2024-03-27 01:02:36.000000 meteva-1.8.2/meteva/perspact/__init__.py
--rw-rw-rw-   0        0        0     8873 2024-04-04 14:21:50.000000 meteva-1.8.2/meteva/perspact/middel_high.py
--rw-rw-rw-   0        0        0    33147 2024-01-27 14:06:47.000000 meteva-1.8.2/meteva/perspact/middle_prepare.py
--rw-rw-rw-   0        0        0    11614 2024-02-23 06:31:38.000000 meteva-1.8.2/meteva/perspact/multi_element_veri.py
--rw-rw-rw-   0        0        0    37870 2024-01-05 07:16:22.000000 meteva-1.8.2/meteva/perspact/score.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.654839 meteva-1.8.2/meteva/product/
--rw-rw-rw-   0        0        0      216 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.757839 meteva-1.8.2/meteva/product/application/
--rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.8.2/meteva/product/application/__init__.py
--rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.8.2/meteva/product/application/data_collection.py
--rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.8.2/meteva/product/application/data_distribute.py
--rw-rw-rw-   0        0        0    24149 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/application/data_prepare.py
--rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.8.2/meteva/product/application/fun.py
--rw-rw-rw-   0        0        0     2951 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/application/terrain_height_correction.py
--rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.8.2/meteva/product/application/time_compare.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.759863 meteva-1.8.2/meteva/product/presentation/
--rw-rw-rw-   0        0        0        0 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/presentation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.973903 meteva-1.8.2/meteva/product/program/
--rw-rw-rw-   0        0        0     1247 2023-07-07 02:14:59.000000 meteva-1.8.2/meteva/product/program/__init__.py
--rw-rw-rw-   0        0        0    19079 2023-01-13 06:11:18.000000 meteva-1.8.2/meteva/product/program/diurnal.py
--rw-rw-rw-   0        0        0    17966 2023-05-25 06:33:55.000000 meteva-1.8.2/meteva/product/program/error_ana_list.py
--rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.8.2/meteva/product/program/error_ana_scatter.py
--rw-rw-rw-   0        0        0    30270 2023-11-16 01:25:36.000000 meteva-1.8.2/meteva/product/program/fun.py
--rw-rw-rw-   0        0        0     6702 2023-10-31 00:43:33.000000 meteva-1.8.2/meteva/product/program/plot.py
--rw-rw-rw-   0        0        0    10578 2023-11-27 13:37:54.000000 meteva-1.8.2/meteva/product/program/process_compare.py
--rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.8.2/meteva/product/program/sample_statistic.py
--rw-rw-rw-   0        0        0    40965 2023-12-26 03:32:01.000000 meteva-1.8.2/meteva/product/program/score.py
--rw-rw-rw-   0        0        0   148120 2024-02-20 02:32:36.000000 meteva-1.8.2/meteva/product/program/space_compare.py
--rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.8.2/meteva/product/program/table.py
--rw-rw-rw-   0        0        0    63209 2023-11-16 01:27:22.000000 meteva-1.8.2/meteva/product/program/time_compare.py
--rw-rw-rw-   0        0        0     5564 2022-07-11 14:46:12.000000 meteva-1.8.2/meteva/product/program/time_space_compare.py
--rw-rw-rw-   0        0        0     2407 2024-01-17 14:09:44.000000 meteva-1.8.2/meteva/product/program/typhoon.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.038905 meteva-1.8.2/meteva/product/regulation/
--rw-rw-rw-   0        0        0      206 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/regulation/__init__.py
--rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.8.2/meteva/product/regulation/environment.py
--rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.8.2/meteva/product/regulation/short_term_heavy_rainfall.py
--rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.8.2/meteva/product/regulation/temperature.py
--rw-rw-rw-   0        0        0    16261 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/regulation/thunderstrom_gale.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.059904 meteva-1.8.2/meteva.egg-info/
--rw-rw-rw-   0        0        0      940 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11718 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 16:14:42.062904 meteva-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2341 2024-03-26 01:59:36.000000 meteva-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:22.064591 meteva-1.8.3/
+-rw-rw-rw-   0        0        0      931 2024-05-17 09:15:22.062591 meteva-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2024-02-23 15:27:40.000000 meteva-1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:18.987593 meteva-1.8.3/meteva/
+-rw-rw-rw-   0        0        0      460 2024-05-17 01:53:18.000000 meteva-1.8.3/meteva/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:18.994594 meteva-1.8.3/meteva/base/
+-rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.8.3/meteva/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.081592 meteva-1.8.3/meteva/base/basicdata/
+-rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.8.3/meteva/base/basicdata/__init__.py
+-rw-rw-rw-   0        0        0     1266 2024-05-14 06:29:02.000000 meteva-1.8.3/meteva/base/basicdata/const.py
+-rw-rw-rw-   0        0        0     7386 2023-07-03 13:42:46.000000 meteva-1.8.3/meteva/base/basicdata/ctl.py
+-rw-rw-rw-   0        0        0    19260 2023-04-21 03:19:11.000000 meteva-1.8.3/meteva/base/basicdata/dicts.py
+-rw-rw-rw-   0        0        0    11165 2022-12-20 01:27:25.000000 meteva-1.8.3/meteva/base/basicdata/grid.py
+-rw-rw-rw-   0        0        0    33008 2024-05-16 01:29:45.000000 meteva-1.8.3/meteva/base/basicdata/grid_data.py
+-rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.8.3/meteva/base/basicdata/keys.py
+-rw-rw-rw-   0        0        0     7166 2024-05-15 06:37:33.000000 meteva-1.8.3/meteva/base/basicdata/sta_data.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.265592 meteva-1.8.3/meteva/base/fun/
+-rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.8.3/meteva/base/fun/__init__.py
+-rw-rw-rw-   0        0        0    30617 2024-02-12 23:48:02.000000 meteva-1.8.3/meteva/base/fun/combining.py
+-rw-rw-rw-   0        0        0    28007 2024-01-07 04:30:26.000000 meteva-1.8.3/meteva/base/fun/computing.py
+-rw-rw-rw-   0        0        0    18705 2024-03-04 12:58:48.000000 meteva-1.8.3/meteva/base/fun/diagnosing.py
+-rw-rw-rw-   0        0        0    36616 2024-04-16 10:42:41.000000 meteva-1.8.3/meteva/base/fun/grouping.py
+-rw-rw-rw-   0        0        0    34320 2024-05-16 01:49:53.000000 meteva-1.8.3/meteva/base/fun/interpolating.py
+-rw-rw-rw-   0        0        0    14417 2023-04-23 14:30:42.000000 meteva-1.8.3/meteva/base/fun/nearing.py
+-rw-rw-rw-   0        0        0    57181 2024-05-16 01:55:56.000000 meteva-1.8.3/meteva/base/fun/selecting.py
+-rw-rw-rw-   0        0        0    36232 2023-08-31 06:14:58.000000 meteva-1.8.3/meteva/base/fun/statisticing.py
+-rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.8.3/meteva/base/fun/timing.py
+-rw-rw-rw-   0        0        0     7042 2023-04-23 13:10:39.000000 meteva-1.8.3/meteva/base/fun/transformating.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.467601 meteva-1.8.3/meteva/base/io/
+-rw-rw-rw-   0        0        0    21310 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/base/io/CMADaasAccess.py
+-rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.8.3/meteva/base/io/DataBlock_pb2.py
+-rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.8.3/meteva/base/io/GDS_data_service.py
+-rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.8.3/meteva/base/io/SignGenUtil.py
+-rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.8.3/meteva/base/io/__init__.py
+-rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.8.3/meteva/base/io/clienthandler.py
+-rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.8.3/meteva/base/io/encoding.py
+-rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.8.3/meteva/base/io/ftpconn.py
+-rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.8.3/meteva/base/io/httpclient.py
+-rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.8.3/meteva/base/io/httpconn.py
+-rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.8.3/meteva/base/io/loglib.py
+-rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.8.3/meteva/base/io/print_grib_info.py
+-rw-rw-rw-   0        0        0    21041 2024-05-15 06:39:57.000000 meteva-1.8.3/meteva/base/io/read_graphydata.py
+-rw-rw-rw-   0        0        0    83559 2024-05-11 02:15:30.000000 meteva-1.8.3/meteva/base/io/read_griddata.py
+-rw-rw-rw-   0        0        0    91613 2024-02-29 15:27:44.000000 meteva-1.8.3/meteva/base/io/read_stadata.py
+-rw-rw-rw-   0        0        0     4670 2023-03-02 08:36:03.000000 meteva-1.8.3/meteva/base/io/write_array.py
+-rw-rw-rw-   0        0        0    10893 2024-02-23 08:01:29.000000 meteva-1.8.3/meteva/base/io/write_griddata.py
+-rw-rw-rw-   0        0        0    12830 2023-10-10 05:58:04.000000 meteva-1.8.3/meteva/base/io/write_stadata.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.634591 meteva-1.8.3/meteva/base/tool/
+-rw-rw-rw-   0        0        0     1265 2024-04-18 14:15:37.000000 meteva-1.8.3/meteva/base/tool/__init__.py
+-rw-rw-rw-   0        0        0    53922 2024-05-14 06:26:56.000000 meteva-1.8.3/meteva/base/tool/color_tools.py
+-rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.8.3/meteva/base/tool/copy_tools.py
+-rw-rw-rw-   0        0        0     1248 2023-04-04 14:53:16.000000 meteva-1.8.3/meteva/base/tool/frprmn2.py
+-rw-rw-rw-   0        0        0     4695 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/base/tool/grib_tools.py
+-rw-rw-rw-   0        0        0     8797 2023-07-04 02:34:53.000000 meteva-1.8.3/meteva/base/tool/maskout.py
+-rw-rw-rw-   0        0        0    11675 2023-06-20 14:47:49.000000 meteva-1.8.3/meteva/base/tool/math_tools.py
+-rw-rw-rw-   0        0        0    12484 2024-01-18 07:10:32.000000 meteva-1.8.3/meteva/base/tool/path_tools.py
+-rw-rw-rw-   0        0        0   219106 2024-05-17 01:58:38.000000 meteva-1.8.3/meteva/base/tool/plot_tools.py
+-rw-rw-rw-   0        0        0    35471 2024-05-17 02:04:01.000000 meteva-1.8.3/meteva/base/tool/plot_tools_adv.py
+-rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.8.3/meteva/base/tool/process_tools.py
+-rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.8.3/meteva/base/tool/station_tools.py
+-rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.8.3/meteva/base/tool/time_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.645594 meteva-1.8.3/meteva/method/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.382592 meteva-1.8.3/meteva/method/Vector/
+-rw-rw-rw-   0        0        0      624 2024-02-22 04:04:47.000000 meteva-1.8.3/meteva/method/Vector/__init__.py
+-rw-rw-rw-   0        0        0    33207 2024-02-22 07:27:38.000000 meteva-1.8.3/meteva/method/Vector/plot.py
+-rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.8.3/meteva/method/Vector/score.py
+-rw-rw-rw-   0        0        0      387 2024-05-14 06:22:30.000000 meteva-1.8.3/meteva/method/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.742595 meteva-1.8.3/meteva/method/continuous/
+-rw-rw-rw-   0        0        0     1128 2024-01-27 14:08:41.000000 meteva-1.8.3/meteva/method/continuous/__init__.py
+-rw-rw-rw-   0        0        0    40681 2024-05-15 06:46:14.000000 meteva-1.8.3/meteva/method/continuous/plot.py
+-rw-rw-rw-   0        0        0    54412 2024-02-22 03:32:35.000000 meteva-1.8.3/meteva/method/continuous/score.py
+-rw-rw-rw-   0        0        0     1248 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/method/continuous/skill.py
+-rw-rw-rw-   0        0        0     5417 2023-12-26 02:41:16.000000 meteva-1.8.3/meteva/method/continuous/table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.769592 meteva-1.8.3/meteva/method/ensemble/
+-rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.8.3/meteva/method/ensemble/__init__.py
+-rw-rw-rw-   0        0        0     4270 2024-05-14 06:28:10.000000 meteva-1.8.3/meteva/method/ensemble/plot.py
+-rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.8.3/meteva/method/ensemble/score.py
+-rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.8.3/meteva/method/ensemble/table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.794592 meteva-1.8.3/meteva/method/multi_category/
+-rw-rw-rw-   0        0        0      602 2024-04-04 15:25:22.000000 meteva-1.8.3/meteva/method/multi_category/__init__.py
+-rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.8.3/meteva/method/multi_category/plot.py
+-rw-rw-rw-   0        0        0    27982 2024-04-04 16:02:06.000000 meteva-1.8.3/meteva/method/multi_category/score.py
+-rw-rw-rw-   0        0        0     7803 2022-12-28 08:27:35.000000 meteva-1.8.3/meteva/method/multi_category/table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.849593 meteva-1.8.3/meteva/method/probability/
+-rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.8.3/meteva/method/probability/__init__.py
+-rw-rw-rw-   0        0        0    21553 2024-05-14 06:28:10.000000 meteva-1.8.3/meteva/method/probability/plot.py
+-rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.8.3/meteva/method/probability/score.py
+-rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.8.3/meteva/method/probability/table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.872592 meteva-1.8.3/meteva/method/space/
+-rw-rw-rw-   0        0        0      802 2024-02-21 07:49:52.000000 meteva-1.8.3/meteva/method/space/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.898640 meteva-1.8.3/meteva/method/space/acc/
+-rw-rw-rw-   0        0        0       82 2023-10-04 03:56:47.000000 meteva-1.8.3/meteva/method/space/acc/__init__.py
+-rw-rw-rw-   0        0        0    10047 2024-05-14 02:39:53.000000 meteva-1.8.3/meteva/method/space/acc/acc.py
+-rw-rw-rw-   0        0        0      747 2023-09-15 14:42:11.000000 meteva-1.8.3/meteva/method/space/acc/acc_climate_pre.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:19.911591 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/
+-rw-rw-rw-   0        0        0      134 2023-10-01 08:10:28.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.003592 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/
+-rw-rw-rw-   0        0        0      244 2023-10-01 08:15:28.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py
+-rw-rw-rw-   0        0        0      774 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0     1560 2024-02-18 07:34:44.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py
+-rw-rw-rw-   0        0        0     4594 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py
+-rw-rw-rw-   0        0        0     2530 2023-08-21 23:56:50.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0     3977 2024-02-18 07:34:44.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py
+-rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      625 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py
+-rw-rw-rw-   0        0        0     1978 2023-08-22 00:02:02.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py
+-rw-rw-rw-   0        0        0      278 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_prep.py
+-rw-rw-rw-   0        0        0     5528 2023-08-22 00:02:02.000000 meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.007601 meteva-1.8.3/meteva/method/space/cra/
+-rw-rw-rw-   0        0        0       62 2024-02-21 07:47:43.000000 meteva-1.8.3/meteva/method/space/cra/__init__.py
+-rw-rw-rw-   0        0        0     5824 2024-05-06 14:16:03.000000 meteva-1.8.3/meteva/method/space/cra/cra.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.029591 meteva-1.8.3/meteva/method/space/fqi/
+-rw-rw-rw-   0        0        0       65 2023-10-01 08:00:00.000000 meteva-1.8.3/meteva/method/space/fqi/__init__.py
+-rw-rw-rw-   0        0        0     5179 2023-09-23 11:58:12.000000 meteva-1.8.3/meteva/method/space/fqi/fqi.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.098591 meteva-1.8.3/meteva/method/space/fqi/lib/
+-rw-rw-rw-   0        0        0      366 2023-10-01 08:03:25.000000 meteva-1.8.3/meteva/method/space/fqi/lib/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-08-22 02:14:25.000000 meteva-1.8.3/meteva/method/space/fqi/lib/aaft2d.py
+-rw-rw-rw-   0        0        0      658 2023-01-29 06:47:11.000000 meteva-1.8.3/meteva/method/space/fqi/lib/ampstats.py
+-rw-rw-rw-   0        0        0       93 2023-01-24 09:38:13.000000 meteva-1.8.3/meteva/method/space/fqi/lib/cbind.py
+-rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.3/meteva/method/space/fqi/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      947 2023-04-02 10:16:53.000000 meteva-1.8.3/meteva/method/space/fqi/lib/distfun.py
+-rw-rw-rw-   0        0        0      947 2023-03-26 09:44:16.000000 meteva-1.8.3/meteva/method/space/fqi/lib/fft2d.py
+-rw-rw-rw-   0        0        0     2531 2023-08-22 02:11:26.000000 meteva-1.8.3/meteva/method/space/fqi/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/fqi/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0      278 2021-06-01 19:24:10.000000 meteva-1.8.3/meteva/method/space/fqi/lib/locmeasures2d_prep.py
+-rw-rw-rw-   0        0        0     4102 2024-02-18 12:48:31.000000 meteva-1.8.3/meteva/method/space/fqi/lib/locperf.py
+-rw-rw-rw-   0        0        0      262 2023-03-25 10:39:31.000000 meteva-1.8.3/meteva/method/space/fqi/lib/locperfer.py
+-rw-rw-rw-   0        0        0      158 2023-01-28 04:35:01.000000 meteva-1.8.3/meteva/method/space/fqi/lib/mae.py
+-rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.3/meteva/method/space/fqi/lib/solutionset.py
+-rw-rw-rw-   0        0        0     2398 2023-08-22 02:14:05.000000 meteva-1.8.3/meteva/method/space/fqi/lib/surrogater2d.py
+-rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.3/meteva/method/space/fqi/lib/util.py
+-rw-rw-rw-   0        0        0      274 2023-01-26 07:28:17.000000 meteva-1.8.3/meteva/method/space/fqi/lib/zapsmall.py
+-rw-rw-rw-   0        0        0     1008 2023-08-22 02:11:50.000000 meteva-1.8.3/meteva/method/space/fqi/uiqi.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.105591 meteva-1.8.3/meteva/method/space/fss/
+-rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.8.3/meteva/method/space/fss/__init__.py
+-rw-rw-rw-   0        0        0     8387 2023-04-22 14:53:18.000000 meteva-1.8.3/meteva/method/space/fss/fss.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.192593 meteva-1.8.3/meteva/method/space/fuzzy_logic/
+-rw-rw-rw-   0        0        0      194 2023-10-01 07:24:57.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-08-21 03:43:04.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/fss.py
+-rw-rw-rw-   0        0        0     2273 2023-09-06 03:36:58.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/fuzzy.py
+-rw-rw-rw-   0        0        0     1806 2023-09-04 07:58:00.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/joint.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.403592 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/
+-rw-rw-rw-   0        0        0      492 2023-10-01 08:15:28.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/__init__.py
+-rw-rw-rw-   0        0        0      783 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      860 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/fss2dfun.py
+-rw-rw-rw-   0        0        0     1908 2023-08-20 08:53:21.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py
+-rw-rw-rw-   0        0        0     7349 2023-09-06 09:36:29.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2d.py
+-rw-rw-rw-   0        0        0     1016 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py
+-rw-rw-rw-   0        0        0     1243 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py
+-rw-rw-rw-   0        0        0     1266 2023-09-04 08:38:48.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py
+-rw-rw-rw-   0        0        0     6283 2023-08-22 01:44:20.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     3456 2023-09-25 03:11:25.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py
+-rw-rw-rw-   0        0        0     7289 2023-08-20 13:30:27.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      188 2023-08-20 12:21:58.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/mincvg2dfun.py
+-rw-rw-rw-   0        0        0      183 2023-08-21 03:05:37.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/multicon2dfun.py
+-rw-rw-rw-   0        0        0      536 2023-09-06 03:46:36.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py
+-rw-rw-rw-   0        0        0      715 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/thresholder.py
+-rw-rw-rw-   0        0        0      811 2023-08-21 03:06:59.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py
+-rw-rw-rw-   0        0        0     4704 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/vxstats.py
+-rw-rw-rw-   0        0        0      275 2021-06-06 10:14:33.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/zapsmall.py
+-rw-rw-rw-   0        0        0     2255 2023-09-07 06:37:55.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/minimum_coverage.py
+-rw-rw-rw-   0        0        0     2233 2023-09-06 09:01:35.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/multi_event.py
+-rw-rw-rw-   0        0        0     2218 2023-09-06 03:36:58.000000 meteva-1.8.3/meteva/method/space/fuzzy_logic/pragmatic.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.412592 meteva-1.8.3/meteva/method/space/geo_box_plot/
+-rw-rw-rw-   0        0        0     2496 2023-09-25 04:29:49.000000 meteva-1.8.3/meteva/method/space/geo_box_plot/GeoBoxPlot.py
+-rw-rw-rw-   0        0        0       24 2023-10-02 02:14:48.000000 meteva-1.8.3/meteva/method/space/geo_box_plot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.461592 meteva-1.8.3/meteva/method/space/geometric_characterizations/
+-rw-rw-rw-   0        0        0       86 2023-10-01 08:16:08.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/__init__.py
+-rw-rw-rw-   0        0        0     5187 2024-02-18 08:43:27.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/aindex.py
+-rw-rw-rw-   0        0        0     2664 2023-09-24 12:12:06.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/cindex.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.473595 meteva-1.8.3/meteva/method/space/geometric_characterizations/lib/
+-rw-rw-rw-   0        0        0       55 2023-10-01 08:21:38.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/lib/__init__.py
+-rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/lib/util.py
+-rw-rw-rw-   0        0        0     2934 2023-09-24 11:40:50.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/sindex.py
+-rw-rw-rw-   0        0        0     1859 2023-08-22 00:10:29.000000 meteva-1.8.3/meteva/method/space/geometric_characterizations/spatial_index.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.476592 meteva-1.8.3/meteva/method/space/hausdorff_metric/
+-rw-rw-rw-   0        0        0       43 2023-10-01 08:17:18.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.487594 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/
+-rw-rw-rw-   0        0        0      150 2023-10-01 08:21:38.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-05-23 18:14:16.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/as_unitname.py
+-rw-rw-rw-   0        0        0      947 2023-04-02 10:14:50.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/distfun.py
+-rw-rw-rw-   0        0        0     4731 2023-04-02 10:09:41.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/distmap.py
+-rw-rw-rw-   0        0        0     2518 2023-08-22 00:16:03.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-05-23 18:14:16.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/solutionset.py
+-rw-rw-rw-   0        0        0     5361 2024-02-18 09:02:26.000000 meteva-1.8.3/meteva/method/space/hausdorff_metric/locperf.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.881632 meteva-1.8.3/meteva/method/space/mode/
+-rw-rw-rw-   0        0        0     1960 2023-08-24 01:06:15.000000 meteva-1.8.3/meteva/method/space/mode/__init__.py
+-rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.8.3/meteva/method/space/mode/angles_psp.py
+-rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.8.3/meteva/method/space/mode/as_psp.py
+-rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.8.3/meteva/method/space/mode/bearing.py
+-rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/censqdelta.py
+-rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.8.3/meteva/method/space/mode/centmatch.py
+-rw-rw-rw-   0        0        0    13874 2023-12-22 00:57:57.000000 meteva-1.8.3/meteva/method/space/mode/consistent.py
+-rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/data_pre.py
+-rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.8.3/meteva/method/space/mode/deltametric.py
+-rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/deltamm.py
+-rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/deltammSqCen.py
+-rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/deltamm_bak.py
+-rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/distmap.py
+-rw-rw-rw-   0        0        0     6070 2024-02-22 03:58:40.000000 meteva-1.8.3/meteva/method/space/mode/feature_axis.py
+-rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.8.3/meteva/method/space/mode/feature_comps.py
+-rw-rw-rw-   0        0        0    32379 2023-08-22 14:03:20.000000 meteva-1.8.3/meteva/method/space/mode/feature_finder.py
+-rw-rw-rw-   0        0        0    10157 2023-02-07 02:37:08.000000 meteva-1.8.3/meteva/method/space/mode/feature_match_analyzer.py
+-rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.8.3/meteva/method/space/mode/feature_props.py
+-rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.8.3/meteva/method/space/mode/feature_table.py
+-rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.8.3/meteva/method/space/mode/interester.py
+-rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.8.3/meteva/method/space/mode/intersect.py
+-rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.8.3/meteva/method/space/mode/lengths_psp.py
+-rw-rw-rw-   0        0        0     1358 2023-04-23 02:57:31.000000 meteva-1.8.3/meteva/method/space/mode/load.py
+-rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.8.3/meteva/method/space/mode/loc_list_setup.py
+-rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.8.3/meteva/method/space/mode/locperf.py
+-rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.8.3/meteva/method/space/mode/make_SpatialVx_bak.py
+-rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.8.3/meteva/method/space/mode/make_spatialVx.py
+-rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.8.3/meteva/method/space/mode/merge_force.py
+-rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.8.3/meteva/method/space/mode/midpoints_psp.py
+-rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.8.3/meteva/method/space/mode/minboundmatch.py
+-rw-rw-rw-   0        0        0     5727 2023-02-07 02:37:07.000000 meteva-1.8.3/meteva/method/space/mode/operater.py
+-rw-rw-rw-   0        0        0    32351 2024-05-17 02:04:01.000000 meteva-1.8.3/meteva/method/space/mode/plot.py
+-rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.8.3/meteva/method/space/mode/regress2.py
+-rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.8.3/meteva/method/space/mode/sma.py
+-rw-rw-rw-   0        0        0    10465 2023-07-27 07:47:11.000000 meteva-1.8.3/meteva/method/space/mode/tran_to_dataframe.py
+-rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.8.3/meteva/method/space/mode/utils.py
+-rw-rw-rw-   0        0        0     4595 2023-03-20 12:31:25.000000 meteva-1.8.3/meteva/method/space/point_to_area.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.902593 meteva-1.8.3/meteva/method/space/pphindcast/
+-rw-rw-rw-   0        0        0      134 2023-10-01 08:21:38.000000 meteva-1.8.3/meteva/method/space/pphindcast/__init__.py
+-rw-rw-rw-   0        0        0     6295 2023-05-12 01:24:44.000000 meteva-1.8.3/meteva/method/space/pphindcast/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     2976 2023-08-22 02:29:43.000000 meteva-1.8.3/meteva/method/space/pphindcast/kernel2dsmooth.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.917591 meteva-1.8.3/meteva/method/space/pphindcast/lib/
+-rw-rw-rw-   0        0        0      272 2023-10-01 08:21:38.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/as_unitname.py
+-rw-rw-rw-   0        0        0       86 2021-09-05 14:49:53.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/datagrabber.py
+-rw-rw-rw-   0        0        0     1081 2021-10-24 16:33:14.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/hoods2dPrep.py
+-rw-rw-rw-   0        0        0     2512 2023-08-22 00:21:36.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/im.py
+-rw-rw-rw-   0        0        0     6295 2023-05-11 14:59:50.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     2963 2023-08-22 00:21:36.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/kernel2dsmooth.py
+-rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      719 2023-01-11 13:49:43.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/thresholder.py
+-rw-rw-rw-   0        0        0     4704 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/pphindcast/lib/vxstats.py
+-rw-rw-rw-   0        0        0     6087 2023-09-24 15:02:06.000000 meteva-1.8.3/meteva/method/space/pphindcast/pphindcast2d.py
+-rw-rw-rw-   0        0        0      275 2023-05-12 01:24:46.000000 meteva-1.8.3/meteva/method/space/pphindcast/zapsmall.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:20.992592 meteva-1.8.3/meteva/method/space/rigider/
+-rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.8.3/meteva/method/space/rigider/__init__.py
+-rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.8.3/meteva/method/space/rigider/fint2d.py
+-rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.8.3/meteva/method/space/rigider/fint2d_old.py
+-rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.8.3/meteva/method/space/rigider/imomenter.py
+-rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/rigider/mij.py
+-rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/rigider/q_loss_rigid.py
+-rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.8.3/meteva/method/space/rigider/rigid_transform.py
+-rw-rw-rw-   0        0        0    14406 2024-02-21 13:04:04.000000 meteva-1.8.3/meteva/method/space/rigider/rigider.py
+-rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.8.3/meteva/method/space/rigider/zapsmall.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.009591 meteva-1.8.3/meteva/method/space/s1/
+-rw-rw-rw-   0        0        0     2234 2023-09-25 04:01:56.000000 meteva-1.8.3/meteva/method/space/s1/S1.py
+-rw-rw-rw-   0        0        0       16 2023-10-01 09:00:39.000000 meteva-1.8.3/meteva/method/space/s1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.021592 meteva-1.8.3/meteva/method/space/saller/
+-rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.8.3/meteva/method/space/saller/__init__.py
+-rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.8.3/meteva/method/space/saller/saller.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.107591 meteva-1.8.3/meteva/method/space/significance/
+-rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.8.3/meteva/method/space/significance/LocSig.py
+-rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.8.3/meteva/method/space/significance/__init__.py
+-rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.8.3/meteva/method/space/significance/bootstrap.py
+-rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.8.3/meteva/method/space/significance/bootstrap_ci.py
+-rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.8.3/meteva/method/space/significance/is_sig.py
+-rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.8.3/meteva/method/space/significance/sig_coverage.py
+-rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.8.3/meteva/method/space/significance/significance.py
+-rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.8.3/meteva/method/space/significance/spatbiasFS.py
+-rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.8.3/meteva/method/space/significance/tsboot.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.109590 meteva-1.8.3/meteva/method/space/uqi/
+-rw-rw-rw-   0        0        0       20 2023-09-22 07:51:37.000000 meteva-1.8.3/meteva/method/space/uqi/__init__.py
+-rw-rw-rw-   0        0        0      989 2023-09-22 08:31:14.000000 meteva-1.8.3/meteva/method/space/uqi/uqi.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.180592 meteva-1.8.3/meteva/method/space/vgm/
+-rw-rw-rw-   0        0        0      167 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/method/space/vgm/__init__.py
+-rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.8.3/meteva/method/space/vgm/rdist.py
+-rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.8.3/meteva/method/space/vgm/structurogram.py
+-rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.8.3/meteva/method/space/vgm/structurogram_matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.412592 meteva-1.8.3/meteva/method/weather_system/
+-rw-rw-rw-   0        0        0       25 2024-02-22 12:26:37.000000 meteva-1.8.3/meteva/method/weather_system/__init__.py
+-rw-rw-rw-   0        0        0    15304 2024-05-14 06:30:31.000000 meteva-1.8.3/meteva/method/weather_system/identify.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.495593 meteva-1.8.3/meteva/method/yes_or_no/
+-rw-rw-rw-   0        0        0      850 2023-10-02 14:10:45.000000 meteva-1.8.3/meteva/method/yes_or_no/__init__.py
+-rw-rw-rw-   0        0        0    10918 2024-05-14 06:31:28.000000 meteva-1.8.3/meteva/method/yes_or_no/plot.py
+-rw-rw-rw-   0        0        0    36054 2023-10-29 14:33:23.000000 meteva-1.8.3/meteva/method/yes_or_no/score.py
+-rw-rw-rw-   0        0        0     2995 2023-03-03 07:52:23.000000 meteva-1.8.3/meteva/method/yes_or_no/skill.py
+-rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.8.3/meteva/method/yes_or_no/table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.561592 meteva-1.8.3/meteva/perspact/
+-rw-rw-rw-   0        0        0      167 2024-03-27 01:02:36.000000 meteva-1.8.3/meteva/perspact/__init__.py
+-rw-rw-rw-   0        0        0     8009 2024-05-17 03:42:19.000000 meteva-1.8.3/meteva/perspact/middel_high.py
+-rw-rw-rw-   0        0        0    33499 2024-05-05 12:50:10.000000 meteva-1.8.3/meteva/perspact/middle_prepare.py
+-rw-rw-rw-   0        0        0    11614 2024-02-23 06:31:38.000000 meteva-1.8.3/meteva/perspact/multi_element_veri.py
+-rw-rw-rw-   0        0        0    46624 2024-05-17 00:41:49.000000 meteva-1.8.3/meteva/perspact/score.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.574595 meteva-1.8.3/meteva/product/
+-rw-rw-rw-   0        0        0      216 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.675591 meteva-1.8.3/meteva/product/application/
+-rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.8.3/meteva/product/application/__init__.py
+-rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.8.3/meteva/product/application/data_collection.py
+-rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.8.3/meteva/product/application/data_distribute.py
+-rw-rw-rw-   0        0        0    24149 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/application/data_prepare.py
+-rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.8.3/meteva/product/application/fun.py
+-rw-rw-rw-   0        0        0     2951 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/application/terrain_height_correction.py
+-rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.8.3/meteva/product/application/time_compare.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.677592 meteva-1.8.3/meteva/product/presentation/
+-rw-rw-rw-   0        0        0        0 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/presentation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:21.989680 meteva-1.8.3/meteva/product/program/
+-rw-rw-rw-   0        0        0     1247 2023-07-07 02:14:59.000000 meteva-1.8.3/meteva/product/program/__init__.py
+-rw-rw-rw-   0        0        0    19079 2023-01-13 06:11:18.000000 meteva-1.8.3/meteva/product/program/diurnal.py
+-rw-rw-rw-   0        0        0    17821 2024-05-14 06:31:56.000000 meteva-1.8.3/meteva/product/program/error_ana_list.py
+-rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.8.3/meteva/product/program/error_ana_scatter.py
+-rw-rw-rw-   0        0        0    30270 2023-11-16 01:25:36.000000 meteva-1.8.3/meteva/product/program/fun.py
+-rw-rw-rw-   0        0        0     6702 2023-10-31 00:43:33.000000 meteva-1.8.3/meteva/product/program/plot.py
+-rw-rw-rw-   0        0        0    10458 2024-05-17 02:05:20.000000 meteva-1.8.3/meteva/product/program/process_compare.py
+-rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.8.3/meteva/product/program/sample_statistic.py
+-rw-rw-rw-   0        0        0    40965 2023-12-26 03:32:01.000000 meteva-1.8.3/meteva/product/program/score.py
+-rw-rw-rw-   0        0        0   147988 2024-05-17 02:04:01.000000 meteva-1.8.3/meteva/product/program/space_compare.py
+-rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.8.3/meteva/product/program/table.py
+-rw-rw-rw-   0        0        0    63040 2024-05-14 06:32:41.000000 meteva-1.8.3/meteva/product/program/time_compare.py
+-rw-rw-rw-   0        0        0     5277 2024-05-14 06:33:14.000000 meteva-1.8.3/meteva/product/program/time_space_compare.py
+-rw-rw-rw-   0        0        0     2407 2024-01-17 14:09:44.000000 meteva-1.8.3/meteva/product/program/typhoon.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:22.039591 meteva-1.8.3/meteva/product/regulation/
+-rw-rw-rw-   0        0        0      206 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/regulation/__init__.py
+-rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.8.3/meteva/product/regulation/environment.py
+-rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.8.3/meteva/product/regulation/short_term_heavy_rainfall.py
+-rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.8.3/meteva/product/regulation/temperature.py
+-rw-rw-rw-   0        0        0    16261 2023-05-30 01:00:40.000000 meteva-1.8.3/meteva/product/regulation/thunderstrom_gale.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:15:22.061591 meteva-1.8.3/meteva.egg-info/
+-rw-rw-rw-   0        0        0      931 2024-05-17 09:15:18.000000 meteva-1.8.3/meteva.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11718 2024-05-17 09:15:18.000000 meteva-1.8.3/meteva.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:15:18.000000 meteva-1.8.3/meteva.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2024-05-17 09:15:18.000000 meteva-1.8.3/meteva.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 09:15:18.000000 meteva-1.8.3/meteva.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:15:22.064591 meteva-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     2445 2024-05-15 06:16:43.000000 meteva-1.8.3/setup.py
```

### Comparing `meteva-1.8.2/PKG-INFO` & `meteva-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.8.2
+Version: 1.8.3
 Summary: A collections of functions for meteorological verification.
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy>=1.12.1
 Requires-Dist: pandas<=2.0.3,>=1.0.4
 Requires-Dist: netCDF4<=1.6.5,>=1.4.2
 Requires-Dist: scipy>=0.19.0
-Requires-Dist: xarray<=0.20.0,>=0.10.0
+Requires-Dist: xarray>=0.10.0
 Requires-Dist: scikit-learn>=0.21.2
 Requires-Dist: matplotlib>=3.2.2
 Requires-Dist: httplib2>=0.12.0
 Requires-Dist: protobuf<=3.20.0
 Requires-Dist: pyshp>=2.1.0
 Requires-Dist: tables>=3.4.4
 Requires-Dist: urllib3>=1.21.1
```

### Comparing `meteva-1.8.2/meteva/base/basicdata/const.py` & `meteva-1.8.3/meteva/base/basicdata/const.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/basicdata/ctl.py` & `meteva-1.8.3/meteva/base/basicdata/ctl.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/basicdata/dicts.py` & `meteva-1.8.3/meteva/base/basicdata/dicts.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/basicdata/grid.py` & `meteva-1.8.3/meteva/base/basicdata/grid.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/basicdata/grid_data.py` & `meteva-1.8.3/meteva/base/basicdata/grid_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,27 +156,31 @@
 
 
     da = None
     if isinstance(xr0,xr.DataArray):
         ds0 = xr.Dataset({'data0': xr0})
     else:
         if value_name is not None:
-            da = xr0[value_name]
-            ds0 = xr.Dataset({'data0': da})
+            da_ = xr0[value_name]
+            ds0 = xr.Dataset({'data0': da_})
             name = value_name
         else:
             ds0 = xr0
 
 
     if dtime_dim == "time":
         ds0 = ds0.rename_dims({"time": "dtime"})
+        if 'time' in ds0.coords:
+            ds0 = ds0.rename({'time': 'dtime'})
         dtime_dim = "dtime"
 
     if time_dim == "dtime":
         ds0 = ds0.rename_dims({"dtime": "time"})
+        if 'dtime' in ds0.coords:
+            ds0 = ds0.rename({'dtime': 'time'})
         time_dim = "time"
 
     drop_list = []
     ds = xr.Dataset()
     # 1判断要素成员member
     if (member_dim is None):
         member_dim = "member"
@@ -322,15 +326,14 @@
         attrs_name = list(lons.attrs)
         for key in attrs_name:
             ds.lon.attrs[key] = lons.attrs[key]
     else:
         ds.coords["lon"] = ("lon", [0])
 
 
-
     if da is None:
         name_list = list((ds0))
         for name in name_list:
             if name in drop_list: continue
             #print(ds0)
             da = ds0[name]
             shape = da.values.shape
@@ -394,15 +397,14 @@
     if "lon" not in dim_order.keys():
         dim_order["lon"] = "lon"
         da = da.expand_dims("lon")
         da = da.copy()
     da = da.transpose(dim_order["member"], dim_order["level"], dim_order["time"],
                       dim_order["dtime"], dim_order["lat"], dim_order["lon"])
 
-    #print(da)
     ds[name] = (("member", "level", "time", "dtime", "lat", "lon"), da.values)
     attrs_name = list(da.attrs)
     for key in attrs_name:
         ds[name].attrs[key] = da.attrs[key]
     attrs_name = list(ds0.attrs)
     for key in attrs_name:
         ds.attrs[key] = ds0.attrs[key]
@@ -447,29 +449,30 @@
 
     attrs_name = list(da1.attrs)
     if "dtime_type" in attrs_name:
         da1.attrs["dtime_type"] = "hour"
 
     meteva.base.reset(da1)
     lats = da1.lat.values
-    dlats = lats[1:] - lats[:-1]
-    maxdlats = np.max(dlats)
-    mindlats = np.min(dlats)
-    if (maxdlats - mindlats)/maxdlats > 0.001:
-        print("***")
-        nlat = int((lats[-1] - lats[0])/mindlats) + 2
-        dlat = (lats[-1] - lats[0])/(nlat-1)
-        lons = da1.lon.values
-        dlon = (lons[-1] - lons[0])/(len(lons) - 1)
-        grid = meteva.base.grid([lons[0],lons[-1],dlon],[lats[0],lats[-1],dlat])
-        try:
-            da1 = meteva.base.interp_xg_linear(da1,grid)
-        except:
-            #如果不能重置网格就还是返回原来的网格数据
-            pass
+    lons = da1.lon.values
+    if len(lats)>1 and len(lons)>1:
+        dlats = lats[1:] - lats[:-1]
+        maxdlats = np.max(dlats)
+        mindlats = np.min(dlats)
+        if (maxdlats - mindlats)/maxdlats > 0.001:
+            print("***")
+            nlat = int((lats[-1] - lats[0])/mindlats) + 2
+            dlat = (lats[-1] - lats[0])/(nlat-1)
+            dlon = (lons[-1] - lons[0])/(len(lons) - 1)
+            grid = meteva.base.grid([lons[0],lons[-1],dlon],[lats[0],lats[-1],dlat])
+            try:
+                da1 = meteva.base.interp_xg_linear(da1,grid)
+            except:
+                #如果不能重置网格就还是返回原来的网格数据
+                pass
 
     return da1
 
 
 def xarray_to_griddata_bak(xr0,
                        value_name=None, member_dim=None, level_dim=None, time_dim=None, dtime_dim=None, lat_dim=None,
                        lon_dim=None
@@ -882,26 +885,28 @@
     return da
 
 
 
 
 def reset(grd):
     lats = grd["lat"].values
-    if lats[0]>lats[1]:
-        lats = grd["lat"].values[::-1]
-        grd['lat'] = lats
-        dat = grd.values[:, :, :, :, ::-1, :]
-        grd.values = dat
+    if len(lats)>1:
+        if lats[0]>lats[1]:
+            lats = grd["lat"].values[::-1]
+            grd['lat'] = lats
+            dat = grd.values[:, :, :, :, ::-1, :]
+            grd.values = dat
 
     lons = grd["lon"].values
-    if lons[0]>lons[1]:
-        lons = grd["lon"].values[::-1]
-        grd['lon'] = lons
-        dat = grd.values[:, :, :, :, :, ::-1]
-        grd.values = dat
+    if len(lons)>1:
+        if lons[0]>lons[1]:
+            lons = grd["lon"].values[::-1]
+            grd['lon'] = lons
+            dat = grd.values[:, :, :, :, :, ::-1]
+            grd.values = dat
 
     return
 
 
 def set_griddata_attrs(grd, dtime_units = None,data_source = None,level_type =None,
              var_name = None,var_cn_name = None,
              var_units = None,valid_time = None,data_start_columns = None):
```

### Comparing `meteva-1.8.2/meteva/base/basicdata/keys.py` & `meteva-1.8.3/meteva/base/basicdata/keys.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/basicdata/sta_data.py` & `meteva-1.8.3/meteva/base/basicdata/sta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     :param data_name: 要素名
     :return:  站点数据
     '''
     if time is not None:
         time1 = meteva.base.all_type_time_to_time64(time)
         sta.loc[:,'time'] = time1
         if len(sta.index) ==1:
-            sta["time"] = sta["time"].astype(np.datetime64)
+            sta["time"] = sta["time"].astype('datetime64[ns]')
     if dtime is not None:
         sta.loc[:,'dtime'] = dtime
         dtime_type = str(sta["dtime"].dtype)
         if dtime_type.find("int") < 0:
             sta[["dtime"]] = sta[['dtime']].astype(int)
     if level is not None:
         sta.loc[:,'level'] = level
```

### Comparing `meteva-1.8.2/meteva/base/fun/__init__.py` & `meteva-1.8.3/meteva/base/fun/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/combining.py` & `meteva-1.8.3/meteva/base/fun/combining.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/computing.py` & `meteva-1.8.3/meteva/base/fun/computing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/diagnosing.py` & `meteva-1.8.3/meteva/base/fun/diagnosing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/grouping.py` & `meteva-1.8.3/meteva/base/fun/grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 if isinstance(group_list,list):
                     group_list_list0.append(group_list)
                 else:
                     group_list_list0.append([group_list])
             group_list_list = group_list_list0
         valid_group = ["level","time","time_range","year","month","day","dayofyear","hour","xun",
                        "ob_time","ob_time_range","ob_year","ob_month","ob_day","ob_dayofyear","ob_hour",
-                       "dtime","dtime_range","dday","dhour","id","lon_range","lon_step","lat_range","lat_step","last_range","last_step","grid",
+                       "dtime","dtime_range","dday","dhour","id","lon","lon_range","lon_step","lat","lat_range","lat_step","last_range","last_step","grid",
                        "province_name","member","ob_day_hour","ob_year_month","day_hour","year_month"]
 
         data_names = meteva.base.get_stadata_names(sta_ob_and_fos)
 
         data_names_range = []
         for data_name in data_names:
             data_names_range.append(str(data_name) + "_range")
@@ -506,14 +506,40 @@
                     sta_ob_and_fos_list.append(grouped_dict[key])
             else:
                 for group_list in group_list_list:
                     sta = meteva.base.in_id_list(sta_ob_and_fos,group_list)
                     if len(sta.index) !=0:
                         valid_group_list_list.append(group_list)
                         sta_ob_and_fos_list.append(sta)
+        elif g =="lon":
+            if group_list_list is None:
+                grouped_dict = dict(list(sta_ob_and_fos.groupby(g)))
+                keys = grouped_dict.keys()
+                for key in keys:
+                    valid_group_list_list.append([key])
+                    sta_ob_and_fos_list.append(grouped_dict[key])
+            else:
+                for group_list in group_list_list:
+                    sta = meteva.base.in_lon_list(sta_ob_and_fos,group_list)
+                    if len(sta.index) !=0:
+                        valid_group_list_list.append(group_list)
+                        sta_ob_and_fos_list.append(sta)
+        elif g =="lat":
+            if group_list_list is None:
+                grouped_dict = dict(list(sta_ob_and_fos.groupby(g)))
+                keys = grouped_dict.keys()
+                for key in keys:
+                    valid_group_list_list.append([key])
+                    sta_ob_and_fos_list.append(grouped_dict[key])
+            else:
+                for group_list in group_list_list:
+                    sta = meteva.base.in_lat_list(sta_ob_and_fos,group_list)
+                    if len(sta.index) !=0:
+                        valid_group_list_list.append(group_list)
+                        sta_ob_and_fos_list.append(sta)
 
         elif g == "lon_range":
             if group_list_list is None:
                 print("当group_by = lon_range时 group_list_list 参数不能为None")
             else:
                 for group_list in group_list_list:
                     sta = meteva.base.between_lon_range(sta_ob_and_fos,group_list[0],group_list[1])
```

### Comparing `meteva-1.8.2/meteva/base/fun/interpolating.py` & `meteva-1.8.3/meteva/base/fun/interpolating.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,22 +731,7 @@
     elif (n == 0):
         return (dx + 1) * (dx - 1) * (dx - 2) / 2
     elif (n == 1):
         return -(dx + 1) * dx * (dx - 2) / 2
     else:
         return (dx + 1) * dx * (dx - 1) / 6
 
-
-
-if __name__ == "__main__":
-    import datetime
-    import pandas as pd
-    dict1 = {"level":[0],"time":[datetime.datetime(2023,1,1,8)],
-             "dtime":[0],"id":[1],"lon":[110],"lat":[30],"data0":[2]}
-    df = pd.DataFrame(dict1)
-    sta = meteva.base.sta_data(df)
-    print(sta)
-    grid1 = meteva.base.grid([0,180,1],[0,80,1])
-    grd = meteva.base.grid_data(grid1)
-    sta1 = meteva.base.sele_by_para(sta,id = 1)
-    sta_ = interp_gs_linear(grd,sta1)
-    print(sta_)
```

### Comparing `meteva-1.8.2/meteva/base/fun/nearing.py` & `meteva-1.8.3/meteva/base/fun/nearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/selecting.py` & `meteva-1.8.3/meteva/base/fun/selecting.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,26 @@
 def in_id_list(sta,id_list):
     if not isinstance(id_list,list) and not isinstance(id_list,np.ndarray):
         id_list = [id_list]
     sta1 = sta.loc[sta['id'].isin(id_list)]
     return sta1
 
 
+def in_lon_list(sta,lon_list):
+    if not isinstance(lon_list,list) and not isinstance(lon_list,np.ndarray):
+        lon_list = [lon_list]
+    sta1 = sta.loc[sta['lon'].isin(lon_list)]
+    return sta1
+
+def in_lat_list(sta,lat_list):
+    if not isinstance(lat_list,list) and not isinstance(lat_list,np.ndarray):
+        lat_list = [lat_list]
+    sta1 = sta.loc[sta['lat'].isin(lat_list)]
+    return sta1
+
 #为拥有多time层的站点数据，依次增加time层所表示的list列表
 
 #为拥有多time层的站点数据，依次增加time层所表示的list列表
 def in_time_list(data,time_list):
 
     if not isinstance(time_list,list) and not isinstance(time_list,np.ndarray):
         time_list = [time_list]
@@ -936,15 +948,15 @@
         data_names = meteva.base.get_stadata_names(data)
         p_set.extend(data_names)
         data_names_range = []
         for data_name in data_names:
             data_names_range.append(str(data_name)+"_range")
         p_set.extend(data_names_range)
         for key in s.keys():
-            if key in data_names:
+            if key in data_names and key not in ["lon","lat"]:                 #lon,lat 默认表示取值范围，而不是具体的值
                 value_one = s[key]
                 if not isinstance(value_one,list):
                     value_one = [value_one]
                 sta1 = in_one_column_value_list(sta1,key, value_one)
             elif key in data_names_range:
                 value_one = s[key]
                 data_name = key[0:-6]
@@ -1232,19 +1244,26 @@
         sta1 = between_dtime_range(sta1, dtime_range[0],dtime_range[1])
     if dday is not None:
         sta1 = in_dday_list(sta1,dday)
     if dhour is not None:
         sta1 = in_dhour_list(sta1,dhour)
     if lon is not None:
         if not isinstance(lon,list):
-            print("lon参数需为列表形式的包含起始经度（浮点数）和结束经度（浮点）的参数")
+            lon = [lon - 1e-6, lon + 1e-6]
+        elif len(lon)==1:
+            lon = [lon[0]-1e-6,lon[0]+1e-6]
+
+            #print("lon参数需为列表形式的包含起始经度（浮点数）和结束经度（浮点）的参数")
         sta1 = between_lon_range(sta1,lon[0],lon[1])
     if lat is not None:
         if not isinstance(lat,list):
-            print("lat参数需为列表形式的包含起始纬度（浮点数）和结束纬度（浮点）的参数")
+            lat = [lat - 1e-6, lat + 1e-6]
+        elif len(lat) == 1:
+            lat = [lat[0] - 1e-6, lat[0] + 1e-6]
+            #print("lat参数需为列表形式的包含起始纬度（浮点数）和结束纬度（浮点）的参数")
         sta1 = between_lat_range(sta1,lat[0],lat[1])
 
 
     if id is not None:
         sta1 = in_id_list(sta1,id)
     if grid is not None:
         sta1 = in_grid(sta1,grid)
```

### Comparing `meteva-1.8.2/meteva/base/fun/statisticing.py` & `meteva-1.8.3/meteva/base/fun/statisticing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/timing.py` & `meteva-1.8.3/meteva/base/fun/timing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/fun/transformating.py` & `meteva-1.8.3/meteva/base/fun/transformating.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/CMADaasAccess.py` & `meteva-1.8.3/meteva/base/io/CMADaasAccess.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/DataBlock_pb2.py` & `meteva-1.8.3/meteva/base/io/DataBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/GDS_data_service.py` & `meteva-1.8.3/meteva/base/io/GDS_data_service.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/SignGenUtil.py` & `meteva-1.8.3/meteva/base/io/SignGenUtil.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/clienthandler.py` & `meteva-1.8.3/meteva/base/io/clienthandler.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/encoding.py` & `meteva-1.8.3/meteva/base/io/encoding.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/ftpconn.py` & `meteva-1.8.3/meteva/base/io/ftpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/httpclient.py` & `meteva-1.8.3/meteva/base/io/httpclient.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/httpconn.py` & `meteva-1.8.3/meteva/base/io/httpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/loglib.py` & `meteva-1.8.3/meteva/base/io/loglib.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/print_grib_info.py` & `meteva-1.8.3/meteva/base/io/print_grib_info.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/read_graphydata.py` & `meteva-1.8.3/meteva/base/io/read_graphydata.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             for _ in range(number):
                 # symbol code
                 code = int(txt[idx])
                 symbol_code.append(code)
                 idx += 1
 
                 # symbol xyz
-                xyz = np.array(txt[idx:(idx + 3)]).astype(np.float)
+                xyz = np.array(txt[idx:(idx + 3)]).astype(np.float32)
                 symbol_xyz.append(xyz)
                 idx += 3
 
                 # symbol value
                 value = txt[idx]
                 symbol_value.append(value)
                 idx += 1
@@ -231,15 +231,15 @@
 
                 # line xyz point number
                 xyz_num = int(txt[idx])
                 cn_xyz_num.append(xyz_num)
                 idx += 1
 
                 # line xyz
-                xyz = np.array(txt[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                xyz = np.array(txt[idx:(idx + 3 * xyz_num)]).astype(np.float32)
                 xyz.shape = [xyz_num, 3]
                 cn_xyz.append(xyz)
                 idx += 3 * xyz_num
 
                 # line label
                 label = txt[idx]
                 cn_label.append(label)
@@ -249,15 +249,15 @@
                 label_num = int(txt[idx])
                 cn_label_num.append(label_num)
                 idx += 1
 
                 # label xyz
                 if label_num > 0:
                     label_xyz = np.array(
-                        txt[idx:(idx + 3 * label_num)]).astype(np.float)
+                        txt[idx:(idx + 3 * label_num)]).astype(np.float32)
                     label_xyz.shape = [3, label_num]
                     cn_label_xyz.append(label_xyz)
                     idx += label_num * 3
                 else:
                     cn_label_xyz.append([])
 
             closed_contours = {
@@ -449,15 +449,15 @@
             for _ in range(number):
                 # code
                 code = int(txt[idx])
                 nsymbol_code.append(code)
                 idx += 1
 
                 # xyz
-                xyz = np.array(txt[idx:(idx + 3)]).astype(np.float)
+                xyz = np.array(txt[idx:(idx + 3)]).astype(np.float32)
                 nsymbol_xyz.append([xyz])
                 idx += 3
 
                 # character length
                 char_len = int(txt[idx])
                 nsymbol_charLen.append(char_len)
                 idx += 1
@@ -489,15 +489,15 @@
 
                 # font type
                 font_type = txt[idx]
                 nsymbol_fontType.append(font_type)
                 idx += 1
 
                 # color
-                color = np.array(txt[idx:(idx + 4)]).astype(np.int)
+                color = np.array(txt[idx:(idx + 4)]).astype(np.int32)
                 nsymbol_color.append(color)
                 idx += 4
 
             notes_symbol = {
                 "nsymbol_code": nsymbol_code,
                 "nsymbol_xyz": nsymbol_xyz,
                 "nsymbol_charLen": nsymbol_charLen,
```

### Comparing `meteva-1.8.2/meteva/base/io/read_griddata.py` & `meteva-1.8.3/meteva/base/io/read_griddata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1596,62 +1596,109 @@
             if data_name is not None:
                 meteva.base.set_griddata_coords(grd, member_list=[data_name])
             if dtime_start != 0:
                 grd = meteva.base.move_fo_time(grd, -dtime_start)
             return grd
 
         else:
-            grid0 = meteva.base.grid(ctl["glon"],ctl["glat"])
+            grid0 = meteva.base.grid(ctl["glon"], ctl["glat"])
             blocksize_xy = grid0.nlon * grid0.nlat * 4
 
             data_list = []
-            blocksize_one_time = ctl["cumulate_levels"] *blocksize_xy
+            blocksize_one_time = ctl["cumulate_levels"] * blocksize_xy
+
             nlevel = ctl["vars"][value_index]["nlevel"]
+            index_level = []
+            levels_all = ctl["zdef"]
+
+            if level is not None:
+                if nlevel == 1:
+                    # 如果level参数和数据文件里面正好都是一层，就认为level是用来设置层次参数的
+                    if isinstance(level, list):
+                        if len(level) > 1:
+                            print("value " + value_name + " has only one level")
+                            return None
+                    valid_levels = level
+                    index_level = [0]
+                else:
+                    # 需要读取的层次列表
+                    need_levels = []
+                    if isinstance(level, list):
+                        need_levels = level
+                    else:
+                        need_levels = [level]
+                    valid_levels = []
+
+                    index_level_dict = {}
+                    for index1 in range(nlevel):
+                        level1 = ctl["zdef"][index1]
+                        index_level_dict[level1] = index1
+                    for level1 in need_levels:
+                        if level1 not in index_level_dict.keys():
+                            print(str(level1) + " not in zdef list")
+                        else:
+                            index_level.append(index_level_dict[level1])
+                            valid_levels.append(level1)
+
+            else:
+                if nlevel == 1:  # 只有一层的变量
+                    valid_levels = [levels_all[0]]
+                    index_level = [0]
+                else:
+                    # 有多层的变量，level参数为None时，读取全部层次
+                    valid_levels = levels_all
+                    index_level = np.arange(nlevel).tolist()
+
+            nlevel_valid = len(index_level)
+            if nlevel_valid == 0:
+                return None
             for nn in range(ctl["nensemble"]):
                 for t in range(ctl["ntime"]):
-                    start_index =blocksize_one_time *ctl["ntime"] * nn +  t * blocksize_one_time + ctl["vars"][value_index][
-                        "start_bolck_index"] * blocksize_xy
-                    position = file.seek(start_index)
-                    blocksize_one_value = blocksize_xy * nlevel
-                    content = file.read(blocksize_one_value)
-                    data1 = np.frombuffer(content, dtype=endian + "f")
-                    data_list.append(data1)
+                    start_index = blocksize_one_time * ctl["ntime"] * nn + t * blocksize_one_time + \
+                                  ctl["vars"][value_index][
+                                      "start_bolck_index"] * blocksize_xy
+                    for v in range(nlevel_valid):
+                        index1 = index_level[v]
+                        start_index1 = start_index + index1 * blocksize_xy
+                        position = file.seek(start_index1)
+                        blocksize_one_value = blocksize_xy
+                        content = file.read(blocksize_one_value)
+                        data1 = np.frombuffer(content, dtype=endian + "f")
+                        data_list.append(data1)
 
             data = np.array(data_list)
-            data = data.reshape(ctl["nensemble"], ctl["ntime"], nlevel, ctl["nlat"], ctl["nlon"])
-            data = data.transpose(0,2,1,3,4)
-            if nlevel != len(ctl["zdef"]):
-                level_list = np.arange(ctl["vars"][value_index]["nlevel"])
-            else:
-                level_list =ctl["zdef"]
+            data = data.reshape(ctl["nensemble"], ctl["ntime"], nlevel_valid, ctl["nlat"], ctl["nlon"])
+            data = data.transpose(0, 2, 1, 3, 4)
 
             if dtime_dim is None:
-                grid1 = meteva.base.grid(ctl["glon"],ctl["glat"],gtime=ctl["gtime"],dtime_list=[0],level_list=level_list,member_list=ctl["edef"])
+                grid1 = meteva.base.grid(ctl["glon"], ctl["glat"], gtime=ctl["gtime"], dtime_list=[0],
+                                         level_list=valid_levels, member_list=ctl["edef"])
             else:
 
-                grid1 = meteva.base.grid(ctl["glon"], ctl["glat"], gtime=[ctl["gtime"][0]], dtime_list=ctl["dtime_list"] ,
-                                         level_list=level_list, member_list=ctl["edef"])
+                grid1 = meteva.base.grid(ctl["glon"], ctl["glat"], gtime=[ctl["gtime"][0]],
+                                         dtime_list=ctl["dtime_list"],
+                                         level_list=valid_levels, member_list=ctl["edef"])
 
-            #print(grid1)
-            grd_one_var = meteva.base.grid_data(grid1,data)
+            # print(grid1)
+            grd_one_var = meteva.base.grid_data(grid1, data)
             if grid is not None:
-                grd_one_var = meteva.base.interp_gg_linear(grd_one_var,grid=grid,outer_value=outer_value)
+                grd_one_var = meteva.base.interp_gg_linear(grd_one_var, grid=grid, outer_value=outer_value)
             if data_name is not None:
                 meteva.base.set_griddata_coords(grd_one_var, member_list=[data_name])
             file.close()
             grd_one_var.attrs["dtime_units"] = dtime_units
             if dtime_start != 0:
                 grd_one_var = meteva.base.move_fo_time(grd_one_var, -dtime_start)
             return grd_one_var
     except:
         if show:
             exstr = traceback.format_exc()
             print(exstr)
 
-        print(ctl_path + "数据读取错误")
+        print(ctl_path + " read failed")
         return None
 
 
 def decode_griddata_from_swan_d131_byteArray(byteArray,grid = None,level = None,time = None,dtime = 0,data_name = "data0",scale_type=0,outer_value = None):
     head_dtype_raw = [
         ('ZonName', 'S12'),
         ('DataName', 'S38'),
```

### Comparing `meteva-1.8.2/meteva/base/io/read_stadata.py` & `meteva-1.8.3/meteva/base/io/read_stadata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/write_array.py` & `meteva-1.8.3/meteva/base/io/write_array.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/write_griddata.py` & `meteva-1.8.3/meteva/base/io/write_griddata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/io/write_stadata.py` & `meteva-1.8.3/meteva/base/io/write_stadata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/__init__.py` & `meteva-1.8.3/meteva/base/tool/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from .time_tools import all_type_timedelta_to_timedelta64,all_type_timedelta_to_timedelta
 from .grib_tools import grib_to_nc
 from .station_tools import get_station_id_name_dict,station_id_name_dict,station_name_id_dict,find_station_id_by_city_name,get_station_format_province_set
 from .process_tools import multi_run
 from .plot_tools import contourf_2d_grid,pcolormesh_2d_grid,scatter_sta,bar,plot,mesh,set_customized_shpfile_list,add_scatter,bar_line,myheatmap,contourf,barbs_grid_wind
 from .color_tools import cmaps,def_cmap_clevs,merge_cmap_clevs,get_seprated_rgb_method1,get_seprated_rgb_method2,set_plot_color_dict_method0,set_plot_color_dict_method1,set_plot_color_dict_method2
 from .maskout import *
-from .plot_tools_adv import *
+from .plot_tools_adv import *
+from .plot_tools import contourf_xz,contourf_yz
```

### Comparing `meteva-1.8.2/meteva/base/tool/color_tools.py` & `meteva-1.8.3/meteva/base/tool/color_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+import meteva
 import numpy as np
 import matplotlib
 import matplotlib.image as image
 from matplotlib import cm
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import matplotlib.colors as colors
 import pkg_resources
 import math
 import os
 import colorsys
-import meteva
+
 
 def clev_cmap_temper_2m_k():
     path = pkg_resources.resource_filename('meteva', "resources/colormaps/color_temp_2m.txt")
     cmap,clevs =  get_cmap_and_clevs_from_file(path)
     clevs += 273.15
     print("不再推荐使用该函数，推荐使用meb.def_cmap_clevs相应功能,请参考color工具中相关说明")
     return clevs,cmap
@@ -434,26 +433,26 @@
     elif r >= 7:
         inte = inte * 8
 
     inte = inte/2
 
     vmin = inte * ((int)(vmin / inte) - 1)
     vmax = inte * ((int)(vmax / inte) + 2)
-    max_abs_h = math.ceil(max(abs(vmax),abs(vmin)))/2
+    max_abs_h = inte * math.ceil(max(abs(vmax),abs(vmin))/inte)/2
     clevs = []
     colors_list = []
 
     for i in np.arange(vmin,0,inte).tolist():
         clevs.append(i)
         if i <= -max_abs_h:
             rgb = [0,0,(i - vmin)/max_abs_h]
         else:
             rgb = [1+ i/max_abs_h,1+ i/max_abs_h,1]
         #print(rgb)
-        if i>=-inte:
+        if i>=-inte*1.5:
             rgb= [1,1,1]
         colors_list.append(rgb)
 
     for i in np.arange(0,vmax,inte).tolist():
         clevs.append(i)
         if i <= max_abs_h:
             rgb = [1,1- i/max_abs,1- i/max_abs]
```

### Comparing `meteva-1.8.2/meteva/base/tool/copy_tools.py` & `meteva-1.8.3/meteva/base/tool/copy_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/frprmn2.py` & `meteva-1.8.3/meteva/base/tool/frprmn2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/grib_tools.py` & `meteva-1.8.3/meteva/base/tool/grib_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/maskout.py` & `meteva-1.8.3/meteva/base/tool/maskout.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/math_tools.py` & `meteva-1.8.3/meteva/base/tool/math_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/path_tools.py` & `meteva-1.8.3/meteva/base/tool/path_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/plot_tools.py` & `meteva-1.8.3/meteva/base/tool/plot_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import numpy as np
 import pkg_resources
+import meteva
 import matplotlib
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import math
 from matplotlib.colors import BoundaryNorm
 from meteva.base import IV
-import meteva
+
 from matplotlib.collections import LineCollection
 import matplotlib.patches as patches
 import datetime
 import copy
 
 def get_isoline_set(grd):
     values = grd.values
@@ -201,14 +200,192 @@
                 shp1 = readshapefile(shpfile, default_encoding=encoding)
                 lines = LineCollection(shp1, antialiaseds=(1,), zorder=zorder)
                 lines.set_color(edgecolor)
                 lines.set_linewidth(lw)
                 lines.set_label('_nolabel_')
                 ax.add_collection(lines)
 
+def contourf_xz(grd,subplot = "member",sup_title = None,title = None,save_path = None,**kwargs):
+
+    lats = grd["lat"].values
+    if lats.size>1:
+        print("size of latitude coords in griddata is bigger than one, plot failed,if you want to plot, transform gridata to have one one latitude")
+        return
+
+    split = ["member", "time", "dtime"]
+    if subplot is not None:
+        subplot = [subplot]
+        for s in subplot:
+            split.remove(s)
+    grd_list = meteva.base.split_grd(grd, used_coords=split)
+    for i in range(len(grd_list)):
+        grd1 = grd_list[i]
+        if sup_title is None:
+            data_name = grd1["member"].values[0]
+
+            if isinstance(grd1["time"].values[0],np.datetime64):
+                time_str = meteva.base.tool.time_tools.all_type_time_to_str(grd1["time"].values[0])
+                dati_str = time_str[0:4] + "年" + time_str[4:6] + "月" + time_str[6:8] + "日" + time_str[8:10] + "时"
+            else:
+                dati_str = ""
+            dtime_str = str(int(grd1["dtime"].values[0]))
+            if subplot == ["time"]:
+                sup_title1 = data_name +  "_" + dtime_str + "H时效"
+            elif subplot == ["dtime"]:
+                sup_title1 = data_name +  "_" + dati_str
+            elif subplot == ["member"]:
+                sup_title1 =  dati_str +"_"+ dtime_str + "H时效"
+            else:
+                sup_title1 = None
+        else:
+            if isinstance(sup_title, list):
+                sup_title1 = sup_title[i]
+            else:
+                sup_title1 = sup_title
+
+        if subplot is None:
+            grd_list1 = [grd1]
+        else:
+            grd_list1 = meteva.base.split_grd(grd1, used_coords=subplot)
+
+        len1 = len(grd_list1)
+        if title is not None:
+            if isinstance(title, list):
+                title1 = title[i * len1:i * len1 + len1]
+            else:
+                title1 = title
+        else:
+            if subplot is not None:
+                grd_list1 = meteva.base.split_grd(grd1, used_coords=subplot)
+            else:
+                grd_list1 = [grd1]
+            ng = len(grd_list1)
+            title1 = []
+            for kk in range(len(grd_list1)):
+                grd2 = grd_list1[kk]
+
+                data_name = grd2["member"].values[0]
+
+                if isinstance(grd2["time"].values[0], np.datetime64):
+                    time_str = meteva.base.tool.time_tools.all_type_time_to_str(grd2["time"].values[0])
+                    dati_str = time_str[0:4] + "年" + time_str[4:6] + "月" + time_str[6:8] + "日" + time_str[8:10] + "时"
+                else:
+                    dati_str = ""
+                dtime_str = str(int(grd2["dtime"].values[0]))
+                if subplot == ["time"]:
+                    title00 = dati_str
+                elif subplot == ["dtime"]:
+                    title00 = dtime_str + "H时效 "
+                elif subplot == ["member"]:
+                    title00 = data_name
+                else:
+                    title00 = data_name + "_" + dati_str + "_" + dtime_str + "H时效"
+                title1.append(title00)
+
+        data_array = grd1.values.squeeze()
+        name_list_dict = {}
+        for coords in ["member","level","time","dtime","lon","lat"]:
+            values = grd1[coords].values
+            if values.size>1:
+                name_list_dict[coords] = values
+
+        mesh_contour("contour",data_array,name_list_dict,axis_x="lon",axis_y="level",save_path = save_path,
+                     sup_title = sup_title1,
+        title= title1,**kwargs)
+
+
+def contourf_yz(grd,subplot = "member",sup_title = None,title = None,save_path = None,**kwargs):
+
+    lons = grd["lon"].values
+    if lons.size>1:
+        print("size of longitude coords in griddata is bigger than one, plot failed,if you want to plot, transform gridata to have one one longitude")
+        return
+
+    split = ["member", "time", "dtime"]
+    if subplot is not None:
+        subplot = [subplot]
+        for s in subplot:
+            split.remove(s)
+    grd_list = meteva.base.split_grd(grd, used_coords=split)
+    for i in range(len(grd_list)):
+        grd1 = grd_list[i]
+        if sup_title is None:
+            data_name = grd1["member"].values[0]
+
+            if isinstance(grd1["time"].values[0],np.datetime64):
+                time_str = meteva.base.tool.time_tools.all_type_time_to_str(grd1["time"].values[0])
+                dati_str = time_str[0:4] + "年" + time_str[4:6] + "月" + time_str[6:8] + "日" + time_str[8:10] + "时"
+            else:
+                dati_str = ""
+            dtime_str = str(int(grd1["dtime"].values[0]))
+            if subplot == ["time"]:
+                sup_title1 = data_name +  "_" + dtime_str + "H时效"
+            elif subplot == ["dtime"]:
+                sup_title1 = data_name +  "_" + dati_str
+            elif subplot == ["member"]:
+                sup_title1 =  dati_str +"_"+ dtime_str + "H时效"
+            else:
+                sup_title1 = None
+        else:
+            if isinstance(sup_title, list):
+                sup_title1 = sup_title[i]
+            else:
+                sup_title1 = sup_title
+
+        if subplot is None:
+            grd_list1 = [grd1]
+        else:
+            grd_list1 = meteva.base.split_grd(grd1, used_coords=subplot)
+
+        len1 = len(grd_list1)
+        if title is not None:
+            if isinstance(title, list):
+                title1 = title[i * len1:i * len1 + len1]
+            else:
+                title1 = title
+        else:
+            if subplot is not None:
+                grd_list1 = meteva.base.split_grd(grd1, used_coords=subplot)
+            else:
+                grd_list1 = [grd1]
+            ng = len(grd_list1)
+            title1 = []
+            for kk in range(len(grd_list1)):
+                grd2 = grd_list1[kk]
+
+                data_name = grd2["member"].values[0]
+
+                if isinstance(grd2["time"].values[0], np.datetime64):
+                    time_str = meteva.base.tool.time_tools.all_type_time_to_str(grd2["time"].values[0])
+                    dati_str = time_str[0:4] + "年" + time_str[4:6] + "月" + time_str[6:8] + "日" + time_str[8:10] + "时"
+                else:
+                    dati_str = ""
+                dtime_str = str(int(grd2["dtime"].values[0]))
+                if subplot == ["time"]:
+                    title00 = dati_str
+                elif subplot == ["dtime"]:
+                    title00 = dtime_str + "H时效 "
+                elif subplot == ["member"]:
+                    title00 = data_name
+                else:
+                    title00 = data_name + "_" + dati_str + "_" + dtime_str + "H时效"
+                title1.append(title00)
+
+        data_array = grd1.values.squeeze()
+        name_list_dict = {}
+        for coords in ["member","level","time","dtime","lon","lat"]:
+            values = grd1[coords].values
+            if values.size>1:
+                name_list_dict[coords] = values
+
+        mesh_contour("contour",data_array,name_list_dict,axis_x="lat",axis_y="level",save_path = save_path,
+                     sup_title = sup_title1,
+        title= title1,**kwargs)
+
+
 
 def contourf(grd,save_path = None,title = None,clevs= None,cmap ="rainbow",add_county_line = False,add_worldmap =False,show = False,dpi = 300,
                      sup_fontsize = 10,height = None,width = None,subplot = None,ncol = None,sup_title = None,clip= None,add_minmap= None):
     contourf_2d_grid(grd,save_path = save_path,title = title,clevs= clevs,cmap =cmap,add_county_line = add_county_line,
                      add_worldmap =add_worldmap,show = show,dpi = dpi,
                      sup_fontsize = sup_fontsize,height = height,width = width,subplot = subplot,ncol = ncol,
                      sup_title = sup_title,clip= clip,add_minmap= add_minmap)
@@ -505,25 +682,25 @@
         ax.set_ylim((slat, elat))
 
 
 
         knext_row = pi + (pj + 1) * ncol
         if knext_row >= nplot:
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8)#, family='Times New Roman')
         else:
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8)#, family='Times New Roman')
 
         if pi ==0:
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8)#, family='Times New Roman')
         else:
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8)#, family='Times New Roman')
         if type == "contour":
 
             #im = ax.contourf(x, y, np.squeeze(grd_list[p].values), levels=clevs1, cmap=cmap1, norm=norm)
             im = ax.contourf(x, y, np.squeeze(grd_list[p].values), levels=clevs1, cmap=cmap1, norm=norm, extend = extend)
             if clip is not None:
                 try:
                     meteva.base.tool.maskout.shp2clip_by_shpfile(im, ax, clip)
@@ -695,15 +872,15 @@
     for x in range(len(xticks)):
         xticks_label.append(str(round(xticks[x],6)))
     if xticks[-1] >0:
         xticks_label[-1] ="   " +xticks_label[-1] + "°E"
     else:
         xticks_label[-1] ="   " +xticks_label[-1] + "°W"
     ax.set_xticks(xticks)
-    ax.set_xticklabels(xticks_label,fontsize = sup_fontsize * 0.9, family='Times New Roman')
+    ax.set_xticklabels(xticks_label,fontsize = sup_fontsize * 0.9) #, family='Times New Roman')
 
     vmax = y[-1]
     vmin = y[0]
     r = rlat
     if r <= 1:
         inte = 0.1
     elif r <= 5 and r > 1:
@@ -723,15 +900,15 @@
     yticks_label = []
     for y in range(len(yticks)):
         if yticks[y] >= 0:
             yticks_label.append(str(round(yticks[y],6))+"°N")
         else:
             yticks_label.append(str(round(-yticks[y], 6)) +"°S")
     ax.set_yticks(yticks)
-    ax.set_yticklabels(yticks_label,fontsize = sup_fontsize * 0.9, family='Times New Roman')
+    ax.set_yticklabels(yticks_label,fontsize = sup_fontsize * 0.9) #, family='Times New Roman')
 
 
     if(save_path is not None):
         file1,extension = os.path.splitext(save_path)
         extension = extension[1:]
         plt.savefig(save_path,format = extension,bbox_inches='tight')
     else:
@@ -1002,18 +1179,18 @@
                           " value:"+str(sta_one_member.iloc[index,6]))
 
             colorbar_position = fig.add_axes([left_low, legend_hight / height, 0.02, 1-title_hight/height])  # 位置[左,下,宽,高]
             plt.colorbar(im, cax=colorbar_position,extend=extend)
 
 
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label,fontsize = sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_xticklabels(xticks_label,fontsize = sup_fontsize * 0.8) #, family='Times New Roman')
 
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label,fontsize = sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_yticklabels(yticks_label,fontsize = sup_fontsize * 0.8 ) #, family='Times New Roman')
 
             if slon< 75 and elon >130 and elat >50 and slat >3 and slat <25:
                 if add_minmap is None:
                     add_minmap = "left"
 
             if add_minmap is not None:
                 minmap_lon_lat = [103, 123, 0, 25]
@@ -1430,25 +1607,25 @@
         else:
             im = ax.scatter(x, y, c=colors, cmap=cmap1, norm=norm, s=fix_size)
 
 
         knext_row = pi + (pj + 1) * ncol
         if knext_row >= nplot:
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
         else:
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
 
         if pi ==0:
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8 ) #, family='Times New Roman')
         else:
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+            ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
 
         if slon< 75 and elon >130 and elat >50 and slat >3 and slat <25:
             if add_minmap is None:
                 add_minmap = "left"
         if add_minmap is not None:
             minmap_lon_lat = [105, 123, 0, 20]
             minmap_height_rate = 0.27
@@ -1634,14 +1811,714 @@
     total_bar_width = bar_num * min_bar_widht * 1.3
     if total_bar_width >=10:
         total_bar_width = 10
     if width < total_bar_width:
         width = total_bar_width
     return width
 
+def lineh(array,name_list_dict = None,legend = None,axis = None,xlabel = "Value",vmin = None,vmax = None,ncol = None,grid = None,tag = -1,save_path = None,show = False
+        ,dpi = 300,bar_width = None,sparsify_yticks = 1,sup_fontsize = 10,title = ""
+             ,height = None,width = None,log_y = False,sup_title = None,ylabel = None,legend_col = None,color_list = None,hline = None,marker = None,
+             legend_loc =  "upper right",linestyle = None,return_axs = False):
+    shape = array.shape
+    array = copy.deepcopy(array)
+
+    if len(array[array != meteva.base.IV]) == 0:
+        print("所有的值都为缺失值")
+        return
+
+    if len(shape) == 1:
+        if name_list_dict is None:
+            name_list_dict = {}
+            name_list_dict["y"] = np.arange(array.size).tolist()
+            axis = "y"
+        else:
+            axis = list(name_list_dict.keys())[0]
+
+        y_one = name_list_dict[axis][0]
+        if isinstance(y_one, datetime.datetime):
+            yticks_labels = meteva.product.get_time_str_list(name_list_dict[axis], 1)
+        else:
+            yticks_labels = []
+            for local in name_list_dict[axis]:
+                if isinstance(local, float):
+                    yticks_labels.append(str(round(local, 6)))
+                else:
+                    yticks_labels.append(str(local))
+
+        if width is None:
+            width = 6
+        if height is None:
+            height = width
+
+        fig = plt.figure(figsize=(width, height), dpi=dpi)
+        x = np.arange(array.size)
+        y_plot = array[array != meteva.base.IV]
+        x_plot = x[array != meteva.base.IV]
+
+        if log_y:
+            array[array == 0] = meteva.base.IV
+        if vmin is None:
+            vmin1 = np.min(array[array != meteva.base.IV])
+        else:
+            vmin1 = vmin
+        if vmax is None:
+            vmax1 = np.max(array[array != meteva.base.IV])
+        else:
+            vmax1 = vmax
+
+        dmax = vmax1 - vmin1
+        if log_y and vmin1 <= 0:
+            print("取对数坐标时数据的最小值不能<=0")
+
+        if vmin is None:
+            if log_y:
+                pass
+                vmin1 = vmin1 * (vmin1 / vmax1) ** 0.2
+            else:
+                vmin1 = vmin1 - 0.1 * dmax
+        if vmax is None:
+            if log_y:
+                vmax1 = vmax1 * (vmax1 / vmin1) ** 0.3
+            else:
+                vmax1 = vmax1 + 0.2 * dmax
+
+
+        dat0 = array
+        index_iv = np.where(dat0 == meteva.base.IV)
+        if len(index_iv[0]) == 0:
+            if color_list is None:
+                plt.plot(dat0,x)
+            else:
+                plt.plot(dat0,x, color=color_list[0])
+        else:
+            dat0_all = set_plot_IV_with_out_start_end(dat0)
+            plt.plot(dat0_all,x,  "--", linewidth=0.5, color="k")
+            x_iv = x[index_iv[0]]
+            dat0_iv = dat0_all[index_iv[0]]
+            plt.plot(dat0_iv,x_iv,  "x", color='k', markersize=1)
+            dat0_notiv = dat0.copy()
+            dat0_notiv[dat0_notiv == meteva.base.IV] = np.nan
+            if color_list is None:
+                plt.plot(dat0_notiv,x, marker=marker)
+            else:
+                plt.plot(dat0_notiv,x, color=color_list[0], marker=marker)
+        if tag >= 0:
+            for ii in range(len(dat0)):
+                a = x[ii]
+                b = dat0[ii]
+                if np.isnan(b) or b == meteva.base.IV: continue
+                va = "center"
+                if ii > 0 and ii < len(dat0) - 1:
+                    if b > dat0[ii - 1] and b > dat0[ii + 1]:
+                        va = "bottom"
+                    elif b < dat0[ii - 1] and b < dat0[ii + 1]:
+                        va = "top"
+                fmt_tag = "%." + str(tag) + "f"
+                plt.text(a, b, fmt_tag % b, ha="center", va=va,
+                         fontsize=sup_fontsize * 0.6)
+
+        yticks = x[sparsify_yticks - 1::sparsify_yticks]
+        plt.yticks(yticks, yticks_labels, fontsize=sup_fontsize*0.8)
+        plt.yticks(fontsize=sup_fontsize * 0.8)
+        if ylabel is None: ylabel = axis
+        plt.xlabel(xlabel, fontsize=sup_fontsize * 0.9)
+        plt.ylabel(ylabel, fontsize=sup_fontsize * 0.9)
+
+        if isinstance(title, list):
+            title = title[0]
+        plt.title(title, fontsize=sup_fontsize)
+        plt.xlim(vmin1, vmax1)
+        plt.ylim(-0.5, array.size - 0.5)
+        if hline is not None:
+            plt.axhline(hline, ls="--", c="k")
+        if log_y:
+            ax_one = plt.gca()
+            for tick in ax_one.yaxis.get_major_ticks():
+                tick.label1.set_fontproperties('stixgeneral')
+            plt.yscale('log')
+        if grid is not None:
+            if grid:
+                plt.grid()
+            else:
+                pass
+        else:
+            if sparsify_yticks > 2:
+                plt.grid()
+
+    elif len(shape) == 2:
+        if name_list_dict is None:
+            name_list_dict = {}
+            list1 = np.arange(shape[0]).tolist()
+            list2 = []
+            for lv in list1:
+                list2.append("x_" + str(lv))
+            name_list_dict["x"] = list2
+            name_list_dict["y"] = np.arange(shape[1]).tolist()
+        keys = list(name_list_dict.keys())
+        dat = None
+        if legend is None:
+            if axis is None:
+                legend = keys[0]
+                axis = keys[1]
+            else:
+                if axis != keys[0]:
+                    legend = keys[0]
+                else:
+                    legend = keys[1]
+                    dat = array.T
+        if legend == keys[1]:
+            dat = array.T
+
+        if dat is None:
+            dat = array
+        if legend not in keys:
+            print("legend 参数的取值必须是name_list_dict的key")
+        if axis not in keys:
+            print("axis 参数的取值必须是name_list_dict的key")
+
+        legend_list = name_list_dict[legend]
+        legend_num = len(legend_list)
+        if linestyle is None:
+            linestyle = []
+            for i in range(legend_num):
+                linestyle.append("-")
+        y_one = name_list_dict[axis][0]
+
+        if isinstance(y_one, datetime.datetime):
+            yticks_labels = meteva.product.get_time_str_list(name_list_dict[axis])
+        else:
+            yticks_labels = []
+            for local in name_list_dict[axis]:
+                if isinstance(local, float):
+                    yticks_labels.append(str(round(local, 6)))
+                else:
+                    yticks_labels.append(str(local))
+
+        #width_axis = meteva.base.plot_tools.caculate_axis_width(yticks_labels, sup_fontsize, legend_num)
+        #width_axis_labels = meteva.base.plot_tools.caculate_axis_width(xticks_labels, sup_fontsize, 1)
+
+
+        if width is None:
+            width = 8
+
+        if height is None:
+            height = width
+
+
+        fig = plt.figure(figsize=(width, height), dpi=dpi)
+
+        x = np.arange(0, len(name_list_dict[axis]), 1)
+        if dat.shape[1] + 1 == len(name_list_dict[axis]):
+            x = x - 0.5
+            if isinstance(name_list_dict[axis][0], str) and name_list_dict[axis][0].find("<") == 0:
+                x[0] += 0.5
+            if isinstance(name_list_dict[axis][0], str) and (name_list_dict[axis][-1].find(">") == 0):
+                x[-1] -= 0.5
+        elif len(x) != len(name_list_dict[axis]):
+            print("坐标的size和数据的size不匹配")
+            return
+
+        yticks = x[sparsify_yticks - 1::sparsify_yticks]
+        yticks_labels = yticks_labels[sparsify_yticks - 1::sparsify_yticks]
+
+        if log_y:
+            array[array == 0] = meteva.base.IV
+        if vmin is None:
+            vmin1 = np.min(array[array != meteva.base.IV])
+        else:
+            vmin1 = vmin
+        if vmax is None:
+            vmax1 = np.max(array[array != meteva.base.IV])
+        else:
+            vmax1 = vmax
+        dmax = vmax1 - vmin1
+
+        if log_y and vmin1 <= 0:
+            print("取对数坐标时数据的最小值不能<=0")
+
+        if vmin is None:
+            if log_y:
+                pass
+                vmin1 = vmin1 * (vmin1 / vmax1) ** 0.2
+            else:
+                vmin1_new = vmin1 - 0.1 * dmax
+                if vmin1 >= 0 and vmin1_new <= 0:
+                    vmin1_new = 0
+                vmin1 = vmin1_new
+
+        if vmax is None:
+            if log_y:
+                vmax1 = vmax1 * (vmax1 / vmin1) ** 0.5
+            else:
+                vmax1 = vmax1 + 0.5 * dmax
+
+        x = np.arange(dat.shape[1])
+        legend0 = str(legend_list[0])
+        if legend0.lower().find("ob") < 0 and legend0.find("观测") < 0 and legend0.find(
+                "实况") < 0 and legend0.find("零场") < 0:
+            # 如果判断第一个legend不是观测想的，则跳过第一个自动颜色
+            plt.plot(0, 0)
+        for i in range(legend_num):
+            dat0 = dat[i, :]
+            index_iv = np.where(dat0 == meteva.base.IV)
+            if len(index_iv) == 0:
+                if color_list is None:
+                    if meteva.base.plot_color_dict is not None and legend_list[
+                        i] in meteva.base.plot_color_dict.keys():
+                        color_set1 = meteva.base.plot_color_dict[legend_list[i]]
+                        plt.plot(dat0,x, label=legend_list[i], color=color_set1, linestyle=linestyle[i])
+                    else:
+                        plt.plot(dat0, x, label=legend_list[i], linestyle=linestyle[i])
+                else:
+                    plt.plot(dat0,x,  label=legend_list[i], color=color_list[i], linestyle=linestyle[i])
+            else:
+                dat0_all = set_plot_IV_with_out_start_end(dat0)
+                plt.plot(dat0_all,x,  "--", linewidth=0.5, color="k")
+                x_iv = x[index_iv[0]]
+                dat0_iv = dat0_all[index_iv[0]]
+                plt.plot(dat0_iv,x_iv,  "x", color='k', markersize=1)
+                dat0_notiv = dat0.copy()
+                dat0_notiv[dat0_notiv == meteva.base.IV] = np.nan
+                if color_list is None:
+                    if meteva.base.plot_color_dict is not None and legend_list[
+                        i] in meteva.base.plot_color_dict.keys():
+                        color_set1 = meteva.base.plot_color_dict[legend_list[i]]
+                        plt.plot(dat0_notiv, x, label=name_list_dict[legend][i], color=color_set1, marker=marker,
+                                 linestyle=linestyle[i])
+                    else:
+                        plt.plot(dat0_notiv,x,  label=name_list_dict[legend][i], marker=marker,
+                                 linestyle=linestyle[i])
+                else:
+                    plt.plot(dat0_notiv, x, label=name_list_dict[legend][i], color=color_list[i], marker=marker,
+                             linestyle=linestyle[i])
+            if tag >= 0:
+                for ii in range(len(dat0)):
+                    a = x[ii]
+                    b = dat0[ii]
+                    if np.isnan(b) or b == meteva.base.IV: continue
+                    va = "center"
+                    if ii > 0 and ii < len(dat0) - 1:
+                        if b > dat0[ii - 1] and b > dat0[ii + 1]:
+                            va = "bottom"
+                        elif b < dat0[ii - 1] and b < dat0[ii + 1]:
+                            va = "top"
+                    fmt_tag = "%." + str(tag) + "f"
+                    plt.text(a, b, fmt_tag % b, ha="center", va=va,
+                             fontsize=sup_fontsize * 0.6)
+        if legend_col is None:legend_col=1
+        plt.legend(fontsize=sup_fontsize * 0.8, ncol=legend_col, loc=legend_loc)
+        plt.yticks(yticks, yticks_labels, fontsize=sup_fontsize*0.8)
+
+        plt.xlabel(xlabel, fontsize=sup_fontsize * 0.9)
+        plt.ylabel(ylabel, fontsize=sup_fontsize * 0.9)
+        if isinstance(title, list):
+            title = title[0]
+        plt.title(title, fontsize=sup_fontsize)
+        plt.ylim(-0.5, dat.shape[1] - 0.5)
+        plt.xlim(vmin1, vmax1)
+        if hline is not None:
+            plt.axhline(hline, ls="--", c="k")
+        if log_y:
+            ax_one = plt.gca()
+            for tick in ax_one.yaxis.get_major_ticks():
+                tick.label1.set_fontproperties('stixgeneral')
+            plt.yscale('log')
+        if grid is not None:
+            if grid:
+                plt.grid()
+            else:
+                pass
+        else:
+            if sparsify_yticks > 2:
+                plt.grid()
+
+    elif len(shape) == 3:
+        if name_list_dict is None:
+            name_list_dict = {}
+            name_list_dict["z"] = np.arange(shape[0])
+            list1 = np.arange(shape[1]).tolist()
+            list2 = []
+            for lv in list1:
+                list2.append("x_" + str(lv))
+            name_list_dict["y"] = list2
+            name_list_dict["y"] = np.arange(shape[2])
+            legend = "x"
+            axis = "y"
+            subplot = "z"
+        keys = list(name_list_dict.keys())
+        if legend is None:
+            if axis is None:
+                legend = keys[1]
+                axis = keys[2]
+                subplot = keys[0]
+            else:
+                if axis == keys[2]:
+                    legend = keys[1]
+                    subplot = keys[0]
+                elif axis == keys[1]:
+                    legend = keys[2]
+                    subplot = keys[0]
+                else:
+                    legend = keys[2]
+                    subplot = keys[1]
+        else:
+            if axis is None:
+                if legend == keys[0]:
+                    axis = keys[2]
+                    subplot = keys[1]
+                elif legend == keys[1]:
+                    axis = keys[2]
+                    subplot = keys[0]
+                else:
+                    axis = keys[1]
+                    subplot = keys[0]
+            else:
+                indexlist = [0, 1, 2]
+                indexlist.remove(keys.index(legend))
+                indexlist.remove(keys.index(axis))
+                subplot = keys[indexlist[0]]
+        if legend not in keys:
+            print("legend 参数的取值必须是name_list_dict的key")
+        if axis not in keys:
+            print("axis 参数的取值必须是name_list_dict的key")
+        newshape = (keys.index(subplot), keys.index(legend), keys.index(axis))
+        data = array.transpose(newshape)
+        legend_num = len(name_list_dict[legend])
+        if linestyle is None:
+            linestyle = []
+            for i in range(legend_num):
+                linestyle.append("-")
+        y_one = name_list_dict[axis][0]
+        if isinstance(y_one, datetime.datetime):
+            yticks_labels = meteva.product.get_time_str_list(name_list_dict[axis], 1)
+        elif axis.find("dayofyear") >= 0:
+            yticks_labels = meteva.product.get_dayofyear_str_list(name_list_dict[axis])
+        else:
+            yticks_labels = []
+            for local in name_list_dict[axis]:
+                if isinstance(local, float):
+                    if local == int(local):
+                        yticks_labels.append(str(int(local)))
+                    else:
+                        yticks_labels.append(str(round(local, 6)))
+                else:
+                    yticks_labels.append(str(local))
+
+        yticks_labels = yticks_labels[sparsify_yticks - 1::sparsify_yticks]
+
+        subplot_num = len(name_list_dict[subplot])
+
+        x = np.arange(len(name_list_dict[axis]))
+        if data.shape[2] + 1 == len(name_list_dict[axis]):
+            x = x - 0.5
+            if isinstance(name_list_dict[axis][0], str) and name_list_dict[axis][0].find("<") == 0:
+                x[0] += 0.5
+            if isinstance(name_list_dict[axis][0], str) and (name_list_dict[axis][-1].find(">") == 0):
+                x[-1] -= 0.5
+        elif len(x) != len(name_list_dict[axis]):
+            print("坐标的size和数据的size不匹配")
+            return
+
+        yticks = x[sparsify_yticks - 1::sparsify_yticks]
+
+        width_one_subplot = 3
+
+
+        if ncol is None:
+            ncol = int(8 / width_one_subplot)
+            nrow = int(math.ceil(subplot_num / ncol))
+            ncol = int(math.ceil(subplot_num / nrow))
+        else:
+            nrow = int(math.ceil(len(name_list_dict[subplot]) / ncol))
+
+        if width is None:
+            width_fig = 8
+        else:
+            width_fig = width
+
+        wspace = sup_fontsize * 0.03
+        height_hspace = sup_fontsize * 0.03
+        height_suplegend = 1
+        if height is None:
+            height_fig = 6
+        else:
+            height_fig = height
+
+        fig = plt.figure(figsize=(width_fig, height_fig), dpi=dpi)
+        x = np.arange(data.shape[2])
+
+        plt.subplots_adjust(left=0, bottom=0.0, right=1.0, top=1 - height_suplegend / height_fig,
+                            hspace=height_hspace, wspace=wspace)
+
+        if bar_width is None:
+            width = 0.7 / (legend_num + 2)
+        else:
+            width = bar_width
+        ax_top = None
+        for k in range(subplot_num):
+            # print(data.shape)
+            data_k = data[k, :, :]
+            if log_y:
+                data_k[data_k == 0] = meteva.base.IV
+            if vmin is None:
+                dat_k0 = data_k[data_k != meteva.base.IV]
+                if dat_k0.size > 0:
+                    vmin1 = np.min(dat_k0)
+                else:
+                    vmin1 = 0
+            else:
+                if isinstance(vmin, list):
+                    if len(vmin) != subplot_num:
+                        print("vmin 参数的个数和 子图个数不一致，请重新设置")
+                        return
+                    else:
+                        vmin1 = vmin[k]
+                else:
+                    vmin1 = vmin
+
+            if vmax is None:
+                dat_k0 = data_k[data_k != meteva.base.IV]
+                if dat_k0.size > 0:
+                    vmax1 = np.max(dat_k0)
+                else:
+                    vmax1 = vmin1 + 0.1
+            else:
+                if isinstance(vmax, list):
+                    if len(vmax) != subplot_num:
+                        print("vmin 参数的个数和 子图个数不一致，请重新设置")
+                        return
+                    else:
+                        vmax1 = vmax[k]
+                else:
+                    vmax1 = vmax
+
+            dmax = vmax1 - vmin1
+
+            if log_y and vmin1 < 0:
+                print("取对数坐标时数据的最小值不能<0")
+            if vmin is None:
+                if log_y:
+                    pass
+                    vmin1 = vmin1 * (vmin1 / vmax1) ** 0.2
+                else:
+                    vmin1_new = vmin1 - 0.1 * dmax
+                    if vmin1 >= 0 and vmin1_new <= 0:
+                        vmin1_new = 0
+                    vmin1 = vmin1_new
+
+            if vmax is None:
+                if log_y:
+                    vmax1 = vmax1 * (vmax1 / vmin1) ** 0.5
+                else:
+                    vmax1 = vmax1 + 0.5 * dmax
+
+            ax_one = plt.subplot(nrow, ncol, k + 1)
+            if k == 0: ax_top = ax_one
+            legend0 = str(name_list_dict[legend][0])
+            if legend0.lower().find("ob") < 0 and legend0.find("观测") < 0 and legend0.find(
+                    "实况") < 0 and legend0.find("零场") < 0:
+                plt.bar(0, 0)
+                plt.plot(0, 0)
+            for i in range(legend_num):
+
+                dat0 = data[k, i, :]
+                index_iv = np.where(dat0 == meteva.base.IV)
+                if len(index_iv[0]) == 0:
+                    if color_list is None:
+                        if meteva.base.plot_color_dict is not None and name_list_dict[legend][
+                            i] in meteva.base.plot_color_dict.keys():
+                            color_set1 = meteva.base.plot_color_dict[name_list_dict[legend][i]]
+                            if k == 0:
+                                plt.plot( data[k, i, :], x,label=name_list_dict[legend][i], color=color_set1,
+                                         marker=marker, linestyle=linestyle[i])
+                            else:
+                                plt.plot( data[k, i, :],x, color=color_set1, marker=marker, linestyle=linestyle[i])
+                        else:
+                            if k == 0:
+                                plt.plot(data[k, i, :],x,  label=name_list_dict[legend][i], marker=marker,
+                                         linestyle=linestyle[i])
+                            else:
+                                plt.plot( data[k, i, :], x,marker=marker, linestyle=linestyle[i])
+                    else:
+                        if k == 0:
+                            plt.plot(data[k, i, :],x,  label=name_list_dict[legend][i], color=color_list[i],
+                                     marker=marker, linestyle=linestyle[i])
+                        else:
+                            plt.plot( data[k, i, :],x, color=color_list[i], marker=marker, linestyle=linestyle[i])
+                else:
+                    dat0_all = set_plot_IV_with_out_start_end(dat0)
+                    plt.plot(dat0_all,x,  "--", linewidth=0.5, color="k")
+                    x_iv = x[index_iv[0]]
+                    dat0_iv = dat0_all[index_iv[0]]
+                    plt.plot(dat0_iv,x_iv,  "x", color='k', markersize=1)
+                    dat0_notiv = dat0.copy()
+                    dat0_notiv[dat0_notiv == meteva.base.IV] = np.nan
+                    if color_list is None:
+                        if meteva.base.plot_color_dict is not None and name_list_dict[legend][
+                            i] in meteva.base.plot_color_dict.keys():
+                            color_set1 = meteva.base.plot_color_dict[name_list_dict[legend][i]]
+                            if k == 0:
+                                plt.plot( dat0_notiv,x, label=name_list_dict[legend][i], color=color_set1,
+                                         marker=marker, linestyle=linestyle[i])
+                            else:
+                                plt.plot(dat0_notiv, x, color=color_set1, marker=marker, linestyle=linestyle[i])
+                        else:
+                            if k == 0:
+                                plt.plot( dat0_notiv,x, label=name_list_dict[legend][i], marker=marker,
+                                         linestyle=linestyle[i])
+                            else:
+                                plt.plot( dat0_notiv,x, marker=marker, linestyle=linestyle[i])
+                    else:
+                        if k == 0:
+                            plt.plot( dat0_notiv,x, label=name_list_dict[legend][i], color=color_list[i],
+                                     marker=marker, linestyle=linestyle[i])
+                        else:
+                            plt.plot( dat0_notiv, x,color=color_list[i], marker=marker, linestyle=linestyle[i])
+
+                if tag >= 0:
+                    for ii in range(len(dat0)):
+                        a = x[ii]
+                        b = dat0[ii]
+                        if np.isnan(b) or b == meteva.base.IV: continue
+                        va = "center"
+                        if ii > 0 and ii < len(dat0) - 1:
+                            if b > dat0[ii - 1] and b > dat0[ii + 1]:
+                                va = "bottom"
+                            elif b < dat0[ii - 1] and b < dat0[ii + 1]:
+                                va = "top"
+                        fmt_tag = "%." + str(tag) + "f"
+                        plt.text(a, b, fmt_tag % b, ha="center", va=va,
+                                 fontsize=sup_fontsize * 0.6)
+
+            ki = k % ncol
+            kj = int(k / ncol)
+
+            if ylabel is None: ylabel = axis
+
+            plt.yticks(yticks, yticks_labels, fontsize=sup_fontsize*0.8)
+            plt.ylabel(ylabel, fontsize=sup_fontsize * 0.9)
+
+            xminorLocator = mpl.ticker.MultipleLocator(1)  # 将x轴次刻度标签设置xmi
+            ax_one.xaxis.set_minor_locator(xminorLocator)
+
+            plt.xticks(fontsize=sup_fontsize * 0.8)
+            plt.xlabel(xlabel, fontsize=sup_fontsize * 0.9)
+
+            if hline is not None:
+                plt.axhline(hline, ls="--", c="k")
+            if isinstance(title, list):
+                if (len(title) != subplot_num):
+                    print("子图数和设置的子图标题数不一致")
+                    return
+                title1 = title[k]
+            else:
+                if subplot_num > 1:
+                    title1 = title + str(name_list_dict[subplot][k])
+                else:
+                    title1 = title
+            if subplot_num > 1:
+                #y1 = 1 - 0.035 * sup_fontsize / height_fig
+                plt.title(title1, fontsize=sup_fontsize, y=0.94,x = 0.01,ha="left",va = "top")
+            else:
+                plt.title(title1, fontsize=sup_fontsize,x = 0.05,ha="left")
+
+            plt.ylim(-0.5, data.shape[2] - 0.5)
+
+            if log_y:
+                for tick in ax_one.yaxis.get_major_ticks():
+                    tick.label1.set_fontproperties('stixgeneral')
+                plt.yscale('log')
+
+            plt.xlim(vmin1, vmax1)
+            if grid is not None:
+                if grid:
+                    plt.grid()
+                else:
+                    pass
+            else:
+                if sparsify_yticks > 2:
+                    plt.grid()
+
+        if sup_title is not None:
+
+            if legend_num == 1:
+                strss = sup_title.split("\n")
+                by = 1 - (height_suplegend - len(strss) * sup_fontsize * 0.01) / height_fig + 0.025
+                plt.suptitle(sup_title, y=by, fontsize=sup_fontsize)
+            else:
+                width_suptitle = caculate_str_width(sup_title, sup_fontsize)
+                if legend_col is None:
+                    legend_col = int((width_fig - width_suptitle) * 12 / sup_fontsize)
+                    if legend_col < 1: legend_col = 1
+                    legend_row = int(math.ceil(legend_num / legend_col))
+                    legend_col = int(math.ceil(legend_num / legend_row))
+                else:
+                    legend_row = int(math.ceil(legend_num / legend_col))
+                strss = sup_title.split("\n")
+                # by = 1 - (height_suplegend - len(strss) * sup_fontsize * 0.01) / height_fig + 0.025
+
+                by = ax_top.bbox.ymax / fig.bbox.ymax + (len(strss) * sup_fontsize * 0.015 + 0.1) / height_fig
+                plt.suptitle(sup_title, x=0, y=by, fontsize=sup_fontsize, horizontalalignment='left')
+
+                if matplotlib.__version__ == "3.2.2":
+                    by = ax_top.bbox.ymax / fig.bbox.ymax + (legend_row * sup_fontsize * 0.7 * 0.02 + 0.6) / height_fig
+
+                else:
+                    by = ax_top.bbox.ymax / fig.bbox.ymax + (legend_row * sup_fontsize * 0.7 * 0.02 + 0.15) / height_fig
+                if subplot_num > 1:
+                    fig.legend(fontsize=sup_fontsize * 0.7, ncol=legend_col, loc="upper right",
+                               bbox_to_anchor=(1, by))
+                else:
+                    plt.legend(fontsize=sup_fontsize * 0.7, ncol=legend_col, loc="upper right",bbox_to_anchor=(1, by))
+        else:
+            if legend_num > 1:
+                if legend_col is None:
+                    legend_col = int(width_fig * 8 / sup_fontsize)
+                    if legend_col < 1: legend_col = 1
+                    legend_row = int(math.ceil(legend_num / legend_col))
+                    legend_col = int(math.ceil(legend_num / legend_row))
+                else:
+                    legend_row = int(math.ceil(legend_num / legend_col))
+                # print(height_fig)
+                if matplotlib.__version__ == "3.2.2":
+                    by = ax_top.bbox.ymax / fig.bbox.ymax + (legend_row * sup_fontsize * 0.9 * 0.03 + 0.6) / height_fig
+                else:
+                    by = ax_top.bbox.ymax / fig.bbox.ymax + (legend_row * sup_fontsize * 0.9 * 0.03 + 0.1) / height_fig
+
+                # print(by)
+
+                if subplot_num > 1:
+                    fig.legend(fontsize=sup_fontsize * 0.8, ncol=legend_col, loc=legend_loc,
+                               bbox_to_anchor=(0.52, by))
+                else:
+                    plt.legend(fontsize=sup_fontsize * 0.8, ncol=legend_col, loc=legend_loc,bbox_to_anchor=(0.52, by))
+
+    else:
+        print("array不能超过3维")
+        return
+        xticks = []
+        for index in index_list:
+            if not type(index) == str:
+                index = str(index)
+            xticks.append(index)
+
+    if return_axs:
+        return plt.gca()
+    if save_path is None:
+        show = True
+    else:
+        meteva.base.creat_path(save_path)
+        plt.savefig(save_path, bbox_inches='tight')
+        print("检验结果已以图片形式保存至" + save_path)
+    if show:
+        plt.show()
+    plt.close()
+
+
 def plot_bar(plot_type,array,name_list_dict = None,legend = None,axis = None,ylabel = "Value",vmin = None,vmax = None,ncol = None,grid = None,tag = -1,save_path = None,show = False
         ,dpi = 300,bar_width = None,spasify_xticks = None,sparsify_xticks = None,sup_fontsize = 10,title = ""
              ,height = None,width = None,log_y = False,sup_title = None,xlabel = None,legend_col = None,color_list = None,hline = None,marker = None,
              legend_loc =  "upper center",linestyle = None,return_axs = False):
     shape = array.shape
 
 
@@ -2415,23 +3292,21 @@
             ki = k % ncol
             kj = int(k / ncol)
             knext_row = ki + (kj+1) * ncol
             #print(knext_row)
             #print(subplot_num)
             if xlabel is None: xlabel = axis
             if knext_row>=subplot_num:
-                #plt.xticks(x[::spasify], name_list_dict[axis][::spasify], fontsize=sup_fontsize * 0.8)
                 plt.xticks(xticks, xticks_labels, fontsize=xticks_font)
                 plt.xlabel(xlabel, fontsize=sup_fontsize * 0.9)
             else:
                 plt.xticks(xticks,xticks_labels_None)
             xminorLocator = mpl.ticker.MultipleLocator(1)  # 将x轴次刻度标签设置xmi
             ax_one.xaxis.set_minor_locator(xminorLocator)
             plt.yticks(fontsize=sup_fontsize * 0.8)
-
             plt.ylabel(ylabel, fontsize=sup_fontsize * 0.9)
             if hline is not None:
                 plt.axhline(hline, ls="--", c="k")
             if isinstance(title, list):
                 if(len(title) != subplot_num):
                     print("子图数和设置的子图标题数不一致")
                     return
@@ -3262,35 +4137,15 @@
                 y1 = 1 - 0.035 * sup_fontsize / (height_fig / nrow)
                 plt.title(title1, fontsize=sup_fontsize, y=y1)
             else:
                 plt.title(title1, fontsize=sup_fontsize)
 
             plt.xlim(-0.5, data.shape[2] - 0.5)
 
-            # if log_y:
-            #     for tick in ax_one.yaxis.get_major_ticks():
-            #         tick.label1.set_fontproperties('stixgeneral')
-            #     plt.yscale('log')
-            # plt.ylim(vmin1, vmax1)
-            # if grid is not None:
-            #     if grid:
-            #         if plot_type == "bar":
-            #             plt.grid(axis="y")
-            #         else:
-            #             plt.grid()
-            #     else:
-            #         pass
-            # else:
-            #     if spasify > 2:
-            #         if plot_type == "bar":
-            #             plt.grid(axis="y")
-            #         else:
-            #             plt.grid()
 
-        print("a")
         if sup_title is not None:
 
             if legend_num == 1:
                 strss = sup_title.split("\n")
                 by = 1 - (height_suplegend - len(strss) * sup_fontsize * 0.01) / height_fig + 0.025
                 plt.suptitle(sup_title, y=by, fontsize=sup_fontsize)
             else:
@@ -3411,15 +4266,23 @@
                     text_color = ".15" if lum > .408 else "w"
                     ax_one.text(i, j, fmt_tag % data_ijk, ha="center", va="center",
                              fontsize=fontsize, c=text_color)
     fig = plt.gcf()
     fig.colorbar(im, ax=ax_one)
 
 def mesh(array,name_list_dict = None,axis_x = None,axis_y = None,cmap = "rainbow",clevs = None,ncol = None,annot =None,save_path = None,show = False,dpi = 300,
-         spasify_xticks = None,sup_fontsize = 10,title ="",width = None,height = None,rect = None,rect_color = "r"):
+         spasify_xticks = None,sup_fontsize = 10,title ="",sup_title = None,width = None,height = None,rect = None,rect_color = "r"):
+
+    mesh_contour("mesh",array,name_list_dict=name_list_dict,axis_x=axis_x,axis_y=axis_y,cmap=cmap,clevs=clevs,
+                 ncol=ncol,annot=annot,save_path=save_path,show=show,dpi=dpi,spasify_xticks=spasify_xticks,
+                 sup_fontsize=sup_fontsize,title=title,sup_title = sup_title,width=width,height=height,rect=rect,rect_color=rect_color)
+
+
+def mesh_contour(type,array,name_list_dict = None,axis_x = None,axis_y = None,cmap = "rainbow",clevs = None,ncol = None,annot =None,save_path = None,show = False,dpi = 300,
+         spasify_xticks = None,sup_fontsize = 10,title ="",sup_title =None,width = None,height = None,rect = None,rect_color = "r",extend = None):
 
     shape = array.shape
     if len(array[array != meteva.base.IV]) == 0:
         print("所有的值都为缺失值")
         return
 
     if len(shape) == 3 or len(shape) == 2:
@@ -3491,14 +4354,17 @@
 
         x_one = name_list_dict[axis_x][0]
         if isinstance(x_one, datetime.datetime):
             xticks_labels = meteva.product.get_time_str_list(name_list_dict[axis_x], 3)
         else:
             xticks_labels = []
             for local in name_list_dict[axis_x]:
+                if isinstance(local,float):
+                    if int(local) == local:
+                        local = int(local)
                 xticks_labels.append(str(local))
 
         width_axis = meteva.base.plot_tools.caculate_axis_width(xticks_labels, sup_fontsize, legend_num)
         width_axis_labels = meteva.base.plot_tools.caculate_axis_width(xticks_labels, sup_fontsize, 1)
 
         width_wspace = sup_fontsize * 0.1
         width_one_subplot = width_axis + width_wspace
@@ -3510,41 +4376,58 @@
                 spasify = int(math.ceil(width_axis_labels / (10 / ncol - width_wspace)))
                 width_one_subplot = 8/ ncol
         else:
             if width_one_subplot > 8:
                 spasify = int(math.ceil(width_axis_labels / (10 - width_wspace)))
                 width_one_subplot = 8
 
+
         if spasify_xticks is not None:
             xticks_font = sup_fontsize * 1.0 * spasify_xticks * (width - width_wspace) / width_axis_labels
             spasify = spasify_xticks
         else:
             xticks_font = sup_fontsize * 0.8
 
         x = np.arange(len(name_list_dict[axis_x]))
         xticks = x[spasify-1::spasify]
         if isinstance(x_one, datetime.datetime):
-            xticks_labels = meteva.product.get_time_str_list(name_list_dict[axis_x][::spasify], 3)
+            xticks_labels = meteva.product.get_time_str_list(name_list_dict[axis_x][spasify-1::spasify], 3)
         else:
             xticks_labels = xticks_labels[spasify-1::spasify]
 
+        if axis_x =="lon":
+            xticks_labels[-1] +="°E"
+        if axis_x=="lat":
+            if int(xticks_labels[-1]) >0:
+                xticks_labels[-1] += "°N"
+            else:
+                xticks_labels_new = []
+                for xticks1 in xticks_labels:
+                    xticks_labels_new.append(xticks1[1:]) #remove  "-"
+                xticks_labels_new[-1] += "°S"
+                xticks_labels = xticks_labels_new
+
+
         xticks_labels_None = []
         for i in range(len(xticks_labels)):
             xticks_labels_None.append("")
 
         y = np.arange(len(name_list_dict[axis_y])+1) -0.5
         yticks = np.arange(len(name_list_dict[axis_y]))
         y_one = name_list_dict[axis_y][0]
         yticks_labels =[]
         if isinstance(y_one, datetime.datetime):
             for time1 in  name_list_dict[axis_y]:
                 str1 = "%02d" % time1.day + "日" + "%02d" % time1.hour + "时"
                 yticks_labels.append(str1)
         else:
             for local in name_list_dict[axis_y]:
+                if isinstance(local, float):
+                    if int(local) == local:
+                        local = int(local)
                 yticks_labels.append(str(local))
 
         if ncol is None:
             ncol = int(round(8 / width_one_subplot))
 
             nrow = int(math.ceil(subplot_num / ncol))
             ncol = int(math.ceil(subplot_num / nrow))
@@ -3602,31 +4485,45 @@
                 vmin = np.min(data_k_copy[data_k_copy != meteva.base.IV])
                 vmax = np.max(data_k_copy[data_k_copy != meteva.base.IV])
             else:
                 cmap0 = cmap
                 clevs0 = clevs
             cmap1,clevs1= meteva.base.color_tools.def_cmap_clevs(cmap = cmap0,clevs=clevs0,vmin=vmin,vmax = vmax)
             ax_one = plt.subplot(nrow, ncol, k + 1)
-            myheatmap(ax_one,data_k,cmap1,clevs1,annot,sup_fontsize)
+            if type == "mesh":
+                myheatmap(ax_one,data_k,cmap1,clevs1,annot,sup_fontsize)
+            else:
+                cmap1, clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap=cmap, clevs=clevs, vmin=vmin,
+                                                                            vmax=vmax, extend=extend)
+
+                norm = BoundaryNorm(clevs1, ncolors=cmap1.N)
+                im = ax_one.contourf(data_k, levels=clevs1, cmap=cmap1, norm=norm,
+                                 extend=extend)
+                fig.colorbar(im, ax=ax_one)
 
             ki = k % ncol
             kj = int(k / ncol)
             knext_row = ki + (kj + 1) * ncol
-            # print(knext_row)
-            # print(subplot_num)
-            plt.xticks(xticks, xticks_labels, fontsize=xticks_font)
-            if knext_row >= subplot_num:
-                # plt.xticks(x[::spasify], name_list_dict[axis][::spasify], fontsize=sup_fontsize * 0.8)
 
+            if axis_x=="lon" or axis_x=="lat":
+                #为了让°E显示得更紧凑
+                plt.xticks(xticks, xticks_labels, fontsize=xticks_font) #, family='Times New Roman')
+            else:
+                #为了显示中文字体
+                plt.xticks(xticks, xticks_labels, fontsize=xticks_font)
+            if knext_row >= subplot_num:
                 plt.xlabel(axis_x, fontsize=sup_fontsize * 0.9)
-            #else:
-            #    plt.xticks(xticks, xticks_labels_None)
+
             xminorLocator = mpl.ticker.MultipleLocator(1)  # 将x轴次刻度标签设置xmi
-            #ax_one.xaxis.set_minor_locator(xminorLocator)
-            plt.yticks(yticks,yticks_labels,fontsize=sup_fontsize * 0.8)
+            if axis_y =="lat" or axis_y == "lon":
+                # 为了让°E显示得更紧凑
+                plt.yticks(yticks,yticks_labels,fontsize=sup_fontsize * 0.8) #,family='Times New Roman')
+            else:
+                #为了显示中文字体
+                plt.yticks(yticks, yticks_labels, fontsize=sup_fontsize * 0.8)
             plt.ylabel(axis_y, fontsize=sup_fontsize * 0.9)
             if rect is not None:
                 rect1 = patches.Rectangle((rect[0], rect[1]), rect[2], rect[3], linewidth=2, edgecolor=rect_color, facecolor='none')
                 ax_one.add_patch(rect1)
             #plt.ylabel(ylabel, fontsize=sup_fontsize * 0.9)
 
             if isinstance(title, list):
@@ -3637,31 +4534,40 @@
             else:
                 if subplot_num > 1:
                     title1 = title  + str(name_list_dict[subplot][k])
                 else:
                     title1 = title
             plt.title(title1, fontsize=sup_fontsize)
 
+            #提取第1个绘图框的
+            if sup_title is not None:
+                if k==0:
+                    y = ax_one.bbox.y1 / fig.dpi / height_fig
+                    if title1 =="":
+                        y_sup_title = y + (sup_fontsize * 0.03) / height_fig
+                    else:
+                        y_sup_title = y + (sup_fontsize * 0.05) / height_fig
+                    plt.suptitle(sup_title, y=y_sup_title, fontsize=sup_fontsize * 1.2)
     else:
         print("array只能绘制2维或3维数据")
         return
 
+
     if save_path is None:
         show = True
     else:
         meteva.base.creat_path(save_path)
         plt.savefig(save_path, bbox_inches='tight')
         print("检验结果已以图片形式保存至" + save_path)
     if show:
         plt.show()
     plt.close()
 
 
 
-
 def mesh_obtime_time(sta0,save_dir = None,save_path = None,
                    clevs = None,cmap = None,show = False,xtimetype = "mid",dpi = 300,annot =None,
                      sup_fontsize = 10,title = "预报准确性和稳定性对比图",width = None,height = None,multiple = 1):
 
     sta = sta0.copy()
     sta.iloc[:,6:] *= multiple
     ids = list(set(sta.loc[:, "id"]))
```

### Comparing `meteva-1.8.2/meteva/base/tool/plot_tools_adv.py` & `meteva-1.8.3/meteva/base/tool/plot_tools_adv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import meteva
 import numpy as np
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import math
 from matplotlib.colors import BoundaryNorm
 
 
 def add_map(ax,add_county_line = False,add_worldmap = True,title = None,sup_fontsize = 12,linewidth = [0.3,0.3,0.2],color = ["k","k","k"]):
 
     if meteva.base.customized_basemap_list is None:
@@ -231,25 +229,25 @@
         ax.set_xlim((slon, elon))
         ax.set_ylim((slat, elat))
 
         if keep_ticks>=0:
             if p >= nplot - ncol or keep_ticks:
                 # 最底行画横坐标
                 ax.set_xticks(xticks)
-                ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             else:
-                ax.set_xticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_xticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
 
 
             if pi ==0 or keep_ticks:
                 # 最左侧画纵坐标
                 ax.set_yticks(yticks)
-                ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             else:
-                ax.set_yticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_yticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
         else:
             ax.set_xticks([])
             ax.set_yticks([])
         if grid: plt.grid(linestyle = "--",linewidth = 0.5)
         if title_list is None:
             sub_title = None
         else:
@@ -298,14 +296,15 @@
                 min_ax_list.append(ax_min)
     if len(min_ax_list)==0:
         return ax_list
     else:
         return ax_list,min_ax_list
 
 
+
 def add_contourf(ax,grd,cmap ="rainbow",clevs= None,add_colorbar = True,cut_colorbar = True,title = None,title_fontsize = 8,clip = None,
                  extend = None,colorbar_location = None,alpha=1):
     slon = ax.transLimits._boxin.x0
     elon = ax.transLimits._boxin.x1
     slat = ax.transLimits._boxin.y0
     elat = ax.transLimits._boxin.y1
     if grd is None:return
@@ -900,8 +899,9 @@
                 cent1 = meteva.base.sele_by_para(cent,level = level,time = time,dtime = dtime,id = id)
 
 
 
     ax.set_xlim(slon,elon)
     ax.set_ylim(slat,elat)
     ax.set_title(title,fontsize =title_fontsize)
-    return
+    return
+
```

### Comparing `meteva-1.8.2/meteva/base/tool/process_tools.py` & `meteva-1.8.3/meteva/base/tool/process_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/station_tools.py` & `meteva-1.8.3/meteva/base/tool/station_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/base/tool/time_tools.py` & `meteva-1.8.3/meteva/base/tool/time_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/Vector/__init__.py` & `meteva-1.8.3/meteva/method/Vector/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/Vector/plot.py` & `meteva-1.8.3/meteva/method/Vector/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/Vector/score.py` & `meteva-1.8.3/meteva/method/Vector/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/continuous/__init__.py` & `meteva-1.8.3/meteva/method/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/continuous/plot.py` & `meteva-1.8.3/meteva/method/continuous/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import meteva
 import numpy as np
 import  math
-#from sklearn.linear_model import LinearRegression
 from  matplotlib import  cm
 from matplotlib.ticker import NullFormatter, FixedLocator
 import copy
 import pandas as pd
 import datetime
 import scipy.stats as st
 
@@ -116,17 +115,17 @@
         colors = sta_count["data0"]
         sort_index = colors.argsort()
         fo_s = fo[sort_index]
         ob_s = ob[sort_index]
         colors = colors[sort_index]
         #plt.scatter(fo_s, ob_s, c=colors,s = markersize,cmap="tab20c")
 
-        if matplotlib.__version__=="3.3.4":
+        try:
             plt.scatter(fo_s, ob_s, c=colors, s=markersize, cmap="turbo")
-        else:
+        except:
             plt.scatter(fo_s, ob_s, c=colors, s=markersize, cmap="rainbow")
         #plt.plot(fo, ob, '.', color='b', markersize=markersize)
 
         plt.subplots_adjust(left=0, bottom=0.0, right=1.0, top = 1 - height_suptitle/height_fig,
                             hspace=height_hspace/heidht_axis,wspace=width_wspace/width_axis)
         if rtype == "rate":
             ob_line = np.arange(num_min, num_max, dmm / 30)
```

### Comparing `meteva-1.8.2/meteva/method/continuous/score.py` & `meteva-1.8.3/meteva/method/continuous/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/continuous/skill.py` & `meteva-1.8.3/meteva/method/continuous/skill.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/continuous/table.py` & `meteva-1.8.3/meteva/method/continuous/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/ensemble/plot.py` & `meteva-1.8.3/meteva/method/ensemble/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
+import meteva
 import numpy as np
 import copy
-import meteva
+
 
 
 def box_plot_ensemble(ob, fo,member_list = None, vmax = None,vmin = None,save_path=None,show = False,dpi = 300,title ="频率对比箱须图",
                       sup_fontsize = 10,width = None,height = None):
     '''
     box_plot 画一两组数据的箱型图
     ---------------
```

### Comparing `meteva-1.8.2/meteva/method/ensemble/score.py` & `meteva-1.8.3/meteva/method/ensemble/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/multi_category/__init__.py` & `meteva-1.8.3/meteva/method/multi_category/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/multi_category/plot.py` & `meteva-1.8.3/meteva/method/multi_category/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/multi_category/score.py` & `meteva-1.8.3/meteva/method/multi_category/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/multi_category/table.py` & `meteva-1.8.3/meteva/method/multi_category/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/probability/plot.py` & `meteva-1.8.3/meteva/method/probability/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
+import meteva
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
-plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
 from meteva.method.yes_or_no.score import pofd_hfmc, pod_hfmc
 from meteva.base.tool.plot_tools import set_plot_IV
 from meteva.base import IV
-import meteva
+
 import math
 
 
 def reliability(Ob, Fo, grade_count=10, member_list=None, vmax = None,log_y = False,save_path=None,show = False,dpi = 300, title="可靠性图",
                 sup_fontsize =10,width = None,height = None):
     '''
     :param Ob:
```

### Comparing `meteva-1.8.2/meteva/method/probability/score.py` & `meteva-1.8.3/meteva/method/probability/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/probability/table.py` & `meteva-1.8.3/meteva/method/probability/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/__init__.py` & `meteva-1.8.3/meteva/method/space/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/acc/acc.py` & `meteva-1.8.3/meteva/method/space/acc/acc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-#import meteva.base as meb
-#import meteva.method as mem
-#import meteva.product as mpd
-#import meteva.perspact as mps
 import datetime
 import copy
 import numpy as np
 import xarray as xr
 import pandas as pd
 import matplotlib.pyplot as plt
 import os
```

### Comparing `meteva-1.8.2/meteva/method/space/acc/acc_climate_pre.py` & `meteva-1.8.3/meteva/method/space/acc/acc_climate_pre.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/im.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py` & `meteva-1.8.3/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/cra/cra.py` & `meteva-1.8.3/meteva/method/space/cra/cra.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/fqi.py` & `meteva-1.8.3/meteva/method/space/fqi/fqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/aaft2d.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/aaft2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/ampstats.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/ampstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/datagrabber_spatialVx.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/distfun.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/distfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/fft2d.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/fft2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/im.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/loc_list_setup.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/locperf.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/solutionset.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/lib/surrogater2d.py` & `meteva-1.8.3/meteva/method/space/fqi/lib/surrogater2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fqi/uiqi.py` & `meteva-1.8.3/meteva/method/space/fqi/uiqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fss/__init__.py` & `meteva-1.8.3/meteva/method/space/fss/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fss/fss.py` & `meteva-1.8.3/meteva/method/space/fss/fss.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/fss.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/fss.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/fuzzy.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/fuzzy.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/joint.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/joint.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fss2dfun.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/fss2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2d.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/thresholder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/vxstats.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/lib/vxstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/minimum_coverage.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/minimum_coverage.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/multi_event.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/multi_event.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/fuzzy_logic/pragmatic.py` & `meteva-1.8.3/meteva/method/space/fuzzy_logic/pragmatic.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geo_box_plot/GeoBoxPlot.py` & `meteva-1.8.3/meteva/method/space/geo_box_plot/GeoBoxPlot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geometric_characterizations/aindex.py` & `meteva-1.8.3/meteva/method/space/geometric_characterizations/aindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geometric_characterizations/cindex.py` & `meteva-1.8.3/meteva/method/space/geometric_characterizations/cindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py` & `meteva-1.8.3/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geometric_characterizations/sindex.py` & `meteva-1.8.3/meteva/method/space/geometric_characterizations/sindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/geometric_characterizations/spatial_index.py` & `meteva-1.8.3/meteva/method/space/geometric_characterizations/spatial_index.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/as_unitname.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distfun.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/distfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distmap.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/im.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/solutionset.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/hausdorff_metric/locperf.py` & `meteva-1.8.3/meteva/method/space/hausdorff_metric/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/__init__.py` & `meteva-1.8.3/meteva/method/space/mode/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/bearing.py` & `meteva-1.8.3/meteva/method/space/mode/bearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/censqdelta.py` & `meteva-1.8.3/meteva/method/space/mode/censqdelta.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/centmatch.py` & `meteva-1.8.3/meteva/method/space/mode/centmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/consistent.py` & `meteva-1.8.3/meteva/method/space/mode/consistent.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/data_pre.py` & `meteva-1.8.3/meteva/method/space/mode/data_pre.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/deltametric.py` & `meteva-1.8.3/meteva/method/space/mode/deltametric.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/deltamm.py` & `meteva-1.8.3/meteva/method/space/mode/deltamm.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/deltammSqCen.py` & `meteva-1.8.3/meteva/method/space/mode/deltammSqCen.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/deltamm_bak.py` & `meteva-1.8.3/meteva/method/space/mode/deltamm_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/distmap.py` & `meteva-1.8.3/meteva/method/space/mode/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_axis.py` & `meteva-1.8.3/meteva/method/space/mode/feature_axis.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_comps.py` & `meteva-1.8.3/meteva/method/space/mode/feature_comps.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_finder.py` & `meteva-1.8.3/meteva/method/space/mode/feature_finder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_match_analyzer.py` & `meteva-1.8.3/meteva/method/space/mode/feature_match_analyzer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_props.py` & `meteva-1.8.3/meteva/method/space/mode/feature_props.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/feature_table.py` & `meteva-1.8.3/meteva/method/space/mode/feature_table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/interester.py` & `meteva-1.8.3/meteva/method/space/mode/interester.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/intersect.py` & `meteva-1.8.3/meteva/method/space/mode/intersect.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/load.py` & `meteva-1.8.3/meteva/method/space/mode/load.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/loc_list_setup.py` & `meteva-1.8.3/meteva/method/space/mode/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/locperf.py` & `meteva-1.8.3/meteva/method/space/mode/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/make_SpatialVx_bak.py` & `meteva-1.8.3/meteva/method/space/mode/make_SpatialVx_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/make_spatialVx.py` & `meteva-1.8.3/meteva/method/space/mode/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/merge_force.py` & `meteva-1.8.3/meteva/method/space/mode/merge_force.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/minboundmatch.py` & `meteva-1.8.3/meteva/method/space/mode/minboundmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/operater.py` & `meteva-1.8.3/meteva/method/space/mode/operater.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/plot.py` & `meteva-1.8.3/meteva/method/space/mode/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             for x in range(len(xticks)):
                 xticks_label.append(str(round(xticks[x], 6)))
             if xticks[-1] > 0:
                 xticks_label[-1] = "   " + xticks_label[-1] + "°E"
             else:
                 xticks_label[-1] = "   " + xticks_label[-1] + "°W"
             ax.set_xticks(xticks)
-            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+            ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
 
             vmax = elat
             vmin = slat
             r = rlat
             if r <= 1:
                 inte = 0.1
             elif r <= 5 and r > 1:
@@ -229,15 +229,15 @@
                 elif yticks[y] < 0 and y == 0:
                     yticks_label.append(str(round(-yticks[y], 6)) + "°S")
                 elif yticks[y] == 0:
                     yticks_label.append("EQ" + "  ")
                 else:
                     yticks_label.append(str(round(yticks[y], 6)) + "    ")
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             if title_list is None:
                 sub_title = None
             else:
                 sub_title = title_list[p]
             add_map(ax, add_county_line=add_county_line, add_worldmap=add_worldmap, sup_fontsize=sup_fontsize,
                     title=sub_title)
             ax_list.append(ax)
```

### Comparing `meteva-1.8.2/meteva/method/space/mode/regress2.py` & `meteva-1.8.3/meteva/method/space/mode/regress2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/sma.py` & `meteva-1.8.3/meteva/method/space/mode/sma.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/tran_to_dataframe.py` & `meteva-1.8.3/meteva/method/space/mode/tran_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/mode/utils.py` & `meteva-1.8.3/meteva/method/space/mode/utils.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/point_to_area.py` & `meteva-1.8.3/meteva/method/space/point_to_area.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/kernel2dmeitsjer.py` & `meteva-1.8.3/meteva/method/space/pphindcast/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/kernel2dsmooth.py` & `meteva-1.8.3/meteva/method/space/pphindcast/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/as_unitname.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/hoods2dPrep.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/hoods2dPrep.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/im.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dsmooth.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/make_spatialVx.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/thresholder.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/thresholder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/lib/vxstats.py` & `meteva-1.8.3/meteva/method/space/pphindcast/lib/vxstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/pphindcast/pphindcast2d.py` & `meteva-1.8.3/meteva/method/space/pphindcast/pphindcast2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/rigider/fint2d.py` & `meteva-1.8.3/meteva/method/space/rigider/fint2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/rigider/fint2d_old.py` & `meteva-1.8.3/meteva/method/space/rigider/fint2d_old.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/rigider/imomenter.py` & `meteva-1.8.3/meteva/method/space/rigider/imomenter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/rigider/rigider.py` & `meteva-1.8.3/meteva/method/space/rigider/rigider.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/s1/S1.py` & `meteva-1.8.3/meteva/method/space/s1/S1.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/saller/saller.py` & `meteva-1.8.3/meteva/method/space/saller/saller.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/LocSig.py` & `meteva-1.8.3/meteva/method/space/significance/LocSig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/bootstrap.py` & `meteva-1.8.3/meteva/method/space/significance/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/bootstrap_ci.py` & `meteva-1.8.3/meteva/method/space/significance/bootstrap_ci.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/is_sig.py` & `meteva-1.8.3/meteva/method/space/significance/is_sig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/sig_coverage.py` & `meteva-1.8.3/meteva/method/space/significance/sig_coverage.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/significance.py` & `meteva-1.8.3/meteva/method/space/significance/significance.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/spatbiasFS.py` & `meteva-1.8.3/meteva/method/space/significance/spatbiasFS.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/significance/tsboot.py` & `meteva-1.8.3/meteva/method/space/significance/tsboot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/uqi/uqi.py` & `meteva-1.8.3/meteva/method/space/uqi/uqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/vgm/rdist.py` & `meteva-1.8.3/meteva/method/space/vgm/rdist.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/vgm/structurogram.py` & `meteva-1.8.3/meteva/method/space/vgm/structurogram.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/space/vgm/structurogram_matrix.py` & `meteva-1.8.3/meteva/method/space/vgm/structurogram_matrix.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/weather_system/identify.py` & `meteva-1.8.3/meteva/method/weather_system/identify.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import json
 import traceback
 import numpy as np
 import pandas as pd
 import meteva
 import matplotlib.pyplot as plt
 import pkg_resources
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import xarray as xr
 
 
 def set_jar_path(path):
     if os.path.exists(path):
         meteva.base.ws_jar_path = path
         meteva.base.height_oy = os.path.split(path)[0] +"\\height_oy.nc"
@@ -219,14 +217,16 @@
             "h_nlon": grid_h.nlon, "h_nlat": grid_h.nlat,
             "h_slon": grid_h.slon, "h_slat": grid_h.slat,
             "h_dlon": grid_h.dlon, "h_dlat": grid_h.dlat,
             "h_data": h_data
             }
     para_json = json.dumps(para)
 
+
+
     str_json = java_class_func(meteva.base.ws_jar_path,"Jpype","ws",None,para_json)
     if str_json !="null" and len(str_json)>0:
         graphy = json.loads(str_json)
         return graphy
     else:
         return None
 
@@ -245,14 +245,18 @@
             "h_nlon": grid_h.nlon, "h_nlat": grid_h.nlat,
             "h_slon": grid_h.slon, "h_slat": grid_h.slat,
             "h_dlon": grid_h.dlon, "h_dlat": grid_h.dlat,
             "h_data": h_data
             }
     para_json = json.dumps(para)
 
+    # file1 = open(r"H:\task\develop\java\sysIdentify\para_json.txt","w")
+    # file1.write(para_json)
+    # file1.close()
+
     str_json = java_class_func(meteva.base.ws_jar_path,"Jpype","ws",None,para_json)
     if str_json !="null" and len(str_json)>0:
         graphy = json.loads(str_json)
         return graphy
     else:
         return None
```

### Comparing `meteva-1.8.2/meteva/method/yes_or_no/__init__.py` & `meteva-1.8.3/meteva/method/yes_or_no/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/yes_or_no/plot.py` & `meteva-1.8.3/meteva/method/yes_or_no/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
-from meteva.method.yes_or_no.score import *
 import meteva
+from meteva.method.yes_or_no.score import *
+
 
 
 def performance(ob, fo,grade_list=[1e-30],compare =">=",compair = None, member_list=None,x_y = "sr_pod", save_path=None,show = False,dpi = 300, title="综合表现图",
                 sup_fontsize =10,width = None,height = None):
     '''
 
     :param ob:
```

### Comparing `meteva-1.8.2/meteva/method/yes_or_no/score.py` & `meteva-1.8.3/meteva/method/yes_or_no/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/yes_or_no/skill.py` & `meteva-1.8.3/meteva/method/yes_or_no/skill.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/method/yes_or_no/table.py` & `meteva-1.8.3/meteva/method/yes_or_no/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/perspact/middel_high.py` & `meteva-1.8.3/meteva/perspact/middel_high.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,48 +24,47 @@
         "read_method": meteva.base.read_griddata_from_nc,
         "read_para": {},
         "time_type": "UT",  # 实况数据时间类型
         "multiple": 1,  # 当文件数据的单位是位势米，通过乘以9.8转换成位势
         }
     },
     "fo_data": {
-        "ECMWF":{
-            "dirm": r"\\10.28.16.234\data2\AI\ECMWF\grib\YYMMDD\YYMMDDHH.TTT.grib",
+        "Fu":{
+            "dirm": r"\\10.28.16.234\data2\AI\fuxi\Z\LLL\YYYYMMDDHH\YYYYMMDDHH.TTT.nc",
             "dtime": [12, 240, 12],
-            "read_method": meteva.base.read_griddata_from_grib,
-            "read_para": {"level_type":"isobaricInhPa","value_name":"gh"},
+            "read_method": meteva.base.read_griddata_from_nc,
+            "read_para": {},
             "time_type": "UT",  # 预报数据时间类型是北京时，即08时起报
             "multiple": 1,  # 当文件数据的单位是位势米，通过乘以9.8转换成位势
             "move_fo_time":0,
-            "veri_by":"self"
+            "veri_by":"CRA40"
         },
 
-        "NMC1": {
-            "dirm":  r"\\10.28.16.177\NMC_Tsinghua_reforecast\cra40\YYYYMMDDHH.nc",
+        "pa": {
+            "dirm":   r"\\10.28.16.234\data2\AI\Pangu_ERA5\Z\LLL\YYYYMMDDHH\YYYYMMDDHH.TTT.nc",
             "dtime": [12, 240, 12],
             "read_method": meteva.base.read_griddata_from_nc,
-            "read_para": {"value_name": "GPH"},
+            "read_para": {},
             "time_type": "UT",#预报数据时间类型是北京时，即08时起报
             "multiple":1, #当文件数据的单位是位势米，通过乘以9.8转换成位势
             "move_fo_time": 12,
             "veri_by": "CRA40"
         },
     },
 }
 
 
-
 def middle_of_score(para):
     middle_result_path = para["middle_result_path"]
     meteva.base.creat_path(middle_result_path)
     model_name_list = list(para["fo_data"].keys())
     mid_method = para["mid_method"]
     grid0 = para["grid"]
     # grid0 = meteva.base.grid([0,359.75,0.25],[-89.75,89.75,0.25])
-    marker = meteva.perspact.get_grid_marker(grid0, step=10)
+    marker = meteva.perspact.get_grid_marker(grid0, step=para["step"])
     # marker = None
     level_list =para["level_list"]
     mid_list = []
     # 创建一个空的DataFrame，用来记录哪些中间量已经收集
     df1 = pd.DataFrame(data=None, columns=['level', 'time', 'dtime', 'member'])
     if os.path.exists(middle_result_path):
         if not para["recover"]:
@@ -150,30 +149,26 @@
                             if save_k % 500 == 0:
                                 mid_all = meteva.base.concat(mid_list)
                                 # 先删除文件在重新输出文件，避免文件大小膨胀
                                 if os.path.exists(middle_result_path):
                                     os.remove(middle_result_path)
                                 mid_all.to_hdf(middle_result_path, "df")  # 将结果输出到文件
 
-                # 在统计时段内时间递增，遍历所有时间。在程序调试阶段，参数hours的取值可以设得大一点，比如2400，全年先算个几天看看结果是否合理,如果合理再改成240，再看结果合理再改成24，或12
-                time1 = time1 + datetime.timedelta(hours=para["time_step"])
+
+            time1 = time1 + datetime.timedelta(hours=para["time_step"])
     mid_all = meteva.base.concat(mid_list)
     # 先删除文件在重新输出文件，避免文件大小膨胀
     if os.path.exists(middle_result_path):
         os.remove(middle_result_path)
     mid_all.to_hdf(middle_result_path, "df")  # 将结果输出到文件
     print("中间量统计程序运行完毕")
     print("中间结果已输出至"+middle_result_path)
     return
 
 
+
+
+
 if __name__ == "__main__":
-    # path = meteva.base.get_path(r"\\10.28.16.234\data2\AI\ECMWF\grib\YYMMDD\YYMMDDHH.TTT.grib",datetime.datetime(2018,1,1,0))
-    # #meteva.base.print_grib_file_info(path,filter_by_keys={"typeOfLevel":"isobaricInhPa"})
-    #
-    # grd = meteva.base.read_griddata_from_grib(path,level_type="isobaricInhPa",value_name="gh",level=[850,500])
-    #print(grd)
-    middle_of_score(para)
-    path = r"H:\test_data\output\mps\tase_z.h5"
-    df = pd.read_hdf(path)
-    print(df)
-    meteva.perspact.score_df(df,meteva.method.rmse,g = ["member","dtime"],plot = "line")
+
+
+    pass
```

### Comparing `meteva-1.8.2/meteva/perspact/middle_prepare.py` & `meteva-1.8.3/meteva/perspact/middle_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,19 @@
         method_args["grade_list"] = grade_list
     if compare is not None:
         method_args["compare"] = compare
     grade_exp = None
     names_exp = None
     group_name = None
     if need_g:
+        #may be some id in gid is not in sta_all,valid group is not same as group in grid
+        sta_all_id = copy.deepcopy(sta_all[["id"]])
+        sta_all_id.drop_duplicates()
+        sta = meteva.base.combine_on_id(gid,sta_all_id,how="inner")
+        gid = sta
         group_name = gid.columns[1]
         groups = gid[group_name]
         groups = groups.drop_duplicates(keep = "first")
         names = groups.values
         gll = []
         for i in range(len(names)):
             ids = gid.loc[gid[group_name] == names[i]].values[:, 0]
@@ -550,15 +555,15 @@
 def tran_middle_df_to_ds(df_all,mid_columns = None):
     '''
 
     :param df_all:
     :param mid_columns: 中间数据对应的列名称，列表形式
     :return:
     '''
-
+    print("该函数有bug，在相邻格点取值完全相同时，会产生nan")
     all_columns = df_all.columns
     if mid_columns is None:
 
         list_list = method_coluns_dict.values()
         for list1 in list_list:
             eq = True
             for c in range(1,len(list1)+1):
```

### Comparing `meteva-1.8.2/meteva/perspact/multi_element_veri.py` & `meteva-1.8.3/meteva/perspact/multi_element_veri.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/perspact/score.py` & `meteva-1.8.3/meteva/perspact/score.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 
 # 实现任意纬度分类的函数
 def score_df(df, method, s = None,g=None,gll_dict = None,plot = None,excel_path = None,first = True,**kwargs):
     '''
 
     :param df:
     :param method:
+    :param s:
     :param g:
+    :param gll_dict:
+    :param plot:
+    :param excel_path:
+    :param first:  first参数不是面对用户的，是程序自我递归调用时用到的参数
+    :param kwargs:
     :return:
     '''
     method_name = method.__name__
 
     method_mid = meteva.perspact.get_middle_method(method)
     column_list = meteva.perspact.get_middle_columns(method_mid)
     score_method_with_mid = meteva.perspact.get_score_method_with_mid(method)
@@ -112,15 +118,20 @@
                 if g[gg] in g_time:
                     _,gll = meteva.base.group(df1,g = g[gg])
                     gll.sort()
                 else:
                     #为了保持原有排序，不用group函数
                     groups = df1[g[gg]]
                     groups = groups.drop_duplicates(keep="first")
-                    gll = groups.values
+                    gll = groups.values.tolist()
+                    if not  isinstance(gll[0],str):
+                        if g[gg] =="level":
+                            gll.sort(reverse=True)
+                        else:
+                            gll.sort()
 
                 gll_dict[g[gg]] = gll
 
         # 将分组方式统一成单层列表，或者两层列表
         gll_dict1 = {}
         for gg in range(len(g)):
             list_list = gll_dict[g[gg]]
@@ -140,15 +151,14 @@
             gll_dict1[g[gg]] = list_list1
         gll_dict = gll_dict1
 
         #取出第一个分类维度的分类方式备用
         gll0 = gll_dict[g[0]]
 
     g0 = g[0]
-
     df1_list, gll = meteva.base.group(df1, g=g0, gll=gll0)
     if len(g) == 1:
         score_list = []
         gll_i_dict ={}
         score1 = None
         for i in range(len(df1_list)):
             if method_mid == meteva.method.tmmsss:
@@ -191,19 +201,20 @@
                     score2 = score1 * 0 + meteva.base.IV
                 score_list_with_iv.append(score2)
 
         score_array = np.array(score_list_with_iv)
         if method_name.find("ob_fo_")>=0:
              score_array = score_array[...,1,0]
 
-
-        if plot =="line" or plot =="bar":
+        if plot =="line" or plot =="bar" or plot =="barh":
             meteva.base.plot_tools.plot_bar(plot,score_array,name_list_dict=gll_dict,**kwargs)
-        if plot =="mesh":
-            meteva.base.plot_tools.mesh(score_array,name_list_dict=gll_dict,**kwargs)
+        if plot =="mesh" or plot =="contour":
+            meteva.base.plot_tools.mesh_contour(plot,score_array, name_list_dict=gll_dict, **kwargs)
+        if plot =="lineh":
+            meteva.base.plot_tools.lineh(score_array,name_list_dict=gll_dict,**kwargs)
         return  score_array,gll_dict
     else:
         if len(g) == 2:
             g_left = g[1]
         else:
             g_left = g[1:]
 
@@ -226,18 +237,20 @@
                 score2 = score_all_list[gll_i_dict[gll_str]]
             else:
                 score2 = score_array * 0 + meteva.base.IV
             score_list_with_iv.append(score2)
         score_all_array = np.array(score_list_with_iv)
 
 
-        if plot =="line" or plot =="bar":
+        if plot =="line" or plot =="bar" or plot == "barh":
             meteva.base.plot_tools.plot_bar(plot, score_all_array, name_list_dict=gll_dict, **kwargs)
-        if plot =="mesh":
-            meteva.base.plot_tools.mesh( score_all_array, name_list_dict=gll_dict, **kwargs)
+        if plot =="mesh" or plot =="contour":
+            meteva.base.plot_tools.mesh_contour(plot,score_all_array, name_list_dict=gll_dict, **kwargs)
+        if plot =="lineh":
+            meteva.base.plot_tools.lineh( score_all_array, name_list_dict=gll_dict, **kwargs)
 
         if excel_path is not None:
             meteva.base.write_array_to_excel(score_all_array,excel_path,gll_dict)
 
         return score_all_array,gll_dict
 
 def sele_by_dict(ds0,s):
@@ -793,170 +806,402 @@
         score_all_array = np.array(score_list_with_iv)
         score_all_array[np.isnan(score_all_array)] = meteva.base.IV
         if plot is not None: meteva.base.plot_tools.plot_bar(plot, score_all_array, name_list_dict=gll_dict, **kwargs)
 
         return score_all_array, gll_dict
 
 
-def score_xy_df(df_mid,method,s = None,g = None,gll_dict = None,save_path = None,**kwargs):
+def score_xy_df(df_mid,method,s = None,g = None,gll_dict = None,save_path = None,plot = True,**kwargs):
 
     g_list = []
     if isinstance(g,list):
         if len(g)>1:
             print("score_xy_df函数暂时不支持多维分类功能")
             return
         else:
             g_list = g
     else:
         if g is not None:
             g_list = [g]
-    g_list.append("id")
+    #g_list.append("id")
+    g_list.append("lon")
+    g_list.append(("lat"))
 
     if s is not None:
         if "member" in s.keys():
             df_mid  = df_mid.loc[df_mid['member'].isin(s["member"])]
             s.pop("member")
         if "grade" in s.keys():
             df_mid = df_mid.loc[df_mid['grade']== s["grade"]]
             s.pop("grade")
 
 
+    region_ids = df_mid["id"]
+    max_id = np.max(region_ids)
+    min_id = np.min(region_ids)
+    max_ = max(max_id, abs(min_id))
+    if max_ < 1000000:
+        lat = np.round(region_ids / 1000)
+        lon = region_ids - lat * 1000
+    else:
+        lat = np.round(region_ids / 10000)
+        lon = region_ids - lat * 10000
+        lon /= 10
+        lat /= 10
+    df_mid["lon"] =lon
+    df_mid["lat"] =lat
+
     #print(df_mid)
     df_mid = meteva.base.sele_by_dict(df_mid, s)
+    if len(df_mid.index)==0:
+        print("no middle data had been seleted")
+        return None
     score_array,g_dict =score_df(df_mid,method,g = g_list,gll_dict = gll_dict)
-    grd_list = []
 
     g_time = ["time","year","month","day","hour","minute","dtime","xun","hou",
               "ob_time","ob_year","ob_month","ob_day","ob_hour","ob_minute","ob_xun","ob_hou"]
 
-    region_ids = g_dict["id"]
-    max_id = np.max(region_ids)
-    min_id = np.min(region_ids)
-    max_ = max(max_id,abs(min_id))
-    if max_ <1000000:
-        lat = np.round(region_ids  / 1000)
-        lon = region_ids - lat * 1000
-    else:
-        lat = np.round(region_ids / 10000)
-        lon = region_ids - lat * 10000
-        lon /=10
-        lat /=10
+    # region_ids = g_dict["id"]
+    # if region_ids is not None:
+    #     region_ids = np.array(region_ids)
+    # max_id = np.max(region_ids)
+    # min_id = np.min(region_ids)
+    # max_ = max(max_id,abs(min_id))
+    # if max_ <1000000:
+    #     lat = np.round(region_ids  / 1000)
+    #     lon = region_ids - lat * 1000
+    # else:
+    #     lat = np.round(region_ids / 10000)
+    #     lon = region_ids - lat * 10000
+    #     lon /=10
+    #     lat /=10
     grd_list = []
     gnames0 = None
-    if len(g_list) == 1:
-        dict1 = {"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],
-            "id": region_ids, "lon": lon, "lat": lat,  "score": score_array}
-        df = pd.DataFrame(dict1)
-        score_sta = meteva.base.sta_data(df)
-        score_grd = meteva.base.trans_sta_to_grd(score_sta)
+    if len(g_list) == 2:
+        # dict1 = {"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],
+        #     "id": region_ids, "lon": lon, "lat": lat,  "score": score_array}
+        # df = pd.DataFrame(dict1)
+        # score_sta = meteva.base.sta_data(df)
+        # score_grd = meteva.base.trans_sta_to_grd(score_sta)
+        grd1 = xr.DataArray(score_array,coords=[("lon",g_dict["lon"]),("lat",g_dict["lat"])])
+        score_grd = meteva.base.xarray_to_griddata(grd1)
         grd_list.append(score_grd)
-        #score_grd.values[score_grd.values == meteva.base.IV] = 0
-        #meteva.base.plot_tools.contourf_2d_grid(score_grd, save_path,**kwargs)
-        #return [score_grd],None
-    elif len(g_list) == 2:
+
+    elif len(g_list) == 3:
 
         gnames0 = g_dict[g_list[0]]
         #print(gnames0)
         ng0 = len(gnames0)
-        if g_list[0] =="grade":
-            grd_list = []
-            vmin = 10e30
-            vmax = -10e30
-            for i in range(ng0):
-                name = gnames0[i]
-                value = score_array[i,:]
-                df = pd.DataFrame({"level": df_mid["level"].values[0], "time": df_mid["time"].values[0],
-                                   "dtime": df_mid["dtime"].values[0], "id": region_ids,
-                                   "lon": lon, "lat": lat, name: value})
-                score_sta = meteva.base.sta_data(df)
-
-                score_grd = meteva.base.trans_sta_to_grd(score_sta)
-                score_grd.values[score_grd.values == meteva.base.IV] = 0
-                grd_list.append(score_grd)
-
-                # vmax1 = np.max(score_grd.values)
-                # vmin1 = np.max(score_grd.values)
-                # if vmax1 > vmax: vmax = vmax1
-                # if vmin1 < vmin: vmin = vmin1
-
-            #meteva.base.plot_tools.plot_2d_grid_list(grd_list,save_path=save_path,vmax=vmax,vmin = vmin,**kwargs)
-
-        elif g_list[0] in g_time:
-            for i in range(ng0):
-                #name = gnames0[i]
-                value = score_array[i, :]
-
-                dict1 = {"id": region_ids, "lon": lon, "lat": lat,  "score": value}
-                if "level" not in dict1:
-                    dict1["level"] = df_mid["level"].values[0]
-                if "time" not in dict1:
-                    dict1["time"] = df_mid["time"].values[0]
-                if "dtime" not in dict1:
-                    dict1["dtime"] = df_mid["dtime"].values[0]
-                df = pd.DataFrame(dict1)
-                score_sta = meteva.base.sta_data(df)
-                score_grd = meteva.base.trans_sta_to_grd(score_sta)
-                grd_list.append(score_grd)
-                #title_list.append(g_list[0] + ":" + str(name))
-            #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
-        else:
-            for i in range(ng0):
-                name = gnames0[i]
-                value = score_array[i,:]
-                if g_list[0] == "member":
-                    df = pd.DataFrame({"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],"id":region_ids,
-                                       "lon": lon, "lat": lat, name: value})
-                else:
-                    dict1 = {"id":region_ids,"lon":lon,"lat":lat,g_list[0]:name,"score":value}
-                    if "level" not in dict1:
-                        dict1["level"] = df_mid["level"].values[0]
-                    if "time" not in dict1:
-                        dict1["time"] = df_mid["time"].values[0]
-                    if "dtime" not in dict1:
-                        dict1["dtime"] = df_mid["dtime"].values[0]
-                    df = pd.DataFrame(dict1)
-                score_sta = meteva.base.sta_data(df)
-
-                score_grd = meteva.base.trans_sta_to_grd(score_sta)
-                grd_list.append(score_grd)
-            score_grd = meteva.base.concat(grd_list)
-            #title_list = score_grd.coords[g_list[0]].values.tolist()
-            #kwargs["title"]  = title
-            #score_grd.values[score_grd.values == meteva.base.IV] = 0
-            #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
+        for i in range(ng0):
+            grd1 = xr.DataArray(score_array[i,:], coords=[("lon", g_dict["lon"]), ("lat", g_dict["lat"])])
+            score_grd = meteva.base.xarray_to_griddata(grd1)
+            meteva.base.set_griddata_coords(score_grd,member_list=[gnames0[i]])
+            grd_list.append(score_grd)
+
+
+        # if g_list[0] =="grade":
+        #     grd_list = []
+        #     vmin = 10e30
+        #     vmax = -10e30
+        #     for i in range(ng0):
+        #         name = gnames0[i]
+        #         value = score_array[i,:]
+        #         df = pd.DataFrame({"level": df_mid["level"].values[0], "time": df_mid["time"].values[0],
+        #                            "dtime": df_mid["dtime"].values[0], "id": region_ids,
+        #                            "lon": lon, "lat": lat, name: value})
+        #         score_sta = meteva.base.sta_data(df)
+        #
+        #         score_grd = meteva.base.trans_sta_to_grd(score_sta)
+        #         score_grd.values[score_grd.values == meteva.base.IV] = 0
+        #         grd_list.append(score_grd)
+        #
+        #         # vmax1 = np.max(score_grd.values)
+        #         # vmin1 = np.max(score_grd.values)
+        #         # if vmax1 > vmax: vmax = vmax1
+        #         # if vmin1 < vmin: vmin = vmin1
+        #
+        #     #meteva.base.plot_tools.plot_2d_grid_list(grd_list,save_path=save_path,vmax=vmax,vmin = vmin,**kwargs)
+        #
+        # elif g_list[0] in g_time:
+        #     for i in range(ng0):
+        #         #name = gnames0[i]
+        #         value = score_array[i, :]
+        #
+        #         dict1 = {"id": region_ids, "lon": lon, "lat": lat,  "score": value}
+        #         if "level" not in dict1:
+        #             dict1["level"] = df_mid["level"].values[0]
+        #         if "time" not in dict1:
+        #             dict1["time"] = df_mid["time"].values[0]
+        #         if "dtime" not in dict1:
+        #             dict1["dtime"] = df_mid["dtime"].values[0]
+        #         df = pd.DataFrame(dict1)
+        #         score_sta = meteva.base.sta_data(df)
+        #         score_grd = meteva.base.trans_sta_to_grd(score_sta)
+        #         grd_list.append(score_grd)
+        #         #title_list.append(g_list[0] + ":" + str(name))
+        #     #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
+        # else:
+        #     for i in range(ng0):
+        #         name = gnames0[i]
+        #         value = score_array[i,:]
+        #         if g_list[0] == "member":
+        #             df = pd.DataFrame({"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],"id":region_ids,
+        #                                "lon": lon, "lat": lat, name: value})
+        #         else:
+        #             dict1 = {"id":region_ids,"lon":lon,"lat":lat,g_list[0]:name,"score":value}
+        #             if "level" not in dict1:
+        #                 dict1["level"] = df_mid["level"].values[0]
+        #             if "time" not in dict1:
+        #                 dict1["time"] = df_mid["time"].values[0]
+        #             if "dtime" not in dict1:
+        #                 dict1["dtime"] = df_mid["dtime"].values[0]
+        #             df = pd.DataFrame(dict1)
+        #         score_sta = meteva.base.sta_data(df)
+        #
+        #         score_grd = meteva.base.trans_sta_to_grd(score_sta)
+        #         grd_list.append(score_grd)
+        #     score_grd = meteva.base.concat(grd_list)
+        #     #title_list = score_grd.coords[g_list[0]].values.tolist()
+        #     #kwargs["title"]  = title
+        #     #score_grd.values[score_grd.values == meteva.base.IV] = 0
+        #     #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
+
+
+    if plot:
+        grd_list_plot = []
+        for i in range(len(grd_list)):
+            score_grd = grd_list[i].copy()
+            score_grd.values[score_grd.values == meteva.base.IV] = 0
+            grd_list_plot.append(score_grd)
+        if gnames0 is None:
+            title_list = None
+        else:
+            title_list = []
+            for i in range(len(gnames0)):
+                title_list.append(str(gnames0[i]))
+            kwargs["title"] = title_list
+        meteva.base.plot_tools.plot_2d_grid_list(grd_list_plot, save_path = save_path, **kwargs)
+
+    return grd_list,gnames0
 
 
+def score_xy_df_delta(df_mid,method,reference_member,s = None,gll_dict = None,save_path = None,cmap ="me_bwr",**kwargs):
+    '''
+    绘制多个模式预报评分相对其中某一个模式的评分的正负技巧
+    :param df_mid:
+    :param method:
+    :param reference_member:
+    :param s:
+    :param save_path:
+    :param kwargs:
+    :return:
+    '''
+    grd_list, gnames0 = score_xy_df(df_mid,method,s = s,g = "member",gll_dict=gll_dict,plot = False)
+    grd_ref = None
+    for i in range(len(gnames0)):
+        if reference_member == gnames0[i]:
+            grd_ref = copy.deepcopy(grd_list[i])
+    if grd_ref is None:
+        print(reference_member + " not exist in DataFrame of middle result")
+
+    for i in range(len(grd_list)):
+        grd_list[i].values -= grd_ref.values
+
     grd_list_plot = []
     for i in range(len(grd_list)):
         score_grd = grd_list[i].copy()
         score_grd.values[score_grd.values == meteva.base.IV] = 0
         grd_list_plot.append(score_grd)
-    if gnames0 is None:
-        title_list = None
-    else:
-        title_list = []
-        for i in range(len(gnames0)):
-            title_list.append(str(gnames0[i]))
-        kwargs["title"] = title_list
-    meteva.base.plot_tools.plot_2d_grid_list(grd_list_plot, type="mesh", save_path = save_path, **kwargs)
+
+    title_list = []
+    for i in range(len(gnames0)):
+        title_list.append(str(gnames0[i]))
+    kwargs["title"] = title_list
+    meteva.base.plot_tools.plot_2d_grid_list(grd_list_plot,  save_path = save_path,cmap=cmap, **kwargs)
 
     return grd_list,gnames0
 
 
-if __name__ =="__main__":
-    import pandas as pd
-    #path = r"O:\data\hdf\gongbao\wind3h_update12h_station2k\wind3h_update12h_station2k.h5"
-    path = r"H:/a.txt"
-    uv = pd.read_hdf(path)
-    uv = meteva.base.sele_by_para(uv,time_range = ["2022081408","2022081720"],dtime = [12,24,36,48])
-    uv = meteva.base.in_member_list(uv,member_list=[0,1,2,3,4,5],name_or_index="index")
-    #uv.to_hdf(r"H:\test_data\input\mps\wind.h5","df")
-
-    speed,_ = meteva.base.wind_to_speed_angle(uv)
-    df = meteva.perspact.middle_df_sta(speed,meteva.method.nasws_s)
-    score = meteva.perspact.score_df(df,meteva.method.acs,g = "member")
-    #print(score)
-    score = meteva.product.score(speed,meteva.method.acs)
-    print(score)
-    pass
+def score_xz_df(df_mid,method,s = None,g = None,gll_dict = None,save_path = None,plot = True,**kwargs):
+    g_list = []
+    if isinstance(g,list):
+        if len(g)>1:
+            print("score_xz_df函数暂时不支持多维分类功能")
+            return
+        else:
+            g_list = g
+    else:
+        if g is not None:
+            g_list = [g]
 
+    g_list.append("lon")
+    g_list.append("level")
+    if s is not None:
+        if "member" in s.keys():
+            df_mid  = df_mid.loc[df_mid['member'].isin(s["member"])]
+            s.pop("member")
+        if "grade" in s.keys():
+            df_mid = df_mid.loc[df_mid['grade']== s["grade"]]
+            s.pop("grade")
+
+
+    #print(df_mid)
+
+    ids = df_mid["id"] #所有格点的编号
+    max_id = np.max(ids)
+    min_id = np.min(ids)
+    max_ = max(max_id, abs(min_id))
+    if max_ < 1000000:
+        lat = np.round(ids / 1000)
+        lon = ids - lat * 1000
+    else:
+        lat = np.round(ids / 10000)
+        lon = ids - lat * 10000
+        lon /= 10
+        lat /= 10
+    df_mid["lon"] = lon
+    df_mid["lat"] = lat
+    df_mid = meteva.base.sele_by_dict(df_mid, s)
 
+    score_array,g_dict =score_df(df_mid,method,g = g_list,gll_dict = gll_dict)
+
+    coords = []
+    for g1 in g_dict.keys():
+        coords.append((g1,g_dict[g1]))
+    da = xr.DataArray(score_array,coords=coords)
+    grd = meteva.base.xarray_to_griddata(da)
+    if plot:meteva.base.contourf_xz(grd, save_path=save_path,**kwargs)
+    return grd
+
+
+def score_xz_df_delta(df_mid,method,reference_member,s = None,gll_dict = None,save_path = None,cmap ="me_bwr",sup_title = "",**kwargs):
+    '''
+    绘制多个模式预报评分相对其中某一个模式的评分的正负技巧
+    :param df_mid:
+    :param method:
+    :param reference_member:
+    :param s:
+    :param save_path:
+    :param kwargs:
+    :return:
+    '''
+    grd = score_xz_df(df_mid,method,s = s,g = "member",gll_dict=gll_dict,plot = False)
+    grd_delta = copy.deepcopy(grd)
+    member = grd["member"].values
+    for i in range(member.size):
+        if reference_member==member[i]:
+            grd_delta.values[:] -= grd.values[i,:]
+
+    meteva.base.contourf_xz(grd_delta, save_path=save_path,cmap = cmap,sup_title=sup_title,**kwargs)
+    return grd_delta
+
+def score_yz_df(df_mid, method, s=None, g=None, gll_dict=None, save_path=None,plot = True,sup_title = "", **kwargs):
+    g_list = []
+    if isinstance(g, list):
+        if len(g) > 1:
+            print("score_xz_df函数暂时不支持多维分类功能")
+            return
+        else:
+            g_list = g
+    else:
+        if g is not None:
+            g_list = [g]
+
+    g_list.append("lat")
+    g_list.append("level")
+    if s is not None:
+        if "member" in s.keys():
+            df_mid = df_mid.loc[df_mid['member'].isin(s["member"])]
+            s.pop("member")
+        if "grade" in s.keys():
+            df_mid = df_mid.loc[df_mid['grade'] == s["grade"]]
+            s.pop("grade")
+
+
+    ids = df_mid["id"]  # 所有格点的编号
+    max_id = np.max(ids)
+    min_id = np.min(ids)
+    max_ = max(max_id, abs(min_id))
+    if max_ < 1000000:
+        lat = np.round(ids / 1000)
+        lon = ids - lat * 1000
+    else:
+        lat = np.round(ids / 10000)
+        lon = ids - lat * 10000
+        lon /= 10
+        lat /= 10
+    df_mid["lat"] = lat
+    df_mid["lon"] = lon
+    # print(df_mid)
+    df_mid = meteva.base.sele_by_dict(df_mid, s)
+
+    score_array, g_dict = score_df(df_mid, method, g=g_list, gll_dict=gll_dict)
+
+    coords = []
+    for g1 in g_dict.keys():
+        coords.append((g1, g_dict[g1]))
+    da = xr.DataArray(score_array, coords=coords)
+
+    grd = meteva.base.xarray_to_griddata(da)
+    if plot :meteva.base.contourf_yz(grd, save_path=save_path,sup_title=sup_title, **kwargs)
+    return grd
+
+
+def score_tdt_df(df_mid, method, s=None, g=None, gll_dict=None, save_path=None,sup_title = "", **kwargs):
+    g_list = []
+    if isinstance(g, list):
+        if len(g) > 1:
+            print("score_tdt_df函数暂时不支持多维分类功能")
+            return
+        else:
+            g_list = g
+    else:
+        if g is not None:
+            g_list = [g]
+
+    g_list.append("dtime")
+    g_list.append("time")
+
+    result = score_df(df_mid,method,s = s,g= g_list,gll_dict=gll_dict,save_path = save_path,plot="mesh",sup_title=sup_title,**kwargs)
+    return result
+
+
+def score_tdt_df_delta(df_mid, method,reference_member, s=None, gll_dict=None,cmap ="me_bwr", **kwargs):
+
+    g_list=["member","dtime","time"]
+    score_array,gll_dict = score_df(df_mid,method,s = s,g= g_list,gll_dict=gll_dict)
+    member = gll_dict["member"]
+    for i in range(len(member)):
+        if reference_member == member[i]:
+            score_array[:] -= score_array[i, :]
+    meteva.base.plot_tools.mesh_contour("mesh", score_array, name_list_dict=gll_dict,cmap=cmap, **kwargs)
+    return score_array,gll_dict
+
+def score_yz_df_delta(df_mid,method,reference_member,s = None,gll_dict = None,save_path = None,cmap ="me_bwr",sup_title = "",**kwargs):
+    '''
+    绘制多个模式预报评分相对其中某一个模式的评分的正负技巧
+    :param df_mid:
+    :param method:
+    :param reference_member:
+    :param s:
+    :param save_path:
+    :param kwargs:
+    :return:
+    '''
+    grd = score_yz_df(df_mid,method,s = s,g = "member",gll_dict=gll_dict,plot = False)
+    grd_delta = copy.deepcopy(grd)
+    member = grd["member"].values
+    for i in range(member.size):
+        if reference_member==member[i]:
+            grd_delta.values[:] -= grd.values[i,:]
+    meteva.base.contourf_yz(grd_delta, save_path=save_path,cmap = cmap,sup_title=sup_title,**kwargs)
+    return grd_delta
+
+
+if __name__ =="__main__":
+    #
+    path = r"H:\task\other\202308-AImodel\mid\z500_tmmsss_ec.h5"
+    df = pd.read_hdf(path)
+
+    score_xy_df_delta(df,method=meteva.method.ob_fo_std,reference_member="OBS",save_path=r"H:\task\other\202308-AImodel\mid\me_test_.png",
+                     s = {"member":["ECMWF","CMA_GFS"]},
+                      gll_dict={"member":["OBS","CMA_GFS","ECMWF"]})
```

### Comparing `meteva-1.8.2/meteva/product/application/__init__.py` & `meteva-1.8.3/meteva/product/application/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/data_collection.py` & `meteva-1.8.3/meteva/product/application/data_collection.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/data_distribute.py` & `meteva-1.8.3/meteva/product/application/data_distribute.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/data_prepare.py` & `meteva-1.8.3/meteva/product/application/data_prepare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/fun.py` & `meteva-1.8.3/meteva/product/application/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/terrain_height_correction.py` & `meteva-1.8.3/meteva/product/application/terrain_height_correction.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/application/time_compare.py` & `meteva-1.8.3/meteva/product/application/time_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/__init__.py` & `meteva-1.8.3/meteva/product/program/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/diurnal.py` & `meteva-1.8.3/meteva/product/program/diurnal.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/error_ana_list.py` & `meteva-1.8.3/meteva/product/program/error_ana_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签\
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
-import math
 import meteva
+import math
 import json
 
 def error_boxplot(sta_ob_and_fos0,s = None, g = None, gll=None,
                   group_name_list=None,threshold = 2,save_dir=None,save_path = None,show = False,dpi = 200,title="误差综合分析图",
                   vmin  = None,vmax = None,spasify_xticks = None,sup_fontsize =10,width = None,height = None,json_dir = None,json_path = None,
                   **kwargs):
     '''
```

### Comparing `meteva-1.8.2/meteva/product/program/error_ana_scatter.py` & `meteva-1.8.3/meteva/product/program/error_ana_scatter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/fun.py` & `meteva-1.8.3/meteva/product/program/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/plot.py` & `meteva-1.8.3/meteva/product/program/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/process_compare.py` & `meteva-1.8.3/meteva/product/program/process_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import meteva
 import math
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import datetime
 
 
 def process_compare(ob_list ,fo_list_list ,map_extend = None ,width = 12 ,dpi = 300 ,sup_title = None ,sup_fontsize = 10,
                     add_county_line = False ,add_worldmap = True, xticks_inter = None ,yticks_inter = None ,grid = True,
                     linewidth = [0.3 ,0.3 ,0.2] ,color = ["k" ,"k" ,"k"] ,cmap ="rainbow" ,clevs= None ,save_path = None):
     nrow = len(fo_list_list) + 1
@@ -185,21 +183,21 @@
 
         ax = plt.axes(rect1)
         ax.set_xlim((slon, elon))
         ax.set_ylim((slat, elat))
 
         if i == 0:
             ax.set_yticks(yticks)
-            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+            ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
         else:
             ax.set_yticks(yticks)
-            ax.set_yticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+            ax.set_yticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
 
         ax.set_xticks(xticks)
-        ax.set_xticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+        ax.set_xticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
         im = meteva.base.add_contourf(ax, ob_list[i], add_colorbar=False, cmap=cmap, cut_colorbar=False)
         if grid: plt.grid(linestyle="--", linewidth=0.5)
         meteva.base.tool.plot_tools_adv.add_map(ax, add_county_line=add_county_line, add_worldmap=add_worldmap,
                                         sup_fontsize=sup_fontsize, title=None,
                                         linewidth=linewidth, color=color)
 
         tex = meteva.base.get_path(r"DD日HH时", time1)
@@ -239,28 +237,28 @@
             ax.set_xlim((slon, elon))
             ax.set_ylim((slat, elat))
             meteva.base.add_contourf(ax, fo_list[i], add_colorbar=False, cmap=cmap)
             if i == 0:
                 ylable = meteva.base.get_path("DD\n日\nHH\n时", time0)
                 ax.set_ylabel(ylable, fontsize=sup_fontsize * 0.9, rotation="horizontal", verticalalignment="center")
                 ax.set_yticks(yticks)
-                ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             else:
                 ax.set_yticks(yticks)
-                ax.set_yticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_yticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
 
             if pj == len(fo_list_list) and pi == ncol - 1:
                 ax.set_xticks(xticks)
-                ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             elif pj == len(fo_list_list):
                 ax.set_xticks(xticks[:-1])
-                ax.set_xticklabels(xticks_label[:-1], fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_xticklabels(xticks_label[:-1], fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
             else:
                 ax.set_xticks(xticks)
-                ax.set_xticklabels("", fontsize=sup_fontsize * 0.9, family='Times New Roman')
+                ax.set_xticklabels("", fontsize=sup_fontsize * 0.9) #, family='Times New Roman')
 
             if grid: plt.grid(linestyle="--", linewidth=0.5)
             meteva.base.tool.plot_tools_adv.add_map(ax, add_county_line=add_county_line, add_worldmap=add_worldmap,
                                             sup_fontsize=sup_fontsize, title=None,
                                             linewidth=linewidth, color=color)
 
             tex = str(dh).zfill(3) + "H"
```

### Comparing `meteva-1.8.2/meteva/product/program/sample_statistic.py` & `meteva-1.8.3/meteva/product/program/sample_statistic.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/score.py` & `meteva-1.8.3/meteva/product/program/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/space_compare.py` & `meteva-1.8.3/meteva/product/program/space_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+import meteva
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import numpy  as np
 from meteva.base.tool.plot_tools import add_china_map_2basemap
 #from sklearn.linear_model import LinearRegression
-import meteva
 from meteva.base import IV
 import math
 from matplotlib.colors import BoundaryNorm
 from matplotlib.patches import Polygon
 import os
 import datetime
 import scipy.stats as st
@@ -421,26 +419,26 @@
                         else:
                             dtime_str = str(dtime1 - valid_time) + "-"+ str(dtime1)
                             ax.set_title(dtime_str)
 
                     knext_row = pi + (pj + 1) * ncol
                     if knext_row >= nplot:
                         ax.set_xticks(xticks)
-                        ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+                        ax.set_xticklabels(xticks_label, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
                     else:
                         ax.set_xticks(xticks)
-                        ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+                        ax.set_xticklabels(xticks_label_None, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
 
                     if ylabel_seted == 0:
                         ax.set_yticks(yticks)
-                        ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+                        ax.set_yticklabels(yticks_label, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
                         plt.ylabel(member1)
                     else:
                         ax.set_yticks(yticks)
-                        ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8, family='Times New Roman')
+                        ax.set_yticklabels(yticks_label_None, fontsize=sup_fontsize * 0.8) #, family='Times New Roman')
 
 
                     if dat[0,0] == meteva.base.IV:continue
                     im1 = ax.contourf(x, y,dat, clevs, colors=colors_grid)
                     im2 = ax.scatter(x_ob, y_ob, c=dat_ob, cmap=cmap1, norm=norm,s = point_size)
                     grd2_to_sta = meteva.base.interp_gs_nearest(grd2, sta_ob_in)
                     ts = meteva.method.ts(sta_ob_in.values[:, -1], grd2_to_sta.values[:, -1], grade_list=[ts_grade])
```

### Comparing `meteva-1.8.2/meteva/product/program/table.py` & `meteva-1.8.3/meteva/product/program/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/program/time_compare.py` & `meteva-1.8.3/meteva/product/program/time_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import datetime
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签\
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
-#import seaborn as sns
 import meteva
 import matplotlib.patches as patches
 import math
 import pandas as pd
 import json
```

### Comparing `meteva-1.8.2/meteva/product/program/time_space_compare.py` & `meteva-1.8.3/meteva/product/program/time_space_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 import numpy as np
-import matplotlib.pyplot as plt
 import datetime
-plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签\
-plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
-#import seaborn as sns
 import meteva
-import matplotlib.patches as patches
-import math
-import pandas as pd
-import json
 from scipy.ndimage.filters import uniform_filter
 
 
 def mesh_lon_time(grd_ob,grd_fo,method = np.mean,grid = None,interval = None,smooth = 1,cmap = "rainbow",clevs = None,ncol = None,annot =None,dpi = 300,
          spasify_xticks = None,sup_fontsize = 10,title ="",width = None,height = None,save_path = None,show = None):
 
     if grid is not None:
```

### Comparing `meteva-1.8.2/meteva/product/program/typhoon.py` & `meteva-1.8.3/meteva/product/program/typhoon.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/regulation/environment.py` & `meteva-1.8.3/meteva/product/regulation/environment.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/regulation/short_term_heavy_rainfall.py` & `meteva-1.8.3/meteva/product/regulation/short_term_heavy_rainfall.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/regulation/temperature.py` & `meteva-1.8.3/meteva/product/regulation/temperature.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva/product/regulation/thunderstrom_gale.py` & `meteva-1.8.3/meteva/product/regulation/thunderstrom_gale.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/meteva.egg-info/PKG-INFO` & `meteva-1.8.3/meteva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.8.2
+Version: 1.8.3
 Summary: A collections of functions for meteorological verification.
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy>=1.12.1
 Requires-Dist: pandas<=2.0.3,>=1.0.4
 Requires-Dist: netCDF4<=1.6.5,>=1.4.2
 Requires-Dist: scipy>=0.19.0
-Requires-Dist: xarray<=0.20.0,>=0.10.0
+Requires-Dist: xarray>=0.10.0
 Requires-Dist: scikit-learn>=0.21.2
 Requires-Dist: matplotlib>=3.2.2
 Requires-Dist: httplib2>=0.12.0
 Requires-Dist: protobuf<=3.20.0
 Requires-Dist: pyshp>=2.1.0
 Requires-Dist: tables>=3.4.4
 Requires-Dist: urllib3>=1.21.1
```

### Comparing `meteva-1.8.2/meteva.egg-info/SOURCES.txt` & `meteva-1.8.3/meteva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meteva-1.8.2/setup.py` & `meteva-1.8.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # _*_ coding: utf-8 _*_
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
+# python setup.py develop  进入meteva目录后执行该命令可将程序库安装为一个开发模式的包
 
 from os import path
 from setuptools import find_packages, setup
 from codecs import open
 name = "meteva"
 author ="liucouhua,daikan,wangbaoli,tangbuxing"
 version =__import__(name).__version__
@@ -39,15 +40,15 @@
     exclude_package_data={'': ['.gitignore']},
 
     install_requires=[
                       'numpy>=1.12.1',
                       'pandas>=1.0.4,<=2.0.3',
                       "netCDF4>=1.4.2,<=1.6.5",
                       'scipy>=0.19.0',
-                      'xarray>=0.10.0,<=0.20.0',
+                      'xarray>=0.10.0',
                       'scikit-learn>=0.21.2',
                       'matplotlib>=3.2.2',
                       "httplib2>=0.12.0",
                       "protobuf<=3.20.0",
                       "pyshp>=2.1.0",
                       "tables>=3.4.4",
                       "urllib3>=1.21.1",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

