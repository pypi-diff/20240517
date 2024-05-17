# Comparing `tmp/influx_si-7.0.2.tar.gz` & `tmp/influx_si-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influx_si-7.0.2.tar", last modified: Thu Feb 29 14:21:33 2024, max compression
+gzip compressed data, was "influx_si-7.0.3.tar", last modified: Wed Mar 13 11:28:25 2024, max compression
```

## Comparing `influx_si-7.0.2.tar` & `influx_si-7.0.3.tar`

### file list

```diff
@@ -1,399 +1,401 @@
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.437258 influx_si-7.0.2/
--rw-r--r--   0 sokol     (1000) sokol     (1000)       36 2024-02-29 13:58:46.000000 influx_si-7.0.2/MANIFEST.in
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1734 2024-02-29 14:21:33.437258 influx_si-7.0.2/PKG-INFO
--rw-r--r--   0 sokol     (1000) sokol     (1000)      719 2023-07-19 15:08:46.000000 influx_si-7.0.2/README.rst
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.365254 influx_si-7.0.2/influx_si/
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)   136233 2024-02-16 15:48:34.000000 influx_si-7.0.2/influx_si/C13_ftbl.py
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.377255 influx_si-7.0.2/influx_si/R/
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5759 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/R/funlab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1136 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/R/libs.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      652 2019-10-18 14:41:01.000000 influx_si-7.0.2/influx_si/R/load.R
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    51437 2024-02-29 10:38:12.000000 influx_si-7.0.2/influx_si/R/opt_cumo_tools.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)    28715 2024-02-29 13:20:32.000000 influx_si-7.0.2/influx_si/R/opt_icumo_tools.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8544 2023-12-06 13:22:19.000000 influx_si-7.0.2/influx_si/R/plot_ilab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)     4436 2023-06-13 13:34:16.000000 influx_si-7.0.2/influx_si/R/plot_imass.R
--rwx------   0 sokol     (1000) sokol     (1000)      993 2023-06-13 12:55:58.000000 influx_si-7.0.2/influx_si/R/plot_session.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)     9683 2023-06-19 14:15:06.000000 influx_si-7.0.2/influx_si/R/plot_smeas.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      420 2023-06-13 12:52:24.000000 influx_si-7.0.2/influx_si/R/preamble.R
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    11267 2020-07-27 12:46:47.000000 influx_si-7.0.2/influx_si/R/psoptim_ic.R
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      383 2023-07-10 10:39:27.000000 influx_si-7.0.2/influx_si/R/save_all.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2023-06-19 14:14:07.000000 influx_si-7.0.2/influx_si/R/save_minenv.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1060 2020-07-23 14:26:23.000000 influx_si-7.0.2/influx_si/R/test_psoptim_ic.R
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    49994 2023-07-20 09:40:50.000000 influx_si-7.0.2/influx_si/R/tools_ssg.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      694 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/R/upd_deps.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      295 2024-02-19 14:34:54.000000 influx_si-7.0.2/influx_si/__init__.py
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.377255 influx_si-7.0.2/influx_si/bin/
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)     5480 2023-07-03 15:21:19.000000 influx_si-7.0.2/influx_si/bin/ff2ftbl.py
--rw-r--r--   0 sokol     (1000) sokol     (1000)    72686 2024-02-28 16:47:58.000000 influx_si-7.0.2/influx_si/bin/ftbl2code.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    13309 2022-12-20 10:09:57.000000 influx_si-7.0.2/influx_si/bin/ftbl2cumoAb.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)     1604 2022-12-20 10:09:57.000000 influx_si-7.0.2/influx_si/bin/ftbl2kvh.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)     3438 2024-02-22 17:57:44.000000 influx_si-7.0.2/influx_si/bin/ftbl2netan.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    82689 2024-02-29 10:19:19.000000 influx_si-7.0.2/influx_si/bin/ftbl2optR.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    12584 2023-07-03 15:14:19.000000 influx_si-7.0.2/influx_si/bin/ftbl2xgmml.py
--rwx------   0 sokol     (1000) sokol     (1000)     7543 2023-07-03 15:21:41.000000 influx_si-7.0.2/influx_si/bin/res2ftbl_meas.py
--rw-r--r--   0 sokol     (1000) sokol     (1000)      224 2020-03-05 15:05:10.000000 influx_si-7.0.2/influx_si/cli.py
--rw-r--r--   0 sokol     (1000) sokol     (1000)     4249 2023-07-03 15:30:18.000000 influx_si-7.0.2/influx_si/ftbl2labcin.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    10714 2023-10-04 09:13:14.000000 influx_si-7.0.2/influx_si/ftbl2metxml.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    17194 2023-07-03 15:33:48.000000 influx_si-7.0.2/influx_si/ftbl2mtf.py
--rwx------   0 sokol     (1000) sokol     (1000)      158 2021-12-15 14:50:19.000000 influx_si-7.0.2/influx_si/influx_i.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    29090 2024-02-28 17:45:37.000000 influx_si-7.0.2/influx_si/influx_s.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)        6 2024-02-20 16:41:34.000000 influx_si-7.0.2/influx_si/influx_version.txt
--rwx------   0 sokol     (1000) sokol     (1000)    18756 2019-10-16 09:03:50.000000 influx_si-7.0.2/influx_si/licence_en.txt
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.381255 influx_si-7.0.2/influx_si/test/
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2007 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/README.txt
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15839 2021-10-22 15:50:37.000000 influx_si-7.0.2/influx_si/test/e_coli.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    15660 2020-07-23 14:26:23.000000 influx_si-7.0.2/influx_si/test/e_coli_growth.ftbl
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    16648 2024-02-22 14:45:46.000000 influx_si-7.0.2/influx_si/test/e_coli_i.ftbl
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    16698 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/e_coli_iv.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2021-02-26 08:09:25.000000 influx_si-7.0.2/influx_si/test/e_coli_iv_funlab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)    11407 2016-04-14 10:13:26.000000 influx_si-7.0.2/influx_si/test/e_coli_msen.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1579 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/ex_i_2box_var.ftbl
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.389255 influx_si-7.0.2/influx_si/test/mtf/
--rw-r--r--   0 sokol     (1000) sokol     (1000)    20406 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/Akin.tsv
--rw-r--r--   0 sokol     (1000) sokol     (1000)      396 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      188 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      125 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2747 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3919 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2073 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      366 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      523 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      203 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3447 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      608 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1774 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      317 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1643 2023-06-30 08:33:36.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      846 2023-06-30 08:33:54.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.tvar.def
--rw-r--r--   0 sokol     (1000) sokol     (1000)      398 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10790 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.ikin
--rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      127 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)    27670 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      296 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3921 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      392 2024-02-22 14:47:24.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3011 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_i.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      399 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      128 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2750 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      297 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3922 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      410 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3012 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/e_coli_iv_funlab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      123 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.funlab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      140 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.ikin
--rw-r--r--   0 sokol     (1000) sokol     (1000)      282 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      231 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      185 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      170 2024-02-22 14:47:11.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)      234 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_lin.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      148 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_var.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      189 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_var.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      144 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_var.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      275 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_var.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)      193 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/mtf/ex_i_2box_var.tvar
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.361254 influx_si-7.0.2/influx_si/test/ok/
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.397256 influx_si-7.0.2/influx_si/test/ok/mtf/
--rw-r--r--   0 sokol     (1000) sokol     (1000)    20406 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/Akin.tsv
--rw-r--r--   0 sokol     (1000) sokol     (1000)      396 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      188 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      125 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2747 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3919 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2073 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1546 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.tvar.def
--rw-r--r--   0 sokol     (1000) sokol     (1000)      366 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      523 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      203 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3447 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      608 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1774 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      317 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1643 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      589 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.tvar.def
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.397256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1840 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      109 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mflux.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5599 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      729 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mmet.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    37739 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      278 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.stat
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     3844 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.tvar.sim
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.397256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    11750 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1147 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   258684 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     2753 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.netflux.e_coli_growth.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     2177 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.xchflux.e_coli_growth.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      326 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/node.log2pool.e_coli_growth.attrs
--rw-r--r--   0 sokol     (1000) sokol     (1000)      398 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      127 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)    27670 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      296 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3921 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      392 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3011 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1555 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.tvar.def
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.401256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1960 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      113 2024-02-29 13:25:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.mflux.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44073 2024-02-29 13:25:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      452 2024-02-29 13:25:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.mmet.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   107550 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      275 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.stat
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     7635 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.tvar.sim
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.401256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    14720 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10790 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ikin
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      708 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   891104 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6151 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.netflux.e_coli_i.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     4340 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.xchflux.e_coli_i.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      693 2024-02-29 13:25:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/node.log2pool.e_coli_i.attrs
--rw-r--r--   0 sokol     (1000) sokol     (1000)      399 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      128 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.mflux
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2750 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      297 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.mmet
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3922 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      410 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3012 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1556 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.tvar.def
--rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_funlab.R
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.405256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1354 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       82 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.mflux.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      343 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.mmet.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    66594 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6479 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.tvar.sim
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.405256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    14852 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      369 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   229477 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5957 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.netflux.e_coli_iv.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     4157 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.xchflux.e_coli_iv.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      470 2024-02-29 13:24:58.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/node.log2pool.e_coli_iv.attrs
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.405256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1511 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      112 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.mflux.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     4394 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    36526 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      278 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.stat
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6027 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.tvar.sim
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.409256 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    12805 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      701 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   191825 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6112 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/edge.netflux.e_coli.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     4338 2024-02-29 13:24:13.000000 influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/edge.xchflux.e_coli.attrs
--rw-r--r--   0 sokol     (1000) sokol     (1000)      123 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.funlab.R
--rw-r--r--   0 sokol     (1000) sokol     (1000)      140 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.ikin
--rw-r--r--   0 sokol     (1000) sokol     (1000)      282 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      231 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      185 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      170 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)      234 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_lin.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      148 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)      189 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      144 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      275 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)      193 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      238 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var.tvar.def
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.409256 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      904 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    25277 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.pdf
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.409256 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       62 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/edge.netflux.ex_i_2box_var.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       62 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/edge.xchflux.ex_i_2box_var.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1774 2024-02-29 13:24:45.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       34 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    40056 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       37 2024-02-29 13:24:50.000000 influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/node.log2pool.ex_i_2box_var.attrs
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.361254 influx_si-7.0.2/influx_si/test/ok/prl_exp/
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.413257 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/
--rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)    33818 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1072 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      241 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1135 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.tvar
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X_MS.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)    52585 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1069 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      261 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1132 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      378 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar.def
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.417257 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    64494 2024-02-29 13:25:47.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   104458 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1887 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   100269 2024-02-29 13:25:47.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)   143744 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      282 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.stat
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     2411 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.tvar.sim
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.421257 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     2789 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    14918 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ikin
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6510 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    23059 2024-02-29 13:24:46.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ikin
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      439 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)  1591040 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1745 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.netflux.e_coli_GX_prl.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1430 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.xchflux.e_coli_GX_prl.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      453 2024-02-29 13:25:49.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/node.log2pool.e_coli_GX_prl.attrs
--rw-r--r--   0 sokol     (1000) sokol     (1000)      539 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5225 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      269 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2050 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      994 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar.def
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.425257 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.err
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5053 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.log
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6716 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44363 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      271 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.stat
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6690 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.tvar.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6699 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44411 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6714 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44339 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6727 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    43945 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6707 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44229 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.pdf
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     6703 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.miso.sim
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    44270 2024-02-29 13:24:43.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.pdf
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.429257 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    17244 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      850 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.pres.csv
--rw-rw-r--   0 sokol     (1000) sokol     (1000)  1177886 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n_res.kvh
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5702 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc2n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5715 2024-02-29 13:24:08.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc3n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5723 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc4n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5715 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc5n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     5701 2024-02-29 13:24:09.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc6n.ftbl
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    12569 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.netflux.e_coli_glc1-6n.attrs
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     8162 2024-02-29 13:24:42.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.xchflux.e_coli_glc1-6n.attrs
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3616 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3615 2024-02-29 13:24:07.000000 influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.miso
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.429257 influx_si-7.0.2/influx_si/test/prl_exp/
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    23180 2017-04-25 15:23:51.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_MS.txt
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)     4640 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_X.ftbl
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2017-04-25 15:23:51.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_X_MS.txt
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)     4886 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_prl.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10909 2020-04-07 08:28:22.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc1-6n.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10784 2020-04-07 08:07:41.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc2n.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10797 2020-04-07 08:07:41.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc3n.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10805 2020-04-07 08:07:41.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc4n.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10797 2020-04-07 08:07:41.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc5n.ftbl
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10783 2020-04-07 08:07:41.000000 influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc6n.ftbl
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.433257 influx_si-7.0.2/influx_si/test/prl_exp/mtf/
--rw-r--r--   0 sokol     (1000) sokol     (1000)    14918 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.ikin
--rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)    33818 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1072 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      241 2024-02-22 14:50:53.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1135 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.tvar
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2017-04-25 15:23:51.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X_MS.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)    23059 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.ikin
--rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)    52585 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1069 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      261 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     1132 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      539 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.cnstr
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5225 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.netw
--rw-r--r--   0 sokol     (1000) sokol     (1000)      269 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.opt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2050 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.tvar
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc2n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3616 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc2n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc3n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc3n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc4n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc4n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc5n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc5n.miso
--rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc6n.linp
--rw-r--r--   0 sokol     (1000) sokol     (1000)     3615 2022-10-05 07:06:07.000000 influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc6n.miso
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    10311 2024-02-26 16:02:29.000000 influx_si-7.0.2/influx_si/tools_ssg.py
--rwxr-xr-x   0 sokol     (1000) sokol     (1000)    70201 2024-02-28 10:42:46.000000 influx_si-7.0.2/influx_si/txt2ftbl.py
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.365254 influx_si-7.0.2/influx_si.egg-info/
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     1734 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/PKG-INFO
--rw-rw-r--   0 sokol     (1000) sokol     (1000)    17065 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/SOURCES.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)        1 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/dependency_links.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)      486 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/entry_points.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       32 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/requires.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       10 2024-02-29 14:21:33.000000 influx_si-7.0.2/influx_si.egg-info/top_level.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)       38 2024-02-29 14:21:33.437258 influx_si-7.0.2/setup.cfg
--rw-r--r--   0 sokol     (1000) sokol     (1000)     2812 2024-02-29 14:12:06.000000 influx_si-7.0.2/setup.py
-drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-02-29 14:21:33.373255 influx_si-7.0.2/test_cases/
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5087 2016-04-15 14:45:00.000000 influx_si-7.0.2/test_cases/cases_influx_si-v3.0.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5087 2016-04-15 14:45:00.000000 influx_si-7.0.2/test_cases/cases_influx_si-v3.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5440 2016-06-13 14:06:15.000000 influx_si-7.0.2/test_cases/cases_influx_si-v3.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6057 2016-07-29 09:51:56.000000 influx_si-7.0.2/test_cases/cases_influx_si-v3.2.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6855 2016-12-15 16:08:14.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.0.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6855 2016-12-15 16:08:14.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7030 2017-03-03 10:55:03.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7075 2017-03-30 12:52:53.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.2.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-04-26 14:55:16.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.3.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7441 2017-06-15 13:38:40.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.4.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7441 2017-06-15 13:38:40.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.4.2.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7599 2017-07-04 10:21:18.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.4.3.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7750 2019-07-19 14:49:37.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.4.5.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-05-05 14:48:04.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.4.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-05-22 16:20:19.000000 influx_si-7.0.2/test_cases/cases_influx_si-v4.5dev.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8159 2019-11-21 13:48:27.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.0.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8441 2020-02-26 15:23:59.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.0.2.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8482 2020-03-05 10:14:50.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.0.3.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8159 2019-11-21 13:48:27.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8839 2020-04-07 13:12:16.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.1.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8946 2020-05-04 13:27:12.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.1.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8839 2020-05-28 13:10:44.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.2.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     8900 2020-07-24 09:22:29.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.3.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     9325 2021-02-25 15:48:53.000000 influx_si-7.0.2/test_cases/cases_influx_si-v5.4.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10036 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/cases_influx_si-v6.0.3.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10036 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/cases_influx_si-v6.0.4.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10037 2022-10-05 07:06:07.000000 influx_si-7.0.2/test_cases/cases_influx_si-v6.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    10514 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/cases_influx_si-v6.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    12175 2023-10-04 14:44:59.000000 influx_si-7.0.2/test_cases/cases_influx_si-v7.0.1.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    13105 2024-02-28 16:05:36.000000 influx_si-7.0.2/test_cases/cases_influx_si-v7.0.2.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)    11995 2023-07-11 08:05:48.000000 influx_si-7.0.2/test_cases/cases_influx_si-v7.0.tab
--rw-r--r--   0 sokol     (1000) sokol     (1000)     4652 2020-01-13 14:53:57.000000 influx_si-7.0.2/test_cases/test_report_5.0.1.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     4912 2020-02-26 15:27:58.000000 influx_si-7.0.2/test_cases/test_report_5.0.2.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     4977 2020-03-05 10:19:14.000000 influx_si-7.0.2/test_cases/test_report_5.0.3.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5437 2020-04-07 13:26:19.000000 influx_si-7.0.2/test_cases/test_report_5.1.0.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5439 2020-05-28 13:32:32.000000 influx_si-7.0.2/test_cases/test_report_5.2.0.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5517 2020-07-24 13:00:54.000000 influx_si-7.0.2/test_cases/test_report_5.3.0.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     5799 2021-02-26 09:46:06.000000 influx_si-7.0.2/test_cases/test_report_5.4.0.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6506 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/test_report_6.0.3.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6527 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/test_report_6.0.4.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     6516 2022-10-05 07:06:07.000000 influx_si-7.0.2/test_cases/test_report_6.0.txt
--rw-r--r--   0 sokol     (1000) sokol     (1000)     7321 2022-12-20 10:09:57.000000 influx_si-7.0.2/test_cases/test_report_6.1.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     7549 2023-07-03 15:40:05.000000 influx_si-7.0.2/test_cases/test_report_6.2.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     7985 2023-10-04 15:08:08.000000 influx_si-7.0.2/test_cases/test_report_7.0.1.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     8498 2024-02-29 13:46:28.000000 influx_si-7.0.2/test_cases/test_report_7.0.2.txt
--rw-rw-r--   0 sokol     (1000) sokol     (1000)     7645 2023-07-11 08:10:03.000000 influx_si-7.0.2/test_cases/test_report_7.0.txt
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.870634 influx_si-7.0.3/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)       36 2024-02-29 13:58:46.000000 influx_si-7.0.3/MANIFEST.in
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1734 2024-03-13 11:28:25.870634 influx_si-7.0.3/PKG-INFO
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      719 2023-07-19 15:08:46.000000 influx_si-7.0.3/README.rst
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:24.758585 influx_si-7.0.3/influx_si/
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)   136631 2024-03-06 17:05:16.000000 influx_si-7.0.3/influx_si/C13_ftbl.py
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.042597 influx_si-7.0.3/influx_si/R/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5759 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/R/funlab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1136 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/R/libs.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      652 2019-10-18 14:41:01.000000 influx_si-7.0.3/influx_si/R/load.R
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    51568 2024-03-12 10:44:35.000000 influx_si-7.0.3/influx_si/R/opt_cumo_tools.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    31393 2024-03-12 16:35:33.000000 influx_si-7.0.3/influx_si/R/opt_icumo_tools.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8544 2023-12-06 13:22:19.000000 influx_si-7.0.3/influx_si/R/plot_ilab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     4436 2023-06-13 13:34:16.000000 influx_si-7.0.3/influx_si/R/plot_imass.R
+-rwx------   0 sokol     (1000) sokol     (1000)      993 2023-06-13 12:55:58.000000 influx_si-7.0.3/influx_si/R/plot_session.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     9683 2023-06-19 14:15:06.000000 influx_si-7.0.3/influx_si/R/plot_smeas.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      420 2023-06-13 12:52:24.000000 influx_si-7.0.3/influx_si/R/preamble.R
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    11267 2020-07-27 12:46:47.000000 influx_si-7.0.3/influx_si/R/psoptim_ic.R
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      383 2023-07-10 10:39:27.000000 influx_si-7.0.3/influx_si/R/save_all.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2023-06-19 14:14:07.000000 influx_si-7.0.3/influx_si/R/save_minenv.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1060 2020-07-23 14:26:23.000000 influx_si-7.0.3/influx_si/R/test_psoptim_ic.R
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    49994 2024-03-08 09:28:16.000000 influx_si-7.0.3/influx_si/R/tools_ssg.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      694 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/R/upd_deps.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      295 2024-02-19 14:34:54.000000 influx_si-7.0.3/influx_si/__init__.py
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.046598 influx_si-7.0.3/influx_si/bin/
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)     5480 2023-07-03 15:21:19.000000 influx_si-7.0.3/influx_si/bin/ff2ftbl.py
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    72670 2024-03-11 11:36:12.000000 influx_si-7.0.3/influx_si/bin/ftbl2code.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    14943 2024-03-13 11:02:27.000000 influx_si-7.0.3/influx_si/bin/ftbl2cumoAb.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)     1604 2022-12-20 10:09:57.000000 influx_si-7.0.3/influx_si/bin/ftbl2kvh.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)     3438 2024-02-22 17:57:44.000000 influx_si-7.0.3/influx_si/bin/ftbl2netan.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    86738 2024-03-12 16:46:50.000000 influx_si-7.0.3/influx_si/bin/ftbl2optR.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    12584 2023-07-03 15:14:19.000000 influx_si-7.0.3/influx_si/bin/ftbl2xgmml.py
+-rwx------   0 sokol     (1000) sokol     (1000)     7543 2023-07-03 15:21:41.000000 influx_si-7.0.3/influx_si/bin/res2ftbl_meas.py
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      224 2020-03-05 15:05:10.000000 influx_si-7.0.3/influx_si/cli.py
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     4249 2023-07-03 15:30:18.000000 influx_si-7.0.3/influx_si/ftbl2labcin.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    10714 2023-10-04 09:13:14.000000 influx_si-7.0.3/influx_si/ftbl2metxml.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    17194 2023-07-03 15:33:48.000000 influx_si-7.0.3/influx_si/ftbl2mtf.py
+-rwx------   0 sokol     (1000) sokol     (1000)      134 2024-03-13 10:21:59.000000 influx_si-7.0.3/influx_si/influx_i.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    29087 2024-03-13 10:19:29.000000 influx_si-7.0.3/influx_si/influx_s.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)        6 2024-03-13 10:24:51.000000 influx_si-7.0.3/influx_si/influx_version.txt
+-rwx------   0 sokol     (1000) sokol     (1000)    18756 2019-10-16 09:03:50.000000 influx_si-7.0.3/influx_si/licence_en.txt
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.154602 influx_si-7.0.3/influx_si/test/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2007 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/README.txt
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15839 2021-10-22 15:50:37.000000 influx_si-7.0.3/influx_si/test/e_coli.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    15660 2020-07-23 14:26:23.000000 influx_si-7.0.3/influx_si/test/e_coli_growth.ftbl
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    16648 2024-02-22 14:45:46.000000 influx_si-7.0.3/influx_si/test/e_coli_i.ftbl
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    16698 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/e_coli_iv.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2021-02-26 08:09:25.000000 influx_si-7.0.3/influx_si/test/e_coli_iv_funlab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    11407 2016-04-14 10:13:26.000000 influx_si-7.0.3/influx_si/test/e_coli_msen.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1579 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/ex_i_2box_var.ftbl
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.266607 influx_si-7.0.3/influx_si/test/mtf/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    20406 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/Akin.tsv
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      396 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      188 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      125 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2747 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3919 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2073 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      366 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      523 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      203 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3447 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      608 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1774 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      317 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1643 2023-06-30 08:33:36.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      846 2023-06-30 08:33:54.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.tvar.def
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      398 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10790 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.ikin
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      127 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    27670 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      296 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3921 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      392 2024-02-22 14:47:24.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3011 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_i.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      399 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      128 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2750 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      297 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3922 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      410 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3012 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/e_coli_iv_funlab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      123 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.funlab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      140 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.ikin
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      282 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      231 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      185 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      170 2024-02-22 14:47:11.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      234 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_lin.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      148 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_var.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      189 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_var.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      144 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_var.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      275 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_var.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      193 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/mtf/ex_i_2box_var.tvar
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:24.746584 influx_si-7.0.3/influx_si/test/ok/
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.338611 influx_si-7.0.3/influx_si/test/ok/mtf/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    20406 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/Akin.tsv
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      396 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      188 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      125 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2747 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3919 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      150 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2073 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1546 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.tvar.def
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      366 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      523 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      203 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3447 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      608 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1774 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      317 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1643 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      589 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.tvar.def
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.374612 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1840 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      109 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mflux.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5599 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      729 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mmet.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    37739 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      278 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.stat
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     3844 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.tvar.sim
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.390613 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    11750 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1147 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   258684 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     2753 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.netflux.e_coli_growth.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     2177 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.xchflux.e_coli_growth.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      326 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/node.log2pool.e_coli_growth.attrs
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      398 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      127 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    27670 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      296 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3921 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      392 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3011 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1555 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.tvar.def
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.426614 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1960 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      113 2024-02-29 13:25:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.mflux.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44073 2024-02-29 13:25:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      452 2024-02-29 13:25:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.mmet.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   107550 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      275 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.stat
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     7635 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.tvar.sim
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.462616 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    14720 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10790 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ikin
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      708 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   891104 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6151 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.netflux.e_coli_i.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     4340 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.xchflux.e_coli_i.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      693 2024-02-29 13:25:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/node.log2pool.e_coli_i.attrs
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      399 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      190 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      128 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.mflux
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2750 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      297 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.mmet
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3922 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      410 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3012 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1556 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.tvar.def
+-rw-r--r--   0 sokol     (1000) sokol     (1000)       10 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_funlab.R
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.486617 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1354 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       82 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.mflux.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      343 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.mmet.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    66594 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6479 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.tvar.sim
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.510618 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    14852 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      369 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   229477 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5957 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.netflux.e_coli_iv.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     4157 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.xchflux.e_coli_iv.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      470 2024-02-29 13:24:58.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/node.log2pool.e_coli_iv.attrs
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.514618 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1511 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      112 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.mflux.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     4394 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    36526 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      278 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.stat
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6027 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.tvar.sim
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.534619 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    12805 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      701 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   191825 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6112 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/edge.netflux.e_coli.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     4338 2024-02-29 13:24:13.000000 influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/edge.xchflux.e_coli.attrs
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      123 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.funlab.R
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      140 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.ikin
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      282 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      231 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      185 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      170 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      234 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_lin.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      148 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      189 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      144 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      275 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      193 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      238 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var.tvar.def
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.534619 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      904 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    25277 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.pdf
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.538620 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       62 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/edge.netflux.ex_i_2box_var.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       62 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/edge.xchflux.ex_i_2box_var.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1774 2024-02-29 13:24:45.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       34 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    40056 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       37 2024-02-29 13:24:50.000000 influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/node.log2pool.ex_i_2box_var.attrs
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:24.746584 influx_si-7.0.3/influx_si/test/ok/prl_exp/
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.550620 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    33818 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1072 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      241 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1135 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.tvar
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X_MS.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    52585 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1069 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      261 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1132 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      378 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar.def
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.598622 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    64494 2024-02-29 13:25:47.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   104458 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1887 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   100269 2024-02-29 13:25:47.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)   143744 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      282 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.stat
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     2411 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.tvar.sim
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.658625 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     2789 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    14918 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ikin
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6510 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    23059 2024-02-29 13:24:46.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ikin
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      439 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)  1591040 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1745 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.netflux.e_coli_GX_prl.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1430 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.xchflux.e_coli_GX_prl.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      453 2024-02-29 13:25:49.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/node.log2pool.e_coli_GX_prl.attrs
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      539 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5225 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      269 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2050 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      994 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar.def
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.714627 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        0 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.err
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5053 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.log
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6716 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44363 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      271 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.stat
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6690 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.tvar.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6699 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44411 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6714 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44339 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6727 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    43945 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6707 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44229 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.pdf
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     6703 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.miso.sim
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    44270 2024-02-29 13:24:43.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.pdf
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.790631 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    17244 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      850 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.pres.csv
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)  1177886 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n_res.kvh
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5702 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc2n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5715 2024-02-29 13:24:08.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc3n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5723 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc4n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5715 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc5n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     5701 2024-02-29 13:24:09.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc6n.ftbl
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    12569 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.netflux.e_coli_glc1-6n.attrs
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     8162 2024-02-29 13:24:42.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.xchflux.e_coli_glc1-6n.attrs
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3616 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3615 2024-02-29 13:24:07.000000 influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.miso
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.838633 influx_si-7.0.3/influx_si/test/prl_exp/
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    23180 2017-04-25 15:23:51.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_MS.txt
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)     4640 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_X.ftbl
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2017-04-25 15:23:51.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_X_MS.txt
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)     4886 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_prl.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10909 2020-04-07 08:28:22.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc1-6n.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10784 2020-04-07 08:07:41.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc2n.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10797 2020-04-07 08:07:41.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc3n.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10805 2020-04-07 08:07:41.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc4n.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10797 2020-04-07 08:07:41.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc5n.ftbl
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10783 2020-04-07 08:07:41.000000 influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc6n.ftbl
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:25.870634 influx_si-7.0.3/influx_si/test/prl_exp/mtf/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    14918 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.ikin
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    33818 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1072 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      241 2024-02-22 14:50:53.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1135 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.tvar
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    15077 2017-04-25 15:23:51.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X_MS.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    23059 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.ikin
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      153 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    52585 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1069 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      261 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     1132 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      539 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.cnstr
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5225 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.netw
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      269 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.opt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2050 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.tvar
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc2n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3616 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc2n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc3n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc3n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc4n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3637 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc4n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc5n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3629 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc5n.miso
+-rw-r--r--   0 sokol     (1000) sokol     (1000)      179 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc6n.linp
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     3615 2022-10-05 07:06:07.000000 influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc6n.miso
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    10311 2024-02-26 16:02:29.000000 influx_si-7.0.3/influx_si/tools_ssg.py
+-rwxr-xr-x   0 sokol     (1000) sokol     (1000)    70203 2024-03-05 17:00:52.000000 influx_si-7.0.3/influx_si/txt2ftbl.py
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:24.758585 influx_si-7.0.3/influx_si.egg-info/
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     1734 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/PKG-INFO
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)    17162 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/SOURCES.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)        1 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/dependency_links.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)      486 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/entry_points.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       32 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/requires.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       10 2024-03-13 11:28:24.000000 influx_si-7.0.3/influx_si.egg-info/top_level.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)       38 2024-03-13 11:28:25.870634 influx_si-7.0.3/setup.cfg
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     2816 2024-03-13 11:25:10.000000 influx_si-7.0.3/setup.py
+drwxrwxr-x   0 sokol     (1000) sokol     (1000)        0 2024-03-13 11:28:24.958593 influx_si-7.0.3/test_cases/
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5087 2016-04-15 14:45:00.000000 influx_si-7.0.3/test_cases/cases_influx_si-v3.0.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5087 2016-04-15 14:45:00.000000 influx_si-7.0.3/test_cases/cases_influx_si-v3.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5440 2016-06-13 14:06:15.000000 influx_si-7.0.3/test_cases/cases_influx_si-v3.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6057 2016-07-29 09:51:56.000000 influx_si-7.0.3/test_cases/cases_influx_si-v3.2.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6855 2016-12-15 16:08:14.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.0.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6855 2016-12-15 16:08:14.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7030 2017-03-03 10:55:03.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7075 2017-03-30 12:52:53.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.2.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-04-26 14:55:16.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.3.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7441 2017-06-15 13:38:40.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.4.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7441 2017-06-15 13:38:40.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.4.2.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7599 2017-07-04 10:21:18.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.4.3.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7750 2019-07-19 14:49:37.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.4.5.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-05-05 14:48:04.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.4.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7270 2017-05-22 16:20:19.000000 influx_si-7.0.3/test_cases/cases_influx_si-v4.5dev.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8159 2019-11-21 13:48:27.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.0.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8441 2020-02-26 15:23:59.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.0.2.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8482 2020-03-05 10:14:50.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.0.3.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8159 2019-11-21 13:48:27.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8839 2020-04-07 13:12:16.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.1.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8946 2020-05-04 13:27:12.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.1.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8839 2020-05-28 13:10:44.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.2.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     8900 2020-07-24 09:22:29.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.3.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     9325 2021-02-25 15:48:53.000000 influx_si-7.0.3/test_cases/cases_influx_si-v5.4.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10036 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/cases_influx_si-v6.0.3.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10036 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/cases_influx_si-v6.0.4.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10037 2022-10-05 07:06:07.000000 influx_si-7.0.3/test_cases/cases_influx_si-v6.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    10514 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/cases_influx_si-v6.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    12175 2023-10-04 14:44:59.000000 influx_si-7.0.3/test_cases/cases_influx_si-v7.0.1.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    13105 2024-02-28 16:05:36.000000 influx_si-7.0.3/test_cases/cases_influx_si-v7.0.2.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    13246 2024-03-13 10:39:59.000000 influx_si-7.0.3/test_cases/cases_influx_si-v7.0.3.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)    11995 2023-07-11 08:05:48.000000 influx_si-7.0.3/test_cases/cases_influx_si-v7.0.tab
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     4652 2020-01-13 14:53:57.000000 influx_si-7.0.3/test_cases/test_report_5.0.1.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     4912 2020-02-26 15:27:58.000000 influx_si-7.0.3/test_cases/test_report_5.0.2.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     4977 2020-03-05 10:19:14.000000 influx_si-7.0.3/test_cases/test_report_5.0.3.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5437 2020-04-07 13:26:19.000000 influx_si-7.0.3/test_cases/test_report_5.1.0.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5439 2020-05-28 13:32:32.000000 influx_si-7.0.3/test_cases/test_report_5.2.0.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5517 2020-07-24 13:00:54.000000 influx_si-7.0.3/test_cases/test_report_5.3.0.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     5799 2021-02-26 09:46:06.000000 influx_si-7.0.3/test_cases/test_report_5.4.0.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6506 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/test_report_6.0.3.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6527 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/test_report_6.0.4.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     6516 2022-10-05 07:06:07.000000 influx_si-7.0.3/test_cases/test_report_6.0.txt
+-rw-r--r--   0 sokol     (1000) sokol     (1000)     7321 2022-12-20 10:09:57.000000 influx_si-7.0.3/test_cases/test_report_6.1.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     7549 2023-07-03 15:40:05.000000 influx_si-7.0.3/test_cases/test_report_6.2.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     7985 2023-10-04 15:08:08.000000 influx_si-7.0.3/test_cases/test_report_7.0.1.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     8498 2024-02-29 13:46:28.000000 influx_si-7.0.3/test_cases/test_report_7.0.2.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     8670 2024-03-13 11:10:09.000000 influx_si-7.0.3/test_cases/test_report_7.0.3.txt
+-rw-rw-r--   0 sokol     (1000) sokol     (1000)     7645 2023-07-11 08:10:03.000000 influx_si-7.0.3/test_cases/test_report_7.0.txt
```

### Comparing `influx_si-7.0.2/PKG-INFO` & `influx_si-7.0.3/influx_si.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: influx_si
-Version: 7.0.2
+Name: influx-si
+Version: 7.0.3
 Summary: Metabolic flux and concentration estimation based on stable isotope labeling
 Home-page: https://github.com/sgsokol/influx/
 Author: Serguei Sokol
 Author-email: sokol@insa-toulouse.fr
 License: GNU General Public License v2 or later (GPLv2+)
 Project-URL: Documentation, https://influx-si.readthedocs.io/
 Project-URL: Source, https://github.com/sgsokol/influx
