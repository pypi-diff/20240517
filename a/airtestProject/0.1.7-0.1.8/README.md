# Comparing `tmp/airtestproject-0.1.7.tar.gz` & `tmp/airtestproject-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-ng2y3l89\airtestproject-0.1.7.tar", last modified: Tue May 14 08:08:14 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-sy2adf9u\airtestproject-0.1.8.tar", last modified: Fri May 17 10:57:23 2024, max compression
```

## Comparing `airtestproject-0.1.7.tar` & `airtestproject-0.1.8.tar`

### file list

```diff
@@ -1,75 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.232102 airtestproject-0.1.7/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      786 2024-05-14 08:08:14.231104 airtestproject-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-05-11 00:14:26.000000 airtestproject-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.147936 airtestproject-0.1.7/airtestProject/
--rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.7/airtestProject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.160902 airtestproject-0.1.7/airtestProject/abstractBase/
--rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.7/airtestProject/abstractBase/OperateBase.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/abstractBase/__init__.py
--rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.7/airtestProject/abstractBase/loginBase.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.163893 airtestproject-0.1.7/airtestProject/commons/
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.165887 airtestproject-0.1.7/airtestProject/commons/Position/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/Position/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.168880 airtestproject-0.1.7/airtestProject/commons/Position/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/Position/odin/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.7/airtestProject/commons/Position/odin/odinPos.py
--rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.7/airtestProject/commons/UWA.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.169876 airtestproject-0.1.7/airtestProject/commons/page/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/page/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.177857 airtestproject-0.1.7/airtestProject/commons/page/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/__init__.py
--rw-rw-rw-   0        0        0    18812 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/funcListCheck.py
--rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/login.py
--rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/run.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.179852 airtestproject-0.1.7/airtestProject/commons/process/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/process/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.182842 airtestproject-0.1.7/airtestProject/commons/process/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/process/odin/__init__.py
--rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/process/odin/profile.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.212120 airtestproject-0.1.7/airtestProject/commons/utils/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/air.py
--rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.7/airtestProject/commons/utils/appStart.py
--rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/command.py
--rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.7/airtestProject/commons/utils/deploy.py
--rw-rw-rw-   0        0        0     5655 2024-05-11 00:07:48.000000 airtestproject-0.1.7/airtestProject/commons/utils/excel_image.py
--rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.7/airtestProject/commons/utils/exception.py
--rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.7/airtestProject/commons/utils/factory.py
--rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/ganaratePyCase.py
--rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/genaratePy.py
--rw-rw-rw-   0        0        0     3786 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/gotCommon.py
--rw-rw-rw-   0        0        0     5616 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/logger.py
--rw-rw-rw-   0        0        0    11825 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/myAirtest.py
--rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/myPoco.py
--rw-rw-rw-   0        0        0     8139 2024-05-10 23:57:10.000000 airtestproject-0.1.7/airtestProject/commons/utils/ocrTemplate.py
--rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/page.py
--rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.7/airtestProject/commons/utils/reportUtil.py
--rw-rw-rw-   0        0        0        0 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/test.py
--rw-rw-rw-   0        0        0     1744 2024-05-11 00:02:22.000000 airtestproject-0.1.7/airtestProject/commons/utils/tools.py
--rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/utils.py
--rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.7/airtestProject/config.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.216141 airtestproject-0.1.7/airtestProject/factory/
--rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.7/airtestProject/factory/SingletonFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/factory/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/factory/operateFactory.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.226117 airtestproject-0.1.7/airtestProject/manager/
--rw-rw-rw-   0        0        0     9352 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/manager/DeviceManager.py
--rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.7/airtestProject/manager/LogManager.py
--rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/PackageManager.py
--rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/ReportManager.py
--rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/TaskManager.py
--rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/TestCaseManager.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.229110 airtestproject-0.1.7/airtestProject/scripts/
--rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.7/airtestProject/scripts/OdinExample.py
--rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.7/airtestProject/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.230106 airtestproject-0.1.7/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      786 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:08:14.233103 airtestproject-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      848 2024-05-14 08:07:14.000000 airtestproject-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.780642 airtestproject-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      786 2024-05-17 10:57:23.778647 airtestproject-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-11 00:14:26.000000 airtestproject-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.671534 airtestproject-0.1.8/airtestProject/
+-rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.8/airtestProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.686521 airtestproject-0.1.8/airtestProject/abstractBase/
+-rw-rw-rw-   0        0        0     1997 2024-05-17 08:50:57.000000 airtestproject-0.1.8/airtestProject/abstractBase/OperateBase.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/abstractBase/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-05-15 11:52:58.000000 airtestproject-0.1.8/airtestProject/abstractBase/aiBase.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.689485 airtestproject-0.1.8/airtestProject/abstractBase/aiBaseImp/
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:29:27.000000 airtestproject-0.1.8/airtestProject/abstractBase/aiBaseImp/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-05-15 11:52:58.000000 airtestproject-0.1.8/airtestProject/abstractBase/aiBaseImp/aiBaseImp.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.694473 airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/
+-rw-rw-rw-   0        0        0        0 2024-05-15 06:44:53.000000 airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/__init__.py
+-rw-rw-rw-   0        0        0    11892 2024-05-17 02:28:26.000000 airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/airtestOperate.py
+-rw-rw-rw-   0        0        0     7329 2024-05-16 03:34:11.000000 airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/pocoOperate.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.698462 airtestproject-0.1.8/airtestProject/commons/
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.700457 airtestproject-0.1.8/airtestProject/commons/Position/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/Position/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.703449 airtestproject-0.1.8/airtestProject/commons/Position/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/Position/odin/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.8/airtestProject/commons/Position/odin/odinPos.py
+-rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.8/airtestProject/commons/UWA.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.705443 airtestproject-0.1.8/airtestProject/commons/page/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/page/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.711428 airtestproject-0.1.8/airtestProject/commons/page/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/page/odin/__init__.py
+-rw-rw-rw-   0        0        0    18854 2024-05-17 08:22:26.000000 airtestproject-0.1.8/airtestProject/commons/page/odin/funcListCheck.py
+-rw-rw-rw-   0        0        0     9170 2024-05-17 08:50:57.000000 airtestproject-0.1.8/airtestProject/commons/page/odin/login.py
+-rw-rw-rw-   0        0        0     6434 2024-05-15 04:45:40.000000 airtestproject-0.1.8/airtestProject/commons/page/odin/run.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.713719 airtestproject-0.1.8/airtestProject/commons/process/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/process/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.716739 airtestproject-0.1.8/airtestProject/commons/process/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/process/odin/__init__.py
+-rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/process/odin/profile.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.753611 airtestproject-0.1.8/airtestProject/commons/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/utils/air.py
+-rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.8/airtestProject/commons/utils/appStart.py
+-rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/utils/command.py
+-rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.8/airtestProject/commons/utils/deploy.py
+-rw-rw-rw-   0        0        0     5655 2024-05-11 00:07:48.000000 airtestproject-0.1.8/airtestProject/commons/utils/excelPicture.py
+-rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.8/airtestProject/commons/utils/exception.py
+-rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.8/airtestProject/commons/utils/factory.py
+-rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/utils/ganaratePyCase.py
+-rw-rw-rw-   0        0        0     2731 2024-05-15 11:13:04.000000 airtestproject-0.1.8/airtestProject/commons/utils/genaratePy.py
+-rw-rw-rw-   0        0        0     3786 2024-05-14 03:10:27.000000 airtestproject-0.1.8/airtestProject/commons/utils/gotCommon.py
+-rw-rw-rw-   0        0        0     5714 2024-05-17 09:08:55.000000 airtestproject-0.1.8/airtestProject/commons/utils/logger.py
+-rw-rw-rw-   0        0        0     2765 2024-05-16 10:33:08.000000 airtestproject-0.1.8/airtestProject/commons/utils/myTemplate.py
+-rw-rw-rw-   0        0        0     8802 2024-05-17 08:53:36.000000 airtestproject-0.1.8/airtestProject/commons/utils/ocrTemplate.py
+-rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/utils/page.py
+-rw-rw-rw-   0        0        0     8367 2024-05-17 09:15:06.000000 airtestproject-0.1.8/airtestProject/commons/utils/reportUtil.py
+-rw-rw-rw-   0        0        0       81 2024-05-16 13:38:53.000000 airtestproject-0.1.8/airtestProject/commons/utils/setting.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:10:27.000000 airtestproject-0.1.8/airtestProject/commons/utils/test.py
+-rw-rw-rw-   0        0        0     2790 2024-05-17 08:34:24.000000 airtestproject-0.1.8/airtestProject/commons/utils/tools.py
+-rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/commons/utils/utils.py
+-rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.8/airtestProject/config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.758599 airtestproject-0.1.8/airtestProject/factory/
+-rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.8/airtestProject/factory/SingletonFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/factory/__init__.py
+-rw-rw-rw-   0        0        0     2059 2024-05-17 08:06:45.000000 airtestproject-0.1.8/airtestProject/factory/operateFactory.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.772662 airtestproject-0.1.8/airtestProject/manager/
+-rw-rw-rw-   0        0        0     9352 2024-05-14 03:10:27.000000 airtestproject-0.1.8/airtestProject/manager/DeviceManager.py
+-rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.8/airtestProject/manager/LogManager.py
+-rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/manager/PackageManager.py
+-rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/manager/ReportManager.py
+-rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/manager/TaskManager.py
+-rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.8/airtestProject/manager/TestCaseManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.8/airtestProject/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.775655 airtestproject-0.1.8/airtestProject/scripts/
+-rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.8/airtestProject/scripts/OdinExample.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.8/airtestProject/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:57:23.777650 airtestproject-0.1.8/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      786 2024-05-17 10:57:23.000000 airtestproject-0.1.8/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2024-05-17 10:57:23.000000 airtestproject-0.1.8/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:57:23.000000 airtestproject-0.1.8/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-05-17 10:57:23.000000 airtestproject-0.1.8/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 10:57:23.000000 airtestproject-0.1.8/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:57:23.780642 airtestproject-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      848 2024-05-17 09:07:06.000000 airtestproject-0.1.8/setup.py
```

### Comparing `airtestproject-0.1.7/LICENSE` & `airtestproject-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/PKG-INFO` & `airtestproject-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.7
+Version: 0.1.8
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.7/airtestProject/abstractBase/OperateBase.py` & `airtestproject-0.1.8/airtestProject/abstractBase/OperateBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 #!-*- coding = utf-8 -*-
 # @Time : 2024/4/7 2:44
 # @Author : 苏嘉浩
 # @File : OperateBase.py
 # @Software : PyCharm
 from abc import ABC, abstractmethod
 
