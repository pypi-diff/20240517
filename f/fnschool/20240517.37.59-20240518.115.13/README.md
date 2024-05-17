# Comparing `tmp/fnschool-20240517.37.59.tar.gz` & `tmp/fnschool-20240518.115.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240517.37.59.tar", last modified: Thu May 16 16:38:03 2024, max compression
+gzip compressed data, was "fnschool-20240518.115.13.tar", last modified: Fri May 17 17:15:15 2024, max compression
```

## Comparing `fnschool-20240517.37.59.tar` & `fnschool-20240518.115.13.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.985209 fnschool-20240517.37.59/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240517.37.59/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12294 2024-05-16 16:38:03.984209 fnschool-20240517.37.59/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240517.37.59/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240517.37.59/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 16:38:03.985209 fnschool-20240517.37.59/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.961209 fnschool-20240517.37.59/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.968209 fnschool-20240517.37.59/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)     1762 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.975209 fnschool-20240517.37.59/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6663 2024-05-16 16:07:48.000000 fnschool-20240517.37.59/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240517.37.59/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      949 2024-05-16 16:14:41.000000 fnschool-20240517.37.59/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.977209 fnschool-20240517.37.59/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240517.37.59/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240517.37.59/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240517.37.59/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240517.37.59/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240517.37.59/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240517.37.59/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.981209 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1858 2024-05-16 15:54:26.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-16 15:54:49.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9332 2024-05-16 16:35:43.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-16 15:55:13.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-16 15:53:12.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10929 2024-05-16 15:53:38.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9750 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2282 2024-05-16 15:52:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240517.37.59/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.981209 fnschool-20240517.37.59/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240517.37.59/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.964209 fnschool-20240517.37.59/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.963209 fnschool-20240517.37.59/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.982209 fnschool-20240517.37.59/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.963209 fnschool-20240517.37.59/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.982209 fnschool-20240517.37.59/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    18082 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.963209 fnschool-20240517.37.59/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.982209 fnschool-20240517.37.59/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.964209 fnschool-20240517.37.59/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.982209 fnschool-20240517.37.59/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.964209 fnschool-20240517.37.59/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.983209 fnschool-20240517.37.59/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 16:37:59.000000 fnschool-20240517.37.59/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 15:51:57.000000 fnschool-20240517.37.59/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 16:38:03.983209 fnschool-20240517.37.59/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12294 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 16:38:03.000000 fnschool-20240517.37.59/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.703045 fnschool-20240518.115.13/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-17 17:15:15.703045 fnschool-20240518.115.13/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-17 17:15:15.703045 fnschool-20240518.115.13/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.686046 fnschool-20240518.115.13/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.691046 fnschool-20240518.115.13/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      378 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3116 2024-05-17 17:07:47.000000 fnschool-20240518.115.13/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.697045 fnschool-20240518.115.13/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240518.115.13/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-17 16:08:29.000000 fnschool-20240518.115.13/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240518.115.13/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      949 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.698046 fnschool-20240518.115.13/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240518.115.13/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240518.115.13/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240518.115.13/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240518.115.13/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240518.115.13/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-17 16:33:52.000000 fnschool-20240518.115.13/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.701045 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-17 16:02:00.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2282 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4492 2024-05-17 16:33:53.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-17 16:33:56.000000 fnschool-20240518.115.13/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240518.115.13/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.701045 fnschool-20240518.115.13/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240518.115.13/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-17 16:08:56.000000 fnschool-20240518.115.13/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.688046 fnschool-20240518.115.13/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.687046 fnschool-20240518.115.13/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.701045 fnschool-20240518.115.13/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.687046 fnschool-20240518.115.13/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.702045 fnschool-20240518.115.13/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18082 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.687046 fnschool-20240518.115.13/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.702045 fnschool-20240518.115.13/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.687046 fnschool-20240518.115.13/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.702045 fnschool-20240518.115.13/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.688046 fnschool-20240518.115.13/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.702045 fnschool-20240518.115.13/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-17 17:15:13.000000 fnschool-20240518.115.13/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-17 16:00:10.000000 fnschool-20240518.115.13/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240518.115.13/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-17 17:15:15.702045 fnschool-20240518.115.13/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-17 17:15:15.000000 fnschool-20240518.115.13/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240517.37.59/LICENSE` & `fnschool-20240518.115.13/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/PKG-INFO` & `fnschool-20240518.115.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240517.37.59
+Version: 20240518.115.13
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240517.37.59/README.md` & `fnschool-20240518.115.13/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/pyproject.toml` & `fnschool-20240518.115.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/bill.cp.py` & `fnschool-20240518.115.13/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/bill.py` & `fnschool-20240518.115.13/src/fnschool/canteen/bill.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         self._time_nodes = None
         self._operator_name = None
         self._food_classes = None
         self._operator = None
         self.currency = Currency().CNY
         self._consuming = None
 