```

### Comparing `influx_si-7.0.2/README.rst` & `influx_si-7.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/C13_ftbl.py` & `influx_si-7.0.3/influx_si/C13_ftbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,18 +275,18 @@
                 # fc.close()
                 # fc=open(f, "r")
                 # lines=fc.readlines()
                 # fc.close()
     ftbl["pathway"]=dict()
     
     #print f;##
-    reblank=re.compile("^[\t ]*$")
-    recomm=re.compile("^[\t ]*//.*$")
-    repath=re.compile("^[\t ]*//##[\t ]*(.*)[\t ]*$")
-    comm=re.compile("^([^(//)]+|.+)//.*$")
+    reblank=re.compile(r"^[\t ]*$")
+    recomm=re.compile(r"^[\t ]*//.*$")
+    repath=re.compile(r"^[\t ]*//##[\t ]*(.*)[\t ]*$")
+    comm=re.compile(r"^([^(//)]+|.+)//.*$")
     reading="sec_name"
     col_names=[]
     sec_name=subsec_name=""
     irow=0
     dic=dict()
     pathway=""
     #pdb.set_trace()
@@ -418,14 +418,15 @@
                         try:
                             fval=float(val)
                             dic[col_names[i]]=val
                         except:
                             dic[col_names[i]]=oldval
                 except IndexError:
                     pass