+"""
+airtest核心api的二次封装，操作具体基类
+"""
+
 
 class OperateABC(ABC):
 
     @abstractmethod
     def click(self, value, *args, **kwargs):
+        """
+        :param value:
+        :param args:
+        :param kwargs: ocrPlus=True,可以开启二值化
+        :return:
+        """
         pass
 
     @abstractmethod
     def exists(self, pos, **kwargs):
         pass
 
     @abstractmethod
@@ -25,15 +35,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def pinch(self, in_or_out, pos=None, *args, **kwargs):
         pass
 
     @abstractmethod
-    def set_text(self, pos, text,  *args, **kwargs):
+    def set_text(self, pos, text, *args, **kwargs):
         pass
 
     @abstractmethod
     def wait(self, pos, timeout=None, *args, **kwargs):
         pass
 
     @abstractmethod
@@ -70,11 +80,10 @@
     def wait_next_element(self, last_click_pos, next_pos):
         pass
 
     @abstractmethod
     def get_text(self, pos, *args, **kwargs):
         pass
 
-
 # class OperateClass:
 #     def __init__(self, operate: OperateABC):
 #         self.operate = operate
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/UWA.py` & `airtestproject-0.1.8/airtestProject/commons/UWA.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/page/odin/login.py` & `airtestproject-0.1.8/airtestProject/commons/page/odin/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         operate(fun_name).wait_for_any([create_role_page, select_role_page])
         bool = operate(fun_name).exists(create_role_page)
         log.step(f'是否未创角-{bool}')
         # random_name = factory.random_word()
         if bool:
             operate(fun_name).click(role, focus=reset_pos)