-        print_app_name()
         pass
 
     @property
     def consuming(self):
         if not self._consuming:
             self._consuming = Consuming(self)
         return self._consuming
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/canteen.toml` & `fnschool-20240518.115.13/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/config.py` & `fnschool-20240518.115.13/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/consuming.py` & `fnschool-20240518.115.13/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240518.115.13/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240518.115.13/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240518.115.13/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/food.cp.py` & `fnschool-20240518.115.13/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/food.py` & `fnschool-20240518.115.13/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/food_classes.toml` & `fnschool-20240518.115.13/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/operator.py` & `fnschool-20240518.115.13/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/path.py` & `fnschool-20240518.115.13/src/fnschool/canteen/path.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 if not canteen_links_dpath.exists():
     os.makedirs(canteen_links_dpath, exist_ok=True)
 
 if not operator_name_fpath.exists():
     with open(operator_name_fpath, "w", encoding="utf-8") as f:
         f.write("")
-    os.link(
-        operator_name_fpath.as_posix(), operator_name_link_fpath.as_posix()
-    )
+    os.link(operator_name_fpath.as_posix(), operator_name_link_fpath.as_posix())
 
 
 def get_food_classes_config_fpath(user_name):
     fpath = user_config_dir / user_name / "food_classes.toml"
 
     if not fpath.exists():
         shutil.copy(food_classes_config0_fpath, fpath)
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/profile.py` & `fnschool-20240518.115.13/src/fnschool/canteen/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,15 @@
                         + "    ]\n"
                         + "]\n"
                         + "# {the_end}"
                     ).format(
                         profile_label=_("Profile label"),
                         operator_name=_("Operator name"),
                         operator_email=_("Operator email"),
-                        organization_name=_(
-                            "Organization name or school name"
-                        ),
+                        organization_name=_("Organization name or school name"),
                         supplier_name_1=_("Supplier name 1"),
                         supplier_name_2=_("Supplier name 2"),
                         the_end=_("The end."),
                     )
                 )
             print_warning(_("Please update your profile file."))
             print_info(
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         self.spreadsheet = self.bill.spreadsheet
         self.s = self.spreadsheet
         self.bill_workbook = self.spreadsheet.bill_workbook
         self.bwb = self.bill_workbook
         self.sheet_name = None
         self._sheet = None
         self._form_indexes = None
-        self.cell_alignment0 = Alignment(
-            horizontal="center", vertical="center"
-        )
+        self.cell_alignment0 = Alignment(horizontal="center", vertical="center")
         self.cell_side0 = Side(border_style="thin")
         self.cell_border0 = Border(
             top=self.cell_side0,
             left=self.cell_side0,
             right=self.cell_side0,
             bottom=self.cell_side0,
         )
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,22 +90,22 @@
 
             csheet.cell(
                 form_index1 + 1,
                 1,
                 (
                     "   "
                     + "审核人："
-                    + "        "
+                    + "          "
                     + "经办人："
+                    + self.operator.name
                     + "　    "
                     + "过称人："
-                    + self.operator.name
-                    + "      "
+                    + "         "
                     + "仓管人："
-                    + " 　"
+                    + " 　      "
                 ),
             )
 
             row_difference = (
                 tfoods_len + len(classes_without_food) - food_index_len
             )
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,15 @@
                         [
                             _count * food.unit_price
                             for _date, _count in food.consumptions
                         ]
                     )
             total_price += m_total_price
             cssheet.cell(row[0].row, 2, m_total_price)