+            #import pdb; pdb.set_trace()
             if sec_name == "NETWORK" and pathway:
                 if pathway not in ftbl["pathway"]:
                     ftbl["pathway"][pathway]=[]
                 ftbl["pathway"][pathway]+=[dic["FLUX_NAME"]]
             if sec_name == "FLUXES" and subsec_name in ("NET", "XCH") and dic["FCD"] in ("F", "C"):
                 try:
                     val=float(eval(dic["VALUE(F/C)"]))
@@ -1291,29 +1292,31 @@
                             #    netan["cumo_input"][in_cumo])
                             res["b"][w-1][cumo][flux][imetab].append(in_cumo)
                             #print "b="+str(res["b"][w-1][cumo][flux]);##
                         # if in_w==0 then in_cumo=1 by definition => ignore here
                         # in_w cannot be > w because of src_ind()
     except Exception as inst:
         werr(": ".join(inst)+"\n")
+    #netan["cumo_input"]=[dict((k,(v if v==v else 0.)) for k,v in d.items()) for d in netan["cumo_input"]]
     # ordered cumomer lists
-    for w in range(1,netan["Cmax"]+1):
+    #for w in range(1,netan["Cmax"]+1):
         # weight 1 equations have all metabolites
         ##aff("A "+str(w), netan["cumo_sys"]["A"][w-1]);#
         ##aff("b "+str(w), netan["cumo_sys"]["b"][w-1]);#
         # order cumos along pathways
         # starts are input cumomers
-        starts=[cumo for cumo in netan["cumo_sys"]["A"][w-1] \
-            if cumo.split(":")[0] in netan["input"]]
+    #    starts=[cumo for cumo in netan["cumo_sys"]["A"][w-1] \
+    #        if cumo.split(":")[0] in netan["input"]]
         ##aff("st "+str(w), starts)
         # complete starts by all others cumomers
-        starts+=[c for c in netan["cumo_sys"]["A"][w-1] if not c in starts]
-        cumo_paths=cumo_path(starts, netan["cumo_sys"]["A"][w-1], oset())
+    #    starts+=[c for c in netan["cumo_sys"]["A"][w-1] if not c in starts]
+    #    cumo_paths=cumo_path(starts, netan["cumo_sys"]["A"][w-1], oset())
         # order
-        netan["vcumo"].append([cumo for cumo in valval(cumo_paths)])
+    #    netan["vcumo"].append([cumo for cumo in valval(cumo_paths)])
+    netan["vcumo"]=[[*a.keys()] for a in netan["cumo_sys"]["A"]]
 
     # ordered unknown flux lists
     # get all reactions which are not constrained, not free and not growth
     netan["vflux"]["net"].extend(reac for reac in netan["reac"]|eqflux
         if reac not in netan["flux_constr"]["net"] and
         reac not in netan["flux_free"]["net"] and
         reac not in netan["flux_vgrowth"]["net"])
@@ -2400,14 +2403,16 @@
                     A[w-1][cumo]=A[w-1].get(cumo,{cumo:[]})
                     #print("adding A:", incumo, "->", cumo, A[w-1][cumo][incumo]);##
                     A[w-1][cumo][cumo]+=A[w-1][cumo][incumo]
                 if cumo in b[w-1]:
                     A[w-1][cumo]=A[w-1].get(cumo,{cumo:[]})
                     #print("adding b:", cumo, b[w-1][cumo].keys());##
                     A[w-1][cumo][cumo]+=[*b[w-1][cumo].keys()]
+    #import pdb; pdb.set_trace()
+    #netan["rcumo_input"]=[dict((k, (v if v==v else 0.)) for k,v in d.items()) for d in netan["rcumo_input"]]
     #aff("to_v", to_visit);##
     # make ordered list for reduced cumomer set
     netan["vrcumo"]=[[*a.keys()] for a in A]
     netan["rcumo2i0"]=dict((cumo,i) for (i, cumo) in enumerate(valval(netan["vrcumo"])))
     #print("A=", A)
     netan["rcumo_sys"]={"A": A, "b": b}
     # make order list for emu_input
@@ -2552,23 +2557,24 @@
             break
     return(frags)
 def ntimes(n):
     """Return charcater string 'once' for n=1, 'twice' for n=2 and 'n times' for other n"""
     return("once" if n==1 else "twice" if n==2 else "%d times"%n)
 def proc_label_input(ftbl, netan, case_i=False):
     """Proceed LABEL_INPUT section in ftbl and add result to the list netan["iso_input"] and netan["funlab"] (case_i)
-    List item is a dict {}metab;{isotop_int_index:fraction}}
+    List item is a dict {metab;{isotop_int_index:fraction}}
     """
     ili=len(netan["iso_input"]) # label_input list index
     netan["iso_input"]+=[{}]
     if case_i:
         netan["funlab"]+=[{}]
         resf=netan["funlab"][ili]
     res=netan["iso_input"][ili]
     # input isotopomers