-            operate(fun_name).click(gender, focus=reset_pos)
+            operate(fun_name).click(gender, focus=reset_pos, ocrPlus=True)
             operate(fun_name).set_text(input_name_pos, r_user_name())
             operate(fun_name).sleep(1.0)
             log.step(f'创建角色-test')
             for i in range(3):
                 if operate(fun_name).exists(next_page_pos) is False:
                     operate(fun_name).click(create_pos)
                     log.step('点击进入游戏')
@@ -217,23 +217,23 @@
         self.create_role(create_role_page, select_role_page, create_role_page, all_role_pos['tangsan']
                          , gender_pos['male'], input_name_pos, enter_pos, enter_pos, tip_pos, "poco")
         # self.check_login_success()
         if self.check_enter_success(tip_pos, "poco"):
             return True
 
     def odin_login_air(self):
-        self.check_enter_login_view("登陆按钮")
-        self.input_account("账号输入框")
-        self.click_login("登陆按钮", "点击换区按钮")
-        self.open_server_list("点击换区按钮")
-        self.select_server("Odin外网公共服按钮")
-        self.click_enter_game("进入游戏")
-        self.create_role("创建角色", "进入游戏（选择角色）", "马红俊", "女",
-                               "姓名输入框", "进入游戏（选择角色）", "创建角色", "等待条")
-        if self.check_enter_success("等待条"):
+        self.check_enter_login_view("LoginBtn")
+        self.input_account("AccountInputBox")
+        self.click_login("LoginBtn", "ZoneChangeButton")
+        self.open_server_list("ZoneChangeButton")
+        self.select_server("Odin外网共公服")
+        self.click_enter_game("EnterGame")
+        self.create_role("CreateRole", "EnterGame (SelectCharacter)", "马红俊", "女",
+                               "NameTxt", "EnterGame (SelectCharacter)", "CreateRole", "WaitingBar")
+        if self.check_enter_success("WaitingBar"):
             return True
 
 
 if __name__ == '__main__':
     # poco("inputFieldAccountName").set_text("fdshj")
     connect_device("Android:///e7970f92")
     # odin_login_air()
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/page/odin/run.py` & `airtestproject-0.1.8/airtestProject/commons/page/odin/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,28 @@
 exit_pos = "btnExit"
 
 axis_pos = "txtDes"
 index = re.compile(r'\b(\d+)\.\d+')
 running_pos_end_1 = ["884", "29", "699"]
 
 