-            cssheet.cell(row[0].row, 2).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            cssheet.cell(row[0].row, 2).number_format = numbers.FORMAT_NUMBER_00
 
         total_price_CNY = self.bill.get_CNY_chars(total_price)
         cssheet.cell(
             2,
             1,
             f"编制单位：{self.purchaser}       "
             + f"单位：元         "
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,17 +212,15 @@
         consuming_m_cp = consuming_m
         consuming_m = (
             _("Consuming of this month: ") + currency_mark + str(consuming_m)
         )
 
         month_day_m1 = sorted([f.xdate for f in cfoods])[0]
         for f in cfoods:
-            month_day_m1 = max(
-                [d for d, __ in f.consumptions] + [month_day_m1]
-            )
+            month_day_m1 = max([d for d, __ in f.consumptions] + [month_day_m1])
 
         inventory_m = sum(
             [
                 f.get_remainder(month_day_m1) * f.unit_price
                 for f in cfoods
                 if f.get_remainder(month_day_m1) > 0
             ]
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,15 @@
             tn1 = time_nodes[i + 1]
             tn0 = time_nodes[i]
             tn0_cp = tn0
             if not tn0.month == tn1.month:
                 tn0 = datetime(tn1.year, tn1.month, 1)
 
             wbfoods = [
-                f
-                for f in cfoods
-                if f.get_remainder(tn0) > 0 and f.xdate <= tn0
+                f for f in cfoods if f.get_remainder(tn0) > 0 and f.xdate <= tn0
             ]
             for wbfood in [f for f in wbfoods if f.xdate < tn0]:
                 if not wbfood.name.endswith(residual_mark):
                     wbfood.name = wbfood.name + residual_mark
 
             col_index = 0
             for d_index in range(0, (tn1 - tn0).days + 1):
@@ -130,32 +128,28 @@
                 _(
                     "Sheet '{0}' of \"{1}\" was updated.\n"
                     + "Press any key to continue when you have "
                     + "completed the foods allocation."
                 ).format(sheet.title, wb_fpath)
             )
             new_wbfoods = [
-                f
-                for f in cfoods
-                if f.get_remainder(tn1) > 0 and f.xdate == tn1
+                f for f in cfoods if f.get_remainder(tn1) > 0 and f.xdate == tn1
             ]
             if len(new_wbfoods) > 0:
                 print_info(
                     (
                         _("New purchased food for date {0} is:")
                         if len(new_wbfoods) > 1
                         else _("New purchased foods for date {0} are:")
                     ).format(tn1.strftime("%Y.%m.%d"))
                 )
 
                 new_wbfoods_count_len = len(str(len(new_wbfoods)))
 
-                number_mark = random.choice(
-                    [" ", ".", ">", "-", ")", ":", "|"]
-                )
+                number_mark = random.choice([" ", ".", ">", "-", ")", ":", "|"])
                 new_wbfood_tips = [
                     (
                         f"{i+1:>{new_wbfoods_count_len}}"
                         + number_mark
                         + f"{f.name} {f.count} {f.unit_name}"
                     )
                     for i, f in enumerate(new_wbfoods)
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,15 @@
 
     def update_fclass(self):
         wb = load_workbook(self.path)
         sheet = wb.active
         headers = [
             h
             for h in [
-                sheet.cell(1, ci).value
-                for ci in range(1, sheet.max_column + 1)
+                sheet.cell(1, ci).value for ci in range(1, sheet.max_column + 1)
             ]
             if h
         ]
         if self.food_class_col_name in headers:
             wb.close
             return
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,20 +94,16 @@
             total_price += food.total_price
             unwsheet.cell(row_index, 1, food.xdate.strftime("%Y.%m.%d"))
             unwsheet.cell(row_index, 2, food.name)
             unwsheet.cell(row_index, 3, food.unit_name)
             unwsheet.cell(row_index, 4, food.count)
             unwsheet.cell(row_index, 5, food.unit_price)
             unwsheet.cell(row_index, 6, food.total_price)
-            unwsheet.cell(row_index, 5).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
-            unwsheet.cell(row_index, 6).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            unwsheet.cell(row_index, 5).number_format = numbers.FORMAT_NUMBER_00
+            unwsheet.cell(row_index, 6).number_format = numbers.FORMAT_NUMBER_00
 
             for u_col_index in range(1, 7):
                 cell = unwsheet.cell(row_index, u_col_index)
                 cell.alignment = self.cell_alignment0
                 cell.border = self.cell_border0
 
             if (
```

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240518.115.13/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/test.py` & `fnschool-20240518.115.13/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/canteen/workbook.py` & `fnschool-20240518.115.13/src/fnschool/canteen/workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,15 @@
         self._unit_df = None
         self._negligible_class_list = None
         self._base_class_df = None
         self.purchase_workbook_fdpath = None
         self.pre_consuming_sheet_col_index_offset = 5
         self.pre_consuming_sheet_row_index_offset = 3
         self.spreadsheet_ext_names = ["xlsx"]
-        self.cell_alignment0 = Alignment(
-            horizontal="center", vertical="center"
-        )
+        self.cell_alignment0 = Alignment(horizontal="center", vertical="center")
         self.cell_side0 = Side(border_style="thin")
         self.cell_border0 = Border(
             top=self.cell_side0,
             left=self.cell_side0,
             right=self.cell_side0,
             bottom=self.cell_side0,
         )
@@ -483,19 +481,15 @@
                     _total_price += f.count * f.unit_price
             cvsheet.cell(row[0].row, 2, _total_price)
 
             total_price += _total_price
         cvsheet.cell(10, 2, total_price)
 
         w_seasoning_total_price = sum(
-            [
-                f.count * f.unit_price
-                for f in wfoods
-                if ("调味" in f.class_name)
-            ]
+            [f.count * f.unit_price for f in wfoods if ("调味" in f.class_name)]
         )
         unw_seasoning_total_price = sum(
             [
                 f.count * f.unit_price
                 for f in uwfoods
                 if ("调味" in f.class_name)
             ]
@@ -1034,18 +1028,15 @@
                 if ptimes:
                     print_info(
                         _(
                             "The food purchasing times of preadsheet {0} is {1} ."
                         ).format(
                             _file,
                             " | ".join(
-                                [
-                                    ptime.strftime("%Y.%m.%d")
-                                    for ptime in ptimes
-                                ]
+                                [ptime.strftime("%Y.%m.%d") for ptime in ptimes]
                             ),
                         )
                     )
                     properties.append([_file, sheet_name, chwb_fpath, ptimes])
 
         return properties if properties else None
 
@@ -1141,17 +1132,15 @@
             t0, t1 = time_node
             wb = load_workbook(fpath)
             sheet = wb[self.pre_consuming_sheet0_name]
             ckt0, ckt1 = self.bill.get_check_times(time_node)
             _foods = [
                 f
                 for f in foods
-                if (
-                    f.xdate <= ckt1 and f.remainder > 0 and not f.is_negligible
-                )
+                if (f.xdate <= ckt1 and f.remainder > 0 and not f.is_negligible)
             ]
             if len(_foods) < 1:
                 print_warning(
                     _(
                         "There is not food of time node %s ,skip workbook designing."
                     )
                     % (t0.strftime("%Y.%m.%d") + t1.strftime("%Y.%m.%d"))
@@ -1311,17 +1300,15 @@
                 if not any(
                     [o == self.bill.profile.org_name for o in _org_names]
                 ):
                     print_warning(
                         (
                             _('Organization name read from {0} are "{1}",')
                             if len(_org_names) > 1
-                            else _(
-                                'Organization name read from {0} is "{1}", '
-                            )
+                            else _('Organization name read from {0} is "{1}", ')
                         ).format(wb_fpath, " | ".join(_org_names))
                         + _('but organization name of {0} is "{1}".').format(
                             f"{self.profile.label}({self.profile.name})",
                             self.profile.org_name,
                         )
                     )
                     print_error(
@@ -1633,17 +1620,15 @@
         indexes_len = len(indexes)
         _index = None
         if indexes_len <= tn_index:
             return None
         _index = indexes[tn_index]
         return _index
 
-    def update_inventory_sheet_of_time_node(
-        self, fd_path=None, time_node=None
-    ):
+    def update_inventory_sheet_of_time_node(self, fd_path=None, time_node=None):
         fd_path = self.purchase_workbook_fd_path or fd_path
         time_node = time_node or self.bill.time_node
         t0, t1 = time_node
         isheet = self.get_inventory_sheet()
         foods = self.food.time_node_residue_foods
         (
             iform_index0,
@@ -1773,17 +1758,15 @@
                             _count * food.unit_price
                             for _date, _count in food.consuming_list
                             if _date.month == self.bill.month
                         ]
                     )
             total_price += _total_price
             cssheet.cell(row[0].row, 2, _total_price)
-            cssheet.cell(row[0].row, 2).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            cssheet.cell(row[0].row, 2).number_format = numbers.FORMAT_NUMBER_00
 
         total_price_cn = self.bill.convert_num_to_cnmoney_chars(total_price)
         cssheet.cell(
             2,
             1,
             f"编制单位：{self.bill.profile.org_name}       "
             + f"单位：元         "
@@ -1795,17 +1778,15 @@
             (f"总金额（大写)：{total_price_cn}    " + f"¥{total_price:.2f}"),
         )
         cssheet.cell(12, 1, f"经办人：{self.bill.profile.name}  ")
 
         wb = self.get_bill_workbook()
         wb.active = cssheet
 
-        print_info(
-            _("Sheet '%s' was updated.") % self.consuming_sum_sheet_name
-        )
+        print_info(_("Sheet '%s' was updated.") % self.consuming_sum_sheet_name)
 
     def update_consuming_sheet(self):
         foods = self.food.get_foods()
         csheet = self.get_consuming_sheet()
         form_indexes = self.get_consuming_form_indexes()
 
         time_nodes = self.bill.get_time_nodes()
@@ -2082,17 +2063,15 @@
         return none
 
     def get_unwarehousing_form_indexes(self):
         unwsheet = self.get_unwarehousing_sheet()
         indexes = []
         row_index = 1
         for row in unwsheet.iter_rows(max_row=unwsheet.max_row + 1, max_col=7):
-            if row[0].value and "未入库明细表" in row[0].value.replace(
-                " ", ""
-            ):
+            if row[0].value and "未入库明细表" in row[0].value.replace(" ", ""):
                 indexes.append([row_index + 1, 0])
 
             if row[1].value and "合计" in row[1].value.replace(" ", ""):
                 indexes[-1][1] = row_index
 
             row_index += 1
 
@@ -2267,17 +2246,15 @@
                     start_column=1,
                     end_column=8,
                 )
 
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(
-            _("Sheet '%s' was formatted.") % self.warehousing_sheet_name
-        )
+        print_info(_("Sheet '%s' was formatted.") % self.warehousing_sheet_name)
 
     def update_unwarehousing_sheet(self):
         unwsheet = self.get_unwarehousing_sheet()
         form_indexes = self.get_unwarehousing_form_indexes()
         time_nodes = [
             tn
             for tn in self.bill.get_time_nodes()
@@ -2321,20 +2298,16 @@
             total_price += food.total_price
             unwsheet.cell(row_index, 1, food.xdate.strftime("%Y.%m.%d"))
             unwsheet.cell(row_index, 2, food.name)
             unwsheet.cell(row_index, 3, food.unit_name)
             unwsheet.cell(row_index, 4, food.count)
             unwsheet.cell(row_index, 5, food.unit_price)
             unwsheet.cell(row_index, 6, food.total_price)
-            unwsheet.cell(row_index, 5).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
-            unwsheet.cell(row_index, 6).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            unwsheet.cell(row_index, 5).number_format = numbers.FORMAT_NUMBER_00
+            unwsheet.cell(row_index, 6).number_format = numbers.FORMAT_NUMBER_00
             if (
                 str(unwsheet.cell(row_index + 1, 2).value)
                 .replace(" ", "")
                 .endswith("合计")
                 and len(foods) - 1 > _index
             ):
                 unwsheet.cell(row_index + 1, 2, "合计")
@@ -2352,17 +2325,15 @@
                         " ", ""
                     ).endswith("合计"):
                         row[2].value = "总合计" if use_forms else "合计"
                         row[6].value = total_price
                         break
                 break
 
-        print_info(
-            _("Sheet '%s' was updated.") % self.unwarehousing_sheet_name
-        )
+        print_info(_("Sheet '%s' was updated.") % self.unwarehousing_sheet_name)
 
     def update_warehousing_sheet(self):
         wsheet = self.get_warehousing_sheet()
         foods = [
             f
             for f in self.food.get_foods()
             if (
@@ -2410,17 +2381,15 @@
             food_index1 = form_index1 - 1
             entry_index = food_index0
             warehousing_n = windex + 1
 
             wfoods = [f for f in foods if (f.xdate == time_point)]
             foods_class_names = [f.class_name for f in wfoods]
             class_names_without_food = [
-                _name
-                for _name in class_names
-                if not _name in foods_class_names
+                _name for _name in class_names if not _name in foods_class_names
             ]
             row_difference = (
                 len(wfoods)
                 + len(class_names_without_food)
                 - (food_index1 - food_index0 + 1)
             )
 
@@ -2538,17 +2507,15 @@
                     for cell in row:
                         cell.value = ""
 
         self.format_warehousing_sheet()
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(
-            _("Sheet '%s' was updated.") % (self.warehousing_sheet_name)
-        )
+        print_info(_("Sheet '%s' was updated.") % (self.warehousing_sheet_name))
 
     def get_unit_df(self):
         if not self._unit_df is None:
             return self._unit_df
         self._unit_df = pd.read_excel(
             self.get_main_spreadsheet_path(),
             sheet_name=self.unit_sheet_name,
```

### Comparing `fnschool-20240517.37.59/src/fnschool/entry.py` & `fnschool-20240518.115.13/src/fnschool/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from fnschool import *
 
 
 def set_canteen(args):
     from fnschool.canteen.bill import Bill
 
+    print_app()
+
     bill = Bill()
     if args.action in "mk_bill":
         bill.make_spreadsheets()
 
     else:
         print_info(_("Function is not found."))
```

### Comparing `fnschool-20240517.37.59/src/fnschool/external.py` & `fnschool-20240518.115.13/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/fnprint.py` & `fnschool-20240518.115.13/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/language.py` & `fnschool-20240518.115.13/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240518.115.13/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-16 21:56+0800\n"
+"POT-Creation-Date: 2024-05-18 00:29+0800\n"
 "PO-Revision-Date: 2024-05-16 21:56+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `fnschool-20240517.37.59/src/fnschool/path.py` & `fnschool-20240518.115.13/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool/test.py` & `fnschool-20240518.115.13/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240517.37.59/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240518.115.13/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240517.37.59
+Version: 20240518.115.13
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240517.37.59/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240518.115.13/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