+    #import pdb; pdb.set_trace()
     for row in ftbl.get("LABEL_INPUT",[]):
         metab=row.get("META_NAME", "") or metab
         if metab not in netan["Clen"]:
             raise Exception("Label input metabolite `%s` is not defined in NETWORK (%s: %s)."%(metab, ftbl["name"], row["irow"]))
         ilen=len(row.get("ISOTOPOMER", ""))-1; # -1 for '#' sign
         if ilen != netan["Clen"][metab]:
             raise Exception("Input isotopomer `%s` is of bad length (%d). A length of %d is expected (%s: %s)."%
```

### Comparing `influx_si-7.0.2/influx_si/R/funlab.R` & `influx_si-7.0.3/influx_si/R/funlab.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/libs.R` & `influx_si-7.0.3/influx_si/R/libs.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/load.R` & `influx_si-7.0.3/influx_si/R/load.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/opt_cumo_tools.R` & `influx_si-7.0.3/influx_si/R/opt_cumo_tools.R`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,17 @@
    for (item in nm_local) {
       assign(item, labargs[[item]])
    }
    if (fullsys) {
       nb_x=nb_f$xf
       nb_xi=nb_f$xif
       xi=xif
-      nm_x=nm_list$xf
+      nm_x=nm_list$cumo
       spa=spaf
+      rcumo_in_cumo=match(nm_list$rcumo, nm_x)
    } else {
       nb_x=nb_f$x
       nb_xi=nb_f$xi
       nm_x=nm_list$x
       nb_x=nb_f$x
    }
    nb_w=length(nb_x)
@@ -174,24 +175,24 @@
    nb_sc_tot=nb_f$nb_sc_tot
    fg=nb_f$mu*param[nm$poolf] # the same alphabetical order
    names(fg)=nm$fgr
    pool[nm$poolf]=param[nm$poolf] # inject variable pools to pool vector
 
    # calculate all fluxes from free fluxes
    lf=param2fl(param, labargs)
-   if (is.null(jx_f$x)) {
+   if (is.null(jx_f$x) || nrow(jx_f$x) != sum(nb_x)) {
       jx_f$x=matrix(0, nrow=sum(nb_x), nb_exp)
       dimnames(jx_f$x)=list(nm_x, nm_exp)
       jx_f$usimlab=vector("list", nb_exp)
       names(jx_f$usimlab)=nm_exp
    }
    x=jx_f$x
    usimlab=jx_f$usimlab
 #browser()
-   if (is.null(labargs$incu)) {
+   if (is.null(labargs$incu) || length(labargs$incu) != 1+nb_xi+nbc_x[nb_w+1L]) {
       labargs$incu=incu=lapply(seq_len(nb_exp), function(iexp) c(1, xi[[iexp]], double(nbc_x[nb_w+1L])))
       # unreduced residuals derivated by scale params
       labargs$dur_dsc=dur_dsc=lapply(seq_len(nb_exp), function(iexp) matrix(0., nrow=nb_meas[[iexp]], ncol=nb_sc_tot))
       labargs$dux_dp=dux_dp=lapply(seq_len(nb_exp), function(iexp) matrix(0., nb_meas[[iexp]], nb_ff+nb_sc_tot+nb_poolf))
    }
    Ali=lapply(seq_len(nb_w), function(iw) fwrv2Abr(lf$fwrv, spa[[iw]], NULL, NULL, getb=FALSE, emu=emu)$A)
    if (cjac) {
@@ -227,24 +228,24 @@
       for (iw in seq_len(nb_w)) {
          nb_c=spa[[iw]]$nb_c
          emuw=ifelse(emu, iw, 1L)
          if (nb_c == 0) {
             next
          }
          ixw=nbc_x[iw]+seq_len(nb_x[iw])
-         incuw=(1L+nb_xi[1L])+ixw
+         incuw=(1L+nb_xi)+ixw
 #cat("iw=", iw, "\there 1\n")
 #if (iw==1) {
 #   print(labargs)
 #   print(spa[[iw]])
 #}
          if (emu) {
             b=fwrv2Abr(lf$fwrv, spa[[iw]], incu[[iexp]], nm$emu[[iexp]][ixw], getA=FALSE, emu=emu)$b
          } else {
-            b=fwrv2Abr(lf$fwrv, spa[[iw]], incu[[iexp]], nm$rcumo[[iexp]][ixw], getA=FALSE, emu=emu)$b
+            b=fwrv2Abr(lf$fwrv, spa[[iw]], incu[[iexp]], nm_x[ixw], getA=FALSE, emu=emu)$b
          }
 #browser()
          xw=try(solve(Ali[[iw]], b), silent=TRUE)
 #print(head(xw))
          if (inherits(xw, "try-error")) {
 #browser()
             rerr=attr(xw, "condition")
@@ -252,15 +253,15 @@
                # find 0 rows if any
                l=spa[[iw]]
                ag=aggregate(abs(lf$fwrv[l$ind_a[,"indf"]]), list(l$ind_a[,"ir0"]), sum)
                izc=ag$Group.1[ag$x <= 1.e-10]
                izf=names(which(abs(lf$fwrv)<1.e-7))
                mes=paste("Cumomer matrix is singular. Try '--clownr N' or/and '--zc N' options with small N, say 1.e-3\nor constrain some of the fluxes listed below to be non zero\n",
                   "Zero rows in cumomer matrix A at weight ", iw, ":\n",
-                  paste(nm$rcumo[ixw][izc+1], collapse="\n"), "\n",
+                  paste(nm$x[ixw][izc+1], collapse="\n"), "\n",
                   "Zero fluxes are:\n",
                   paste(izf, collapse="\n"), "\n",
                   sep="")
             } else {
                mes=as.character(rerr$message)
             }
             return(list(x=NULL, iw=iw, fA=Ali[[iw]], err=1L, mes=mes))
@@ -301,21 +302,21 @@
                bop(x_f, c(1, ba_x, nb_c), "=", j_rhsw)
             }
          }
          ba_x=ba_x+nb_x[iw]
       }
    
       #rownames(incu)=c("one", nm$inp, nm$x)
-      x[, iexp]=tail(incu[[iexp]], -nb_xi[1L]-1L)
+      x[, iexp]=tail(incu[[iexp]], -nb_xi-1L)
       
       # calculate unreduced and unscaled measurements
       if (nrow(x) == ncol(measmat[[iexp]])) {
          mx=(measmat[[iexp]]%stm%x[, iexp])[,1]+memaone[[iexp]]
       } else {
-         mx=(measmat[[iexp]]%stm%x[nm$rcumo_in_cumo, iexp])[,1]+memaone[[iexp]]
+         mx=(measmat[[iexp]]%stm%x[rcumo_in_cumo, iexp])[,1]+memaone[[iexp]]
       }
       # measurement vector before pool ponderation
 #browser()
       if (length(ipooled[[iexp]]) > 1L) {
          mv=meas2sum[[iexp]]%stm%(pwe[[iexp]]*mx)
       } else {
          mv=mx
@@ -744,15 +745,15 @@
       # no system at this weight
       return(list(j_rhsw=NULL, b_x=NULL, j_rhswp=NULL, b_xp=NULL))
    }
    emu=is.matrix(spAbr$ind_b_emu)
    nb_fwrv=spAbr$nb_fwrv
    nb_cl=spAbr$nb_cl
    w=spAbr$w
-   nb_xi=nb$xi[1L]
+   nb_xi=nb$xi
    
    # a_fx
    ind_a=spAbr$ind_a
    if (!is.matrix(ind_a))
       ind_a=t(ind_a)
    i=ind_a[,"ic0"]==ind_a[,"ir0"]
    incu=as.matrix(incu)
@@ -1152,15 +1153,15 @@
    # 2012-07-12 sokol
    # 2016-09-25 sokol: adapted for arbitrary reaction length
    nw=length(spr)
    spemu=spr
    if (nw < 1) {
       return(spemu)
    }
-   nb_xiemu=nb$xiemu[1L]
+   nb_xiemu=nb$xiemu
    #x2tb_f=spr[[1]]$x2tb_f
    nme2iemu=seq_along(nm_inemu)
    names(nme2iemu)=nm_inemu
    ba_e=length(nm_inemu)
    
    # cumo weights are allways start from 1 to weigth max
    # if there is only one weight (max), the lower weights must be present
@@ -1471,14 +1472,15 @@
       lrepx$values=seq_along(lrep$values)
       xmat=simple_triplet_matrix(i=unlist(lapply(lrep$lengths, seq_len)),
          j=inverse.rle(lrepx), v=rep(1, length(iv0)))
       iu0=lrep$values
       i=as.integer(iu0%%nb_c)
       j=as.integer(iu0%/%nb_c)
       l$a=Rmumps$new(i, j, rep(pi, length(iu0)), nb_c)
+#cat("sparse2spa: nb_c=", nb_c, "\n")
       if (!is.null(control_ftbl$mumps)) {
 #browser()
          lapply(grep("^icntl_", names(control_ftbl$mumps), v=TRUE), function(nm) {
             i=suppressWarnings(as.integer(strsplit(nm, "_")[[1L]][2]))
             v=suppressWarnings(as.integer(control_ftbl$mumps[[nm]]))
             if (!is.na(i) && !is.na(v))
                l$a$set_icntl(v, i)
```

### Comparing `influx_si-7.0.2/influx_si/R/opt_icumo_tools.R` & `influx_si-7.0.3/influx_si/R/opt_icumo_tools.R`

 * *Files 4% similar despite different names*

```diff
@@ -176,68 +176,84 @@
    # jacobian is directly derived form discrete scheme and not from ODE solving
    
    # branched from param2fl_usm_eul().
    # 2014-07-09 sokol
    
 #browser()
    # from labargs to local vars
-   #cat("labargs=", format(labargs), "\n")
    for (item in ls(labargs)) {
       assign(item, get(item, env=labargs))
    }
    if (is.null(labargs$getx))
       getx=FALSE
    if (fullsys) {
       spa=spaf
-      nb_rcumos=nb_f$cumos
-      nbc_cumos=c(0L, cumsum(nb_rcumos))
-      nm_x=nm$xf
+      nb_rcumos=nb_f$xf
+      nb_x=nb_f$xf
+      nm_x=nm_list$cumo
       nbc_x=nb_f$nbc_xf
       xi=xif
-      nm_xi=nm$xif
+      rcumo_in_cumo=match(nm_list$rcumo, nm_x)
+      nm_inp=nm_list$xif
+      ip2ix=nb_f$ip2icumo
+      ipf2ix=nb_f$ipf2icumo
    } else {
       nb_rcumos=nb_f$rcumos
-      nbc_cumos=c(0L, cumsum(nb_rcumos))
-      nm_x=nm$x
+      nm_x=nm_list$x
+      nbc_x=nb_f$nbc_x
+      nb_x=nb_f$x
+      nm_inp=nm_list$inp
+      ip2ix=nb_f$ip2ircumo
+      ipf2ix=nb_f$ipf2ircumo
    }
+#print(c(calc="", f=fullsys, labargs=labargs, a=spa[[1]]$a))
+   nbc_cumos=c(0L, cumsum(nb_rcumos))
    nb_w=length(spa)
    nb_ti=nb_f$ti
    nb_tifu=nb_f$tifu
    # cumulated sum
    
    # calculate all fluxes from free fluxes
    fgr=numeric(nb_f$nb_fgr)
-   names(fgr)=nm$nm_fgr
+   names(fgr)=nm_list$fgr
    if (nb_f$nb_fgr) {
       fgr[paste("g.n.", substring(nm$poolf, 4), "_gr", sep="")]=nb_f$mu*param[nm$poolf]
    }
    lf=param2fl(param, labargs)
    fwrv=lf$fwrv
    nb_fwrv=length(lf$fwrv)
-   nb_xi=nb_f$xi
+   nb_xi=length(nm_inp)
    nb_ff=nb_f$nb_ff
    nb_poolf=nb_f$nb_poolf
    nb_fgr=nb_f$nb_fgr
    nb_meas=nb_f$nb_meas
    nb_sc=nb_f$nb_sc
    # fullfill pool with free pools
    if (nb_poolf > 0) {
       pool[nm$poolf]=param[nm$poolf]
    }
    # prepare pool vectors
    # vm has the same length as the full label vector
-   vm=pool[nb_f$ip2ircumo]
+   vm=pool[ip2ix]
    if (cjac) {
       #cat("param2fl_usm_eul2: recalculate jacobian\n")
       jx_f$df_dffp=df_dffp(param, lf$flnx, nb_f, nm_list)
    }
-   Alit=lapply(seq_len(nb_w), function(iw) -fwrv2Abr(fwrv, spa[[iw]], NULL, nm_x[nbc_x[iw]+seq_len(nb_x[iw])], getb=FALSE,  emu=emu)$A$triplet())
+#if (interactive() && fullsys)
+#browser()
+#for (iw in seq_len(nb_w))
+#print(c(iw=iw, f=fullsys, labargs=labargs, a=spa[[iw]]$a))
+   Alit=lapply(seq_len(nb_w), function(iw) {-fwrv2Abr(fwrv, spa[[iw]], NULL, nm_x[nbc_x[iw]+seq_len(nb_x[iw])], getb=FALSE,  emu=emu)$A$triplet()})
+#print(c(calc2="", f=fullsys, labargs=labargs, a=labargs$spa[[1]]$a))
+#stop("aha")
    dtru=unique(unlist(lapply(seq_len(nb_exp), function(iexp) as.character(round(diff(tifull[[iexp]]), 6)))))
    # prepare place for (diag(vm)/dt-a)^-1 common to all iexp
-   if (is.null(labargs$ali_w)) {
+   if (is.null(labargs$ali_w) || sum(sapply(ali_w, function(s) nrow(s[[1]]))) != tail(nbc_x, 1)) {
+#cat("fullsys=", fullsys, "; rebuild ali_w for", tail(nbc_x, 1), "\n", file=fclog)
+#browser()
       ali_w=list()
       for (iw in seq_len(nb_w)) {
          nb_c=spa[[iw]]$nb_c
          emuw=ifelse(emu, iw, 1L)
          vmw=vm[nbc_cumos[iw]+seq_len(nb_c)]
          vmw=rep(vmw, emuw)
          redim(vmw, c(nb_c, emuw))
@@ -250,14 +266,15 @@
             #asp$set_icntl(400, 14) # increase by 400% working space
             #if (packageVersion("rmumps") >= "5.1.1-1")
             #   asp$set_keep(40, 1) # undocumented feature of mumps (cf. their mail on mumps-user group from 12/04/2017)
             return(asp)
          })
          names(ali_w[[iw]])=dtru
       }
+      labargs$ali_w=ali_w
    }
    ntico_max=max(sapply(seq_len(nb_exp), function(iexp) nb_tifu[[iexp]]-1L))
    nb_row_max=max(sapply(seq_len(nb_w), function(iw) {emuw=ifelse(emu, iw, 1L); spa[[iw]]$nb_c*emuw}))
    xpf=double(nbc_x[nb_w+1L]*(nb_ff+nb_poolf)*ntico_max)
    #sfpw=double(nb_row_max*ntico_max*nb_poolf)
    xpfw=double(nb_row_max*(nb_ff+nb_poolf)*ntico_max)
    #xpf1=double(nb_row_max*(nb_ff+nb_poolf))
@@ -267,36 +284,37 @@
       }
       if (!all(ti[[iexp]] %in% tifull[[iexp]])) {
          return(list(err=1, mes="Not all time moments in ti are present in tifull vector"))
       }
       
       # prepare vectors at t1=0 with zero labeling
       # incu, xi is supposed to be in [0; 1]
+      stopifnot(!is.null(dim(xi[[iexp]])))
       x1=c(1., xi[[iexp]][,1L], rep(0., nbc_x[nb_w+1])) # later set m+0 to 1 in x1
-      names(x1)=c("one", nm_inp[[iexp]], nm_x)
+      names(x1)=c("one", nm_inp, nm_x)
       # prepare time vectors
       dt=diff(tifull[[iexp]])
       stopifnot(all(dt > 0.))
       ntico=nb_tifu[[iexp]]-1L # number of time columns
       idt=seq_len(ntico)
       itifu=seq_len(nb_tifu[[iexp]])
       invdt=1./dt
       
       nb_mcol=ncol(measmat[[iexp]])
       # prepare ponderation with actual metab pools
       pwe[[iexp]][ipwe[[iexp]]]=pool[ip2ipwe[[iexp]]]
       spwe=tapply(pwe[[iexp]], pool_factor[[iexp]], sum)
       spwe=1./as.numeric(spwe[nm$measmat[[iexp]]])
       pwe[[iexp]]=pwe[[iexp]]*spwe
-      
-#browser()
       xsim=matrix(x1, nrow=length(x1), ncol=ntico)
-      bop(xsim, c(1, 1, nb_xi[iexp]), "=", xi[[iexp]][,-1])
+      bop(xsim, c(1, 1, nb_xi), "=", xi[[iexp]][,-1])
       
       dimnames(xsim)=list(names(x1), tifull[[iexp]][-1L])
+#if (interactive() && fullsys)
+#browser()
       if (cjac) {
          #cat("param2fl_usm_eul2: recalculate jacobian\n")
          #xpf=double(nbc_x[nb_w+1L]*(nb_ff+nb_poolf)*ntico)
          #redim(xpf, c(nbc_x[nb_w+1L], nb_ff+nb_poolf, ntico))
          resize(xpf, c(nbc_x[nb_w+1L], nb_ff+nb_poolf, ntico))
          if (length(ijpwef[[iexp]])) {
             dpwe=-pwe[[iexp]]*spwe
@@ -310,17 +328,17 @@
       for (iw in seq_len(nb_w)) {
          emuw=ifelse(emu, iw, 1L)
          nb_c=spa[[iw]]$nb_c
          if (nb_c == 0)
             next
 #browser()
          ixw=nbc_x[iw]+seq_len(nb_x[iw])
-         inxw=(1L+nb_xi[iexp])+ixw
+         inxw=(1L+nb_xi)+ixw
          nb_row=nb_c*emuw
-         inrow=(1L+nb_xi[iexp]+nbc_x[iw])+seq_len(nb_row)
+         inrow=(1L+nb_xi+nbc_x[iw])+seq_len(nb_row)
          imw=nbc_x[iw]+seq_len(nb_row) # mass index in x (all but last)
          vmw=vm[nbc_cumos[iw]+seq_len(nb_c)]
          vmw=rep(vmw, emuw)
          redim(vmw, c(nb_c, emuw))
          # prepare (diag(vm)/dt-a)^-1
          if (iexp == 1) {
             ali_w[[iw]][]=lapply(names(ali_w[[iw]]), function(dtu) {
@@ -336,24 +354,27 @@
                   attr(m, "asp")=asp
                   return(m)
                } else {
                   return(asp)
                }
             })
          }
-         ilua=pmatch(dtr, names(ali_w[[iw]]), dup=T)
+         ilua=pmatch(dtr, names(ali_w[[iw]]), dup=TRUE)
          if (emu) {
             # for the first time point, set m+0 to 1 in x1
-            x1[(1L+nb_xi[iexp]+nbc_x[iw])+seq_len(nb_c)]=1.
+            x1[(1L+nb_xi+nbc_x[iw])+seq_len(nb_c)]=1.
             xsim[inxw,1L]=x1[inxw]
             imwl=nbc_x[iw]+nb_row+seq_len(nb_c) # the last mass index in x
          }
          # source terms
          st=fwrv2sp(fwrv, spa[[iw]], xsim, emu=emu)
+         if (any(is.na(st)))
+            return(list(x=NULL, iw=iw, err=1L, mes="NA appeared in source term"))
          st=as.matrix(st)
+#st_save=st+0.
          # calculate labeling for all time points
          xw1=x1[inrow]
          redim(xw1, c(nb_c, emuw))
          #xsim[inxw,]=vapply(idt, function(idtr) {
          #   xw2=lusolve(iadt[[dtr]], (xw1+st[,idtr]))
          #   xw1[] <<- xw2
          #   if (emu) {
@@ -362,23 +383,48 @@
          #      return(xw2)
          #   }
          #}, x1[inxw])
          #xw2=vapply(idt, function(idtr) {
          #   xw2=solve(ali[[ilua[idtr]]], vmw*xw1/dt[idtr]+st[,idtr])
          #   xw1[] <<- xw2
          #}, xw1)
+#if (interactive() && fullsys)
 #browser()
          redim(st, c(nb_c, emuw, ntico))
-         solve_ieu(invdt, xw1, vmw, ali_w[[iw]], st, ilua)
+         tmp=try(solve_ieu(invdt, xw1, vmw, ali_w[[iw]], st, ilua), silent=TRUE)
+         if (inherits(tmp, "try-error")) {
+#browser()
+            rerr=attr(tmp, "condition")
+            if (length(grep("rmumps:.*info\\[1\\]=-10,", rerr$message, fixed=FALSE))) {
+               # find 0 rows if any
+               l=spa[[iw]]
+               ag=aggregate(abs(lf$fwrv[l$ind_a[,"indf"]]), list(l$ind_a[,"ir0"]), sum)
+               izc=ag$Group.1[ag$x <= 1.e-10]
+               izf=names(which(abs(lf$fwrv)<1.e-7))
+               mes=paste("Cumomer matrix is singular. Weight=", iw, ". Try '--clownr N' or/and '--zc N' options with small N, say 1.e-3\nor constrain some of the fluxes listed below to be non zero\n",
+                  "Zero rows in cumomer matrix A at weight ", iw, ":\n",
+                  paste(nm$x[ixw][izc+1], collapse="\n"), "\n",
+                  "Zero fluxes are:\n",
+                  paste(izf, collapse="\n"), "\n",
+                  sep="")
+            } else {
+               mes=as.character(rerr$message)
+            }
+            return(list(x=NULL, iw=iw, err=1L, mes=mes))
+         }
+         if (any(is.na(st))) {
+#browser()
+            return(list(x=NULL, iw=iw, err=1L, mes="NA appeared in ODE solution"))
+         }
          #       dim(xw2)=c(nb_c, emuw, ntico)
          #xsim[inrow,]=st #xw2
-         bop(xsim, c(1, 1L+nb_xi[iexp]+nbc_x[iw], nb_row), "=", st)
+         bop(xsim, c(1, 1L+nb_xi+nbc_x[iw], nb_row), "=", st)
          if (emu) {
-            #xsim[1L+nb_xi[iexp]+imwl,]=1.-arrApply(st, 2, "sum")
-            bop(xsim, c(1, 1L+nb_xi[iexp]+nbc_x[iw]+nb_row, nb_c), "=", 1.-arrApply(st, 2, "sum"))
+            #xsim[1L+nb_xi+imwl,]=1.-arrApply(st, 2, "sum")
+            bop(xsim, c(1, 1L+nb_xi+nbc_x[iw]+nb_row, nb_c), "=", 1.-arrApply(st, 2, "sum"))
          }
          if (cjac) {
 #browser()
             # prepare jacobian ff, pf
             # rhs for all time points on this weight
             # parts before b_x%*%...
             #Rprof(file="fx2jr.Rprof", append=TRUE)
@@ -402,16 +448,16 @@
                jrhs_ff(sj$j_rhs, jx_f$df_dffp, xpfw)
                #if (sum(xpfw[,seq(nb_ff+nb_fgr),]-aperm(tmp, c(1L, 3L, 2L))) > 1.e-14)
                #   browser()
             }
             # poolf part
             if (nb_poolf > 0) {
 #browser()
-               i2x=nb_f$ipf2ircumo[[iexp]][[iw]]
-               i2xf=nb_f$ipf2ircumo[[iexp]][[iw]]
+               i2x=ipf2ix[[iexp]][[iw]]
+               i2xf=ipf2ix[[iexp]][[iw]]
                #bop(i2xf, c(2,2,1), "+=", nb_ff)
                i2xf[,3]=i2xf[,3]+nb_ff
                xw2=(cbind(x1[inrow], xsim[inrow, -ntico, drop=FALSE])-xsim[inrow, , drop=FALSE])%mrv%invdt
                redim(xw2, c(nb_c, emuw, ntico))
                #dim(xw2)=c(nb_c, emuw*ntico)
                #tmp=at%stm%xw2+c(st)
                #dim(tmp)=c(nb_c, emuw, ntico)
@@ -467,29 +513,29 @@
             }
          }
       } # iw loop
       #jx_f$xsim=xsim # for debugging only
       # get ti moments corresponding to measurements
       isel=itifu[tifull[[iexp]] %in% ti[[iexp]]][-1L]-1L
       ntise=length(isel)
-      xsim=xsim[-seq_len(1L+nb_xi[iexp]),, drop=FALSE]
+      xsim=xsim[-seq_len(1L+nb_xi),, drop=FALSE]
       if (getx) {
          xsimf=xsim # full simulation (in time)
          xsim=xsim[,isel,drop=FALSE]
          # usm
-         mx=measmat[[iexp]]%stm%(if (nrow(xsim) == nb_mcol) xsimf else xsimf[nm$rcumo_in_cumo,,drop=FALSE])+memaone[[iexp]]
+         mx=measmat[[iexp]]%stm%(if (nrow(xsim) == nb_mcol) xsimf else xsimf[rcumo_in_cumo,,drop=FALSE])+memaone[[iexp]]
          if (length(ipooled[[iexp]]) > 1L) {
             usmf=as.matrix(meas2sum[[iexp]]%stm%(pwe[[iexp]]*mx)) # full simulated measurements (in time)
          } else {
             usmf=mx
          }
          usm=usmf[,isel,drop=FALSE]
       } else {
          # usm
-         mx=measmat[[iexp]]%stm%(if (nrow(xsim) == nb_mcol) xsim[,isel,drop=FALSE] else xsim[nm$rcumo_in_cumo,isel,drop=FALSE])+memaone[[iexp]]
+         mx=measmat[[iexp]]%stm%(if (nrow(xsim) == nb_mcol) xsim[,isel,drop=FALSE] else xsim[rcumo_in_cumo,isel,drop=FALSE])+memaone[[iexp]]
          if (length(ipooled[[iexp]]) > 1L) {
             usm=as.matrix(meas2sum[[iexp]]%stm%(pwe[[iexp]]*mx))
          } else {
             usm=mx
          }
       }
       
@@ -532,28 +578,27 @@
       jx_f$usm[[iexp]]=usm
       if (getx) {
          jx_f$usmf[[iexp]]=usmf
          jx_f$xsim[[iexp]]=xsim
          jx_f$xsimf[[iexp]]=xsimf
       }
    }
-   if (is.null(labargs$ali_w))
-      labargs$ali_w=ali_w
    if (getx) {
       names(jx_f$usm)=names(jx_f$usmf)=names(jx_f$xsim)=names(jx_f$xsimf)=nm$nm_exp
       res=list(usm=jx_f$usm, usmf=jx_f$usmf, x=jx_f$xsim, xf=jx_f$xsimf, dux_dp=jx_f$dux_dp, lf=lf, df_dffp=jx_f$df_dffp)
    } else {
       names(jx_f$usm)=nm$nm_exp
       res=list(usm=jx_f$usm, dux_dp=jx_f$dux_dp, lf=lf, df_dffp=jx_f$df_dffp)
    }
    return(res)
 }
 
 param2fl_usm_rich=function(param, cjac, labargs, fullsys=FALSE) {
    # Richardson extrapolation to get order 2 in ODE solve
+#print(c(rich="", labargs=labargs, spa_a1=labargs$spa[[1L]]$a))
    if (labargs$time_order=="2") {
       getx=FALSE
       if (!is.null(labargs$getx))
          getx=labargs$getx
       labargs$labargs2$getx=getx
       # solve with step=h/2
       if (!is.null(labargs$cl) && is.null(.GlobalEnv$mc_iter)) {
@@ -564,27 +609,50 @@
 #cat("lila=\n")
 #print(lila)
 #clusterEvalQ(labargs$cl, {cat("usm idth=", idth, "\n"); print(labargs)})
          if (getx)
             clusterEvalQ(labargs$cl, {labargs$labargs2$getx=labargs$getx=TRUE})
          else
             clusterEvalQ(labargs$cl, {labargs$labargs2$getx=labargs$getx=FALSE})
-         res=clusterEvalQ(labargs$cl, if (idw < 3) param2fl_usm_eul2(param, cjac, if (idw == 1) labargs else labargs$labargs2, fullsys))
-         #res=parLapply(labargs$cl, seq(2), function(ith) {cat ("parlap ith=", ith, "\n"); print (labargs); cl_worker(funth=param2fl_usm_eul2, argth=list(param=param, cjac=cjac, labargs=if (ith == 1) labargs else labargs$labargs2))})
+         res=clusterEvalQ(labargs$cl, {
+#print(c(evalq="", labargs=labargs, a=labargs$spa[[1]]$a))
+            if (idw < 3)
+               try(param2fl_usm_eul2(param, cjac, if (idw == 1) labargs else labargs$labargs2, fullsys))
+         })
+         if (length(labargs$cl) < 2L) {
+            res=c(res, clusterEvalQ(labargs$cl, {
+#print(c(evalq2="", labargs=labargs, a=labargs$spa[[1]]$a))
+               try(param2fl_usm_eul2(param, cjac, labargs$labargs2, fullsys))
+            }))
+         }
+#clusterEvalQ(labargs$cl, print(c(rich_cl="", labargs=labargs, spa_a1=labargs$spa[[1L]]$a)))
+         #res=parLapply(labargs$cl, seq(2), function(ith) {
+         #   param2fl_usm_eul2(param, cjac, if (ith == 1) labargs else labargs$labargs2, fullsys)
+         #}) # parLapply() creates new labargs which does not have valid spa[[iw]]$a
       } else {
          # do sequentially
-         res=lapply(seq(2), function(i) param2fl_usm_eul2(param, cjac, if (i == 1) labargs else labargs$labargs2, fullsys))
+         res=lapply(seq(2), function(i) try(param2fl_usm_eul2(param, cjac, if (i == 1) labargs else labargs$labargs2, fullsys), silent=TRUE))
+      }
+      for (i in seq_along(res)) {
+         r=res[[i]]
+         if (inherits(r, "try-error")) {
+            if (interactive())
+               recover()
+            attributes(r)=NULL
+#browser()
+            return(list(err=1L, mes=r, ithread=i))
+         }
       }
       res1=res[[1]]
       if (!is.null(res1$err) && res1$err) {
-         return(list(err=1, mes=res1$mes))
+         return(res1)
       }
       res2=res[[2]]
       if (!is.null(res2$err) && res2$err) {
-         return(list(err=1, mes=res2$mes))
+         return(res2)
       }
       # Richardson interpolation
       jx_f=labargs$jx_f
 #browser()
       for (iexp in seq_len(labargs$nb_exp)) {
          jx_f$usm[[iexp]]=2*res2$usm[[iexp]]-res1$usm[[iexp]]
          if (getx) {
```

### Comparing `influx_si-7.0.2/influx_si/R/plot_ilab.R` & `influx_si-7.0.3/influx_si/R/plot_ilab.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/plot_imass.R` & `influx_si-7.0.3/influx_si/R/plot_imass.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/plot_session.R` & `influx_si-7.0.3/influx_si/R/plot_session.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/plot_smeas.R` & `influx_si-7.0.3/influx_si/R/plot_smeas.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/psoptim_ic.R` & `influx_si-7.0.3/influx_si/R/psoptim_ic.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/test_psoptim_ic.R` & `influx_si-7.0.3/influx_si/R/test_psoptim_ic.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/tools_ssg.R` & `influx_si-7.0.3/influx_si/R/tools_ssg.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/R/upd_deps.R` & `influx_si-7.0.3/influx_si/R/upd_deps.R`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/bin/ff2ftbl.py` & `influx_si-7.0.3/influx_si/bin/ff2ftbl.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2code.py` & `influx_si-7.0.3/influx_si/bin/ftbl2code.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 #  ind_b - dense matrix of indexes for  b_pre$v=f[ind_b[,"indf"]*x[ind_b[,2+1]]*x[ind_b[,2+2]], ...]
 #  b_pre - sparse matrix whose colsum gives b@x
 
 #  a - unsigned sparse cumomer A matrix (off-diagonal part)
 #  b - unsigned sparse vector of right hand side
 
 if (TIMEIT) {
-   cat("spAbr   : ", format(Sys.time()), " cpu=", proc.time()[1], "\\n", sep="", file=fclog)
+   cat("%(var)-8s: ", format(Sys.time()), " cpu=", proc.time()[1], "\\n", sep="", file=fclog)
 }
 
 nb_fwrv=%(n)d
 nb_w=%(nb_w)d
 %(var)s=list()
     """%{
     "var": varname,
@@ -118,15 +118,15 @@
             l_ia.append(atuple)
             #nb_ax+=len(atuple)
             l_ib.append(btuple)
         #print("w=", w, "A=", A, "l_ia=", l_ia, "\n")
         f.write(
 """
 if (TIMEIT) {
-   cat("weight %(w)d: ", format(Sys.time()), " cpu=", proc.time()[1], "\\n", sep="", file=fclog)
+   cat("weight %(w)2d: ", format(Sys.time()), " cpu=", proc.time()[1], "\\n", sep="", file=fclog)
 }
 w=%(w)d
 nb_c=%(nbc)d
 ba_x=%(ba_x)d; # base of cumomer indexes in incu vector
 l=new.env()
 l$w=w
 l$nb_c=nb_c
@@ -524,55 +524,55 @@
     rc_keys_all=[list(d.keys()) for d in netan["rcumo_input"]]
     emu_keys_all=[list(d.keys()) for d in netan["emu_input"]] if emu else []
     #pdb.set_trace()
     f.write("""
 nb_exp=%(nb_exp)d
 nm_exp=c(%(nm_exp)s)
 nm_list$nm_exp=nm_exp
-# input cumomer vectors
+# input cumomer vectors, list of vectors for case_s and matrices (nb_inp x nb_time) for case_i
 xi=list(%(xi)s)
 if (any(lengths(xi) == 0)) {
    stop_mes("No reduced label entry is defined (may be because no measurement provided). Cannot continue.", file=fcerr)
 }
-nm_xi=list(%(nm_xi)s)
+nm_xi=c(%(nm_xi)s) # same for all parallel exps
 for (i in seq_along(xi)) {
-   names(xi[[i]])=nm_xi[[i]]
+   names(xi[[i]])=nm_xi
 }
 nm_list$xi=nm_xi
-nb_xi=lengths(nm_xi)
+nb_xi=length(nm_xi)
 nb_f$xi=nb_xi
 nb_cumoi=nb_xi
 nm_inp=nm_xi
-nm_incu=c("one", nm_xi[[1L]], nm_rcumo)
+nm_incu=c("one", nm_xi, nm_rcumo)
 nm_inlab=nm_incu
 spa=spAbr
 nm_x=nm_rcumo
 nb_x=nb_rcumos
 nb_f$rcumos=nb_rcumos
 nb_f$cumoi=nb_cumoi
 if (emu) {
    nm_emu=c(%(nm_emu)s)
    nb_emus=nb_rcumos*(seq_len(nb_rw)+1)
    nb_f$emus=nb_emus
    nm_list$emu=nm_emu
    nm_x=nm_emu
    nb_x=nb_emus
    xiemu=list(%(xiemu)s)
-   nm_xiemu=list(%(nm_xiemu)s)
+   nm_xiemu=c(%(nm_xiemu)s)
    nm_list$xiemu=nm_xiemu
    for (i in seq_along(xiemu)) {
-       names(xiemu[[i]])=nm_xiemu[[i]]
-    }
-   nb_xiemu=lengths(nm_xiemu)
+       names(xiemu[[i]])=nm_xiemu
+   }
+   nb_xiemu=length(nm_xiemu)
    nb_f$xiemu=nb_xiemu
    nb_f$xi=nb_xiemu
    nb_xi=nb_xiemu
    nm_inp=nm_xiemu
    xi=xiemu
-   nm_inemu=c("one", nm_xiemu[[1L]], nm_emu)
+   nm_inemu=c("one", nm_xiemu, nm_emu)
    nm_inlab=nm_inemu
    spa=spr2emu(spAbr, nm_incu, nm_inemu, nb_f)
 }
 # reorder indexes to accelerate sparse matrix construction
 spa=sparse2spa(spa)
 #browser()
 # composite labeling vector incu c(1, xi, xc) names
@@ -580,17 +580,17 @@
 nm_list$x=nm_x
 nm_list$inp=nm_inp
 nb_f$x=nb_x
     """%{
         "nb_exp": len(netan["iso_input"]),
         "nm_exp": join(", ", netan["exp_names"], '"', '"', width=120),
         "xi": join(",\n", list(join(", ", [li[k] if li[k]==li[k] else "NA"  for k in rc_keys_all[i]], width=120) for i,li in enumerate(netan["rcumo_input"])), "c(", ")"),
-        "nm_xi": join(",\n", list(join(", ", rc_keys, '"', '"', width=120) for rc_keys in rc_keys_all), "c(", ")"),
+        "nm_xi": join(", ", rc_keys_all[0], '"', '"', width=120),
         "xiemu": join(",\n", list(join(", ", [li[k] if li[k]==li[k] else "NA" for k in emu_keys_all[i]], width=120) for i,li in enumerate(netan["emu_input"])), "c(", ")"),
-        "nm_xiemu": join(",\n", list(join(", ", emu_keys, '"', '"', width=120) for emu_keys in emu_keys_all), "c(", ")"),
+        "nm_xiemu": join(", ", emu_keys_all[0] if emu else [], '"', '"', width=120),
         "nm_emu": join(", ", valval(netan.get('vemu', [])), '"', '"', width=120),
         })
     if fullsys:
         d=netan2R_cumo(netan, org, f)
         res.update(d)
         f.write("""
 spaf=sparse2spa(spAbr_f)
```

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2cumoAb.py` & `influx_si-7.0.3/influx_si/bin/ftbl2cumoAb.py`

 * *Files 6% similar despite different names*

```diff
@@ -234,14 +234,31 @@
         "fxch": "\t".join(("" if coef==0 else ssign(coef)+(str(abs(coef)) if abs(coef) !=1. else "")+
             "d.x."+netan["vflux"]["xch"][i-nb_fnet]) for (i,coef) in enumerate(row)
             if i >= nb_fnet),
         "b": join(" + ", ((str(coef) if abs(coef) != 1 else "" if coef == 1 else "-") +("*" if (abs(coef) != 1 and fl) else "")+str(fl)
             for (fl,coef) in netan["bfl"][ir].items()), a="0"),
     })
 
+# prepare numerical values for forward/revers fluxes (from dep, free, constr but not growth (yet))
+fwrv=dict()
+nx2dfcg=netan["nx2dfcg"]
+#import pdb; pdb.set_trace()
+if d_avail:
+    for (fnx, fdfcg) in nx2dfcg.items():
+        nx=fnx[:1]
+        if nx == "x":
+            break # xch fluxes are proceeded simultaneously with their net counterparts
+        reac=fnx[2:]
+        vnet=dfc_val[fdfcg]
+        vxch=dfc_val[nx2dfcg["x."+reac]]
+        vxch=vxch/(1.-vxch)
+        fwd=vxch + (vnet if vnet > 0 else 0)
+        rev=vxch - (vnet if vnet < 0 else 0)
+        fwrv["fwd."+reac]=fwd
+        fwrv["rev."+reac]=rev
 if not invAfl is None:
     # show formulas for dependent fluxes using inverted Afl
     # free, constrained and constant value name to index translator
     nfn=len(netan["vflux_free"]["net"])
     nfx=len(netan["vflux_free"]["xch"])
     nf=nfn+nfx
     ncn=len(netan["vflux_constr"]["net"])
@@ -267,39 +284,38 @@
     # inverse: from index to name
     fl,i=list(zip(*iter(fcv2i.items())))
     i2fcv=np.array(fl)
     i2fcv[np.array(i)]=fl
     
     i,j,v=[ np.array(i) for i in zip(*((i,fcv2i[f],v) for (i,row) in enumerate(netan["bfl"]) if row for (f,v) in row.items())) ]
     
+    ndn=len(netan["vflux"]["net"])
+    ndx=len(netan["vflux"]["xch"])
+    nd=ndn+ndx
     f2bfl=np.zeros((Afl.shape[0], nf+nc+ng+1))
     f2bfl[i,j]=v
     fcv2dep=invAfl*np.matrix(f2bfl)
     f.write("""
 Dependent fluxes as functions of free and constrained fluxes:
 dep.flux=f(free.flux, constr.flux)
 ----------------------------------
 """)
-    ndn=len(netan["vflux"]["net"])
-    ndx=len(netan["vflux"]["xch"])
-    nd=ndn+ndx
     assert fcv2dep.shape[0] == nd, "Bad dimensions dependent fluxes as function of free, constrained and constant values.\nWe should have %d rows, instead we got %d."%(nd, fcv2dep.shape[0])
     ira=np.arange(fcv2dep.shape[1])
     for (ir,row) in enumerate(fcv2dep.A):
         nz=abs(row) >= 1.e-10
         #pdb.set_trace()
         formula=join("", ( (("+" if v > 0 else "-") if abs(abs(v)-1.) < 1.e-10 and f != "" else ("+" if v > 0 else "") + "%s"% Frac.from_float(v).limit_denominator(10000)) + ("*" if f != "" and abs(abs(v)-1) > 1.e-10 else "") + f for (v,f) in zip(row[nz],i2fcv[nz])))
         formula="0" if not formula else formula if formula[0] != "+" else formula[1:]
         f.write("%(dep)s=%(formula)s\n"%{
             "dep": "d.n."+netan["vflux"]["net"][ir] if ir < ndn else "d.x."+netan["vflux"]["xch"][ir-ndn],
             "formula": formula,
         })
 
-# cumomer or emu balance equations
-#pdb.set_trace()
+#import pdb; pdb.set_trace()
 measures={"label": {}, "mass": {}, "peak": {}}
 o_meas=list(measures.keys()); # ordered measure types
 # calculate measure matrices (mapping cumomers to observations)
 f.write("""
 Measurements:
 """)
 for meas in o_meas:
@@ -308,15 +324,16 @@
     #aff(meas, measures[meas]);##
     for iexp in range(len(measures[meas])):
         f.write("%s:\n"%netan["exp_names"][iexp])
         f.write(meas+":\n"+join("\n", (row["scale"]+" "+str(i)+": "+
             join(", ", iter(row["coefs"].items())) for (i,row) in
             enumerate(measures[meas][iexp]["mat"]) if row["coefs"] is not None))+"\n")
 
-Ab=C13_ftbl.rcumo_sys(netan, emu)
+# cumomer or emu balance equations
+Ab=C13_ftbl.rcumo_sys(netan, emu) # will be overwritten if fullsys
 vcumo=netan.get("vrcumo")
 if emu:
     f.write("\n# EMU fragment system\n")
 elif reduced:
     f.write("\n# reduced to measurable cumomers system\n")
 else:
     Ab=netan["cumo_sys"]
@@ -330,27 +347,52 @@
     #for r_cumo in sorted(A.keys()):
     for r_cumo in vcumo[w]:
         # output term
         f.write("%(c)s*(%(f)s)" % ({
                 "c": r_cumo,
                 "f": join("+", A[r_cumo][r_cumo]),
             }))
+        # central numerical value
+        numstr=""
+        if d_avail:
+            numstr += "%(c)s*(%(f)s)" % {
+                "c": r_cumo,
+                "f": sum(fwrv[v] for v in A[r_cumo][r_cumo]),
+            }
         # input terms
-        term=join("+",("%(c)s*(%(f)s)" % ({
-              "c": c_cumo,
-              "f": join("+", A[r_cumo][c_cumo]),
-            }) for c_cumo in vcumo[w] if c_cumo in A[r_cumo] and c_cumo != r_cumo))
-            #}) for c_cumo in sorted(A[r_cumo].keys()) if c_cumo != r_cumo))
+        term=join(" + ",("%(c)s*(%(f)s)" % {
+            "c": c_cumo,
+            "f": join("+", A[r_cumo][c_cumo]),
+        } for c_cumo in A[r_cumo].keys() if c_cumo != r_cumo))
+        #}) for c_cumo in sorted(A[r_cumo].keys()) if c_cumo != r_cumo))
+        
         if term:
-            f.write("-("+term+")")
+            f.write(" - ("+term+")")
+            if d_avail:
+                numstr += " - (%(term)s"%{
+                    "term": join("+",("%(c)s*(%(f)s)" % ({
+                      "c": c_cumo,
+                      "f": sum(fwrv[v] for v in A[r_cumo][c_cumo]),
+                    }) for c_cumo in A[r_cumo].keys() if c_cumo != r_cumo))
+                }
         # rhs
         if r_cumo not in Ab["b"][w]:
-            f.write("=0.\n")
-            continue
-        f.write("="+join("+", ("%(f)s*(%(pc)s)" % ({
+            f.write(" = 0.\n")
+            if d_avail:
+                numstr += " = 0.\n"
+        else:
+            f.write(" = "+join("+", ("%(f)s*(%(pc)s)" % ({
                 "f": fl,
                 "pc": join("+", (join("*", Ab["b"][w][r_cumo][fl][i])
                     for i in Ab["b"][w][r_cumo][fl]))
             }) for fl in Ab["b"][w][r_cumo]))+"\n")
-
+            # numeric values
+            if d_avail :
+                numstr += " = "+join("+", ("%(f)s*(%(pc)s)" % ({
+                    "f": fwrv[fl],
+                    "pc": join("+", (join("*", Ab["b"][w][r_cumo][fl][i])
+                        for i in Ab["b"][w][r_cumo][fl]))
+                }) for fl in Ab["b"][w][r_cumo]))+"\n"
+        if d_avail:
+            f.write(numstr)
 #f.close(); # no need to close stdout
 #f.write(str(netan["emu_input"])+"\n")
```

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2kvh.py` & `influx_si-7.0.3/influx_si/bin/ftbl2kvh.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2netan.py` & `influx_si-7.0.3/influx_si/bin/ftbl2netan.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2optR.py` & `influx_si-7.0.3/influx_si/bin/ftbl2optR.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,17 @@
 
 # read measvecti from file(s) specified in ftbl(s)
 flabcin=c(%(flabcin)s)
 measvecti=ti=tifull=tifull2=vector("list", nb_exp)
 nb_ti=nb_tifu=nb_tifu2=integer(nb_exp)
 nsubdiv_dt=pmax(1L, as.integer(c(%(nsubdiv_dt)s)))
 nb_f$ipf2ircumo=nb_f$ipf2ircumo2=list()
-nminvm=nm_poolall[matrix(unlist(strsplit(nm_rcumo, ":", fixed=TRUE)), ncol=2, byrow=T)[,1L]]
+nminvm=nm_poolall[matrix(unlist(strsplit(nm_rcumo, ":", fixed=TRUE)), ncol=2L, byrow=TRUE)[,1L]]
+if (fullsys)
+   nminvmf=nm_poolall[matrix(unlist(strsplit(nm_cumo, ":", fixed=TRUE)), ncol=2L, byrow=TRUE)[,1L]]
 for (iexp in seq_len(nb_exp)) {
    if (tmax[iexp] < 0) {
       stop_mes(sprintf("The parameter tmax must not be negative (tmax=%%g in '%%s.ftbl')", tmax[iexp], nm_exp[iexp]), file=fcerr)
    }
    if (dt[iexp] <= 0) {
       stop_mes(sprintf("The parameter dt must be positive (dt=%%g in '%%s.ftbl')", dt[iexp], nm_exp[iexp]), file=fcerr)
    }
@@ -508,42 +510,71 @@
       colnames(i2)=c("ipoolf", "ic", "iw", "iti")
       i=i[i[,1L]!=0L,,drop=FALSE]
       i2=i2[i2[,1L]!=0L,,drop=FALSE]
       # put the poolf column last
       nb_f$ipf2ircumo[[iexp]][[iw]]=i[, c("ic", "iw", "ipoolf", "iti"), drop=FALSE]
       nb_f$ipf2ircumo2[[iexp]][[iw]]=i2[, c("ic", "iw", "ipoolf", "iti"), drop=FALSE]
    }
+   if (fullsys) {
+      # prepare mapping of metab pools on cumomers for full system (emu is FALSE here)
+      nb_f$ipf2icumo[[iexp]]=nb_f$ipf2icumo2[[iexp]]=list()
+      for (iw in seq_len(nb_w)) {
+         ix=seq_len(nb_cumos[iw])
+         ipf2icumo=ipf2icumo2=match(nminvmf[nbc_cumos[iw]+ix], nm_poolf, nomatch=0L)
+         dims=c(1L, nb_cumos[iw], 1L, nb_tifu[iexp]-1L)
+         dims2=c(1L, nb_cumos[iw], 1L, nb_tifu2[iexp]-1L)
+         i=as.matrix(ipf2icumo)
+         i2=as.matrix(ipf2icumo2)
+         for (id in 2L:length(dims)) {
+            cstr=sprintf("cbind(%srep(seq_len(dims[id]), each=prod(dims[seq_len(id-1L)])))", paste("i[, ", seq_len(id-1L), "], ", sep="", collapse=""))
+            i=eval(parse(text=cstr))
+         }
+         for (id in 2L:length(dims2)) {
+            cstr=sprintf("cbind(%srep(seq_len(dims2[id]), each=prod(dims2[seq_len(id-1L)])))", paste("i2[, ", seq_len(id-1L), "], ", sep="", collapse=""))
+            i2=eval(parse(text=cstr))
+         }
+         colnames(i)=c("ipoolf", "ic", "iw", "iti")
+         colnames(i2)=c("ipoolf", "ic", "iw", "iti")
+         i=i[i[,1L]!=0L,,drop=FALSE]
+         i2=i2[i2[,1L]!=0L,,drop=FALSE]
+         # put the poolf column last
+         nb_f$ipf2icumo[[iexp]][[iw]]=i[, c("ic", "iw", "ipoolf", "iti"), drop=FALSE]
+         nb_f$ipf2icumo2[[iexp]][[iw]]=i2[, c("ic", "iw", "ipoolf", "iti"), drop=FALSE]
+      }
+   }
 }
 xil=vector("list", nb_exp)
 xi2=vector("list", nb_exp)
 for (iexp in seq(nb_exp)) {
    fli=funlabli[[iexp]]
    if (length(fli) == 0) {
       # replicate first column in xi as many times as there are time points
       if (time_order == "2" || time_order == "1,2")
          xi2[[iexp]]=matrix(xi[[iexp]], nrow=length(xi[[iexp]]), ncol=nb_tifu2[[iexp]])
       xil[[iexp]]=matrix(xi[[iexp]], nrow=length(xi[[iexp]]), ncol=nb_tifu[[iexp]])
    }  else {
       # use funlab
-      env=new.env() # funlab code won't see influx's variables
+      envfunlab=new.env() # funlab code won't see influx's variables
       if (nchar(funlabR[[iexp]])) {
          if (file.exists(funlabR[[iexp]])) {
-            es=try(source(funlabR[[iexp]], local=env), outFile=fcerr)
+            es=try(source(funlabR[[iexp]], local=envfunlab), outFile=fcerr)
          } else {
             stop_mes("funlab script R '", funlabR[[iexp]], "' from '", nm_exp[[iexp]],"' does not exist.", file=fcerr)
          }
       }
-      xil[[iexp]]=funlab(tifull[[iexp]], nm_inp[[iexp]], fli, env, emu, nm_exp[[iexp]], fcerr)
+      xil[[iexp]]=funlab(tifull[[iexp]], nm_inp, fli, envfunlab, emu, nm_exp[[iexp]], fcerr)
       if (time_order == "2" || time_order == "1,2")
-         xi2[[iexp]]=funlab(tifull2[[iexp]], nm_inp[[iexp]], fli, env, emu, nm_exp[[iexp]], fcerr)
+         xi2[[iexp]]=funlab(tifull2[[iexp]], nm_inp, fli, envfunlab, emu, nm_exp[[iexp]], fcerr)
    }
 }
 xi=xil
 
 nb_f$ip2ircumo=match(nminvm, nm_poolall)
+if (fullsys)
+   nb_f$ip2icumo=match(nminvmf, nm_poolall)
 nb_f$tifu=nb_tifu
 nb_f$tifu2=nb_tifu2
 
 # label state at t=0 (by default=0 but later it should be able to be specified by user)
 x0=NULL
 nb_f$ti=nb_ti
     """)
@@ -657,15 +688,15 @@
 if (nb_poolf > 0L) {
    dupm_dp=cbind(dupm_dp, measurements$mat$pool[,nm_list$poolf, drop=FALSE])
 }
 dimnames(dupm_dp)=list(rownames(measurements$mat$pool), nm_par)
 
 #browser()
 # prepare argument list for passing to label simulating functions
-nm_labargs=c("jx_f", "nb_f", "nm_list", "nb_x", "invAfl", "p2bfl", "g2bfl", "bp", "fc", "xi", "spa", "spaf", "emu", "pool", "measurements", "ipooled", "ir2isc",  "nb_w", "nb_rw", "nbc_x", "measmat", "memaone", "dufm_dp", "dupm_dp", "pwe", "ipwe", "ip2ipwe", "pool_factor", "ijpwef", "ipf_in_ppw", "meas2sum", "dp_ones", "clen", "dirr", "dirw", "dirres", "baseshort", "case_i", "nb_exp", "noscale", "dpw_dpf")
+nm_labargs=c("jx_f", "nb_f", "nm_list", "nb_x", "invAfl", "p2bfl", "g2bfl", "bp", "fc", "xi", "spa", "spaf", "emu", "pool", "measurements", "ipooled", "ir2isc",  "nb_w", "nb_rw", "nbc_x", "measmat", "memaone", "dufm_dp", "dupm_dp", "pwe", "ipwe", "ip2ipwe", "pool_factor", "ijpwef", "ipf_in_ppw", "meas2sum", "dp_ones", "clen", "dirr", "dirw", "dirres", "baseshort", "case_i", "nb_exp", "noscale", "dpw_dpf", "fclog", "fcerr")
     """)
     if case_i:
         f.write("""nm_labargs=c(nm_labargs, "ti", "tifull", "tifull2", "x0", "time_order")
         """)
     f.write("""
 if (TIMEIT) {
    cat("labargs : ", format(Sys.time()), " cpu=", proc.time()[1], "\\n", sep="", file=fclog)
@@ -702,15 +733,16 @@
 cl=NULL
 if ((case_i && (time_order %in% c("1,2", "2"))) || sensitive == "mc") {
    if (np > 1L) {
       # prepare cluster
       nodes=if (sensitive == "mc") np else 2
 
       # prepare cluster
-      cl=makeCluster(nodes, cl_type) #, outfile="cl.log")
+      cl=makeCluster(nodes, cl_type) #)
+      #cl=makeCluster(1L, cl_type, manual=TRUE, outfile="")
 #cat("make cluster=")
 #print(cl[[1]])
       labargs[["cl"]]=cl
       nodes=length(cl)
       if (TIMEIT) {
          cat("cl expor: ", format(Sys.time()), " cpu=", proc.time()[1], "\n", sep="", file=fclog)
       }
@@ -736,24 +768,32 @@
          #loadcmp(file.path(dirr, "nlsic.Rc"))
          #loadcmp(file.path(dirr, "opt_cumo_tools.Rc"))
          #loadcmp(file.path(dirr, "opt_icumo_tools.Rc"))
          labargs$spa=sparse2spa(labargs$spa)
          if (case_i && (time_order == "2" || time_order == "1,2")) {
             labargs$labargs2$spa=labargs$spa
          }
+         if (fullsys) {
+            labargs$spaf=sparse2spa(labargs$spaf)
+            if (case_i && (time_order == "2" || time_order == "1,2")) {
+               labargs$labargs2$spaf=labargs$spaf
+            }
+         }
 #cat("evalQ idth=", idth, "\n")
 #print(labargs)
 #print(labargs$labargs2)
 #print(labargs$spa)
 #print(labargs$labargs2$spa)
+#print(list(cre_cl="", labargs=labargs, spa_a1=labargs$spa[[1L]]$a))
          NULL
       })
       clusterSetRNGStream(cl)
       # set worker id
       idw=parLapply(cl, seq_along(cl), function(i) assign("idw", i, envir=.GlobalEnv))
+
    } else {
       labargs$cl=NULL
    }
 }
 for (irun in seq_len(nseries)) {
    if (TIMEIT) {
       cat(sprintf("run %4d: %s cpu=%g\n", irun, format(Sys.time()), proc.time()[1]), "\n", sep="", file=fclog)
@@ -1000,15 +1040,16 @@
       cat("starting point\\n", file=fkvh)
       names(param)=nm_par
       obj2kvh(param, "starting free parameters", fkvh, indent=1)
    }
 #browser()
    if (!length(rres)) {
       if (write_res) {
-         capture.output(rres <- lab_resid(param, cjac=FALSE, labargs), file=fclog)
+         #capture.output(rres <- lab_resid(param, cjac=FALSE, labargs), file=fclog)
+         rres <- lab_resid(param, cjac=FALSE, labargs)
       } else {
          rres <- lab_resid(param, cjac=FALSE, labargs)
       }
       if (!is.null(rres$err) && rres$err) {
          cat("lab_resid", runsuf, ": ", rres$mes, "\\n", file=fcerr, sep="")
          #close(fkvh)
          retcode[irun]=rres$err
@@ -1541,28 +1582,75 @@
    if (fullsys) {
    """)
     cu_keys=list(netan["cumo_input"][0].keys()) if netan["fullsys"] else []
     f.write("""
       nm_xif=c(%s)
       # full label input is the same for all experiments
       xif=rep(list(c(%s)), nb_exp)"""%(join(", ", cu_keys, '"', '"'),
-         join(", ", [li[k] for li in netan["cumo_input"] for k in cu_keys]),
+         join(", ", [(li[k] if li[k]==li[k] else "NA") for li in netan["cumo_input"] for k in cu_keys]),
     ))
     f.write("""
       xif=lapply(xif, setNames, nm_xif)
-      nm_list$xif=nm_xif
+      if (case_i) {
+         # prepare xif from funlab
+         xilf=vector("list", nb_exp)
+         xi2f=vector("list", nb_exp)
+         for (iexp in seq(nb_exp)) {
+            fli=funlabli[[iexp]]
+            if (length(fli) == 0) {
+               # replicate first column in xi as many times as there are time points
+               if (time_order == "2" || time_order == "1,2")
+                  xi2f[[iexp]]=matrix(xif[[iexp]], nrow=length(xif[[iexp]]), ncol=nb_tifu2[[iexp]])
+               xilf[[iexp]]=matrix(xif[[iexp]], nrow=length(xif[[iexp]]), ncol=nb_tifu[[iexp]])
+            }  else {
+               # use funlab
+               xilf[[iexp]]=funlab(tifull[[iexp]], nm_xif, fli, envfunlab, emu=FALSE, nm_exp[[iexp]], fcerr)
+               if (time_order == "2" || time_order == "1,2")
+                  xi2f[[iexp]]=funlab(tifull2[[iexp]], nm_xif, fli, envfunlab, emu=FALSE, nm_exp[[iexp]], fcerr)
+            }
+         }
+         xif=xilf
+         if (time_order == "2" || time_order == "1,2") {
+            labargs$labargs2$xif=xi2f
+            labargs$labargs2$nm_list$inp=nm_xif
+            labargs$labargs2$emu=FALSE
+         }
+      }
+      labargs$nm_list$xif=nm_xif
+      labargs$nm_list$inp=nm_xif
       labargs$emu=FALSE
       labargs$xif=xif
-      labargs$nb_f$xif=lengths(xif)
+      labargs$nb_f$xif=length(xif[[1L]])
+      labargs$labargs2$nm_list$xif=nm_xif
+      labargs$labargs2nm_list$inp=nm_xif
+      labargs$labargs2emu=FALSE
+      labargs$labargs2xif=xif
+      labargs$labargs2nb_f$xif=length(xif[[1L]])
+      if (case_i && !is.null(labargs$cl)) {
+         clusterExport(labargs$cl, c("labargs"))
+         clusterEvalQ(labargs$cl, {
+            labargs$spa=sparse2spa(labargs$spa)
+            labargs$labargs2$spa=labargs$spa
+            labargs$spaf=sparse2spa(labargs$spaf)
+            labargs$labargs2$spaf=labargs$spaf
+#print(c(lab_new="", labargs=labargs, labargs2=labargs$labargs2, a1_1=labargs$spaf[[1]]$a, a1_2=labargs$labrags2spaf[[1]]$a))
+         })
+      }
       v=lab_sim(param, cjac=FALSE, labargs, fullsys)
       if (identical(v$err, 1L)) {
-         save(v$fA$triplet(), file="singular237_triplet.RData")
+         #save(v$fA$triplet(), file="singular237_triplet.RData")
          stop_mes("fullsys: weight=", v$iw, "; ", v$mes, file=fcerr)
       }
+#browser()
       labargs$emu=emu
+      labargs$nm_list$inp=nm_inp
+      if (time_order == "2" || time_order == "1,2") {
+         labargs$labargs2$nm_list$inp=nm_inp
+         labargs$labargs2$emu=emu
+      }
       x=if (case_i) v$xf else v$x
    } else {
       v=lab_sim(param, cjac=FALSE, labargs)
       x=if (case_i) v$xf else v$x
    }
 
    # write some info in result kvh
```

### Comparing `influx_si-7.0.2/influx_si/bin/ftbl2xgmml.py` & `influx_si-7.0.3/influx_si/bin/ftbl2xgmml.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/bin/res2ftbl_meas.py` & `influx_si-7.0.3/influx_si/bin/res2ftbl_meas.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/ftbl2labcin.py` & `influx_si-7.0.3/influx_si/ftbl2labcin.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/ftbl2metxml.py` & `influx_si-7.0.3/influx_si/ftbl2metxml.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/ftbl2mtf.py` & `influx_si-7.0.3/influx_si/ftbl2mtf.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/influx_s.py` & `influx_si-7.0.3/influx_si/influx_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     return(retcode)
 
 def main(argv=sys.argv[1:]):
     """example: influx_s.main(["--prefix", "path/to/mtf"])
 Call influx_s.main(["-h"]) for a help message"""
     global me
     # my own name
-    me=os.path.realpath(sys.argv[0])
+    me=os.path.realpath(__file__)
     # my install dir
     dirinst=os.path.dirname(os.path.realpath(influx_si.__file__))
     dirbin=os.path.join(dirinst, "bin")
 
     me=os.path.basename(me)
     if me[:8]=="influx_i":
         case_i=True
```

### Comparing `influx_si-7.0.2/influx_si/licence_en.txt` & `influx_si-7.0.3/influx_si/licence_en.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/README.txt` & `influx_si-7.0.3/influx_si/test/README.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/e_coli.ftbl` & `influx_si-7.0.3/influx_si/test/e_coli.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/e_coli_growth.ftbl` & `influx_si-7.0.3/influx_si/test/e_coli_growth.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/e_coli_i.ftbl` & `influx_si-7.0.3/influx_si/test/e_coli_i.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/e_coli_iv.ftbl` & `influx_si-7.0.3/influx_si/test/e_coli_iv.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/e_coli_msen.txt` & `influx_si-7.0.3/influx_si/test/e_coli_msen.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ex_i_2box_var.ftbl` & `influx_si-7.0.3/influx_si/test/ex_i_2box_var.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/Akin.tsv` & `influx_si-7.0.3/influx_si/test/mtf/Akin.tsv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli.miso` & `influx_si-7.0.3/influx_si/test/mtf/e_coli.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli.netw` & `influx_si-7.0.3/influx_si/test/mtf/e_coli.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli.tvar` & `influx_si-7.0.3/influx_si/test/mtf/e_coli.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.linp` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.linp`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.miso` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.mmet` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.mmet`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.netw` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.tvar` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_growth.tvar.def` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_growth.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_i.ikin` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_i.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_i.miso` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_i.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_i.netw` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_i.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_i.tvar` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_i.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.miso` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.netw` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/mtf/e_coli_iv.tvar` & `influx_si-7.0.3/influx_si/test/mtf/e_coli_iv.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/Akin.tsv` & `influx_si-7.0.3/influx_si/test/ok/mtf/Akin.tsv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.miso` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.netw` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.tvar` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli.tvar.def` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.linp` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.linp`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.miso` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.mmet` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.mmet`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.netw` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.tvar` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth.tvar.def` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.log` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mmet.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.mmet.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.pdf` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/e_coli_growth.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.ftbl` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.pres.csv` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth.pres.csv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/e_coli_growth_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.netflux.e_coli_growth.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.netflux.e_coli_growth.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.xchflux.e_coli_growth.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_growth_res/tmp/edge.xchflux.e_coli_growth.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.miso` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.netw` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.tvar` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i.tvar.def` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.log` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.pdf` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/e_coli_i.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ftbl` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ikin` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.pres.csv` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i.pres.csv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/e_coli_i_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.netflux.e_coli_i.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.netflux.e_coli_i.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.xchflux.e_coli_i.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/edge.xchflux.e_coli_i.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_i_res/tmp/node.log2pool.e_coli_i.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_i_res/tmp/node.log2pool.e_coli_i.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.miso` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.netw` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.tvar` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv.tvar.def` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.log` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.pdf` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/e_coli_iv.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.ftbl` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/e_coli_iv_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.netflux.e_coli_iv.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.netflux.e_coli_iv.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.xchflux.e_coli_iv.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_iv_res/tmp/edge.xchflux.e_coli_iv.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.log` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.pdf` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/e_coli.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/e_coli.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.ftbl` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.pres.csv` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli.pres.csv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/e_coli_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/edge.netflux.e_coli.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/edge.netflux.e_coli.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/e_coli_res/tmp/edge.xchflux.e_coli.attrs` & `influx_si-7.0.3/influx_si/test/ok/mtf/e_coli_res/tmp/edge.xchflux.e_coli.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.log` & `influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.pdf` & `influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/ex_i_2box_var.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.ftbl` & `influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/mtf/ex_i_2box_var_res/tmp/ex_i_2box_var_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.netw` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.tvar` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X_MS.txt` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_X_MS.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.netw` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_X.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.log` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/e_coli_GX_prl.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ikin` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_X.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ikin` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/e_coli_GX_prl_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.netflux.e_coli_GX_prl.attrs` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.netflux.e_coli_GX_prl.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.xchflux.e_coli_GX_prl.attrs` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_GX_prl_res/tmp/edge.xchflux.e_coli_GX_prl.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.cnstr` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.cnstr`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.netw` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar.def` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n.tvar.def`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.log` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.log`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.tvar.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc1-6n.tvar.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc2n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc3n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc4n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc5n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.miso.sim` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.miso.sim`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.pdf` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/e_coli_glc6n.pdf`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.pres.csv` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n.pres.csv`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n_res.kvh` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc1-6n_res.kvh`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc2n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc2n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc3n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc3n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc4n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc4n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc5n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc5n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc6n.ftbl` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/e_coli_glc6n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.netflux.e_coli_glc1-6n.attrs` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.netflux.e_coli_glc1-6n.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.xchflux.e_coli_glc1-6n.attrs` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc1-6n_res/tmp/edge.xchflux.e_coli_glc1-6n.attrs`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc2n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc3n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc4n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc5n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.miso` & `influx_si-7.0.3/influx_si/test/ok/prl_exp/mtf/e_coli_glc6n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_MS.txt` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_MS.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_X.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_X.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_X_MS.txt` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_X_MS.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_GX_prl.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_GX_prl.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc1-6n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc1-6n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc2n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc2n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc3n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc3n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc4n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc4n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc5n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc5n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/e_coli_glc6n.ftbl` & `influx_si-7.0.3/influx_si/test/prl_exp/e_coli_glc6n.ftbl`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.ikin` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.netw` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X.tvar` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_X_MS.txt` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_X_MS.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.ikin` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.ikin`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.netw` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_GX_prl.tvar` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_GX_prl.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.cnstr` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.cnstr`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.netw` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.netw`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.tvar` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc1-6n.tvar`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc2n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc2n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc3n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc3n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc4n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc4n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc5n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc5n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/test/prl_exp/mtf/e_coli_glc6n.miso` & `influx_si-7.0.3/influx_si/test/prl_exp/mtf/e_coli_glc6n.miso`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/tools_ssg.py` & `influx_si-7.0.3/influx_si/tools_ssg.py`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/influx_si/txt2ftbl.py` & `influx_si-7.0.3/influx_si/txt2ftbl.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,17 +455,17 @@
             ffrag=""
         else:
             ffrag=frag.replace("-", "~")
         val=df.loc[ligr, "Value"].to_numpy()
         sdv=df.loc[ligr, "SD"].to_numpy()
         # detect kind of species
         spec=df.loc[ligr, "Isospecies"]
-        if all(spec.str.match("^ *M\d+ *$")):
+        if all(spec.str.match(r"^ *M\d+ *$")):
             kind="ms"
-        elif all(spec.str.match("^[ 01x+]+$")):
+        elif all(spec.str.match(r"^[ 01x+]+$")):
             kind="lab"
         elif all(spec.str.contains("->")):
             sep="->"
             kind="peak"
         elif all(spec.str.contains("→")):
             sep="→"
             kind="peak"
@@ -497,23 +497,23 @@
                 werr("parse_miso: invalid MS weight '%s' in group %s in '%s':%d-%d"%(w[w>flen].astype(str)[0], kgr, fname, ist, iend))
             if not case_i and len(ligr) > flen+1:
                 raise Excpetion("parse_miso: too many MS entries %d (max %d expected) in group %s in '%s':%d-%d"%(kgr, len(ligr) , flen+1, fname, ist, iend))
             # add this group to results
             #if frag == "":
             #    frag=",".join(str(i) for i in range(1,flen+1))
             if case_i:
-                #if met == "Phe":
-                    #pdb.set_trace()
                 res["ms"] += [f"\t{met}\t{ffrag}\t{w[0]}\tNA\t{sdv[0]}"+"   // %s: %d"%(fname, ist)]
                 res["ms"] += [f"\t\t\t{w[i0]}\tNA\t{sdv[i0]}"+"   // %s: %s"%(fname, df.loc[ligr[i0], "iline"]) for i,i0 in zip(range(1, len(spli)), ii0[1:])]
                 #pdb.set_trace()
                 if not dfgr[dfgr["Time"] != ""].empty:
                     for sp,spi in dsp.items():
                         df_kin=dfconcat(df_kin, pa.DataFrame(df.loc[spi, "Value"].to_numpy().reshape(1, -1), columns=df.loc[spi, "Time"], index=[f"m:{met}:{ffrag}:{sp[1:]}:{df.loc[spi[0],'iline']}"]))
             else:
+                #if met == "Phe":
+                    #pdb.set_trace()
                 res["ms"] += [f"\t{met}\t{ffrag}\t{w[0]}\t{val[0]}\t{sdv[0]}"+"   // %s: %d"%(fname, ist)]
                 res["ms"] += [f"\t\t\t{w[i]}\t{val[i]}\t{sdv[i]}"+"   // %s: %s"%(fname, df.loc[ligr[i], "iline"]) for i in range(1, len(ligr))]
         elif kind == "lab" or kind == "mean":
             # label group (like 01x+1x1)
             if kind == "lab":
                 labs=[[vv.strip() for vv in v.split("+")] for v in df.loc[ligr, "Isospecies"]]
             elif kind == "peak":
@@ -1218,15 +1218,15 @@
 Auxiliary ftbl names will be put in 'OPTIONS/prl_exp' field on the main ftbl file.
 These names will be written there in a form relative to the main ftbl.
 To shorten the writings, it is possible to indicate only one of two .miso/.linp files.
 The other one will be guessed if it has canonical extension. If extension is omitted then .miso and .linp files are searched with these extensions. In this case, several parallel experiments can be given with one --eprl option. So that above example can be shorten to:
   'txt2ftbl --mtf ec.netw,glc6.linp,glc6.miso --eprl glc1,glc4'
 """)
     parser.add_argument("--inst", action="store_true", default=False, help=
-"""Prepare FTBL for instationary case. File 'netw' is supposed to have 
+"""Prepare FTBL for instationary case. File 'miso' is supposed to have 
 column 'Time' non empty. Isotopic kinetic data will be written to a TSV 
 file with 'ikin' extension. Its name will be the same as in FTBL file, 
 and FTBL field 'OPTIONS/file_labcin' will contain 'ikin' file name.
 """)
     parser.add_argument("--force", action="store_true", default=False, help=
 """Overwrite an existent result file not produced by this script.
 NB. If a result file exists and is actually produced by this script,
```

### Comparing `influx_si-7.0.2/influx_si.egg-info/PKG-INFO` & `influx_si-7.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: influx-si
-Version: 7.0.2
+Name: influx_si
+Version: 7.0.3
 Summary: Metabolic flux and concentration estimation based on stable isotope labeling
 Home-page: https://github.com/sgsokol/influx/
 Author: Serguei Sokol
 Author-email: sokol@insa-toulouse.fr
 License: GNU General Public License v2 or later (GPLv2+)
 Project-URL: Documentation, https://influx-si.readthedocs.io/
 Project-URL: Source, https://github.com/sgsokol/influx
```

### Comparing `influx_si-7.0.2/influx_si.egg-info/SOURCES.txt` & `influx_si-7.0.3/influx_si.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 influx_si/../test_cases/cases_influx_si-v5.4.0.tab
 influx_si/../test_cases/cases_influx_si-v6.0.3.tab
 influx_si/../test_cases/cases_influx_si-v6.0.4.tab
 influx_si/../test_cases/cases_influx_si-v6.0.tab
 influx_si/../test_cases/cases_influx_si-v6.1.tab
 influx_si/../test_cases/cases_influx_si-v7.0.1.tab
 influx_si/../test_cases/cases_influx_si-v7.0.2.tab
+influx_si/../test_cases/cases_influx_si-v7.0.3.tab
 influx_si/../test_cases/cases_influx_si-v7.0.tab
 influx_si/../test_cases/test_report_5.0.1.txt
 influx_si/../test_cases/test_report_5.0.2.txt
 influx_si/../test_cases/test_report_5.0.3.txt
 influx_si/../test_cases/test_report_5.1.0.txt
 influx_si/../test_cases/test_report_5.2.0.txt
 influx_si/../test_cases/test_report_5.3.0.txt
@@ -60,14 +61,15 @@
 influx_si/../test_cases/test_report_6.0.3.txt
 influx_si/../test_cases/test_report_6.0.4.txt
 influx_si/../test_cases/test_report_6.0.txt
 influx_si/../test_cases/test_report_6.1.txt
 influx_si/../test_cases/test_report_6.2.txt
 influx_si/../test_cases/test_report_7.0.1.txt
 influx_si/../test_cases/test_report_7.0.2.txt
+influx_si/../test_cases/test_report_7.0.3.txt
 influx_si/../test_cases/test_report_7.0.txt
 influx_si/R/funlab.R
 influx_si/R/libs.R
 influx_si/R/load.R
 influx_si/R/opt_cumo_tools.R
 influx_si/R/opt_icumo_tools.R
 influx_si/R/plot_ilab.R
```

### Comparing `influx_si-7.0.2/setup.py` & `influx_si-7.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    keywords='metabolic flux analysis, least squares, isotope labeling, systems biology',
    license="GNU General Public License v2 or later (GPLv2+)",
    long_description=long_description,
    author='Serguei Sokol',
    author_email='sokol@insa-toulouse.fr',
    url="https://github.com/sgsokol/influx/",
    packages=['influx_si'],
-   package_data={'influx_si': ['licence_en.txt', 'influx_version.txt', 'R/*.R', 'test/*/*/*/*', '../test_cases/test_report_[0-9]*.txt', '../test_cases/cases_influx_si-v*.tab']},
+   package_data={'influx_si': ['licence_en.txt', 'influx_version.txt', 'R/*.R', 'test/*/*/*/*', f'../test_cases/test_report_{version}.txt', '../test_cases/cases_influx_si-v*.tab']},
    include_package_data=True,
    install_requires=['scipy', 'python-libsbml', 'pandas', 'kvh'],
    scripts=[
       'influx_si/bin/ff2ftbl.py',
       'influx_si/bin/ftbl2code.py',
       'influx_si/bin/ftbl2cumoAb.py',
       'influx_si/bin/ftbl2kvh.py',
```

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v3.0.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v3.0.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v3.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v3.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v3.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v3.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v3.2.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v3.2.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.0.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.0.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.2.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.2.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.3.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.3.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.4.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.4.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.4.2.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.4.2.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.4.3.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.4.3.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.4.5.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.4.5.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.4.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.4.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v4.5dev.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v4.5dev.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.0.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.0.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.0.2.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.0.2.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.0.3.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.0.3.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.1.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.1.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.1.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.1.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.2.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.2.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.3.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.3.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v5.4.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v5.4.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v6.0.3.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v6.0.3.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v6.0.4.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v6.0.4.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v6.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v6.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v6.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v6.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v7.0.1.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v7.0.1.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v7.0.2.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v7.0.2.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/cases_influx_si-v7.0.tab` & `influx_si-7.0.3/test_cases/cases_influx_si-v7.0.tab`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.0.1.txt` & `influx_si-7.0.3/test_cases/test_report_5.0.1.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.0.2.txt` & `influx_si-7.0.3/test_cases/test_report_5.0.2.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.0.3.txt` & `influx_si-7.0.3/test_cases/test_report_5.0.3.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.1.0.txt` & `influx_si-7.0.3/test_cases/test_report_5.1.0.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.2.0.txt` & `influx_si-7.0.3/test_cases/test_report_5.2.0.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.3.0.txt` & `influx_si-7.0.3/test_cases/test_report_5.3.0.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_5.4.0.txt` & `influx_si-7.0.3/test_cases/test_report_5.4.0.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_6.0.3.txt` & `influx_si-7.0.3/test_cases/test_report_6.0.3.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_6.0.4.txt` & `influx_si-7.0.3/test_cases/test_report_6.0.4.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_6.0.txt` & `influx_si-7.0.3/test_cases/test_report_6.0.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_6.1.txt` & `influx_si-7.0.3/test_cases/test_report_6.1.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_6.2.txt` & `influx_si-7.0.3/test_cases/test_report_6.2.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_7.0.1.txt` & `influx_si-7.0.3/test_cases/test_report_7.0.1.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_7.0.2.txt` & `influx_si-7.0.3/test_cases/test_report_7.0.2.txt`

 * *Files identical despite different names*

### Comparing `influx_si-7.0.2/test_cases/test_report_7.0.txt` & `influx_si-7.0.3/test_cases/test_report_7.0.txt`

 * *Files identical despite different names*