-class MainPage:
+class RunPage:
 
-    def __init__(self, project=None):
+    def __init__(self, adb, script_root, Project=None, log_path=None):
         """
 
         :param project: 如果想采用命名代替文件夹路径的方法需要传入一个文件夹名让air生成对应字典。
         """
-        if project is not None:
-            operate("air").set_dict(project)
+        self.adb = adb
+        if Project is not None:
+            operate("air").set_dict(script_root, Project)
+        if log_path is not None:
+            self.log_path = log_path
+        else:
+            self.log_path = None
 
     @log.wrap('点击场景按钮成功')
     def click_scene(self, scenes_pos, scenes_view_pos, fun_name="air"):
         start_time = time.time()
         while operate(fun_name).exists(scenes_view_pos) is False:
             operate(fun_name).click(scenes_pos)
             log.step('点击场景按钮')
@@ -147,25 +152,27 @@
     def start_running_2(self):
         self.start_run()
         self.close_running_view()
         self.check_running_end()
 
 
 def run_test_poco():
-    run_main = MainPage()
+    run_main = RunPage(None, __file__, "odin")
     run_main.click_scene(scenes_pos, scenes_view_pos, fun_name="poco")
     run_main.click_streaming_scenes(streaming_scenes_pos, fun_name="poco")
     run_main.close_scene_view(scenes_view_pos, scenes_pos, fun_name="poco")
     run_main.click_fun()
 
+
 def run_test():
-    run_main = MainPage("odin")
-    run_main.click_scene("场景", "场景跳转")
+    run_main = RunPage(None, __file__, "odin")
+    run_main.click_scene("Scene", "场景跳转")
     run_main.click_streaming_scenes("斗罗场景（流式加载）")
-    run_main.close_scene_view("场景跳转", "场景")
-    run_main.click_fun("功能","功能列表")
-    run_main.swipe_fun_view_last("自动跑图", "功能列表滑动点 (2)")
-    run_main.click_running("自动跑图")
+    run_main.close_scene_view("场景跳转", "Scene")
+    run_main.click_fun("Func", "功能列表")
+    run_main.swipe_fun_view_last("AutoMapRunning", "功能列表滑动点 (2)")
+    run_main.click_running("AutoMapRunning")
+
 
 if __name__ == '__main__':
     connect_device("Android:///e7970f92")
     run_test()
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/process/odin/profile.py` & `airtestproject-0.1.8/airtestProject/commons/process/odin/profile.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/air.py` & `airtestproject-0.1.8/airtestProject/commons/utils/air.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/appStart.py` & `airtestproject-0.1.8/airtestProject/commons/utils/appStart.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/command.py` & `airtestproject-0.1.8/airtestProject/commons/utils/command.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/deploy.py` & `airtestproject-0.1.8/airtestProject/commons/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/excel_image.py` & `airtestproject-0.1.8/airtestProject/commons/utils/excelPicture.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/exception.py` & `airtestproject-0.1.8/airtestProject/commons/utils/exception.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/factory.py` & `airtestproject-0.1.8/airtestProject/commons/utils/factory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/ganaratePyCase.py` & `airtestproject-0.1.8/airtestProject/commons/utils/ganaratePyCase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/genaratePy.py` & `airtestproject-0.1.8/airtestProject/commons/utils/genaratePy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 根据Excel表格生成python测试用例
 """
 import os
 import openpyxl
 
 from airtestProject import config
-from airtestProject.commons.utils.excel_image import get_id_name
+from airtestProject.commons.utils.excelPicture import get_id_name
 from utils import *
 
 
 # Utils = Utils()
 
 
 def get_execls(project):
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/gotCommon.py` & `airtestproject-0.1.8/airtestProject/commons/utils/gotCommon.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/logger.py` & `airtestproject-0.1.8/airtestProject/commons/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import functools
 import time
 import sys
 import os
 
 import logging
 
+from airtestProject.commons.utils.tools import log_error_plus
+
 # 设置airtest日志等级，debug会输出很多日志
 air_logger = logging.getLogger("airtest")
 air_logger.setLevel(logging.ERROR)
 
 
 class Logger:
 
@@ -99,16 +101,16 @@
             def inner(*args, **kwargs):
                 start_time = time.time()
                 try:
                     res = func(*args, **kwargs)
                     end_time = time.time()
                     duration = round(end_time - start_time, 2)
                     self.step(f"{msg} - func: {func.__name__} - duration: {duration} s")
-                    if self.adb_log is not None:
-                        air.log(self.adb_log,
+                    if self.adb_log is not None and "Unity" in self.adb_log:
+                        log_error_plus(self.adb_log,
                                 desc=f":😈 😈 {msg} - func: {func.__name__}",
                                 snapshot=True)
                     else:
                         air.log(f"{' '.join(self.random_emoji() * 2)}: {msg} - func: {func.__name__}", snapshot=True)
                     self.adb_log = None
                     return res
                 except Exception as e:
@@ -155,15 +157,14 @@
             end_time = time.time()
             duration = round(end_time - start_time, 2)
             self.step(f"End running testcase : {func.__name__} [ Case duration: {duration} s ]")
             self.step(f"{'- ' * 16} 分割线 {' -' * 16}")
             return res
         return inner
 
-
 log = Logger()
 
 
 if __name__ == '__main__':
     log.info('aaaa')
     log.error('aaaa')
     log.warn('aaaa')
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/myAirtest.py` & `airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/airtestOperate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-airtest核心api的二次封装
+airtest核心api的二次封装，操作具体实现类
 """
 import os
 
 from airtest.core import api as air
-from airtest.core.cv import Template
 from airtest.core.error import TargetNotFoundError
 
 from airtestProject.commons.utils.logger import log
 from airtestProject.abstractBase.OperateBase import OperateABC
 import time
 
+from airtestProject.commons.utils.myTemplate import myTemplate
 from airtestProject.commons.utils.ocrTemplate import OcrTemplate
 from airtestProject.commons.utils.tools import get_folder_path_up
 
 
-class AirTest(OperateABC):
+class myAirTest(OperateABC):
 
     def __init__(self, language):
-        super(AirTest, self).__init__()
+        super(myAirTest, self).__init__()
         self.this_dict = None
         self.language = language
 
     def set_dict(self, script_root: str, project: str):
         """
         各种兼容还有路径转换。ps images文件夹只能在脚本的上级或者同级否则无法正常工作
         :param script_root: 脚本当前目录
@@ -36,15 +36,15 @@
             # images_relative_path = os.path.relpath(images_abs_path, script_root_dir)  # 构造为图片文件夹的相对路径
             images_project_relative_path = os.path.join(images_abs_path, project)  # 构造为图片文件夹和project的相对路径
             # 遍历指定目录下的所有文件
             for filename in os.listdir(images_project_relative_path):
                 file_path = os.path.join(images_project_relative_path, filename)
                 if os.path.isfile(file_path):
                     file_name_without_ext, _ = os.path.splitext(filename)
-                    files_dict[file_name_without_ext] = Template(file_path)
+                    files_dict[file_name_without_ext] = myTemplate(file_path)
             print(files_dict)
             self.this_dict = files_dict
 
     def init_device(self, platform=None, uuid=None, **kwargs):
         try:
             air.init_device(platform=platform, uuid=uuid, **kwargs)
             log.info(f"init device success, platform: {platform}, uuid:  {uuid}")
@@ -176,15 +176,15 @@
         log.info(f"perform key event keyname: {keyname} on the device.")
         return air.keyevent(keyname, **kwargs)
 
     def set_text(self, pos=None, text=None, enter=True, **kwargs):
         try:
             self.click(pos)
             log.info(f"input {text} on the target device")
-            for i in range(30):
+            for i in range(20):
                 air.keyevent("KEYCODE_DEL")
                 log.info(f"我在删除")
             return air.text(text, enter, **kwargs)
         except Exception as e:
             log.error(f"failed to input {text} on the target device")
             raise e
 
@@ -200,24 +200,24 @@
         except Exception as e:
             log.error(f"failed to input {pos} on the target device")
             raise e
 
     def wait_disappear_element(self, pos, *args, **kwargs):
         start_loading_time = time.time()
         while self.exists(pos) is not False:
-            if time.time() - start_loading_time > 300:
+            if time.time() - start_loading_time > 180:
                 log.info(f"{pos}存在超时，请注意查看")
                 return False
         log.info(f"{pos}消失")
         return True
 
     def wait_element_appear(self, pos, *args, **kwargs):
         start_loading_time = time.time()
         while self.exists(pos) is False:
-            if time.time() - start_loading_time > 300:
+            if time.time() - start_loading_time > 180:
                 log.info(f"{pos}寻找超时，请注意查看")
                 return False
         log.info(f"{pos}出现")
         return True
 
     def exists(self, pos, ocrPlus=None, **kwargs):
         try:
@@ -269,15 +269,15 @@
         :return:
         """
         start_time = time.time()
         while self.exists(next_pos) is False:
             log.info(f"{next_pos}没有出现正在尝试点击")
             self.click(last_click_pos)
             air.sleep(0.5)
-            if time.time() - start_time > 300:
+            if time.time() - start_time > 180:
                 log.info(f"{next_pos}没有出现")
                 return False
         return True
 
     def get_text(self, pos, *args, **kwargs):
 
         pass
@@ -292,13 +292,13 @@
         if isinstance(val, str):
             dict_value = None
             if self.this_dict:
                 dict_value = self.this_dict.get(val)
             if dict_value is not None:
                 return dict_value
             log.info(f"字典中不存在{val}对应的路径")
-            return Template(val) if os.path.isfile(val) else OcrTemplate(val, self.language, ocrPlus=ocrPlus)
+            return myTemplate(val) if os.path.isfile(val) else OcrTemplate(val, language=self.language, ocrPlus=ocrPlus)
         return val
 
 
 if __name__ == '__main__':
     air.sleep()
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/myPoco.py` & `airtestproject-0.1.8/airtestProject/abstractBase/operateBaseImp/pocoOperate.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import re
 import time
 
 identifier: str = '-'
 index_compile = re.compile(r'(?<=\[)\d+?(?=\])')
 
 
-class Poco(OperateABC):
+class myPoco(OperateABC):
 
     def __init__(self, poco_instance):
 
         self.poco = poco_instance or UnityPoco()
 
     def get_poco(self, pos):
         return self.parser_pos(pos)
@@ -62,15 +62,15 @@
 
     def scroll(self, pos: str, direction='vertical', percent: float = 0.6, duration: float = 2.0):
         return self.parser_pos(pos).scroll(direction, percent, duration)
 
     def pinch(self, in_or_out='in', pos=None, percent: float = 0.6, duration: float = 2.0, dead_zone: float = 0.1):
         return self.parser_pos(pos).pinch(in_or_out, percent, duration, dead_zone)
 
-    def set_text(self, pos=None, text=None,  **kwargs):
+    def set_text(self, pos=None, text=None, **kwargs):
         return self.parser_pos(pos).set_text(text)
 
     def get_text(self, pos, *args, **kwargs):
         return self.parser_pos(pos).get_text()
 
     def get_name(self, pos: str):
         return self.parser_pos(pos).get_name()
@@ -85,24 +85,24 @@
 
         if wait_type == 'disappearance':
             return self.parser_pos(pos).wait_for_appearance(timeout)
 
     def wait_disappear_element(self, pos, *args, **kwargs):
         start_loading_time = time.time()
         while self.parser_pos(pos).exists() is not False:
-            if time.time() - start_loading_time > 300:
+            if time.time() - start_loading_time > 180:
                 log.info(f"{pos}寻找超时，请注意查看")
                 return False
         log.info(f"{pos}消失")
         return True
 
     def wait_element_appear(self, pos, *args, **kwargs):
         start_loading_time = time.time()
         while self.parser_pos(pos).exists() is False:
-            if time.time() - start_loading_time > 300:
+            if time.time() - start_loading_time > 180:
                 log.info(f"{pos}寻找超时，请注意查看")
                 return False
         log.info(f"{pos}出现")
         return True
 
     def persistent_element_exists(self, pos):
         pass
@@ -123,15 +123,15 @@
         log.step(f"sleep {secs} seconds .")
         time.sleep(secs)
 
     def wait_next_element(self, last_click_pos, next_pos):
         start_time = time.time()
         while self.exists(next_pos) is False:
             self.click(last_click_pos)
-            if time.time() - start_time > 300:
+            if time.time() - start_time > 180:
                 log.info(f"{next_pos}无法进入")
 
     def regex_pos_index(self, pos: str):
         """
         正则匹配定位的下标
         :param pos:
         :return:
@@ -175,16 +175,14 @@
         pos_list = [self.regex_pos_index(value) for value in value_list]
 
         p0, n0 = pos_list[0]
         p1, n1 = pos_list[1]
 
         return self.poco(p0)[n0].child(p1)[n1]
 
-
     def parser_pos_list(self, pos_list: list):
         poco_list = []
 
         for pos in pos_list:
             poco_list.append(self.poco(pos))
 
         return poco_list
-
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/ocrTemplate.py` & `airtestproject-0.1.8/airtestProject/commons/utils/ocrTemplate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!-*- coding = utf-8 -*-
 # @Time : 2024/4/28 8:08
 # @Author : 苏嘉浩
 # @File : ocrTemplate.py
 # @Software : PyCharm
+import threading
+
 import cv2
 import easyocr
 import numpy as np
 
 import torch
 from airtest import aircv
-from PIL import Image
 from airtest.core.cv import Template
 from airtest.core.error import InvalidMatchingMethodError
 from airtest.utils.transform import TargetPos
 from airtest.core.helper import G, logwrap
 from airtest.core.settings import Settings as ST  # noqa
-from airtest.aircv.keypoint_matching import ORBMatching
 from paddleocr import PaddleOCR
+from airtestProject.commons.utils.setting import Setting as SS
 import os
 
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 
 class EasyOcr:
     def __init__(self, language=None):
         """
         :param language: 语言默认为中文和英文。可能会比较慢，后续可以建议为单引擎
         """
         if language is None:
             self.easy_language = ['en', 'ch_sim']
         else:
-            self.easy_language = language.copy()
+            self.easy_language = list(language)
             index = self.easy_language.index('ch')  # 找到 'ch' 的位置,easyocr的中文是分繁体简体
             self.easy_language[index] = 'ch_sim'
         self.reader = easyocr.Reader(self.easy_language, gpu=True)
 
     def ocr_match(self, img, input_text):
         # 读取图像
 
@@ -70,16 +71,16 @@
     """
 
     def __init__(self, language=None):
 
         if language is None:
             self.ppOcr_languages = ['ch']
         else:
-            self.ppOcr_languages = language
-        self.ocr_modules = [PaddleOCR(use_angle_cls=True, lang=lang) for lang in self.ppOcr_languages]
+            self.ppOcr_languages = list(language)
+        self.ocr_modules = [PaddleOCR(use_angle_cls=True, use_gpu=True, lang=lang) for lang in self.ppOcr_languages]
 
     def ocr_match(self, img, input_text):
         pp_results = {}
         for ocr_model in self.ocr_modules:
             result = ocr_model.ocr(img, cls=True)
             for re in result:
                 for line in re:
@@ -106,34 +107,47 @@
             result_list.append(result_dict)
         print(result_list)
         coordinate = next((r_dict for r_dict in result_list if r_dict.get('text').lower() == input_text.lower()), None)
         return coordinate
 
 
 METHOD_LIST = ['easy', 'padd']
-METHOD_DICT = {
-    'easy': EasyOcr,
-    'padd': PpOcr
-}
 
 
 class OcrTemplate(Template):
     """
     ocr模版
         :param filename: 传入的文字
         :param ocrPlus: 是否启用二值化和高斯模糊
         :param
     """
 
+    ocr_instances = {
+        "default": {
+            'easy': EasyOcr(),
+            'padd': PpOcr()
+        }
+    }
+    lock = threading.Lock()
+
     def __init__(self, filename, threshold=None, target_pos=TargetPos.MID, record_pos=None, resolution=(), rgb=False,
                  scale_max=800, scale_step=0.005, ocrPlus=False, language=None):
 
         super().__init__(filename, threshold, target_pos, record_pos, resolution, rgb, scale_max, scale_step)
         self.ocrPlus = ocrPlus
-        self.language = language
+        if language is not None:
+            self.language = tuple(language)
+            with OcrTemplate.lock:
+                if self.language not in OcrTemplate.ocr_instances:
+                    OcrTemplate.ocr_instances[self.language] = {
+                        'easy': EasyOcr(language=self.language),
+                        'padd': PpOcr(language=self.language)
+                    }
+        else:
+            self.language = language
 
     @property
     def filepath(self):
         return self.filename
 
     def match_in(self, screen):
         match_result = self._cv_match(screen)
@@ -175,30 +189,33 @@
             clahe_img = cv2.GaussianBlur(binary_img, (5, 5), 0)
             #
             # cv2.imshow("Image3", binary_img)
             # cv2.waitKey(0)
 
         for method in METHOD_LIST:
             # get function definition and execute:
-            func = METHOD_DICT[method]
+            if self.language is not None:
+                func = OcrTemplate.ocr_instances[self.language][method]
+            else:
+                func = OcrTemplate.ocr_instances["default"][method]
             if func is None:
                 raise InvalidMatchingMethodError(
                     "Undefined method in OCR_METHOD: '%s'" % method)
             else:
                 ret = self._try_match(func, language=self.language, img=clahe_img, input_text=self.filename)
             # 先用easyOCR方法失败则会用下一个
             if ret:
                 break
         return ret
 
     @staticmethod
     def _try_match(func, *args, **kwargs):
-        G.LOGGING.debug("try match with %s" % func.__name__)
+        G.LOGGING.debug("try match with %s" % func)
         try:
-            instance = func(language=kwargs['language'])
+            instance = func
             ret = instance.ocr_match(img=kwargs['img'], input_text=kwargs['input_text'])
         except aircv.NoModuleError as err:
             G.LOGGING.warning(
                 "'Easy/ppd' initialization failed. Alternatively, reinstall easycr or PaddleOCR.")
             return None
         except aircv.BaseError as err:
             G.LOGGING.debug(repr(err))
```

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/page.py` & `airtestproject-0.1.8/airtestProject/commons/utils/page.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/commons/utils/utils.py` & `airtestproject-0.1.8/airtestProject/commons/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/factory/operateFactory.py` & `airtestproject-0.1.8/airtestProject/factory/operateFactory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import threading
 from abc import ABC, abstractmethod
 
 from airtestProject.abstractBase.OperateBase import OperateABC
-from airtestProject.commons.utils.myAirtest import AirTest
-from airtestProject.commons.utils.myPoco import Poco
+from airtestProject.abstractBase.operateBaseImp.airtestOperate import myAirTest
+from airtestProject.abstractBase.operateBaseImp.pocoOperate import myPoco
 from poco.drivers.unity3d import UnityPoco
 from airtestProject.factory.SingletonFactory import SingletonFactory
 
 
 class AbstractFactory(ABC):
     def __init__(self):
         self._local = threading.local()
@@ -23,33 +23,34 @@
         super().__init__()
         self._UnityPoco = None
 
     def create_operate_abc(self, **kwargs) -> OperateABC:
         if self._UnityPoco is None:
             self._UnityPoco = UnityPoco()
         if not hasattr(self._local, '_PageInstance'):
-            self._local._PocoInstance = Poco(self._UnityPoco)
+            self._local._PocoInstance = myPoco(self._UnityPoco)
         return self._local._PocoInstance
 
 
+# 具体工厂
 class AirTestFactory(AbstractFactory, metaclass=SingletonFactory):
     def __init__(self):
         super().__init__()
 
     def create_operate_abc(self, language=None, **kwargs) -> OperateABC:
         if not hasattr(self._local, '_AirTestInstance'):
-            self._local._AirTestInstance = AirTest(language)
+            self._local._AirTestInstance = myAirTest(language)
         return self._local._AirTestInstance
 
 
 def operate(factory_name: str, **kwargs) -> OperateABC:
     """
 
     :param factory_name: 工厂名称，可以是poco或air。
-    :param kwargs: 可选参数。如果factory_name是air，可以传入lang参数。
+    :param kwargs: 可选参数。如果factory_name是air，可以传入language参数。设置语言需要在最开始设置，否者按照默认运行
     :return: 返回具体的工厂实例。
     """
     factories = {
         'poco': PocoFactory,
         'air': AirTestFactory
     }
     factory_class = factories[factory_name]
```

### Comparing `airtestproject-0.1.7/airtestProject/manager/DeviceManager.py` & `airtestproject-0.1.8/airtestProject/manager/DeviceManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/manager/LogManager.py` & `airtestproject-0.1.8/airtestProject/manager/LogManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/manager/PackageManager.py` & `airtestproject-0.1.8/airtestProject/manager/PackageManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/manager/ReportManager.py` & `airtestproject-0.1.8/airtestProject/manager/ReportManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/manager/TaskManager.py` & `airtestproject-0.1.8/airtestProject/manager/TaskManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/manager/TestCaseManager.py` & `airtestproject-0.1.8/airtestProject/manager/TestCaseManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject/scripts/OdinExample.py` & `airtestproject-0.1.8/airtestProject/scripts/OdinExample.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.7/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.8/airtestProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.7
+Version: 0.1.8
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.7/airtestProject.egg-info/SOURCES.txt` & `airtestproject-0.1.8/airtestProject.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 airtestProject.egg-info/PKG-INFO
 airtestProject.egg-info/SOURCES.txt
 airtestProject.egg-info/dependency_links.txt
 airtestProject.egg-info/requires.txt
 airtestProject.egg-info/top_level.txt
 airtestProject/abstractBase/OperateBase.py
 airtestProject/abstractBase/__init__.py
-airtestProject/abstractBase/loginBase.py
+airtestProject/abstractBase/aiBase.py
+airtestProject/abstractBase/aiBaseImp/__init__.py
+airtestProject/abstractBase/aiBaseImp/aiBaseImp.py
+airtestProject/abstractBase/operateBaseImp/__init__.py
+airtestProject/abstractBase/operateBaseImp/airtestOperate.py
+airtestProject/abstractBase/operateBaseImp/pocoOperate.py
 airtestProject/commons/UWA.py
 airtestProject/commons/__init__.py
 airtestProject/commons/Position/__init__.py
 airtestProject/commons/Position/odin/__init__.py
 airtestProject/commons/Position/odin/odinPos.py
 airtestProject/commons/page/__init__.py
 airtestProject/commons/page/odin/__init__.py
@@ -25,26 +30,26 @@
 airtestProject/commons/process/odin/__init__.py
 airtestProject/commons/process/odin/profile.py
 airtestProject/commons/utils/__init__.py
 airtestProject/commons/utils/air.py
 airtestProject/commons/utils/appStart.py
 airtestProject/commons/utils/command.py
 airtestProject/commons/utils/deploy.py
-airtestProject/commons/utils/excel_image.py
+airtestProject/commons/utils/excelPicture.py
 airtestProject/commons/utils/exception.py
 airtestProject/commons/utils/factory.py
 airtestProject/commons/utils/ganaratePyCase.py
 airtestProject/commons/utils/genaratePy.py
 airtestProject/commons/utils/gotCommon.py
 airtestProject/commons/utils/logger.py
-airtestProject/commons/utils/myAirtest.py
-airtestProject/commons/utils/myPoco.py
+airtestProject/commons/utils/myTemplate.py
 airtestProject/commons/utils/ocrTemplate.py
 airtestProject/commons/utils/page.py
 airtestProject/commons/utils/reportUtil.py
+airtestProject/commons/utils/setting.py
 airtestProject/commons/utils/test.py
 airtestProject/commons/utils/tools.py
 airtestProject/commons/utils/utils.py
 airtestProject/factory/SingletonFactory.py
 airtestProject/factory/__init__.py
 airtestProject/factory/operateFactory.py
 airtestProject/manager/DeviceManager.py
```

### Comparing `airtestproject-0.1.7/setup.py` & `airtestproject-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
```

