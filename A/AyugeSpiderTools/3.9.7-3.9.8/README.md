# Comparing `tmp/ayugespidertools-3.9.7.tar.gz` & `tmp/ayugespidertools-3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.9.7.tar", max compression
+gzip compressed data, was "ayugespidertools-3.9.8.tar", max compression
```

## Comparing `ayugespidertools-3.9.7.tar` & `ayugespidertools-3.9.8.tar`

### file list

```diff
@@ -1,97 +1,92 @@
--rw-r--r--   0        0        0     1070 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/LICENSE
--rw-r--r--   0        0        0    10848 2024-03-06 01:41:28.000000 ayugespidertools-3.9.7/README.md
--rw-r--r--   0        0        0      478 2024-03-08 08:03:23.000000 ayugespidertools-3.9.7/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0       79 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      330 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3770 2024-02-23 06:48:44.000000 ayugespidertools-3.9.7/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      270 2023-11-19 14:29:37.000000 ayugespidertools-3.9.7/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-11-23 03:31:26.000000 ayugespidertools-3.9.7/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-23 06:48:44.000000 ayugespidertools-3.9.7/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0    10702 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6085 2024-03-05 01:57:08.000000 ayugespidertools-3.9.7/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    20088 2024-03-02 13:47:09.000000 ayugespidertools-3.9.7/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    10544 2024-02-23 06:48:44.000000 ayugespidertools-3.9.7/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    30778 2024-01-22 01:27:26.000000 ayugespidertools-3.9.7/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4654 2024-02-23 06:48:44.000000 ayugespidertools-3.9.7/ayugespidertools/common/postgreserrhandle.py
--rw-r--r--   0        0        0    13542 2024-02-23 06:48:45.000000 ayugespidertools-3.9.7/ayugespidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3607 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     5484 2024-03-08 03:32:02.000000 ayugespidertools-3.9.7/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    12180 2024-02-23 06:48:44.000000 ayugespidertools-3.9.7/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0      358 2023-10-29 15:43:02.000000 ayugespidertools-3.9.7/ayugespidertools/config.py
--rw-r--r--   0        0        0       68 2023-11-22 01:54:38.000000 ayugespidertools-3.9.7/ayugespidertools/extras/__init__.py
--rw-r--r--   0        0        0    16622 2024-02-23 06:48:45.000000 ayugespidertools-3.9.7/ayugespidertools/extras/cvnpil.py
--rw-r--r--   0        0        0     1937 2023-12-15 13:44:40.000000 ayugespidertools-3.9.7/ayugespidertools/extras/ext.py
--rw-r--r--   0        0        0     2646 2024-03-04 01:51:05.000000 ayugespidertools-3.9.7/ayugespidertools/extras/oss.py
--rw-r--r--   0        0        0     7230 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     5553 2024-03-08 01:18:26.000000 ayugespidertools-3.9.7/ayugespidertools/items.py
--rw-r--r--   0        0        0      653 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     4034 2024-01-17 03:23:40.000000 ayugespidertools-3.9.7/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1114 2024-03-08 05:55:18.000000 ayugespidertools-3.9.7/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     2187 2024-01-29 01:15:54.000000 ayugespidertools-3.9.7/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0      202 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/request.py
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      202 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1510 2024-03-04 01:42:14.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1415 2024-03-08 03:00:54.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      797 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/headers/__init__.py
--rw-r--r--   0        0        0     2000 2024-03-08 01:18:26.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      154 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10197 2024-03-05 06:24:15.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      395 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4069 2024-03-08 01:18:26.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2712 2024-03-08 01:18:26.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0     2345 2024-01-29 09:45:22.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/download/__init__.py
--rw-r--r--   0        0        0     2275 2024-03-05 06:24:15.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0     2368 2024-03-08 02:59:24.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/es/__init__.py
--rw-r--r--   0        0        0     3137 2024-03-08 05:49:25.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/es/asynced.py
--rw-r--r--   0        0        0      147 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/es/fantasy.py
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1768 2024-03-08 03:22:52.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     1633 2024-03-08 03:17:35.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0      919 2024-03-08 03:27:04.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3296 2024-03-08 03:32:37.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     2225 2024-03-08 03:34:00.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0     2781 2024-03-08 02:57:46.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-08 05:59:55.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      162 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     7212 2024-03-08 06:03:18.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2570 2024-03-08 06:18:52.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3211 2024-03-08 05:37:55.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     1543 2024-03-08 05:42:26.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oracle/__init__.py
--rw-r--r--   0        0        0      167 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oracle/fantasy.py
--rw-r--r--   0        0        0     2341 2024-03-08 05:43:39.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oracle/twisted.py
--rw-r--r--   0        0        0        0 2024-01-29 01:15:54.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oss/__init__.py
--rw-r--r--   0        0        0     3531 2024-03-05 06:24:15.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oss/ali.py
--rw-r--r--   0        0        0     2284 2024-03-08 05:46:56.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/__init__.py
--rw-r--r--   0        0        0     2223 2024-03-08 05:51:09.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/asynced.py
--rw-r--r--   0        0        0      177 2024-02-23 08:38:58.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/fantasy.py
--rw-r--r--   0        0        0     2989 2024-03-08 05:52:10.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/twisted.py
--rw-r--r--   0        0        0     6739 2024-03-05 06:24:15.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      336 2024-02-23 07:24:49.000000 ayugespidertools-3.9.7/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      175 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       37 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0     5634 2024-03-08 07:34:20.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      270 2023-10-30 01:40:52.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3663 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      368 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       83 2023-11-07 15:08:20.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      160 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1113 2024-02-16 08:41:51.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      161 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       62 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      273 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1394 2023-12-28 08:04:40.000000 ayugespidertools-3.9.7/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     4027 2024-02-06 07:45:24.000000 ayugespidertools-3.9.7/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1267 2023-12-21 01:11:24.000000 ayugespidertools-3.9.7/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      545 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      543 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-10-13 17:11:34.000000 ayugespidertools-3.9.7/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5850 2024-02-23 06:48:45.000000 ayugespidertools-3.9.7/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     4727 2024-03-08 08:03:31.000000 ayugespidertools-3.9.7/pyproject.toml
--rw-r--r--   0        0        0    13261 1970-01-01 00:00:00.000000 ayugespidertools-3.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/LICENSE
+-rw-r--r--   0        0        0    10706 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/README.md
+-rw-r--r--   0        0        0      462 2024-05-17 14:38:19.000000 ayugespidertools-3.9.8/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0       75 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      330 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0      869 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      357 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     2326 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0    10135 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5973 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    18874 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    10210 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    30172 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4654 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/postgreserrhandle.py
+-rw-r--r--   0        0        0    13151 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3079 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     5300 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11427 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0      315 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/config.py
+-rw-r--r--   0        0        0       68 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/extras/__init__.py
+-rw-r--r--   0        0        0    15954 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/extras/cvnpil.py
+-rw-r--r--   0        0        0     1937 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/extras/ext.py
+-rw-r--r--   0        0        0     2559 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/extras/oss.py
+-rw-r--r--   0        0        0     6980 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     5369 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/items.py
+-rw-r--r--   0        0        0      653 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     4054 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1114 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     2144 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      202 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1451 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      797 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/headers/__init__.py
+-rw-r--r--   0        0        0     1836 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      154 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0     9945 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      395 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3821 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2737 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     2298 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2217 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0     2312 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/es/__init__.py
+-rw-r--r--   0        0        0     3024 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/es/asynced.py
+-rw-r--r--   0        0        0      141 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/es/fantasy.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1719 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     1584 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0      899 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3200 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     2163 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0     2704 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      156 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     7041 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2000 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3121 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     1472 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oracle/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oracle/fantasy.py
+-rw-r--r--   0        0        0     2394 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oracle/twisted.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oss/__init__.py
+-rw-r--r--   0        0        0     3353 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oss/ali.py
+-rw-r--r--   0        0        0     2219 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/asynced.py
+-rw-r--r--   0        0        0      171 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/fantasy.py
+-rw-r--r--   0        0        0     3025 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/twisted.py
+-rw-r--r--   0        0        0     6494 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      175 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     6713 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3663 2024-05-17 09:53:03.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      368 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0     1030 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      161 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-07 06:38:24.000000 ayugespidertools-3.9.8/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0      935 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     2870 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0      851 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      526 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      524 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2024-05-07 06:38:23.000000 ayugespidertools-3.9.8/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     6876 2024-05-17 11:47:05.000000 ayugespidertools-3.9.8/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     4541 2024-05-17 14:38:19.000000 ayugespidertools-3.9.8/pyproject.toml
+-rw-r--r--   0        0        0    13291 1970-01-01 00:00:00.000000 ayugespidertools-3.9.8/PKG-INFO
```

### Comparing `ayugespidertools-3.9.7/LICENSE` & `ayugespidertools-3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/README.md` & `ayugespidertools-3.9.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,221 @@
-<p align="center">
-    <a href="https://ayugespidertools.readthedocs.io" target="_blank" rel="noopener noreferrer">
-        <img src="./artwork/ayugespidertools-logo.png" alt="ayugespidertools-logo">
-    </a>
-</p>
-<hr/>
-
-# AyugeSpiderTools 介绍
-
-![GitHub](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
-![python](https://img.shields.io/badge/python-3.8%2B-blue)
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/codeql.yml?branch=main)
-![Read the Docs](https://img.shields.io/readthedocs/ayugespidertools)
-![GitHub all releases](https://img.shields.io/github/downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/AyugeSpiderTools?label=pypi%20downloads)
-![codecov](https://codecov.io/gh/shengchenyang/AyugeSpiderTools/graph/badge.svg?token=1QLOEW2NTI)
-
-**简体中文** | [English](./README_en.md)
-
-## 概述
-
-> 一句话介绍：用于扩展 Scrapy 功能来解放双手。
-
-在使用 `Scrapy` 开发爬虫时，免不了会重复地编写 `settings`，`items`，`middlewares`，`pipelines`
-和一些通用方法，但各项目中的这些内容都大致相同，那为何不把它们统一整理在一起呢？我也想扩展一些功能，比如当 `spider`
-中添加字段后，不用再修改对应的 `item` 和 `pipeline` 甚至不用手动修改 `Mysql` 和 `PostgreSQL` 的表结构。
-
-项目的主旨是让开发者只需专注于 `spider` 脚本的编写，减少开发和维护流程。理想状态下，只需关注 `spider`
-中字段的解析规则和 `VIT` 下的 `.conf` 配置即可，**脱离无意义的重复操作**。
-
-以 `Mysql` 存储场景举例：可以自动创建相关数据库，数据表，字段注释，自动添加 `spider`
-中新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等）的存储问题。
-
-## 安装
-
-> `python 3.8+` 可以直接输入以下命令：
-
-```shell
-pip install ayugespidertools
-```
-
-> 可选安装1，安装数据库相关的所有依赖：
-
-```shell
-pip install ayugespidertools[database]
-```
-
-> 可选安装2，通过以下命令安装所有依赖：
-
-```shell
-pip install ayugespidertools[all]
-```
-
-*注：详细的安装介绍请查看[安装指南](https://ayugespidertools.readthedocs.io/en/latest/intro/install.html)。*
-
-## 用法
-
-> 开发人员只需根据命令生成示例模板，再配置相关设置即可。
-
-使用方法示例 `GIF` 如下：
-
-![ayugespidertools.gif](./examples/ayugespidertools-use.gif)
-
-对以上 `GIF` 中的步骤进行解释：
-
-```shell
-# 查看库版本
-ayuge version
-
-# 创建项目
-ayuge startproject <project_name>
-
-# 进入项目根目录
-cd <project_name>
-
-# 替换(覆盖)为真实的配置 .conf 文件：
-# 这里是为了演示方便，正常情况是直接在 VIT 中的 .conf 文件填上你需要的配置即可
-cp /root/mytemp/.conf DemoSpider/VIT/.conf
-
-# 生成爬虫脚本
-ayuge genspider <spider_name> <example.com>
-
-# 运行脚本
-scrapy crawl <spider_name>
-# 注：也可以使用 ayuge crawl <spider_name>
-```
-
-具体的场景案例请在 [DemoSpider](https://github.com/shengchenyang/DemoSpider)
-项目中查看，也可以在 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中查看教程。 目前已适配以下场景：
-
-```diff
-+ 0).以下场景全支持从 nacos 或 consul 中获取配置，不一一举例。
-
-# 数据存入 Mysql 的场景：
-+ 1).demo_one: 从 .conf 中获取 mysql 配置
-+ 3).demo_three: 从 consul 中获取 mysql 配置
-+ 21).demo_mysql_nacos: 从 nacos 中获取 mysql 配置
-+ 5).demo_five: Twisted 异步存储示例
-+ 24).demo_aiomysql: 结合 aiomysql 实现的 asyncio 异步存储示例
-+ 13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
-
-# 数据存入 MongoDB 的场景：
-+ 2).demo_two: 从 .conf 中获取 mongodb 配置
-+ 4).demo_four: 从 consul 中获取 mongodb 配置
-+ 6).demo_six: Twisted 异步存储示例
-+ 17).demo_mongo_async: 结合 motor 实现的 asyncio 异步存储示例
-
-# 数据存入 PostgreSQL 的场景(需要安装 ayugespidertools[database])
-+ 22).demo_nine: 从 .conf 中获取 postgresql 配置
-+ 23).demo_ten: Twisted 异步存储示例
-+ 27).demo_eleven: asyncio 异步存储示例
-
-# 数据存入 ElasticSearch 的场景(需要安装 ayugespidertools[database])
-+ 28).demo_es: 普通同步存储示例
-+ 29).demo_es_async: asyncio 异步存储示例
-
-# 数据存入 Oracle 的场景(需要安装 ayugespidertools[database])
-+ 25). demo_oracle: 普通同步存储示例
-+ 26). demo_oracle_twisted: Twisted 异步存储示例
-
-- 7).demo_seven: 使用 requests 来请求的场景(已删除，更推荐 aiohttp 方式)
-+ 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
-+ 9).demo_aiohttp_example: 使用 aiohttp 来请求的场景
-+ 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
-
-+ 11).demo_proxy_one: 快代理动态隧道代理示例
-+ 12).demo_proxy_two: 测试快代理独享代理
-+ 14).demo_crawl: 支持 scrapy CrawlSpider 的示例
-
-# 本库中给出支持 Item Loaders 特性的示例
-+ 15).demo_item_loader: 本库中使用 Item Loaders 的示例
-- 16).demo_item_loader_two: 已删除，可查看 demo_item_loader，可方便的使用 Item Loaders 了
-
-+ 18).demo_mq: 数据存入 rabbitmq 的模板示例
-+ 19).demo_kafka: 数据存入 kafka 的模板示例
-+ 20).demo_file: 使用本库 pipeline 下载图片等文件到本地的示例
-+ 30).demo_file_sec: 自行实现的图片下载示例
-+ 31).demo_oss: 使用本库 pipeline 上传到 oss 的示例
-+ 32).demo_oss_sec: 自行实现的 oss 上传示例
-```
-
-## 跑通测试
-
-前提：需要在 `tests` 的 `VIT` 目录下创建 `.conf` 文件，已给出示例文件，请填写测试所需内容，然后：
-
-- 可以直接使用 `tox` 来运行测试。
-
-- 本库以 [poetry](https://python-poetry.org/docs/) 开发，那么直接新环境下运行 `poetry install`
-  后，手动运行目标测试或 `pytest` 命令来测试等皆可。
-- 也可以使用 `make` 工具，`make start` 然后 `make test` 即可。
-
-## 你可能在意的事
-
-1. 若你觉得某些场景下的功能实现不太符合你的预期，想要修改或添加自定义功能，比如移除对你无用模块、修改库名等，你可以自行修改后 `build`。
-
-2. 本库主推 `scrapy` 扩展（即增强版的自定义模板）的功能，在使用本库时，理论上并不会影响你 `scrapy`
-   项目及其它组件。
-
-3. 代码测试覆盖率有点低，考虑增加吗？
-
-   不考虑，场景所依赖服务太多，且云服务等其它因素导致个人维护成本过高，但不必担心，我会和本地服务的自动化测试结合使用。
-
-4. 如果你想对此项目做出贡献，请参考[pull request 示例](https://ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)。
-
-## 构建你的专属库
-
-> 具体内容请以 [poetry 官方文档](https://python-poetry.org/docs/) 为准。
-
-据[你可能在意的事](#你可能在意的事)可知，你可以 `clone`
-源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry build`
-或 `make build` 即可打包使用。
-
-比如你可能需要更新依赖库中 `kafka-python` 为新版本 `x.x.x`，那只需 `poetry install`
-安装现有依赖后，再 `poetry add kafka-python==x.x.x` 安装目标版本（尽量不要使用 `poetry update kafka-python`
-），确定测试正常了即可 `poetry build` 打包使用。
-
-**希望此项目能在你遇到扩展 scrapy 功能的场景时能对你有所指引。**
-
-## 功能
-
-- [x] `scrapy` 的扩展功能场景
-    - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
-    - [x] 自定义模板，在 `ayuge startproject <projname>` 和 `ayuge genspider <spidername>` 时生成适合本库的模板文件
-    - [x] 从远程应用管理服务中获取项目配置
-        - [x] 从 `consul` 获取项目配置
-        - [x] 从 `nacos` 获取项目配置（注意：优先级小于 `consul`）
-    - [x] 代理中间件（独享代理、动态隧道代理）
-    - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
-    - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-        - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp`
-          的方式）
-        - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
-    - [x] `Mysql` 存储的场景下适配
-        - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
-    - [x] `MongoDB` 存储场景适配
-    - [x] `PostgreSQL` 存储场景适配
-    - [x] `ElasticSearch` 存储场景适配
-    - [x] `Oracle` 存储场景适配
-    - [x] `oss` 上传场景适配
-    - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
-        - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
-        - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
-    - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
-- [x] 常用开发场景
-    - [x] `sql` 语句拼接，只用于简单场景。已给出优化方向，参考库等信息。
-    - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
-    - [x] 字体反爬还原方法
-        - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
-            - [x] 可以直接在字体文件 `xml`
-              中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
-            - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`
-              ，后再通过各种方式识别。
-    - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等
-    - [x] 添加常用的图片验证码中的处理方法
-        - [x] 滑块缺口距离的识别方法（多种实现方式）
-        - [x] 根据滑块距离生成轨迹数组的方法
-        - [x] 识别点选验证码位置及点击顺序
-        - [x] 图片乱序混淆的还原方法示例
-
-注意：功能演示我将放入 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中，以防此部分内容过多。
+<p align="center">
+    <a href="https://ayugespidertools.readthedocs.io" target="_blank" rel="noopener noreferrer">
+        <img src="./artwork/ayugespidertools-logo.png" alt="ayugespidertools-logo">
+    </a>
+</p>
+<hr/>
+
+# AyugeSpiderTools 介绍
+
+![license](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
+![python support](https://img.shields.io/badge/python-3.8%2B-blue)
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/codeql.yml?branch=main)
+![Read the Docs](https://img.shields.io/readthedocs/ayugespidertools)
+![GitHub all releases](https://img.shields.io/github/downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/AyugeSpiderTools?label=pypi%20downloads)
+![codecov](https://codecov.io/gh/shengchenyang/AyugeSpiderTools/graph/badge.svg?token=1QLOEW2NTI)
+
+**简体中文** | [English](./README_en.md)
+
+## 概述
+
+> 一句话介绍：用于扩展 Scrapy 功能来解放双手。
+
+在使用 `Scrapy` 开发爬虫时，免不了会重复地编写 `settings`，`items`，`middlewares`，`pipelines`
+和一些通用方法，但各项目中的这些内容都大致相同，那为何不把它们统一整理在一起呢？我也想扩展一些功能，比如当 `spider`
+中添加字段后，不用再修改对应的 `item` 和 `pipeline` 甚至不用手动修改 `Mysql` 和 `PostgreSQL` 的表结构。
+
+项目的主旨是让开发者只需专注于 `spider` 脚本的编写，减少开发和维护流程。理想状态下，只需关注 `spider`
+中字段的解析规则和 `VIT` 下的 `.conf` 配置即可，**脱离无意义的重复操作**。
+
+以 `Mysql` 存储场景举例：可以自动创建相关数据库，数据表，字段注释，自动添加 `spider`
+中新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等）的存储问题。
+
+## 安装
+
+> `python 3.8+` 可以直接输入以下命令：
+
+```shell
+pip install ayugespidertools
+```
+
+> 可选安装1，安装数据库相关的所有依赖：
+
+```shell
+pip install ayugespidertools[database]
+```
+
+> 可选安装2，通过以下命令安装所有依赖：
+
+```shell
+pip install ayugespidertools[all]
+```
+
+*注：详细的安装介绍请查看[安装指南](https://ayugespidertools.readthedocs.io/en/latest/intro/install.html)。*
+
+## 用法
+
+> 开发人员只需根据命令生成示例模板，再配置相关设置即可。
+
+使用方法示例 `GIF` 如下：
+
+![ayugespidertools.gif](./examples/ayugespidertools-use.gif)
+
+对以上 `GIF` 中的步骤进行解释：
+
+```shell
+# 查看库版本
+ayuge version
+
+# 创建项目
+ayuge startproject <project_name>
+
+# 进入项目根目录
+cd <project_name>
+
+# 替换(覆盖)为真实的配置 .conf 文件：
+# 这里是为了演示方便，正常情况是直接在 VIT 中的 .conf 文件填上你需要的配置即可
+cp /root/mytemp/.conf DemoSpider/VIT/.conf
+
+# 生成爬虫脚本
+ayuge genspider <spider_name> <example.com>
+
+# 运行脚本
+scrapy crawl <spider_name>
+# 注：也可以使用 ayuge crawl <spider_name>
+```
+
+具体的场景案例请在 [DemoSpider](https://github.com/shengchenyang/DemoSpider)
+项目中查看，也可以在 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中查看教程。目前已适配以下场景：
+
+```diff
++ 0).以下场景全支持从 nacos 或 consul 中获取配置，不一一举例。
+
+# 数据存入 Mysql 的场景：
++ 1).demo_one: 从 .conf 中获取 mysql 配置
++ 3).demo_three: 从 consul 中获取 mysql 配置
++ 21).demo_mysql_nacos: 从 nacos 中获取 mysql 配置
++ 5).demo_five: Twisted 异步存储示例
++ 24).demo_aiomysql: 结合 aiomysql 实现的 asyncio 异步存储示例
++ 13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
+
+# 数据存入 MongoDB 的场景：
++ 2).demo_two: 从 .conf 中获取 mongodb 配置
++ 4).demo_four: 从 consul 中获取 mongodb 配置
++ 6).demo_six: Twisted 异步存储示例
++ 17).demo_mongo_async: 结合 motor 实现的 asyncio 异步存储示例
+
+# 数据存入 PostgreSQL 的场景(需要安装 ayugespidertools[database])
++ 22).demo_nine: 从 .conf 中获取 postgresql 配置
++ 23).demo_ten: Twisted 异步存储示例
++ 27).demo_eleven: asyncio 异步存储示例
+
+# 数据存入 ElasticSearch 的场景(需要安装 ayugespidertools[database])
++ 28).demo_es: 普通同步存储示例
++ 29).demo_es_async: asyncio 异步存储示例
+
+# 数据存入 Oracle 的场景(需要安装 ayugespidertools[database])
++ 25). demo_oracle: 普通同步存储示例
++ 26). demo_oracle_twisted: Twisted 异步存储示例
+
+- 7).demo_seven: 使用 requests 来请求的场景(已删除，更推荐 aiohttp 方式)
++ 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
++ 9).demo_aiohttp_example: 使用 aiohttp 来请求的场景
++ 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
+
++ 11).demo_proxy_one: 快代理动态隧道代理示例
++ 12).demo_proxy_two: 测试快代理独享代理
++ 14).demo_crawl: 支持 scrapy CrawlSpider 的示例
+
+# 本库中给出支持 Item Loaders 特性的示例
++ 15).demo_item_loader: 本库中使用 Item Loaders 的示例
+- 16).demo_item_loader_two: 已删除，可查看 demo_item_loader，可方便的使用 Item Loaders 了
+
++ 18).demo_mq: 数据存入 rabbitmq 的模板示例
++ 19).demo_kafka: 数据存入 kafka 的模板示例
++ 20).demo_file: 使用本库 pipeline 下载图片等文件到本地的示例
++ 30).demo_file_sec: 自行实现的图片下载示例
++ 31).demo_oss: 使用本库 pipeline 上传到 oss 的示例
++ 32).demo_oss_sec: 自行实现的 oss 上传示例
+```
+
+## 跑通测试
+
+前提：需要在 `tests` 的 `VIT` 目录下创建 `.conf` 文件，已给出示例文件，请填写测试所需内容，然后：
+
+- 可以直接使用 `tox` 来运行测试。
+- 本库以 [poetry](https://python-poetry.org/docs/) 开发，那么直接新环境下运行 `poetry install`
+  后，手动运行目标测试或 `pytest` 命令来测试等皆可。
+- 也可以使用 `make` 工具，`make start` 然后 `make test` 即可。
+
+## 你可能在意的事
+
+1. 若你觉得某些场景下的功能实现不太符合你的预期，想要修改或添加自定义功能，比如移除对你无用模块、修改库名等，你可以自行修改后 `build`。
+
+2. 本库主推 `scrapy` 扩展功能，在使用本库时，不会影响你 `scrapy` 项目及其它组件。
+
+   也就是说，可使用本库开发原生的 `scrapy`，也可用 `scrapy` 的风格来开发，但还是推荐使用 `DemoSpider` 示例中的风格开发。不会对开发者造成过多的迁移成本。
+
+3. 代码测试覆盖率有点低，考虑增加吗？
+
+   不考虑，场景所依赖服务太多，且云服务等其它因素导致个人维护成本过高，但不必担心，我会和本地服务的自动化测试结合使用。
+
+4. 如果你想对此项目做出贡献，请参考 [pull request 示例](https://ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)。
+
+## 构建你的专属库
+
+> 具体内容请以 [poetry 官方文档](https://python-poetry.org/docs/) 为准。
+
+据[你可能在意的事](#你可能在意的事)可知，你可以 `clone`
+源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry build`
+或 `make build` 即可打包使用。
+
+比如你可能需要更新依赖库中 `kafka-python` 为新版本 `x.x.x`，那只需 `poetry install`
+安装现有依赖后，再 `poetry add kafka-python==x.x.x` 安装目标版本（尽量不要使用 `poetry update kafka-python`
+），确定测试正常了即可 `poetry build` 打包使用。
+
+**希望此项目能在你遇到扩展 scrapy 功能的场景时能对你有所指引。**
+
+## 功能
+
+- [x] `scrapy` 的扩展功能场景
+  - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
+  - [x] 自定义模板，在 `ayuge startproject <projname>` 和 `ayuge genspider <spidername>` 时生成适合本库的模板文件
+  - [x] 从远程应用管理服务中获取项目配置
+    - [x] 从 `consul` 获取项目配置
+    - [x] 从 `nacos` 获取项目配置（注意：优先级小于 `consul`）
+  - [x] 代理中间件（独享代理、动态隧道代理）
+  - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
+  - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
+    - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp`
+      的方式）
+    - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
+  - [x] `Mysql` 存储的场景下适配
+    - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
+  - [x] `MongoDB` 存储场景适配
+  - [x] `PostgreSQL` 存储场景适配
+  - [x] `ElasticSearch` 存储场景适配
+  - [x] `Oracle` 存储场景适配
+  - [x] `oss` 上传场景适配
+  - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
+    - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
+    - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
+  - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
+- [x] 常用开发场景
+  - [x] `sql` 语句拼接，只用于简单场景。
+  - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
+  - [x] 字体反爬还原方法
+    - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
+      - [x] 可以直接在字体文件 `xml`
+        中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
+      - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`
+        ，后再通过各种方式识别。
+    - [x] 字体反爬部分功能迁移到 `FontMapster` 项目中。
+  - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等
+  - [x] 添加常用的图片验证码中的处理方法
+    - [x] 滑块缺口距离的识别方法（多种实现方式）
+    - [x] 根据滑块距离生成轨迹数组的方法
+    - [x] 识别点选验证码位置及点击顺序
+    - [x] 图片乱序混淆的还原方法示例
+
+注意：功能演示我将放入 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中，以防此部分内容过多。
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                             _[_a_y_u_g_e_s_p_i_d_e_r_t_o_o_l_s_-_l_o_g_o_]
 ===============================================================================
-# AyugeSpiderTools ä»ç» ![GitHub](https://img.shields.io/github/license/
-shengchenyang/AyugeSpiderTools) ![python](https://img.shields.io/badge/python-
-3.8%2B-blue) ![GitHub Workflow Status (with branch)](https://img.shields.io/
-github/actions/workflow/status/shengchenyang/AyugeSpiderTools/
+# AyugeSpiderTools ä»ç» ![license](https://img.shields.io/github/license/
+shengchenyang/AyugeSpiderTools) ![python support](https://img.shields.io/badge/
+python-3.8%2B-blue) ![GitHub Workflow Status (with branch)](https://
+img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/
 codeql.yml?branch=main) ![Read the Docs](https://img.shields.io/readthedocs/
 ayugespidertools) ![GitHub all releases](https://img.shields.io/github/
 downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/
 AyugeSpiderTools?label=pypi%20downloads) ![codecov](https://codecov.io/gh/
 shengchenyang/AyugeSpiderTools/graph/badge.svg?token=1QLOEW2NTI)
 **ç®ä½ä¸­æ** | [English](./README_en.md) ## æ¦è¿° >
@@ -38,15 +38,15 @@
 è¿å¥é¡¹ç®æ ¹ç®å½ cd # æ¿æ¢(è¦ç)ä¸ºçå®çéç½® .conf æä»¶ï¼ #
 è¿éæ¯ä¸ºäºæ¼ç¤ºæ¹ä¾¿ï¼æ­£å¸¸æåµæ¯ç´æ¥å¨ VIT ä¸­ç .conf
 æä»¶å¡«ä¸ä½ éè¦çéç½®å³å¯ cp /root/mytemp/.conf DemoSpider/VIT/.conf
 # çæç¬è«èæ¬ ayuge genspider # è¿è¡èæ¬ scrapy crawl #
 æ³¨ï¼ä¹å¯ä»¥ä½¿ç¨ ayuge crawl ``` å·ä½çåºæ¯æ¡ä¾è¯·å¨ [DemoSpider]
 (https://github.com/shengchenyang/DemoSpider) é¡¹ç®ä¸­æ¥çï¼ä¹å¯ä»¥å¨
 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/
-) ææ¡£ä¸­æ¥çæç¨ã ç®åå·²ééä»¥ä¸åºæ¯ï¼ ```diff +
+) ææ¡£ä¸­æ¥çæç¨ãç®åå·²ééä»¥ä¸åºæ¯ï¼ ```diff +
 0).ä»¥ä¸åºæ¯å¨æ¯æä» nacos æ consul
 ä¸­è·åéç½®ï¼ä¸ä¸ä¸ä¸¾ä¾ã # æ°æ®å­å¥ Mysql çåºæ¯ï¼ +
 1).demo_one: ä» .conf ä¸­è·å mysql éç½® + 3).demo_three: ä» consul
 ä¸­è·å mysql éç½® + 21).demo_mysql_nacos: ä» nacos ä¸­è·å mysql éç½®
 + 5).demo_five: Twisted å¼æ­¥å­å¨ç¤ºä¾ + 24).demo_aiomysql: ç»å aiomysql
 å®ç°ç asyncio å¼æ­¥å­å¨ç¤ºä¾ + 13).demo_AyuTurboMysqlPipeline: mysql
 åæ­¥è¿æ¥æ± çç¤ºä¾ # æ°æ®å­å¥ MongoDB çåºæ¯ï¼ + 2).demo_two: ä»
@@ -81,23 +81,26 @@
 å¯ä»¥ç´æ¥ä½¿ç¨ `tox` æ¥è¿è¡æµè¯ã - æ¬åºä»¥ [poetry](https://
 python-poetry.org/docs/) å¼åï¼é£ä¹ç´æ¥æ°ç¯å¢ä¸è¿è¡ `poetry
 install` åï¼æå¨è¿è¡ç®æ æµè¯æ `pytest` å½ä»¤æ¥æµè¯ç­çå¯ã
 - ä¹å¯ä»¥ä½¿ç¨ `make` å·¥å·ï¼`make start` ç¶å `make test` å³å¯ã ##
 ä½ å¯è½å¨æçäº 1.
 è¥ä½ è§å¾æäºåºæ¯ä¸çåè½å®ç°ä¸å¤ªç¬¦åä½ çé¢æï¼æ³è¦ä¿®æ¹ææ·»å èªå®ä¹åè½ï¼æ¯å¦ç§»é¤å¯¹ä½ æ ç¨æ¨¡åãä¿®æ¹åºåç­ï¼ä½ å¯ä»¥èªè¡ä¿®æ¹å
 `build`ã 2. æ¬åºä¸»æ¨ `scrapy`
-æ©å±ï¼å³å¢å¼ºççèªå®ä¹æ¨¡æ¿ï¼çåè½ï¼å¨ä½¿ç¨æ¬åºæ¶ï¼çè®ºä¸å¹¶ä¸ä¼å½±åä½ 
-`scrapy` é¡¹ç®åå¶å®ç»ä»¶ã 3.
+æ©å±åè½ï¼å¨ä½¿ç¨æ¬åºæ¶ï¼ä¸ä¼å½±åä½  `scrapy`
+é¡¹ç®åå¶å®ç»ä»¶ã ä¹å°±æ¯è¯´ï¼å¯ä½¿ç¨æ¬åºå¼ååçç
+`scrapy`ï¼ä¹å¯ç¨ `scrapy` çé£æ ¼æ¥å¼åï¼ä½è¿æ¯æ¨èä½¿ç¨
+`DemoSpider`
+ç¤ºä¾ä¸­çé£æ ¼å¼åãä¸ä¼å¯¹å¼åèé æè¿å¤çè¿ç§»ææ¬ã 3.
 ä»£ç æµè¯è¦ççæç¹ä½ï¼èèå¢å åï¼
 ä¸èèï¼åºæ¯æä¾èµæå¡å¤ªå¤ï¼ä¸äºæå¡ç­å¶å®å ç´ å¯¼è´ä¸ªäººç»´æ¤ææ¬è¿é«ï¼ä½ä¸å¿æå¿ï¼æä¼åæ¬å°æå¡çèªå¨åæµè¯ç»åä½¿ç¨ã
-4. å¦æä½ æ³å¯¹æ­¤é¡¹ç®ååºè´¡ç®ï¼è¯·åè[pull request ç¤ºä¾](https:
-//ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)ã ##
-æå»ºä½ çä¸å±åº > å·ä½åå®¹è¯·ä»¥ [poetry å®æ¹ææ¡£](https://
-python-poetry.org/docs/) ä¸ºåã æ®[ä½ å¯è½å¨æçäº]
-(#ä½ å¯è½å¨æçäº)å¯ç¥ï¼ä½ å¯ä»¥ `clone`
+4. å¦æä½ æ³å¯¹æ­¤é¡¹ç®ååºè´¡ç®ï¼è¯·åè [pull request ç¤ºä¾]
+(https://ayugespidertools.readthedocs.io/en/latest/additional/
+contribute.html)ã ## æå»ºä½ çä¸å±åº > å·ä½åå®¹è¯·ä»¥ [poetry
+å®æ¹ææ¡£](https://python-poetry.org/docs/) ä¸ºåã æ®
+[ä½ å¯è½å¨æçäº](#ä½ å¯è½å¨æçäº)å¯ç¥ï¼ä½ å¯ä»¥ `clone`
 æºç åï¼ä¿®æ¹ä»»ææ¹æ³ï¼æ¯å¦ä½ çé¡¹ç®åºæ¯ä¸å¯è½éè¦å¶å®çæ¥å¿éç½®é»è®¤å¼ï¼ææ·»å å¶å®çé¡¹ç®ç»ææ¨¡æ¿ç­ï¼ï¼ä¿®æ¹å®æå
 `poetry build` æ `make build` å³å¯æåä½¿ç¨ã
 æ¯å¦ä½ å¯è½éè¦æ´æ°ä¾èµåºä¸­ `kafka-python` ä¸ºæ°çæ¬
 `x.x.x`ï¼é£åªé `poetry install` å®è£ç°æä¾èµåï¼å `poetry add
 kafka-python==x.x.x` å®è£ç®æ çæ¬ï¼å°½éä¸è¦ä½¿ç¨ `poetry update
 kafka-python` ï¼ï¼ç¡®å®æµè¯æ­£å¸¸äºå³å¯ `poetry build` æåä½¿ç¨ã
 **å¸ææ­¤é¡¹ç®è½å¨ä½ éå°æ©å± scrapy
@@ -119,24 +122,24 @@
 ç¨æ·åºæ¯ä¸éè¦çæ°æ®åºåæ°æ®è¡¨åå­æ®µæ ¼å¼ï¼è¿æå­æ®µæ³¨é
 - [x] `MongoDB` å­å¨åºæ¯éé - [x] `PostgreSQL` å­å¨åºæ¯éé - [x]
 `ElasticSearch` å­å¨åºæ¯éé - [x] `Oracle` å­å¨åºæ¯éé - [x]
 `oss` ä¸ä¼ åºæ¯éé - [x] `asyncio` è¯­æ³æ¯æä¸ `async`
 ç¬¬ä¸æ¹åºæ¯æç¤ºä¾ - [x] `spider` ä¸­ä½¿ç¨ `asyncio` ç `aiohttp`
 ç¤ºä¾ - [x] `pipeline` ä¸­ä½¿ç¨ `asyncio` ç `aioMysql` ç¤ºä¾ - [x] éæ
 `Kafka`ï¼`RabbitMQ` ç­æ°æ®æ¨éåè½ - [x] å¸¸ç¨å¼ååºæ¯ - [x] `sql`
-è¯­å¥æ¼æ¥ï¼åªç¨äºç®ååºæ¯ãå·²ç»åºä¼åæ¹åï¼åèåºç­ä¿¡æ¯ã
-- [x]
+è¯­å¥æ¼æ¥ï¼åªç¨äºç®ååºæ¯ã - [x]
 æ°æ®æ ¼å¼åå¤çï¼æ¯å¦ï¼å»é¤ç½é¡µæ ç­¾ï¼å»é¤æ æç©ºæ ¼ç­ -
 [x] å­ä½åç¬è¿åæ¹æ³ - [x] åºäº `ttf`ï¼`woff`
 ä¹ç±»çå­ä½æä»¶æ å°ï¼æç»å `css` ç­å®ç° - [x]
 å¯ä»¥ç´æ¥å¨å­ä½æä»¶ `xml` ä¸­æ¾å°æ å°å³ç³»çï¼ä½¿ç¨ [fontforge]
 (https://github.com/fontforge/fontforge/releases) å·¥å·å¯¼åºæ å°å³å¯ã -
 [x] æ æ³æ¾å°æ å°å³ç³»çï¼åä¸è¬ä½¿ç¨ `ocr`
 è¯å«ï¼åç¡®çéç¾åç¾ï¼ï¼éè¿ `fontforge` å¯¼åºæ¯ä¸ªæ å°ç
-`png` ï¼ååéè¿åç§æ¹å¼è¯å«ã - [x] `html`
+`png` ï¼ååéè¿åç§æ¹å¼è¯å«ã - [x]
+å­ä½åç¬é¨ååè½è¿ç§»å° `FontMapster` é¡¹ç®ä¸­ã - [x] `html`
 æ°æ®å¤çï¼å»é¤æ ç­¾ï¼ä¸å¯è§å­ç¬¦ï¼ç¹æ®å­ç¬¦æ¹ææ­£å¸¸æ¾ç¤ºç­
 - [x] æ·»å å¸¸ç¨çå¾çéªè¯ç ä¸­çå¤çæ¹æ³ - [x]
 æ»åç¼ºå£è·ç¦»çè¯å«æ¹æ³ï¼å¤ç§å®ç°æ¹å¼ï¼ - [x]
 æ ¹æ®æ»åè·ç¦»çæè½¨è¿¹æ°ç»çæ¹æ³ - [x]
 è¯å«ç¹ééªè¯ç ä½ç½®åç¹å»é¡ºåº - [x]
 å¾çä¹±åºæ··æ·çè¿åæ¹æ³ç¤ºä¾ æ³¨æï¼åè½æ¼ç¤ºæå°æ¾å¥
 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/encryption.py` & `ayugespidertools-3.9.8/ayugespidertools/common/encryption.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,37 @@
 import hashlib
 import re
 from typing import Union
 
 from ayugespidertools.extras.ext import EncryptMixin
 
 __all__ = [
-    "EncryptOperation",
+    "Encrypt",
 ]
 
 
-class EncryptOperation(EncryptMixin):
+class Encrypt(EncryptMixin):
     """普通加密方法"""
 
-    @classmethod
-    def md5(cls, encrypt_data: str) -> str:
+    @staticmethod
+    def md5(encrypt_data: str) -> str:
         """md5 处理方法
 
         Args:
             encrypt_data: 需要 md5 处理的参数
 
         Returns:
             1): md5 处理后的参数
         """
         hl = hashlib.md5()
         hl.update(encrypt_data.encode(encoding="utf-8"))
         return hl.hexdigest()
 
-    @classmethod
-    def base64_encode(
-        cls, encode_data: Union[bytes, str], url_safe: bool = False
-    ) -> str:
+    @staticmethod
+    def base64_encode(encode_data: Union[bytes, str], url_safe: bool = False) -> str:
         """base64 编码
 
         Args:
             encode_data: 需要 base64 编码的参数
             url_safe: 标准的 Base64 编码后可能出现字符 + 和 /，在 url 中就不能直接作为参数。是否要处理此情况
 
         Returns:
@@ -42,16 +40,16 @@
         """
         if not isinstance(encode_data, bytes):
             encode_data = bytes(encode_data, encoding="utf-8")
         if url_safe:
             return str(base64.urlsafe_b64encode(encode_data), encoding="utf-8")
         return str(base64.b64encode(encode_data), encoding="utf-8")
 
-    @classmethod
-    def base64_decode(cls, decode_data: str, url_safe: bool = False) -> str:
+    @staticmethod
+    def base64_decode(decode_data: str, url_safe: bool = False) -> str:
         """base64 解码
 
         Args:
             decode_data: 需要 base64 解码的参数
             url_safe: 标准的 Base64 编码后可能出现字符 + 和 /，在 url 中就不能直接作为参数。是否要处理此情况
 
         Returns:
@@ -70,9 +68,8 @@
                 如：006A，但它可能是非标准的，可能需要去掉前面的 0x 或 uni。
 
         Returns:
             1). 转换后的字符
         """
         _uni = re.sub(r"^(0x|U\+|uni)", "", uni)
         unicode_value = int(_uni, 16)
-        # 使用 chr() 函数将整数值转换为字符
         return chr(unicode_value)
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/expend.py` & `ayugespidertools-3.9.8/ayugespidertools/common/expend.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,292 +1,288 @@
-import datetime
-from typing import TYPE_CHECKING, Tuple
-
-import pymysql
-from retrying import retry
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
-from ayugespidertools.config import logger
-
-try:
-    import oracledb
-    import psycopg
-except ImportError:
-    # pip install ayugespidertools[database]
-    pass
-
-__all__ = [
-    "MysqlPipeEnhanceMixin",
-    "PostgreSQLPipeEnhanceMixin",
-    "OraclePipeEnhanceMixin",
-]
-
-if TYPE_CHECKING:
-    from oracledb.connection import Connection as OracleConnection
-    from psycopg.connection import Connection as PsycopgConnection
-    from pymysql.connections import Connection as PymysqlConnection
-
-    from ayugespidertools.common.typevars import MysqlConf, OracleConf, PostgreSQLConf
-
-
-class MysqlPipeEnhanceMixin:
-    """扩展 mysql pipelines 的功能"""
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def _connect(
-        self,
-        mysql_conf: "MysqlConf",
-    ) -> "PymysqlConnection":
-        """链接数据库操作：
-            1.如果链接正常，则返回链接句柄；
-            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
-
-        Args:
-            mysql_conf: pymysql 链接所需的参数
-
-        Returns:
-            1). mysql 链接句柄
-        """
-        pymysql_conn_args = {
-            "user": mysql_conf.user,
-            "password": mysql_conf.password,
-            "host": mysql_conf.host,
-            "port": mysql_conf.port,
-            "database": mysql_conf.database,
-            "charset": mysql_conf.charset,
-        }
-        try:
-            conn = pymysql.connect(**pymysql_conn_args)
-        except Exception as e:
-            # (1049, "Unknown database 'xxx'")
-            if "1049" in str(e):
-                logger.warning(
-                    f"目标数据库：{mysql_conf.database} 不存在，尝试创建中..."
-                )
-                # 如果连接目标数据库报不存在的错误时，先创建出此目标数据库
-                ReuseOperation.create_database(db_conf=mysql_conf)
-            else:
-                logger.error(f"connect to mysql failed: {e}")
-        else:
-            # 连接没有问题就直接返回连接对象
-            return conn
-        # 出现数据库不存在问题后，在创建数据库后，再次返回连接对象
-        return pymysql.connect(**pymysql_conn_args)
-
-    def _get_sql_by_item(
-        self, table: str, item: dict, odku_enable: bool = True
-    ) -> Tuple[str, tuple]:
-        """根据处理后的 item 生成 mysql 插入语句
-
-        Args:
-            table: 数据库表名
-            item: 处理后的 item
-            odku_enable: 是否开启 ON DUPLICATE KEY UPDATE
-
-        Returns:
-            1). sql 插入语句
-            2). sql 语句执行和格式化需要的 value
-        """
-        keys = f"""`{"`, `".join(item.keys())}`"""
-        values = ", ".join(["%s"] * len(item))
-        if odku_enable:
-            update = ",".join([f" `{key}` = %s" for key in item])
-            sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-            args = tuple(item.values()) * 2
-        else:
-            sql = f"INSERT INTO `{table}` ({keys}) values ({values})"
-            args = tuple(item.values())
-        return sql, args
-
-    def _get_log_by_spider(self, spider, crawl_time):
-        """获取 spider 的运行日志情况
-
-        Args:
-            spider: scrapy spider
-            crawl_time: 爬取时间
-
-        Returns:
-            log_info: 日志信息
-        """
-        mysql_conf = spider.mysql_conf
-        text = {}
-        stats = spider.crawler.stats.get_stats()
-        error_reason = ""
-        _curr_utc_time = datetime.datetime.now(datetime.timezone.utc)
-        for k, v in stats.items():
-            if isinstance(v, datetime.datetime):
-                text[k.replace("/", "_")] = (v + datetime.timedelta(hours=8)).strftime(
-                    "%Y-%m-%d %H:%M:%S"
-                )
-            else:
-                if all(
-                    [
-                        "response_status_count" in k,
-                        k != "downloader/response_status_count/200",
-                    ]
-                ):
-                    status_code = k.split("/")[-1] if len(k.split("/")) > 0 else ""
-                    if status_code.startswith("4"):
-                        if status_code == "429":
-                            error_reason += f"{status_code}错误：代理超过使用频率限制"
-                        else:
-                            error_reason += (
-                                f"{status_code}错误：网页失效/无此网页/网站拒绝访问"
-                            )
-                    elif status_code.startswith("5"):
-                        error_reason += f"{status_code}错误：网站服务器处理出错"
-                    elif status_code != "":
-                        error_reason += f"{status_code}:待人工排查原因"
-                elif "exception_type_count" in k:
-                    error_name = k.split("/")[-1]
-                    if "Timeout" in error_name:
-                        error_reason += f"{error_name}:网站响应超时错误 "
-                    elif "ConnectionDone" in error_name:
-                        error_reason += f"{error_name}:网站与脚本连接断开 "
-                    else:
-                        # "ResponseNeverReceived" or "ResponseFailed"
-                        error_reason += f"{error_name}:网站无响应 "
-                text[k.replace("/", "_")] = v
-
-        log_info = {
-            "database": mysql_conf.database,
-            "spider_name": spider.name,
-            "uid": f"{mysql_conf.database}|{spider.name}",
-            "request_counts": text.get("downloader_request_count", 0),
-            "received_count": text.get("response_received_count", 0),
-            "item_counts": text.get("item_scraped_count", 0),
-            "info_count": text.get("log_count_INFO", 0),
-            "warning_count": text.get("log_count_WARNING", 0),
-            "error_count": text.get("log_count_ERROR", 0),
-            "start_time": text.get("start_time"),
-            "finish_time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-            "spend_minutes": round(
-                (_curr_utc_time - stats.get("start_time")).seconds / 60,
-                2,
-            ),
-            "crawl_time": crawl_time,
-        }
-
-        # 错误原因
-        if text.get("log_count_ERROR", 0):
-            log_info["log_count_ERROR"] = error_reason or "请人工排查错误原因！"
-
-        else:
-            log_info["log_count_ERROR"] = ""
-        return log_info
-
-
-class PostgreSQLPipeEnhanceMixin:
-    """扩展 postgresql pipelines 的功能"""
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def _connect(
-        self,
-        postgres_conf: "PostgreSQLConf",
-    ) -> "PsycopgConnection":
-        """链接数据库操作：
-            1.如果链接正常，则返回链接句柄；
-            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
-
-        Args:
-            postgres_conf: postgresql 链接所需的参数
-
-        Returns:
-            1). postgresql 链接句柄
-        """
-        try:
-            conn = psycopg.connect(
-                user=postgres_conf.user,
-                password=postgres_conf.password,
-                host=postgres_conf.host,
-                port=postgres_conf.port,
-                dbname=postgres_conf.database,
-            )
-        except Exception as e:
-            # err: connection to server at "x.x.x.x", port x failed: FATAL:  database "x" does not exist
-            if "failed" in str(e).lower():
-                logger.warning(
-                    f"目标数据库：{postgres_conf.database} 不存在，尝试创建中..."
-                )
-                ReuseOperation.create_database(db_conf=postgres_conf)
-            else:
-                logger.error(f"connect to postgresql failed: {e}")
-        else:
-            return conn
-
-        return psycopg.connect(
-            user=postgres_conf.user,
-            password=postgres_conf.password,
-            host=postgres_conf.host,
-            port=postgres_conf.port,
-            dbname=postgres_conf.database,
-        )
-
-    def _get_sql_by_item(self, table: str, item: dict) -> str:
-        """根据处理后的 item 生成 postgresql 插入语句
-
-        Args:
-            table: 数据库表名
-            item: 处理后的 item
-
-        Returns:
-            1). sql 插入语句
-        """
-        keys = f"""{", ".join(item.keys())}"""
-        values = ", ".join(["%s"] * len(item))
-        return f"INSERT INTO {table} ({keys}) values ({values});"
-
-
-class OraclePipeEnhanceMixin:
-    """扩展 oracle pipelines 的功能"""
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def _connect(
-        self,
-        oracle_conf: "OracleConf",
-    ) -> "OracleConnection":
-        """链接数据库返回链接句柄
-
-        Args:
-            oracle_conf: oracle 链接所需的参数
-
-        Returns:
-            1). oracle 链接句柄
-        """
-        if oracle_thick_lib_dir := oracle_conf.thick_lib_dir:
-            oracledb.init_oracle_client(oracle_thick_lib_dir)
-
-        return oracledb.connect(
-            user=oracle_conf.user,
-            password=oracle_conf.password,
-            host=oracle_conf.host,
-            port=oracle_conf.port,
-            service_name=oracle_conf.service_name,
-            encoding=oracle_conf.encoding,
-        )
-
-    def _get_sql_by_item(self, table: str, item: dict) -> str:
-        """根据处理后的 item 生成 oracle 插入语句
-
-        Args:
-            table: 数据库表名
-            item: 处理后的 item
-
-        Returns:
-            1). sql 插入语句
-        """
-        keys = f""":{", :".join(item.keys())}"""
-        table_keys = ", ".join(map(lambda key: f'"{key}"', item.keys()))
-        return f'INSERT INTO "{table}" ({table_keys}) values ({keys})'
+import datetime
+from typing import TYPE_CHECKING, Tuple
+
+import pymysql
+from retrying import retry
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+from ayugespidertools.config import logger
+
+try:
+    import oracledb
+    import psycopg
+except ImportError:
+    # pip install ayugespidertools[database]
+    pass
+
+__all__ = [
+    "MysqlPipeEnhanceMixin",
+    "PostgreSQLPipeEnhanceMixin",
+    "OraclePipeEnhanceMixin",
+]
+
+if TYPE_CHECKING:
+    from oracledb.connection import Connection as OracleConnection
+    from psycopg.connection import Connection as PsycopgConnection
+    from pymysql.connections import Connection as PymysqlConnection
+
+    from ayugespidertools.common.typevars import MysqlConf, OracleConf, PostgreSQLConf
+
+
+class MysqlPipeEnhanceMixin:
+    """扩展 mysql pipelines 的功能"""
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def _connect(
+        self,
+        mysql_conf: "MysqlConf",
+    ) -> "PymysqlConnection":
+        """链接数据库操作：
+            1.如果链接正常，则返回链接句柄；
+            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
+
+        Args:
+            mysql_conf: pymysql 链接所需的参数
+
+        Returns:
+            1). mysql 链接句柄
+        """
+        pymysql_conn_args = {
+            "user": mysql_conf.user,
+            "password": mysql_conf.password,
+            "host": mysql_conf.host,
+            "port": mysql_conf.port,
+            "database": mysql_conf.database,
+            "charset": mysql_conf.charset,
+        }
+        try:
+            conn = pymysql.connect(**pymysql_conn_args)
+        except Exception as e:
+            # (1049, "Unknown database 'xxx'")
+            if "1049" in str(e):
+                logger.warning(
+                    f"目标数据库：{mysql_conf.database} 不存在，尝试创建中..."
+                )
+                ReuseOperation.create_database(db_conf=mysql_conf)
+            else:
+                logger.error(f"connect to mysql failed: {e}")
+        else:
+            return conn
+        return pymysql.connect(**pymysql_conn_args)
+
+    def _get_sql_by_item(
+        self, table: str, item: dict, odku_enable: bool = True
+    ) -> Tuple[str, tuple]:
+        """根据处理后的 item 生成 mysql 插入语句
+
+        Args:
+            table: 数据库表名
+            item: 处理后的 item
+            odku_enable: 是否开启 ON DUPLICATE KEY UPDATE
+
+        Returns:
+            1). sql 插入语句
+            2). sql 语句执行和格式化需要的 value
+        """
+        keys = f"""`{"`, `".join(item.keys())}`"""
+        values = ", ".join(["%s"] * len(item))
+        if odku_enable:
+            update = ",".join([f" `{key}` = %s" for key in item])
+            sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
+            args = tuple(item.values()) * 2
+        else:
+            sql = f"INSERT INTO `{table}` ({keys}) values ({values})"
+            args = tuple(item.values())
+        return sql, args
+
+    def _get_log_by_spider(self, spider, crawl_time):
+        """获取 spider 的运行日志情况
+
+        Args:
+            spider: scrapy spider
+            crawl_time: 爬取时间
+
+        Returns:
+            log_info: 日志信息
+        """
+        mysql_conf = spider.mysql_conf
+        text = {}
+        stats = spider.crawler.stats.get_stats()
+        error_reason = ""
+        _curr_utc_time = datetime.datetime.now(datetime.timezone.utc)
+        for k, v in stats.items():
+            if isinstance(v, datetime.datetime):
+                text[k.replace("/", "_")] = (v + datetime.timedelta(hours=8)).strftime(
+                    "%Y-%m-%d %H:%M:%S"
+                )
+            else:
+                if all(
+                    [
+                        "response_status_count" in k,
+                        k != "downloader/response_status_count/200",
+                    ]
+                ):
+                    status_code = k.split("/")[-1] if len(k.split("/")) > 0 else ""
+                    if status_code.startswith("4"):
+                        if status_code == "429":
+                            error_reason += f"{status_code}错误：代理超过使用频率限制"
+                        else:
+                            error_reason += (
+                                f"{status_code}错误：网页失效/无此网页/网站拒绝访问"
+                            )
+                    elif status_code.startswith("5"):
+                        error_reason += f"{status_code}错误：网站服务器处理出错"
+                    elif status_code != "":
+                        error_reason += f"{status_code}:待人工排查原因"
+                elif "exception_type_count" in k:
+                    error_name = k.split("/")[-1]
+                    if "Timeout" in error_name:
+                        error_reason += f"{error_name}:网站响应超时错误 "
+                    elif "ConnectionDone" in error_name:
+                        error_reason += f"{error_name}:网站与脚本连接断开 "
+                    else:
+                        # "ResponseNeverReceived" or "ResponseFailed"
+                        error_reason += f"{error_name}:网站无响应 "
+                text[k.replace("/", "_")] = v
+
+        log_info = {
+            "database": mysql_conf.database,
+            "spider_name": spider.name,
+            "uid": f"{mysql_conf.database}|{spider.name}",
+            "request_counts": text.get("downloader_request_count", 0),
+            "received_count": text.get("response_received_count", 0),
+            "item_counts": text.get("item_scraped_count", 0),
+            "info_count": text.get("log_count_INFO", 0),
+            "warning_count": text.get("log_count_WARNING", 0),
+            "error_count": text.get("log_count_ERROR", 0),
+            "start_time": text.get("start_time"),
+            "finish_time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            "spend_minutes": round(
+                (_curr_utc_time - stats.get("start_time")).seconds / 60, 2
+            ),
+            "crawl_time": crawl_time,
+        }
+
+        # 错误原因
+        if text.get("log_count_ERROR", 0):
+            log_info["log_count_ERROR"] = error_reason or "请人工排查错误原因！"
+
+        else:
+            log_info["log_count_ERROR"] = ""
+        return log_info
+
+
+class PostgreSQLPipeEnhanceMixin:
+    """扩展 postgresql pipelines 的功能"""
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def _connect(
+        self,
+        postgres_conf: "PostgreSQLConf",
+    ) -> "PsycopgConnection":
+        """链接数据库操作：
+            1.如果链接正常，则返回链接句柄；
+            2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
+
+        Args:
+            postgres_conf: postgresql 链接所需的参数
+
+        Returns:
+            1). postgresql 链接句柄
+        """
+        try:
+            conn = psycopg.connect(
+                user=postgres_conf.user,
+                password=postgres_conf.password,
+                host=postgres_conf.host,
+                port=postgres_conf.port,
+                dbname=postgres_conf.database,
+            )
+        except Exception as e:
+            # err: connection to server at "x.x.x.x", port x failed: FATAL:  database "x" does not exist
+            if "failed" in str(e).lower():
+                logger.warning(
+                    f"目标数据库：{postgres_conf.database} 不存在，尝试创建中..."
+                )
+                ReuseOperation.create_database(db_conf=postgres_conf)
+            else:
+                logger.error(f"connect to postgresql failed: {e}")
+        else:
+            return conn
+
+        return psycopg.connect(
+            user=postgres_conf.user,
+            password=postgres_conf.password,
+            host=postgres_conf.host,
+            port=postgres_conf.port,
+            dbname=postgres_conf.database,
+        )
+
+    def _get_sql_by_item(self, table: str, item: dict) -> str:
+        """根据处理后的 item 生成 postgresql 插入语句
+
+        Args:
+            table: 数据库表名
+            item: 处理后的 item
+
+        Returns:
+            1). sql 插入语句
+        """
+        keys = f"""{", ".join(item.keys())}"""
+        values = ", ".join(["%s"] * len(item))
+        return f"INSERT INTO {table} ({keys}) values ({values});"
+
+
+class OraclePipeEnhanceMixin:
+    """扩展 oracle pipelines 的功能"""
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def _connect(
+        self,
+        oracle_conf: "OracleConf",
+    ) -> "OracleConnection":
+        """链接数据库返回链接句柄
+
+        Args:
+            oracle_conf: oracle 链接所需的参数
+
+        Returns:
+            1). oracle 链接句柄
+        """
+        if oracle_thick_lib_dir := oracle_conf.thick_lib_dir:
+            oracledb.init_oracle_client(oracle_thick_lib_dir)
+
+        return oracledb.connect(
+            user=oracle_conf.user,
+            password=oracle_conf.password,
+            host=oracle_conf.host,
+            port=oracle_conf.port,
+            service_name=oracle_conf.service_name,
+            encoding=oracle_conf.encoding,
+        )
+
+    def _get_sql_by_item(self, table: str, item: dict) -> str:
+        """根据处理后的 item 生成 oracle 插入语句
+
+        Args:
+            table: 数据库表名
+            item: 处理后的 item
+
+        Returns:
+            1). sql 插入语句
+        """
+        keys = f""":{", :".join(item.keys())}"""
+        table_keys = ", ".join(map(lambda key: f'"{key}"', item.keys()))
+        return f'INSERT INTO "{table}" ({table_keys}) values ({keys})'
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.9.8/ayugespidertools/common/mongodbpipe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,193 @@
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Optional, Tuple, TypeVar
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-
-__all__ = [
-    "Synchronize",
-    "TwistedAsynchronous",
-    "AsyncioAsynchronous",
-    "mongodb_pipe",
-]
-
-if TYPE_CHECKING:
-    from motor.core import AgnosticDatabase
-    from pymongo.database import Database
-
-    PymongoDataBaseT = TypeVar("PymongoDataBaseT", Database, AgnosticDatabase)
-
-
-class AbstractClass(ABC):
-    """用于处理 mongodb pipeline 存储的模板方法类"""
-
-    def _get_insert_data(self, item_dict: dict) -> Tuple[dict, str]:
-        """获取要插入的数据，将 item 中的存储数据提取出来
-
-        Args:
-            item_dict: item 的 dict 类型
-
-        Returns:
-            insert_data: 返回 dict 格式的存储数据
-            table_name: item_dict 对应的 table
-        """
-        insert_data = ReuseOperation.get_items_except_keys(
-            dict_conf=item_dict,
-            keys=["_table", "_mongo_update_rule"],
-        )
-        table_name = item_dict["_table"]
-        judge_item = next(iter(insert_data.values()))
-        # 是 namedtuple 类型
-        if ReuseOperation.is_namedtuple_instance(judge_item):
-            insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
-            table_name = item_dict["_table"].key_value
-        # 是普通的 dict 格式，则直接为 insert_data
-        return insert_data, table_name
-
-    def process_item_template(
-        self,
-        item_dict: dict,
-        db: "PymongoDataBaseT",
-        sys_ver_low: Optional[bool] = None,
-    ):
-        """模板方法，用于处理 mongodb pipeline 存储的模板方法类
-
-        Args:
-            item_dict: item 的 dict 类型
-            db: mongodb 数据库连接
-            sys_ver_low: 是否是 py3.11 以下
-        """
-        insert_data, table_name = self._get_insert_data(item_dict)
-        self._data_storage_logic(
-            db=db,
-            item_dict=item_dict,
-            collection_name=table_name,
-            insert_data=insert_data,
-            sys_ver_low=sys_ver_low,
-        )
-
-    def _default_storage(
-        self,
-        db: "PymongoDataBaseT",
-        item_dict: dict,
-        collection_name: str,
-        insert_data: dict,
-        sys_ver_low: Optional[bool] = None,
-    ):
-        if sys_ver_low:
-            # 如果没有查重字段时，就直接插入数据（不去重）
-            if not item_dict.get("_mongo_update_rule"):
-                db[collection_name].insert(insert_data)
-            else:
-                db[collection_name].update(
-                    item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-                )
-        else:
-            if not item_dict.get("_mongo_update_rule"):
-                db[collection_name].insert_one(insert_data)
-            else:
-                db[collection_name].update_many(
-                    item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-                )
-
-    @abstractmethod
-    def _data_storage_logic(
-        self,
-        db: "PymongoDataBaseT",
-        item_dict: dict,
-        collection_name: str,
-        insert_data: dict,
-        sys_ver_low: Optional[bool] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        """数据存储逻辑，需要子类实现
-
-        Args:
-            db: mongodb 数据库连接
-            item_dict: item 的 dict 类型
-            collection_name: 集合名称
-            insert_data: 要插入的数据
-            *args: 可变参数
-            **kwargs:关键字参数
-        """
-        pass
-
-
-class Synchronize(AbstractClass):
-    """pipeline 同步执行 mongodb 存储的场景"""
-
-    def _data_storage_logic(
-        self,
-        db: "PymongoDataBaseT",
-        item_dict: dict,
-        collection_name: str,
-        insert_data: dict,
-        sys_ver_low: Optional[bool] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        self._default_storage(db, item_dict, collection_name, insert_data, sys_ver_low)
-
-
-class TwistedAsynchronous(AbstractClass):
-    """pipeline twisted 异步执行 mongodb 存储的场景"""
-
-    def _data_storage_logic(
-        self,
-        db: "PymongoDataBaseT",
-        item_dict: dict,
-        collection_name: str,
-        insert_data: dict,
-        sys_ver_low: Optional[bool] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        self._default_storage(db, item_dict, collection_name, insert_data, sys_ver_low)
-
-
-class AsyncioAsynchronous(AbstractClass):
-    """pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现"""
-
-    async def _data_storage_logic(  # type: ignore[override]
-        self,
-        db: "PymongoDataBaseT",
-        item_dict: dict,
-        collection_name: str,
-        insert_data: dict,
-        sys_ver_low: Optional[bool] = None,
-        *args,
-        **kwargs,
-    ):  # @override to fix mypy [override] error.
-        if not item_dict.get("_mongo_update_rule"):
-            await db[collection_name].insert_one(insert_data)
-        else:
-            await db[collection_name].update_many(
-                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-            )
-
-    async def process_item_template(
-        self,
-        item_dict: dict,
-        db: "PymongoDataBaseT",
-        sys_ver_low: Optional[bool] = None,
-    ):
-        insert_data, table_name = self._get_insert_data(item_dict)
-        await self._data_storage_logic(
-            db=db,
-            item_dict=item_dict,
-            collection_name=table_name,
-            insert_data=insert_data,
-        )
-
-
-def mongodb_pipe(
-    abstract_class: AbstractClass,
-    item_dict: dict,
-    db: "PymongoDataBaseT",
-    sys_ver_low: bool = True,
-) -> None:
-    """mongodb pipeline 存储的通用调用方法"""
-    abstract_class.process_item_template(item_dict, db, sys_ver_low)
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Optional, Tuple, TypeVar
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+__all__ = [
+    "Synchronize",
+    "TwistedAsynchronous",
+    "AsyncioAsynchronous",
+    "mongodb_pipe",
+]
+
+if TYPE_CHECKING:
+    from motor.core import AgnosticDatabase
+    from pymongo.database import Database
+
+    PymongoDataBaseT = TypeVar("PymongoDataBaseT", Database, AgnosticDatabase)
+
+
+class AbstractClass(ABC):
+    """用于处理 mongodb pipeline 存储的模板方法类"""
+
+    def _get_insert_data(self, item_dict: dict) -> Tuple[dict, str]:
+        """获取要插入的数据，将 item 中的存储数据提取出来
+
+        Args:
+            item_dict: item 的 dict 类型
+
+        Returns:
+            insert_data: 返回 dict 格式的存储数据
+            table_name: item_dict 对应的 table
+        """
+        insert_data = ReuseOperation.get_items_except_keys(
+            dict_conf=item_dict,
+            keys=["_table", "_mongo_update_rule"],
+        )
+        table_name = item_dict["_table"]
+        judge_item = next(iter(insert_data.values()))
+        if ReuseOperation.is_namedtuple_instance(judge_item):
+            insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
+            table_name = item_dict["_table"].key_value
+        return insert_data, table_name
+
+    def process_item_template(
+        self,
+        item_dict: dict,
+        db: "PymongoDataBaseT",
+        pymongo_ver_low: Optional[bool] = None,
+    ):
+        """模板方法，用于处理 mongodb pipeline 存储的模板方法类
+
+        Args:
+            item_dict: item 的 dict 类型
+            db: mongodb 数据库连接
+            pymongo_ver_low: pymongo 版本是否 4.0 以下
+        """
+        insert_data, table_name = self._get_insert_data(item_dict)
+        self._data_storage_logic(
+            db=db,
+            item_dict=item_dict,
+            collection_name=table_name,
+            insert_data=insert_data,
+            pymongo_ver_low=pymongo_ver_low,
+        )
+
+    def _default_storage(
+        self,
+        db: "PymongoDataBaseT",
+        item_dict: dict,
+        collection_name: str,
+        insert_data: dict,
+        pymongo_ver_low: Optional[bool] = None,
+    ):
+        if pymongo_ver_low:
+            # 如果没有查重字段时，就直接插入数据（不去重）
+            if not item_dict.get("_mongo_update_rule"):
+                db[collection_name].insert(insert_data)
+            else:
+                db[collection_name].update(
+                    item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+                )
+        else:
+            if not item_dict.get("_mongo_update_rule"):
+                db[collection_name].insert_one(insert_data)
+            else:
+                db[collection_name].update_many(
+                    item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+                )
+
+    @abstractmethod
+    def _data_storage_logic(
+        self,
+        db: "PymongoDataBaseT",
+        item_dict: dict,
+        collection_name: str,
+        insert_data: dict,
+        pymongo_ver_low: Optional[bool] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        """数据存储逻辑，需要子类实现
+
+        Args:
+            db: mongodb 数据库连接
+            item_dict: item 的 dict 类型
+            collection_name: 集合名称
+            insert_data: 要插入的数据
+            pymongo_ver_low: pymongo 版本是否小于 4.0
+            *args: 可变参数
+            **kwargs:关键字参数
+        """
+        pass
+
+
+class Synchronize(AbstractClass):
+    """pipeline 同步执行 mongodb 存储的场景"""
+
+    def _data_storage_logic(
+        self,
+        db: "PymongoDataBaseT",
+        item_dict: dict,
+        collection_name: str,
+        insert_data: dict,
+        pymongo_ver_low: Optional[bool] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        self._default_storage(
+            db, item_dict, collection_name, insert_data, pymongo_ver_low
+        )
+
+
+class TwistedAsynchronous(AbstractClass):
+    """pipeline twisted 异步执行 mongodb 存储的场景"""
+
+    def _data_storage_logic(
+        self,
+        db: "PymongoDataBaseT",
+        item_dict: dict,
+        collection_name: str,
+        insert_data: dict,
+        pymongo_ver_low: Optional[bool] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        self._default_storage(
+            db, item_dict, collection_name, insert_data, pymongo_ver_low
+        )
+
+
+class AsyncioAsynchronous(AbstractClass):
+    """pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现"""
+
+    async def _data_storage_logic(  # type: ignore[override]
+        self,
+        db: "PymongoDataBaseT",
+        item_dict: dict,
+        collection_name: str,
+        insert_data: dict,
+        pymongo_ver_low: Optional[bool] = None,
+        *args,
+        **kwargs,
+    ):  # @override to fix mypy [override] error.
+        if not item_dict.get("_mongo_update_rule"):
+            await db[collection_name].insert_one(insert_data)
+        else:
+            await db[collection_name].update_many(
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+            )
+
+    async def process_item_template(
+        self,
+        item_dict: dict,
+        db: "PymongoDataBaseT",
+        pymongo_ver_low: Optional[bool] = None,
+    ):
+        insert_data, table_name = self._get_insert_data(item_dict)
+        await self._data_storage_logic(
+            db=db,
+            item_dict=item_dict,
+            collection_name=table_name,
+            insert_data=insert_data,
+        )
+
+
+def mongodb_pipe(
+    abstract_class: AbstractClass,
+    item_dict: dict,
+    db: "PymongoDataBaseT",
+    pymongo_ver_low: bool = True,
+) -> None:
+    """mongodb pipeline 存储的通用调用方法"""
+    abstract_class.process_item_template(item_dict, db, pymongo_ver_low)
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.9.8/ayugespidertools/common/multiplexing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,529 +1,512 @@
-import configparser
-import json
-import os
-import random
-from typing import TYPE_CHECKING, Any, Dict, List, Union
-
-import pymysql
-from itemadapter import ItemAdapter
-
-from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import (
-    AlterItem,
-    AlterItemTable,
-    MysqlConf,
-    PostgreSQLConf,
-)
-from ayugespidertools.config import logger
-from ayugespidertools.items import AyuItem
-
-try:
-    import psycopg
-except ImportError:
-    # pip install ayugespidertools[database]
-    pass
-
-__all__ = [
-    "ReuseOperation",
-]
-
-if TYPE_CHECKING:
-    from pathlib import Path
-
-    from scrapy.settings import BaseSettings
-
-
-class ReuseOperation:
-    """用于存放经常复用的一些操作"""
-
-    @staticmethod
-    def fetch_local_conf(vit_dir: Union[str, "Path"], inner_settings: dict) -> dict:
-        """通过本地 VIT 中的 .conf 获取所需配置，并将其添加到 inner_settings
-
-        Args:
-            vit_dir: 配置文件所在的目录
-            inner_settings: inner_settings 配置
-
-        Returns:
-            inner_settings: 本库所需的配置
-        """
-        cfg = configparser.ConfigParser()
-        cfg.read(f"{vit_dir}/.conf", encoding="utf-8")
-        if "mysql" in cfg:
-            mysql_section = cfg["mysql"]
-            _charset = mysql_section.get("charset", "utf8mb4")
-            inner_settings["MYSQL_CONFIG"] = {
-                "host": mysql_section.get("host", "localhost"),
-                "port": mysql_section.getint("port", 3306),
-                "user": mysql_section.get("user", ""),
-                "password": mysql_section.get("password", ""),
-                "charset": _charset,
-                "database": mysql_section.get("database", ""),
-                "engine": mysql_section.get("engine", "InnoDB"),
-                "collate": mysql_section.get(
-                    "collate",
-                    Param.charset_collate_map.get(_charset, "utf8mb4_general_ci"),
-                ),
-                "odku_enable": mysql_section.getboolean("odku_enable", False),
-            }
-        if "mongodb:uri" in cfg:
-            inner_settings["MONGODB_CONFIG"] = {
-                "uri": cfg.get("mongodb:uri", "uri", fallback=None)
-            }
-        elif "mongodb" in cfg:
-            mongodb_section = cfg["mongodb"]
-            inner_settings["MONGODB_CONFIG"] = {
-                "host": mongodb_section.get("host", "localhost"),
-                "port": mongodb_section.getint("port", 27017),
-                "authsource": mongodb_section.get("authsource", "admin"),
-                "authMechanism": mongodb_section.get("authMechanism", "SCRAM-SHA-1"),
-                "user": mongodb_section.get("user", "admin"),
-                "password": mongodb_section.get("password", None),
-                "database": mongodb_section.get("database", None),
-            }
-        if "postgresql" in cfg:
-            postgres_section = cfg["postgresql"]
-            inner_settings["POSTGRESQL_CONFIG"] = {
-                "host": postgres_section.get("host", "localhost"),
-                "port": postgres_section.getint("port", 5432),
-                "user": postgres_section.get("user", "postgres"),
-                "password": postgres_section.get("password", ""),
-                "database": postgres_section.get("database", ""),
-                "charset": postgres_section.get("charset", "UTF8"),
-            }
-        if "elasticsearch" in cfg:
-            es_section = cfg["elasticsearch"]
-            inner_settings["ES_CONFIG"] = {
-                "hosts": es_section.get("hosts", None),
-                "index_class": json.loads(
-                    es_section.get(
-                        "index_class", '{"settings":{"number_of_shards": 2}}'
-                    )
-                ),
-                "user": es_section.get("user", None),
-                "password": es_section.get("password", None),
-                "init": es_section.getboolean("init", False),
-                "verify_certs": es_section.getboolean("verify_certs", False),
-                "ca_certs": es_section.get("ca_certs", None),
-                "client_cert": es_section.get("client_cert", None),
-                "client_key": es_section.get("client_key", None),
-                "ssl_assert_fingerprint": es_section.get(
-                    "ssl_assert_fingerprint", None
-                ),
-            }
-        if "oracle" in cfg:
-            oracle_section = cfg["oracle"]
-            inner_settings["ORACLE_CONFIG"] = {
-                "host": oracle_section.get("host", "localhost"),
-                "port": oracle_section.getint("port", 1521),
-                "user": oracle_section.get("user", None),
-                "password": oracle_section.get("password", None),
-                "service_name": oracle_section.get("service_name", None),
-                "encoding": oracle_section.get("encoding", "utf8"),
-                "thick_lib_dir": oracle_section.get("thick_lib_dir", False),
-            }
-        if "consul" in cfg:
-            consul_section = cfg["consul"]
-            inner_settings["REMOTE_CONFIG"] = {
-                "token": consul_section.get("token", None),
-                "url": consul_section.get("url", None),
-                "format": consul_section.get("format", "json"),
-                "remote_type": "consul",
-            }
-        elif "nacos" in cfg:
-            nacos_section = cfg["nacos"]
-            inner_settings["REMOTE_CONFIG"] = {
-                "token": nacos_section.get("token", None),
-                "url": nacos_section.get("url", None),
-                "format": nacos_section.get("format", "json"),
-                "remote_type": "nacos",
-            }
-        if "kdl_dynamic_proxy" in cfg:
-            kdl_dynamic_section = cfg["kdl_dynamic_proxy"]
-            inner_settings["DYNAMIC_PROXY_CONFIG"] = {
-                "proxy": kdl_dynamic_section.get("proxy", None),
-                "username": kdl_dynamic_section.get("username", None),
-                "password": kdl_dynamic_section.get("password", None),
-            }
-        if "kdl_exclusive_proxy" in cfg:
-            kdl_exclusive_section = cfg["kdl_exclusive_proxy"]
-            inner_settings["EXCLUSIVE_PROXY_CONFIG"] = {
-                "proxy": kdl_exclusive_section.get("proxy", None),
-                "username": kdl_exclusive_section.get("username", None),
-                "password": kdl_exclusive_section.get("password", None),
-                "index": kdl_exclusive_section.getint("index", 1),
-            }
-        if "mq" in cfg:
-            mq_section = cfg["mq"]
-            inner_settings["MQ_CONFIG"] = {
-                "host": mq_section.get("host", "localhost"),
-                "port": mq_section.getint("port", 5672),
-                "username": mq_section.get("username", "guest"),
-                "password": mq_section.get("password", "guest"),
-                "virtualhost": mq_section.get("virtualhost", "/"),
-                "heartbeat": mq_section.getint("heartbeat", 0),
-                "socket_timeout": mq_section.getint("socket_timeout", 1),
-                "queue": mq_section.get("queue", None),
-                "durable": mq_section.getboolean("durable", True),
-                "exclusive": mq_section.getboolean("exclusive", False),
-                "auto_delete": mq_section.getboolean("auto_delete", False),
-                "exchange": mq_section.get("exchange", None),
-                "routing_key": mq_section.get("routing_key", None),
-                "content_type": mq_section.getint("content_type", "text/plain"),
-                "delivery_mode": mq_section.getint("delivery_mode", 1),
-                "mandatory": mq_section.getboolean("mandatory", True),
-            }
-        if "kafka" in cfg:
-            kafka_section = cfg["kafka"]
-            inner_settings["KAFKA_CONFIG"] = {
-                "bootstrap_servers": kafka_section.get(
-                    "bootstrap_servers", "127.0.0.1:9092"
-                ),
-                "topic": kafka_section.get("topic", None),
-                "key": kafka_section.get("key", None),
-            }
-        if "oss:ali" in cfg:
-            oss_section = cfg["oss:ali"]
-            inner_settings["OSS_CONFIG"] = {
-                "access_key": oss_section.get("access_key", None),
-                "access_secret": oss_section.get("access_secret", None),
-                "endpoint": oss_section.get("endpoint", None),
-                "bucket": oss_section.get("bucket", None),
-                "doc": oss_section.get("doc", None),
-                "upload_fields_suffix": oss_section.get(
-                    "upload_fields_suffix", "_file_url"
-                ),
-                "oss_fields_prefix": oss_section.get("oss_fields_prefix", "_"),
-                "full_link_enable": oss_section.getboolean("full_link_enable", False),
-            }
-        return inner_settings
-
-    @staticmethod
-    def item_to_dict(item: Union[AyuItem, dict]) -> dict:
-        """将 item 转换为 dict 类型；
-        将 spider 中的 yield 的 item 转换为 dict 类型，方便后续处理
-
-        Args:
-            item: spider 中的 yield 的 item
-
-        Returns:
-            1). dict 类型的 item
-        """
-        return (
-            item.asdict() if isinstance(item, AyuItem) else ItemAdapter(item).asdict()
-        )
-
-    @classmethod
-    def reshape_item(cls, item_dict: Dict[str, Any]) -> AlterItem:
-        """重新整合 item
-
-        Args:
-            item_dict: dict 类型的 item
-
-        Returns:
-            1). 整合后的 item
-        """
-        new_item = {}
-        notes_dic = {}
-        is_namedtuple = False
-
-        insert_data = cls.get_items_except_keys(
-            dict_conf=item_dict, keys=["_mongo_update_rule", "_table"]
-        )
-        judge_item = next(iter(insert_data.values()))
-        # 是 namedtuple 类型
-        if cls.is_namedtuple_instance(judge_item):
-            is_namedtuple = True
-            _table_name = item_dict["_table"].key_value
-            _table_notes = item_dict["_table"].notes
-            table_info = AlterItemTable(_table_name, _table_notes)
-            for key, value in insert_data.items():
-                new_item[key] = value.key_value
-                notes_dic[key] = value.notes
-        # 是普通的 dict 类型
-        else:
-            _table_name = item_dict["_table"]
-            table_info = AlterItemTable(_table_name, "")
-            for key, value in insert_data.items():
-                new_item[key] = value
-                notes_dic[key] = ""
-
-        return AlterItem(new_item, notes_dic, table_info, is_namedtuple)
-
-    @staticmethod
-    def is_namedtuple_instance(x: Any) -> bool:
-        """判断 x 是否为 namedtuple 类型
-
-        Args:
-            x: 需要判断的参数
-
-        Returns:
-            1). 是否符合 namedtuple 类型
-        """
-        return isinstance(x, tuple) and hasattr(x, "_fields")
-
-    @staticmethod
-    def get_files_from_path(path: str) -> list:
-        """获取 path 文件夹下的所有文件，并输出以 path 为根目录的相对路径
-
-        Args:
-            path: 需要判断的文件夹路径
-
-        Returns:
-            1). path 文件夹下的文件列表
-        """
-        return [f.path for f in os.scandir(path) if f.is_file()]
-
-    @staticmethod
-    def random_weight(weight_data: list):
-        """带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
-
-        Args:
-            weight_data: 带权重的列表信息，示例：
-                [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
-
-        Returns:
-            ret: 返回当前权重列表 account_arr 中的一个值
-        """
-        total = sum(item["weight"] for item in weight_data)
-        # 在 0 与权重和之间获取一个随机数
-        ra = random.uniform(0, total)
-        curr_sum = 0
-        ret = None
-        for data in weight_data:
-            # 在遍历中，累加当前权重值
-            curr_sum += data["weight"]
-            # 当随机数 <= 当前权重和时，返回权重 key
-            if ra <= curr_sum:
-                ret = data
-                break
-        return ret
-
-    @classmethod
-    def is_dict_meet_min_limit(cls, dict_conf: dict, key_list: List[str]) -> bool:
-        """判断 dict_conf 是否满足 key_list 中的 key 值限定
-
-        Args:
-            dict_conf: 需要判断的参数
-            key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
-
-        Returns:
-            1). 是否满足 key 值限制
-        """
-        if any([not dict_conf, not isinstance(dict_conf, dict)]):
-            return False
-
-        return all(key in dict_conf for key in key_list)
-
-    @classmethod
-    def get_items_by_keys(
-        cls,
-        dict_conf: dict,
-        keys: List[str],
-    ) -> dict:
-        """获取 dict_conf 中的含有 keys 的 key 的字段
-
-        Args:
-            dict_conf: 需要处理的参数
-            keys: 需要取的 key 值列表
-
-        Returns:
-            1). 取值后的 dict，或不满足请求的 False 值
-        """
-        # 参数先要满足最小限定，然后再取出限定的参数值；否则返回空字典
-        return (
-            {k: dict_conf[k] for k in keys}
-            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=keys)
-            else {}
-        )
-
-    @classmethod
-    def get_items_except_keys(cls, dict_conf, keys: List[str]) -> dict:
-        """获取 dict_conf 中的不含有 keys 的 key 的字段
-
-        Args:
-            dict_conf: 需要处理的参数
-            keys: 需要排除的 key 值列表
-
-        Returns:
-            1). dict_conf 排除 keys 中的键值后的值
-        """
-        return {k: dict_conf[k] for k in dict_conf if k not in keys}
-
-    @classmethod
-    def create_database(cls, db_conf: Union[MysqlConf, PostgreSQLConf]) -> None:
-        """创建数据库：由于这是在连接数据库，报数据库不存在错误时的场景，则需要
-        新建(不指定数据库)连接创建好所需数据库即可
-
-        Args:
-            db_conf: 数据库连接配置，目前支持 mysql 和 postgresql
-        """
-        if isinstance(db_conf, MysqlConf):
-            with pymysql.connect(
-                user=db_conf.user,
-                password=db_conf.password,
-                host=db_conf.host,
-                port=db_conf.port,
-                charset=db_conf.charset,
-            ) as conn:
-                with conn.cursor() as cur:
-                    cur.execute(
-                        f"CREATE DATABASE IF NOT EXISTS `{db_conf.database}` character set {db_conf.charset};"
-                    )
-
-        elif isinstance(db_conf, PostgreSQLConf):
-            with psycopg.connect(
-                user=db_conf.user,
-                password=db_conf.password,
-                host=db_conf.host,
-                port=db_conf.port,
-            ) as conn:
-                with conn.cursor() as cur:
-                    conn.autocommit = True
-                    cur.execute(
-                        f"CREATE DATABASE {db_conf.database} WITH ENCODING {db_conf.charset};"
-                    )
-
-        else:
-            assert False, f"Invalid db_conf type: {type(db_conf)}"
-        logger.info(
-            f"创建数据库 {db_conf.database} 成功，其 charset 类型是：{db_conf.charset}!"
-        )
-
-    @classmethod
-    def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
-        """将 dict 中 str 类型的 key 值变成小写
-
-        Args:
-            deal_dict: 需要处理的 dict
-
-        Returns:
-            1).处理后的 dict 值
-        """
-        key_to_lower_dict = {}
-        for key, value in deal_dict.items():
-            if isinstance(value, dict):
-                if isinstance(key, str):
-                    key_to_lower_dict[key.lower()] = cls.dict_keys_to_lower(value)
-                else:
-                    key_to_lower_dict[key] = cls.dict_keys_to_lower(value)
-            elif isinstance(key, str):
-                key_to_lower_dict[key.lower()] = value
-            else:
-                key_to_lower_dict[key] = value
-        return key_to_lower_dict
-
-    @classmethod
-    def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
-        """将 dict 中 str 类型的 key 值变成大写
-
-        Args:
-            deal_dict: 需要处理的 dict
-
-        Returns:
-            1).处理后的 dict 值
-        """
-        key_to_upper_dict = {}
-        for key, value in deal_dict.items():
-            if isinstance(value, dict):
-                if isinstance(key, str):
-                    key_to_upper_dict[key.upper()] = cls.dict_keys_to_upper(value)
-                else:
-                    key_to_upper_dict[key] = cls.dict_keys_to_upper(value)
-            elif isinstance(key, str):
-                key_to_upper_dict[key.upper()] = value
-            else:
-                key_to_upper_dict[key] = value
-        return key_to_upper_dict
-
-    @classmethod
-    def get_remote_option(cls, settings: "BaseSettings") -> dict:
-        """获取项目中 consul 或 nacos 的链接配置
-
-        Args:
-            settings: scrapy 的 settings 信息
-
-        Returns:
-            1). 满足最少要求的远程配置
-        """
-        consul_conf_dict = settings.get("REMOTE_CONFIG", {})
-        return cls.get_items_by_keys(
-            dict_conf=consul_conf_dict, keys=["token", "url", "format", "remote_type"]
-        )
-
-    @classmethod
-    def judge_str_is_json(cls, judge_str: str) -> bool:
-        """判断字符串是否为 json 格式
-
-        Args:
-            judge_str: 需要判断的字符串
-
-        Returns:
-            1). 是否为 json 格式
-        """
-        if not isinstance(judge_str, str):
-            return False
-
-        try:
-            json.loads(judge_str)
-        except Exception:
-            return False
-        else:
-            return True
-
-    @staticmethod
-    def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
-        """从 headers 中的 ck str 格式转化为 dict 格式
-
-        Args:
-            headers_ck_str: request headers ck 的 str 格式
-
-        Returns:
-            1). 转化 dict 格式后的 ck
-        """
-        # 也可以这样写，但不推荐
-        # dict(line.split("=", 1) for line in headers_ck_str.split("; "))
-        return {
-            x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
-            for x in headers_ck_str.split(";")
-        }
-
-    @staticmethod
-    def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
-        """将 scrapy 请求中的 body 对象转为 dict 格式
-
-        Args:
-            req_body_data_str: scrapy 中的 body 参数
-
-        Returns:
-            1). 转化 dict 格式后的 body
-        """
-        return {
-            x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
-        }
-
-    @classmethod
-    def get_array_depth(cls, array: list) -> int:
-        """获取 array 的最大层级，深度
-
-        Args:
-            array: 数组
-
-        Returns:
-            1). 最大层级，深度
-        """
-
-        """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
-        # 先判断是否为数组类型的元素
-        judge_array = isinstance(
-            array,
-            (
-                frozenset,
-                list,
-                set,
-                tuple,
-            ),
-        )
-        return (
-            int(judge_array) and len(array) and 1 + max(map(cls.get_array_depth, array))
-        )
+import configparser
+import json
+import random
+from typing import TYPE_CHECKING, Any, Dict, List, Union
+
+import pymysql
+from itemadapter import ItemAdapter
+
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import (
+    AlterItem,
+    AlterItemTable,
+    MysqlConf,
+    PostgreSQLConf,
+)
+from ayugespidertools.config import logger
+from ayugespidertools.items import AyuItem
+
+try:
+    import psycopg
+except ImportError:
+    # pip install ayugespidertools[database]
+    pass
+
+__all__ = [
+    "ReuseOperation",
+]
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from scrapy.settings import BaseSettings
+
+
+class ReuseOperation:
+    """用于存放经常复用的一些操作"""
+
+    @staticmethod
+    def fetch_local_conf(vit_dir: Union[str, "Path"], inner_settings: dict) -> dict:
+        """通过本地 VIT 中的 .conf 获取所需配置，并将其添加到 inner_settings
+
+        Args:
+            vit_dir: 配置文件所在的目录
+            inner_settings: inner_settings 配置
+
+        Returns:
+            inner_settings: 本库所需的配置
+        """
+        cfg = configparser.ConfigParser()
+        cfg.read(f"{vit_dir}/.conf", encoding="utf-8")
+        if "mysql" in cfg:
+            mysql_section = cfg["mysql"]
+            _charset = mysql_section.get("charset", "utf8mb4")
+            inner_settings["MYSQL_CONFIG"] = {
+                "host": mysql_section.get("host", "localhost"),
+                "port": mysql_section.getint("port", 3306),
+                "user": mysql_section.get("user", ""),
+                "password": mysql_section.get("password", ""),
+                "charset": _charset,
+                "database": mysql_section.get("database", ""),
+                "engine": mysql_section.get("engine", "InnoDB"),
+                "collate": mysql_section.get(
+                    "collate",
+                    Param.charset_collate_map.get(_charset, "utf8mb4_general_ci"),
+                ),
+                "odku_enable": mysql_section.getboolean("odku_enable", False),
+            }
+        if "mongodb:uri" in cfg:
+            inner_settings["MONGODB_CONFIG"] = {
+                "uri": cfg.get("mongodb:uri", "uri", fallback=None)
+            }
+        elif "mongodb" in cfg:
+            mongodb_section = cfg["mongodb"]
+            inner_settings["MONGODB_CONFIG"] = {
+                "host": mongodb_section.get("host", "localhost"),
+                "port": mongodb_section.getint("port", 27017),
+                "authsource": mongodb_section.get("authsource", "admin"),
+                "authMechanism": mongodb_section.get("authMechanism", "SCRAM-SHA-1"),
+                "user": mongodb_section.get("user", "admin"),
+                "password": mongodb_section.get("password", None),
+                "database": mongodb_section.get("database", None),
+            }
+        if "postgresql" in cfg:
+            postgres_section = cfg["postgresql"]
+            inner_settings["POSTGRESQL_CONFIG"] = {
+                "host": postgres_section.get("host", "localhost"),
+                "port": postgres_section.getint("port", 5432),
+                "user": postgres_section.get("user", "postgres"),
+                "password": postgres_section.get("password", ""),
+                "database": postgres_section.get("database", ""),
+                "charset": postgres_section.get("charset", "UTF8"),
+            }
+        if "elasticsearch" in cfg:
+            es_section = cfg["elasticsearch"]
+            inner_settings["ES_CONFIG"] = {
+                "hosts": es_section.get("hosts", None),
+                "index_class": json.loads(
+                    es_section.get(
+                        "index_class", '{"settings":{"number_of_shards": 2}}'
+                    )
+                ),
+                "user": es_section.get("user", None),
+                "password": es_section.get("password", None),
+                "init": es_section.getboolean("init", False),
+                "verify_certs": es_section.getboolean("verify_certs", False),
+                "ca_certs": es_section.get("ca_certs", None),
+                "client_cert": es_section.get("client_cert", None),
+                "client_key": es_section.get("client_key", None),
+                "ssl_assert_fingerprint": es_section.get(
+                    "ssl_assert_fingerprint", None
+                ),
+            }
+        if "oracle" in cfg:
+            oracle_section = cfg["oracle"]
+            inner_settings["ORACLE_CONFIG"] = {
+                "host": oracle_section.get("host", "localhost"),
+                "port": oracle_section.getint("port", 1521),
+                "user": oracle_section.get("user", None),
+                "password": oracle_section.get("password", None),
+                "service_name": oracle_section.get("service_name", None),
+                "encoding": oracle_section.get("encoding", "utf8"),
+                "thick_lib_dir": oracle_section.get("thick_lib_dir", False),
+            }
+        if "consul" in cfg:
+            consul_section = cfg["consul"]
+            inner_settings["REMOTE_CONFIG"] = {
+                "token": consul_section.get("token", None),
+                "url": consul_section.get("url", None),
+                "format": consul_section.get("format", "json"),
+                "remote_type": "consul",
+            }
+        elif "nacos" in cfg:
+            nacos_section = cfg["nacos"]
+            inner_settings["REMOTE_CONFIG"] = {
+                "token": nacos_section.get("token", None),
+                "url": nacos_section.get("url", None),
+                "format": nacos_section.get("format", "json"),
+                "remote_type": "nacos",
+            }
+        if "kdl_dynamic_proxy" in cfg:
+            kdl_dynamic_section = cfg["kdl_dynamic_proxy"]
+            inner_settings["DYNAMIC_PROXY_CONFIG"] = {
+                "proxy": kdl_dynamic_section.get("proxy", None),
+                "username": kdl_dynamic_section.get("username", None),
+                "password": kdl_dynamic_section.get("password", None),
+            }
+        if "kdl_exclusive_proxy" in cfg:
+            kdl_exclusive_section = cfg["kdl_exclusive_proxy"]
+            inner_settings["EXCLUSIVE_PROXY_CONFIG"] = {
+                "proxy": kdl_exclusive_section.get("proxy", None),
+                "username": kdl_exclusive_section.get("username", None),
+                "password": kdl_exclusive_section.get("password", None),
+                "index": kdl_exclusive_section.getint("index", 1),
+            }
+        if "mq" in cfg:
+            mq_section = cfg["mq"]
+            inner_settings["MQ_CONFIG"] = {
+                "host": mq_section.get("host", "localhost"),
+                "port": mq_section.getint("port", 5672),
+                "username": mq_section.get("username", "guest"),
+                "password": mq_section.get("password", "guest"),
+                "virtualhost": mq_section.get("virtualhost", "/"),
+                "heartbeat": mq_section.getint("heartbeat", 0),
+                "socket_timeout": mq_section.getint("socket_timeout", 1),
+                "queue": mq_section.get("queue", None),
+                "durable": mq_section.getboolean("durable", True),
+                "exclusive": mq_section.getboolean("exclusive", False),
+                "auto_delete": mq_section.getboolean("auto_delete", False),
+                "exchange": mq_section.get("exchange", None),
+                "routing_key": mq_section.get("routing_key", None),
+                "content_type": mq_section.getint("content_type", "text/plain"),
+                "delivery_mode": mq_section.getint("delivery_mode", 1),
+                "mandatory": mq_section.getboolean("mandatory", True),
+            }
+        if "kafka" in cfg:
+            kafka_section = cfg["kafka"]
+            inner_settings["KAFKA_CONFIG"] = {
+                "bootstrap_servers": kafka_section.get(
+                    "bootstrap_servers", "127.0.0.1:9092"
+                ),
+                "topic": kafka_section.get("topic", None),
+                "key": kafka_section.get("key", None),
+            }
+        if "oss:ali" in cfg:
+            oss_section = cfg["oss:ali"]
+            inner_settings["OSS_CONFIG"] = {
+                "access_key": oss_section.get("access_key", None),
+                "access_secret": oss_section.get("access_secret", None),
+                "endpoint": oss_section.get("endpoint", None),
+                "bucket": oss_section.get("bucket", None),
+                "doc": oss_section.get("doc", None),
+                "upload_fields_suffix": oss_section.get(
+                    "upload_fields_suffix", "_file_url"
+                ),
+                "oss_fields_prefix": oss_section.get("oss_fields_prefix", "_"),
+                "full_link_enable": oss_section.getboolean("full_link_enable", False),
+            }
+        return inner_settings
+
+    @staticmethod
+    def item_to_dict(item: Union[AyuItem, dict]) -> dict:
+        """将 item 转换为 dict 类型；
+        将 spider 中的 yield 的 item 转换为 dict 类型，方便后续处理
+
+        Args:
+            item: spider 中的 yield 的 item
+
+        Returns:
+            1). dict 类型的 item
+        """
+        return (
+            item.asdict() if isinstance(item, AyuItem) else ItemAdapter(item).asdict()
+        )
+
+    @classmethod
+    def reshape_item(cls, item_dict: Dict[str, Any]) -> AlterItem:
+        """重新整合 item
+
+        Args:
+            item_dict: dict 类型的 item
+
+        Returns:
+            1). 整合后的 item
+        """
+        new_item = {}
+        notes_dic = {}
+        is_namedtuple = False
+
+        insert_data = cls.get_items_except_keys(
+            dict_conf=item_dict, keys=["_mongo_update_rule", "_table"]
+        )
+        judge_item = next(iter(insert_data.values()))
+        if cls.is_namedtuple_instance(judge_item):
+            is_namedtuple = True
+            _table_name = item_dict["_table"].key_value
+            _table_notes = item_dict["_table"].notes
+            table_info = AlterItemTable(_table_name, _table_notes)
+            for key, value in insert_data.items():
+                new_item[key] = value.key_value
+                notes_dic[key] = value.notes
+
+        else:
+            _table_name = item_dict["_table"]
+            table_info = AlterItemTable(_table_name, "")
+            for key, value in insert_data.items():
+                new_item[key] = value
+                notes_dic[key] = ""
+
+        return AlterItem(new_item, notes_dic, table_info, is_namedtuple)
+
+    @staticmethod
+    def is_namedtuple_instance(x: Any) -> bool:
+        """判断 x 是否为 namedtuple 类型
+
+        Args:
+            x: 需要判断的参数
+
+        Returns:
+            1). 是否符合 namedtuple 类型
+        """
+        return isinstance(x, tuple) and hasattr(x, "_fields")
+
+    @staticmethod
+    def random_weight(weight_data: list):
+        """带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
+
+        Args:
+            weight_data: 带权重的列表信息，示例：
+                [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
+
+        Returns:
+            ret: 返回当前权重列表 account_arr 中的一个值
+        """
+        total = sum(item["weight"] for item in weight_data)
+        # 在 0 与权重和之间获取一个随机数
+        ra = random.uniform(0, total)
+        curr_sum = 0
+        ret = None
+        for data in weight_data:
+            # 在遍历中，累加当前权重值
+            curr_sum += data["weight"]
+            # 当随机数 <= 当前权重和时，返回权重 key
+            if ra <= curr_sum:
+                ret = data
+                break
+        return ret
+
+    @staticmethod
+    def is_dict_meet_min_limit(dict_conf: dict, key_list: List[str]) -> bool:
+        """判断 dict_conf 是否满足 key_list 中的 key 值限定
+
+        Args:
+            dict_conf: 需要判断的参数
+            key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
+
+        Returns:
+            1). 是否满足 key 值限制
+        """
+        if any([not dict_conf, not isinstance(dict_conf, dict)]):
+            return False
+
+        return all(key in dict_conf for key in key_list)
+
+    @classmethod
+    def get_items_by_keys(
+        cls,
+        dict_conf: dict,
+        keys: List[str],
+    ) -> dict:
+        """获取 dict_conf 中的含有 keys 的 key 的字段
+
+        Args:
+            dict_conf: 需要处理的参数
+            keys: 需要取的 key 值列表
+
+        Returns:
+            1). 取值后的 dict，或不满足请求的 False 值
+        """
+        return (
+            {k: dict_conf[k] for k in keys}
+            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=keys)
+            else {}
+        )
+
+    @staticmethod
+    def get_items_except_keys(dict_conf, keys: List[str]) -> dict:
+        """获取 dict_conf 中的不含有 keys 的 key 的字段
+
+        Args:
+            dict_conf: 需要处理的参数
+            keys: 需要排除的 key 值列表
+
+        Returns:
+            1). dict_conf 排除 keys 中的键值后的值
+        """
+        return {k: dict_conf[k] for k in dict_conf if k not in keys}
+
+    @staticmethod
+    def create_database(db_conf: Union[MysqlConf, PostgreSQLConf]) -> None:
+        """创建数据库：由于这是在连接数据库，报数据库不存在错误时的场景，则需要
+        新建(不指定数据库)连接创建好所需数据库即可
+
+        Args:
+            db_conf: 数据库连接配置，目前支持 mysql 和 postgresql
+        """
+        if isinstance(db_conf, MysqlConf):
+            with pymysql.connect(
+                user=db_conf.user,
+                password=db_conf.password,
+                host=db_conf.host,
+                port=db_conf.port,
+                charset=db_conf.charset,
+            ) as conn:
+                with conn.cursor() as cur:
+                    cur.execute(
+                        f"CREATE DATABASE IF NOT EXISTS `{db_conf.database}` character set {db_conf.charset};"
+                    )
+
+        elif isinstance(db_conf, PostgreSQLConf):
+            with psycopg.connect(
+                user=db_conf.user,
+                password=db_conf.password,
+                host=db_conf.host,
+                port=db_conf.port,
+            ) as conn:
+                with conn.cursor() as cur:
+                    conn.autocommit = True
+                    cur.execute(
+                        f"CREATE DATABASE {db_conf.database} WITH ENCODING {db_conf.charset};"
+                    )
+
+        else:
+            assert False, f"Invalid db_conf type: {type(db_conf)}"
+        logger.info(
+            f"创建数据库 {db_conf.database} 成功，其 charset 类型是：{db_conf.charset}!"
+        )
+
+    @classmethod
+    def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
+        """将 dict 中 str 类型的 key 值变成小写
+
+        Args:
+            deal_dict: 需要处理的 dict
+
+        Returns:
+            1).处理后的 dict 值
+        """
+        key_to_lower_dict = {}
+        for key, value in deal_dict.items():
+            if isinstance(value, dict):
+                if isinstance(key, str):
+                    key_to_lower_dict[key.lower()] = cls.dict_keys_to_lower(value)
+                else:
+                    key_to_lower_dict[key] = cls.dict_keys_to_lower(value)
+            elif isinstance(key, str):
+                key_to_lower_dict[key.lower()] = value
+            else:
+                key_to_lower_dict[key] = value
+        return key_to_lower_dict
+
+    @classmethod
+    def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
+        """将 dict 中 str 类型的 key 值变成大写
+
+        Args:
+            deal_dict: 需要处理的 dict
+
+        Returns:
+            1).处理后的 dict 值
+        """
+        key_to_upper_dict = {}
+        for key, value in deal_dict.items():
+            if isinstance(value, dict):
+                if isinstance(key, str):
+                    key_to_upper_dict[key.upper()] = cls.dict_keys_to_upper(value)
+                else:
+                    key_to_upper_dict[key] = cls.dict_keys_to_upper(value)
+            elif isinstance(key, str):
+                key_to_upper_dict[key.upper()] = value
+            else:
+                key_to_upper_dict[key] = value
+        return key_to_upper_dict
+
+    @classmethod
+    def get_remote_option(cls, settings: "BaseSettings") -> dict:
+        """获取项目中 consul 或 nacos 的链接配置
+
+        Args:
+            settings: scrapy 的 settings 信息
+
+        Returns:
+            1). 满足最少要求的远程配置
+        """
+        consul_conf_dict = settings.get("REMOTE_CONFIG", {})
+        return cls.get_items_by_keys(
+            dict_conf=consul_conf_dict, keys=["token", "url", "format", "remote_type"]
+        )
+
+    @staticmethod
+    def judge_str_is_json(judge_str: str) -> bool:
+        """判断字符串是否为 json 格式
+
+        Args:
+            judge_str: 需要判断的字符串
+
+        Returns:
+            1). 是否为 json 格式
+        """
+        if not isinstance(judge_str, str):
+            return False
+
+        try:
+            json.loads(judge_str)
+        except Exception:
+            return False
+        else:
+            return True
+
+    @staticmethod
+    def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
+        """从 headers 中的 ck str 格式转化为 dict 格式
+
+        Args:
+            headers_ck_str: request headers ck 的 str 格式
+
+        Returns:
+            1). 转化 dict 格式后的 ck
+        """
+        return {
+            x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
+            for x in headers_ck_str.split(";")
+        }
+
+    @staticmethod
+    def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
+        """将 scrapy 请求中的 body 对象转为 dict 格式
+
+        Args:
+            req_body_data_str: scrapy 中的 body 参数
+
+        Returns:
+            1). 转化 dict 格式后的 body
+        """
+        return {
+            x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
+        }
+
+    @classmethod
+    def get_array_depth(cls, array: list) -> int:
+        """获取 array 的最大层级，深度
+
+        Args:
+            array: 数组
+
+        Returns:
+            1). 最大层级，深度
+        """
+
+        """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
+        # 先判断是否为数组类型的元素
+        judge_array = isinstance(
+            array,
+            (
+                frozenset,
+                list,
+                set,
+                tuple,
+            ),
+        )
+        return (
+            int(judge_array) and len(array) and 1 + max(map(cls.get_array_depth, array))
+        )
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.9.8/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,316 +1,316 @@
-import re
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Optional, Tuple, TypeVar, Union
-
-from ayugespidertools.config import logger
-
-__all__ = [
-    "Synchronize",
-    "TwistedAsynchronous",
-    "deal_mysql_err",
-]
-
-if TYPE_CHECKING:
-    from pymysql.connections import Connection
-    from pymysql.cursors import Cursor, DictCursor
-    from twisted.enterprise.adbapi import Transaction
-
-    from ayugespidertools.common.typevars import MysqlConf
-
-    TwistedTransactionT = TypeVar("TwistedTransactionT", bound=Transaction)
-    PymysqlDictCursorT = TypeVar("PymysqlDictCursorT", bound=DictCursor)
-
-
-class AbstractClass(ABC):
-    """用于处理 mysql 异常的模板方法类"""
-
-    def _create_table(
-        self,
-        cursor: "Cursor",
-        table_name: str,
-        engine: str,
-        charset: str,
-        collate: str,
-        table_notes: str = "",
-    ) -> None:
-        """创建数据库表
-
-        Args:
-            cursor: mysql connect cursor
-            table_name: 创建表的名称
-            engine: 创建表的 engine
-            charset: charset
-            collate: collate
-            table_notes: 创建表的注释
-        """
-        sql = (
-            f"CREATE TABLE IF NOT EXISTS `{table_name}` (`id` int(32) NOT NULL"
-            f" AUTO_INCREMENT COMMENT 'id', PRIMARY KEY (`id`)) ENGINE={engine}"
-            f" DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{table_notes}';"
-        )
-
-        try:
-            cursor.execute(sql)
-            logger.info(f"创建数据表 {table_notes}: {table_name} 成功！")
-        except Exception as e:
-            logger.error(f"创建表 {table_name} 失败，err：{e}")
-
-    def _get_column_type(
-        self,
-        cursor: "Cursor",
-        database: str,
-        table: str,
-        column: str,
-    ) -> Union[str, None]:
-        """获取数据字段存储类型
-
-        Args:
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            column: 字段名称
-
-        Returns:
-            column_type: 字段存储类型
-        """
-        sql = (
-            f"select COLUMN_TYPE from information_schema.columns where table_schema = '{database}'"
-            f" and table_name = '{table}' and COLUMN_NAME= '{column}';"
-        )
-        column_type = None
-        try:
-            cursor.execute(sql)
-            lines = cursor.fetchall()
-            if isinstance(lines, list):
-                # 注意，此处 AyuMysqlPipeline 返回的结构示例为：[{'COLUMN_TYPE': 'varchar(190)'}]
-                column_type = lines[0]["COLUMN_TYPE"] if len(lines) == 1 else ""
-            else:
-                # 注意，此处 AyuTwistedMysqlPipeline 返回的结构示例为：(('varchar(10)',),)
-                column_type = lines[0][0] if len(lines) == 1 else ""
-
-        except Exception as e:
-            logger.error(f"未获取到当前字段的存储类型，err: {e}")
-        return column_type
-
-    def template_method(
-        self,
-        err_msg: str,
-        conn: "Connection[Cursor]",
-        cursor: Union["Cursor", "TwistedTransactionT"],
-        mysql_conf: "MysqlConf",
-        table: str,
-        table_notes: str,
-        note_dic: dict,
-    ) -> None:
-        """模板方法，用于处理 mysql 存储场景的异常
-
-        Args:
-            err_msg: pipeline 存储时报错内容
-            conn: mysql conn
-            cursor: mysql connect cursor
-            mysql_conf: spider mysql_conf
-            table: 数据表
-            table_notes: 数据表注释
-            note_dic: 当前表字段注释
-        """
-        if "1054" in err_msg:
-            sql, possible_err = self.deal_1054_error(
-                err_msg=err_msg, table=table, note_dic=note_dic
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        elif "1146" in err_msg:
-            self._create_table(
-                cursor=cursor,
-                table_name=table,
-                engine=mysql_conf.engine,
-                charset=mysql_conf.charset,
-                collate=mysql_conf.collate,
-                table_notes=table_notes,
-            )
-
-        elif "1406" in err_msg:
-            sql, possible_err = self.deal_1406_error(
-                err_msg=err_msg,
-                cursor=cursor,
-                database=mysql_conf.database,
-                table=table,
-                note_dic=note_dic,
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        elif "1265" in err_msg:
-            sql, possible_err = self.deal_1265_error(
-                err_msg=err_msg,
-                cursor=cursor,
-                database=mysql_conf.database,
-                table=table,
-                note_dic=note_dic,
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        else:
-            raise Exception(f"MYSQL OTHER ERROR: {err_msg}")
-
-    def deal_1054_error(
-        self, err_msg: str, table: str, note_dic: dict
-    ) -> Tuple[str, str]:
-        """解决 1054, u"Unknown column 'xx' in 'field list'"
-
-        Args:
-            err_msg: 报错内容
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            1). sql: 用于添加字段的 sql 语句
-            2). 执行此 sql 可能会报错的信息
-        """
-        colum_pattern = re.compile(r"Unknown column '(.*?)' in 'field list'")
-        text = re.findall(colum_pattern, err_msg)
-        colum = text[0]
-        notes = note_dic[colum]
-
-        sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(255) NULL DEFAULT '' COMMENT '{notes}';"
-        return sql, f"添加字段 {colum} 已存在"
-
-    def deal_1406_error(
-        self,
-        err_msg: str,
-        cursor: "Cursor",
-        database: str,
-        table: str,
-        note_dic: dict,
-    ) -> Tuple[str, str]:
-        """解决 1406, u"Data too long for 'xx' at ..."
-
-        Args:
-            err_msg: 报错内容
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            1). sql: 修改字段类型的 sql
-            2). 执行此 sql 可能会报错的信息
-        """
-        if "Data too long for" in err_msg:
-            colum_pattern = re.compile(r"Data too long for column '(.*?)' at")
-            text = re.findall(colum_pattern, err_msg)
-            colum = text[0]
-            notes = note_dic[colum]
-            column_type = self._get_column_type(
-                cursor=cursor, database=database, table=table, column=colum
-            )
-            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
-            sql = (
-                f"ALTER TABLE `{table}` CHANGE COLUMN `{colum}` `{colum}`"
-                f' {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";'
-            )
-            return sql, f"更新 {colum} 字段类型为 {change_colum_type} 时失败"
-        raise Exception(f"未解决 Data too long 的问题，err: {err_msg}")
-
-    def deal_1265_error(
-        self,
-        err_msg: str,
-        cursor: "Cursor",
-        database: str,
-        table: str,
-        note_dic: dict,
-    ) -> Tuple[str, str]:
-        """解决 1265, u"Data truncated for column 'xx' at ..."
-
-        Args:
-            err_msg: 报错内容
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            1). sql: 修改字段类型的 sql
-            2). 执行此 sql 可能会报错的信息
-        """
-        if "Data truncated for column" in err_msg:
-            colum_pattern = re.compile(r"Data truncated for column '(.*?)' at")
-            text = re.findall(colum_pattern, err_msg)
-            colum = text[0]
-            notes = note_dic[colum]
-            column_type = self._get_column_type(
-                cursor=cursor, database=database, table=table, column=colum
-            )
-            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
-            sql = (
-                f"ALTER TABLE `{table}` CHANGE COLUMN `{colum}` `{colum}`"
-                f' {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";'
-            )
-            return sql, f"更新 {colum} 字段类型为 {change_colum_type} 时失败"
-        raise Exception(f"未解决 Data truncated 问题，err: {err_msg}")
-
-    @abstractmethod
-    def _exec_sql(self, *args, **kwargs) -> None:
-        """子类要实现执行 sql 的不同方法，使得可以正常适配不同的 pipelines 场景"""
-        pass
-
-
-class Synchronize(AbstractClass):
-    """pipeline 同步执行 sql 的场景"""
-
-    def _exec_sql(
-        self,
-        conn: "Connection[Cursor]",
-        cursor: "Cursor",
-        sql: str,
-        possible_err: Optional[str] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        try:
-            cursor.execute(sql)
-        except Exception as e:
-            logger.warning(
-                f"synchronize mysql exec sql err: {str(e)}\n"
-                f"possible_err ->: {possible_err}"
-            )
-
-
-class TwistedAsynchronous(AbstractClass):
-    """pipeline twisted 异步执行 sql 的场景"""
-
-    def _exec_sql(
-        self,
-        cursor: "TwistedTransactionT",
-        sql: str,
-        possible_err: Optional[str] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        try:
-            cursor.execute(sql)
-        except Exception as e:
-            logger.warning(
-                f"twisted mysql exec sql err: {str(e)}\n"
-                f"possible_err: {possible_err}"
-            )
-
-
-def deal_mysql_err(
-    abstract_class: AbstractClass,
-    err_msg: str,
-    cursor: Union["Cursor", "TwistedTransactionT"],
-    mysql_conf: "MysqlConf",
-    table: str,
-    table_notes: str,
-    note_dic: dict,
-    conn: Optional["Connection[Cursor]"] = None,
-) -> None:
-    abstract_class.template_method(
-        err_msg,
-        conn,
-        cursor,
-        mysql_conf,
-        table,
-        table_notes,
-        note_dic,
-    )
+import re
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Optional, Tuple, TypeVar, Union
+
+from ayugespidertools.config import logger
+
+__all__ = [
+    "Synchronize",
+    "TwistedAsynchronous",
+    "deal_mysql_err",
+]
+
+if TYPE_CHECKING:
+    from pymysql.connections import Connection
+    from pymysql.cursors import Cursor, DictCursor
+    from twisted.enterprise.adbapi import Transaction
+
+    from ayugespidertools.common.typevars import MysqlConf
+
+    TwistedTransactionT = TypeVar("TwistedTransactionT", bound=Transaction)
+    PymysqlDictCursorT = TypeVar("PymysqlDictCursorT", bound=DictCursor)
+
+
+class AbstractClass(ABC):
+    """用于处理 mysql 异常的模板方法类"""
+
+    def _create_table(
+        self,
+        cursor: "Cursor",
+        table_name: str,
+        engine: str,
+        charset: str,
+        collate: str,
+        table_notes: str = "",
+    ) -> None:
+        """创建数据库表
+
+        Args:
+            cursor: mysql connect cursor
+            table_name: 创建表的名称
+            engine: 创建表的 engine
+            charset: charset
+            collate: collate
+            table_notes: 创建表的注释
+        """
+        sql = (
+            f"CREATE TABLE IF NOT EXISTS `{table_name}` (`id` int(32) NOT NULL"
+            f" AUTO_INCREMENT COMMENT 'id', PRIMARY KEY (`id`)) ENGINE={engine}"
+            f" DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{table_notes}';"
+        )
+
+        try:
+            cursor.execute(sql)
+            logger.info(f"创建数据表 {table_notes}: {table_name} 成功！")
+        except Exception as e:
+            logger.error(f"创建表 {table_name} 失败，err：{e}")
+
+    def _get_column_type(
+        self,
+        cursor: "Cursor",
+        database: str,
+        table: str,
+        column: str,
+    ) -> Union[str, None]:
+        """获取数据字段存储类型
+
+        Args:
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            column: 字段名称
+
+        Returns:
+            column_type: 字段存储类型
+        """
+        sql = (
+            f"select COLUMN_TYPE from information_schema.columns where table_schema = '{database}'"
+            f" and table_name = '{table}' and COLUMN_NAME= '{column}';"
+        )
+        column_type = None
+        try:
+            cursor.execute(sql)
+            lines = cursor.fetchall()
+            if isinstance(lines, list):
+                # 此处 AyuMysqlPipeline 返回的结构示例为：[{'COLUMN_TYPE': 'varchar(190)'}]
+                column_type = lines[0]["COLUMN_TYPE"] if len(lines) == 1 else ""
+            else:
+                # 此处 AyuTwistedMysqlPipeline 返回的结构示例为：(('varchar(10)',),)
+                column_type = lines[0][0] if len(lines) == 1 else ""
+
+        except Exception as e:
+            logger.error(f"未获取到当前字段的存储类型，err: {e}")
+        return column_type
+
+    def template_method(
+        self,
+        err_msg: str,
+        conn: "Connection[Cursor]",
+        cursor: Union["Cursor", "TwistedTransactionT"],
+        mysql_conf: "MysqlConf",
+        table: str,
+        table_notes: str,
+        note_dic: dict,
+    ) -> None:
+        """模板方法，用于处理 mysql 存储场景的异常
+
+        Args:
+            err_msg: pipeline 存储时报错内容
+            conn: mysql conn
+            cursor: mysql connect cursor
+            mysql_conf: spider mysql_conf
+            table: 数据表
+            table_notes: 数据表注释
+            note_dic: 当前表字段注释
+        """
+        if "1054" in err_msg:
+            sql, possible_err = self.deal_1054_error(
+                err_msg=err_msg, table=table, note_dic=note_dic
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        elif "1146" in err_msg:
+            self._create_table(
+                cursor=cursor,
+                table_name=table,
+                engine=mysql_conf.engine,
+                charset=mysql_conf.charset,
+                collate=mysql_conf.collate,
+                table_notes=table_notes,
+            )
+
+        elif "1406" in err_msg:
+            sql, possible_err = self.deal_1406_error(
+                err_msg=err_msg,
+                cursor=cursor,
+                database=mysql_conf.database,
+                table=table,
+                note_dic=note_dic,
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        elif "1265" in err_msg:
+            sql, possible_err = self.deal_1265_error(
+                err_msg=err_msg,
+                cursor=cursor,
+                database=mysql_conf.database,
+                table=table,
+                note_dic=note_dic,
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        else:
+            raise Exception(f"MYSQL OTHER ERROR: {err_msg}")
+
+    def deal_1054_error(
+        self, err_msg: str, table: str, note_dic: dict
+    ) -> Tuple[str, str]:
+        """解决 1054, u"Unknown column 'xx' in 'field list'"
+
+        Args:
+            err_msg: 报错内容
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 用于添加字段的 sql 语句
+            2). 执行此 sql 可能会报错的信息
+        """
+        colum_pattern = re.compile(r"Unknown column '(.*?)' in 'field list'")
+        text = re.findall(colum_pattern, err_msg)
+        colum = text[0]
+        notes = note_dic[colum]
+
+        sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(255) NULL DEFAULT '' COMMENT '{notes}';"
+        return sql, f"添加字段 {colum} 已存在"
+
+    def deal_1406_error(
+        self,
+        err_msg: str,
+        cursor: "Cursor",
+        database: str,
+        table: str,
+        note_dic: dict,
+    ) -> Tuple[str, str]:
+        """解决 1406, u"Data too long for 'xx' at ..."
+
+        Args:
+            err_msg: 报错内容
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 修改字段类型的 sql
+            2). 执行此 sql 可能会报错的信息
+        """
+        if "Data too long for" in err_msg:
+            colum_pattern = re.compile(r"Data too long for column '(.*?)' at")
+            text = re.findall(colum_pattern, err_msg)
+            colum = text[0]
+            notes = note_dic[colum]
+            column_type = self._get_column_type(
+                cursor=cursor, database=database, table=table, column=colum
+            )
+            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
+            sql = (
+                f"ALTER TABLE `{table}` CHANGE COLUMN `{colum}` `{colum}`"
+                f' {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";'
+            )
+            return sql, f"更新 {colum} 字段类型为 {change_colum_type} 时失败"
+        raise Exception(f"未解决 Data too long 的问题，err: {err_msg}")
+
+    def deal_1265_error(
+        self,
+        err_msg: str,
+        cursor: "Cursor",
+        database: str,
+        table: str,
+        note_dic: dict,
+    ) -> Tuple[str, str]:
+        """解决 1265, u"Data truncated for column 'xx' at ..."
+
+        Args:
+            err_msg: 报错内容
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 修改字段类型的 sql
+            2). 执行此 sql 可能会报错的信息
+        """
+        if "Data truncated for column" in err_msg:
+            colum_pattern = re.compile(r"Data truncated for column '(.*?)' at")
+            text = re.findall(colum_pattern, err_msg)
+            colum = text[0]
+            notes = note_dic[colum]
+            column_type = self._get_column_type(
+                cursor=cursor, database=database, table=table, column=colum
+            )
+            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
+            sql = (
+                f"ALTER TABLE `{table}` CHANGE COLUMN `{colum}` `{colum}`"
+                f' {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";'
+            )
+            return sql, f"更新 {colum} 字段类型为 {change_colum_type} 时失败"
+        raise Exception(f"未解决 Data truncated 问题，err: {err_msg}")
+
+    @abstractmethod
+    def _exec_sql(self, *args, **kwargs) -> None:
+        """子类要实现执行 sql 的不同方法，使得可以正常适配不同的 pipelines 场景"""
+        pass
+
+
+class Synchronize(AbstractClass):
+    """pipeline 同步执行 sql 的场景"""
+
+    def _exec_sql(
+        self,
+        conn: "Connection[Cursor]",
+        cursor: "Cursor",
+        sql: str,
+        possible_err: Optional[str] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        try:
+            cursor.execute(sql)
+        except Exception as e:
+            logger.warning(
+                f"synchronize mysql exec sql err: {str(e)}\n"
+                f"possible_err ->: {possible_err}"
+            )
+
+
+class TwistedAsynchronous(AbstractClass):
+    """pipeline twisted 异步执行 sql 的场景"""
+
+    def _exec_sql(
+        self,
+        cursor: "TwistedTransactionT",
+        sql: str,
+        possible_err: Optional[str] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        try:
+            cursor.execute(sql)
+        except Exception as e:
+            logger.warning(
+                f"twisted mysql exec sql err: {str(e)}\n"
+                f"possible_err: {possible_err}"
+            )
+
+
+def deal_mysql_err(
+    abstract_class: AbstractClass,
+    err_msg: str,
+    cursor: Union["Cursor", "TwistedTransactionT"],
+    mysql_conf: "MysqlConf",
+    table: str,
+    table_notes: str,
+    note_dic: dict,
+    conn: Optional["Connection[Cursor]"] = None,
+) -> None:
+    abstract_class.template_method(
+        err_msg,
+        conn,
+        cursor,
+        mysql_conf,
+        table,
+        table_notes,
+        note_dic,
+    )
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/params.py` & `ayugespidertools-3.9.8/ayugespidertools/common/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,326 +1,318 @@
-import platform
-import random
-
-__all__ = [
-    "Param",
-]
-
-
-class Param:
-    """用于存储项目中需要的参数变量设置"""
-
-    retry_num = 3
-    retry_time_min = 200
-    retry_time_max = 1000
-    # stop_max_delay 限制最长重试时间
-    stop_max_delay = 5000
-
-    requests_req_timeout = 3
-    requests_res_timeout = 5
-    requests_time_sleep_list = [x / 10 for x in range(5, 19)]
-    requests_time_sleep_random = random.choice(requests_time_sleep_list)
-
-    aiohttp_retry_times_default = 3
-
-    # 部署运行的平台为 win 或 linux
-    IS_WINDOWS = platform.system().lower() == "windows"
-    IS_LINUX = platform.system().lower() == "linux"
-
-    # 动态隧道代理配置示例
-    dynamic_proxy_conf_example = {
-        "proxy": "动态隧道代理地址：***.***.com:*****",
-        "username": "隧道代理用户名",
-        "password": "对应用户的密码",
-    }
-    # 独享代理配置示例
-    exclusive_proxy_conf_example = {
-        "proxy": "独享代理地址：'http://***.com/api/***&num=100&format=json'",
-        "username": "独享代理用户名",
-        "password": "对应用户的密码",
-        "index": "需要返回的独享代理的索引",
-    }
-
-    # aiohttp 配置示例
-    aiohttp_conf_example = {
-        "timeout": 5,
-        "proxy": "127.0.0.1:80",
-        "sleep": 1,
-        "retry_times": 3,
-    }
-
-    charset_collate_map = {
-        # utf8mb4_unicode_ci 也是经常使用的
-        "utf8mb4": "utf8mb4_general_ci",
-        "utf8": "utf8_general_ci",
-        "gbk": "gbk_chinese_ci",
-        "latin1": "latin1_swedish_ci",
-        "utf16": "utf16_general_ci",
-        "utf16le": "utf16le_general_ci",
-        "cp1251": "cp1251_general_ci",
-        "euckr": "euckr_korean_ci",
-        "greek": "greek_general_ci",
-    }
-
-    # 随机请求头列表
-    fake_useragent_dict = {
-        "chrome": [
-            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2228.0 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.1 Safari/537.36",
-            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2226.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.4; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2225.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2225.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2224.3 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/40.0.2214.93 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2062.124 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.67 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.67 Safari/537.36",
-            "Mozilla/5.0 (X11; OpenBSD i386) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.125 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1944.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.3319.102 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.2309.372 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.2117.157 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.47 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1866.237 Safari/537.36",
-            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.137 Safari/4E423F",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.116 Safari/537.36 Mozilla/5.0 (iPad; U; CPU OS 3_2 like Mac OS X; en-us) AppleWebKit/531.21.10 (KHTML, like Gecko) Version/4.0.4 Mobile/7B334b Safari/531.21.10",
-            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/33.0.1750.517 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1667.0 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1664.3 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1664.3 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/31.0.1650.16 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/31.0.1623.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/30.0.1599.17 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.62 Safari/537.36",
-            "Mozilla/5.0 (X11; CrOS i686 4319.74.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.57 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.2 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1468.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1467.0 Safari/537.36",
-            "Mozilla/a/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1464.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1500.55 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.90 Safari/537.36",
-            "Mozilla/5.0 (X11; NetBSD) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
-            "Mozilla/5.0 (X11; CrOS i686 3912.101.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1312.60 Safari/537.17",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_2) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1309.0 Safari/537.17",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.15 (KHTML, like Gecko) Chrome/24.0.1295.0 Safari/537.15",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.14 (KHTML, like Gecko) Chrome/24.0.1292.0 Safari/537.14",
-        ],
-        "opera": [
-            "Opera/9.80 (X11; Linux i686; Ubuntu/14.10) Presto/2.12.388 Version/12.16",
-            "Opera/9.80 (Windows NT 6.0) Presto/2.12.388 Version/12.14",
-            "Mozilla/5.0 (Windows NT 6.0; rv:2.0) Gecko/20100101 Firefox/4.0 Opera 12.14",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0) Opera 12.14",
-            "Opera/12.80 (Windows NT 5.1; U; en) Presto/2.10.289 Version/12.02",
-            "Opera/9.80 (Windows NT 6.1; U; es-ES) Presto/2.9.181 Version/12.00",
-            "Opera/9.80 (Windows NT 5.1; U; zh-sg) Presto/2.9.181 Version/12.00",
-            "Opera/12.0(Windows NT 5.2;U;en)Presto/22.9.168 Version/12.00",
-            "Opera/12.0(Windows NT 5.1;U;en)Presto/22.9.168 Version/12.00",
-            "Mozilla/5.0 (Windows NT 5.1) Gecko/20100101 Firefox/14.0 Opera/12.0",
-            "Opera/9.80 (Windows NT 6.1; WOW64; U; pt) Presto/2.10.229 Version/11.62",
-            "Opera/9.80 (Windows NT 6.0; U; pl) Presto/2.10.229 Version/11.62",
-            "Opera/9.80 (Macintosh; Intel Mac OS X 10.6.8; U; fr) Presto/2.9.168 Version/11.52",
-            "Opera/9.80 (Macintosh; Intel Mac OS X 10.6.8; U; de) Presto/2.9.168 Version/11.52",
-            "Opera/9.80 (Windows NT 5.1; U; en) Presto/2.9.168 Version/11.51",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; de) Opera 11.51",
-            "Opera/9.80 (X11; Linux x86_64; U; fr) Presto/2.9.168 Version/11.50",
-            "Opera/9.80 (X11; Linux i686; U; hu) Presto/2.9.168 Version/11.50",
-            "Opera/9.80 (X11; Linux i686; U; ru) Presto/2.8.131 Version/11.11",
-            "Opera/9.80 (X11; Linux i686; U; es-ES) Presto/2.8.131 Version/11.11",
-            "Mozilla/5.0 (Windows NT 5.1; U; en; rv:1.8.1) Gecko/20061208 Firefox/5.0 Opera 11.11",
-            "Opera/9.80 (X11; Linux x86_64; U; bg) Presto/2.8.131 Version/11.10",
-            "Opera/9.80 (Windows NT 6.0; U; en) Presto/2.8.99 Version/11.10",
-            "Opera/9.80 (Windows NT 5.1; U; zh-tw) Presto/2.8.131 Version/11.10",
-            "Opera/9.80 (Windows NT 6.1; Opera Tablet/15165; U; en) Presto/2.8.149 Version/11.1",
-            "Opera/9.80 (X11; Linux x86_64; U; Ubuntu/10.10 (maverick); pl) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (X11; Linux i686; U; ja) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (X11; Linux i686; U; fr) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.1; U; zh-tw) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.1; U; zh-cn) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.1; U; sv) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.1; U; en-US) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.1; U; cs) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 6.0; U; pl) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 5.2; U; ru) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 5.1; U;) Presto/2.7.62 Version/11.01",
-            "Opera/9.80 (Windows NT 5.1; U; cs) Presto/2.7.62 Version/11.01",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US; rv:1.9.2.13) Gecko/20101213 Opera/9.80 (Windows NT 6.1; U; zh-tw) Presto/2.7.62 Version/11.01",
-            "Mozilla/5.0 (Windows NT 6.1; U; nl; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6 Opera 11.01",
-            "Mozilla/5.0 (Windows NT 6.1; U; de; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6 Opera 11.01",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; de) Opera 11.01",
-            "Opera/9.80 (X11; Linux x86_64; U; pl) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (X11; Linux i686; U; it) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1; U; zh-cn) Presto/2.6.37 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1; U; pl) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1; U; ko) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1; U; fi) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1; U; en-GB) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.1 x64; U; en) Presto/2.7.62 Version/11.00",
-            "Opera/9.80 (Windows NT 6.0; U; en) Presto/2.7.39 Version/11.00",
-        ],
-        "firefox": [
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:40.0) Gecko/20100101 Firefox/40.1",
-            "Mozilla/5.0 (Windows NT 6.3; rv:36.0) Gecko/20100101 Firefox/36.0",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10; rv:33.0) Gecko/20100101 Firefox/33.0",
-            "Mozilla/5.0 (X11; Linux i586; rv:31.0) Gecko/20100101 Firefox/31.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:31.0) Gecko/20130401 Firefox/31.0",
-            "Mozilla/5.0 (Windows NT 5.1; rv:31.0) Gecko/20100101 Firefox/31.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:29.0) Gecko/20120101 Firefox/29.0",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:25.0) Gecko/20100101 Firefox/29.0",
-            "Mozilla/5.0 (X11; OpenBSD amd64; rv:28.0) Gecko/20100101 Firefox/28.0",
-            "Mozilla/5.0 (X11; Linux x86_64; rv:28.0) Gecko/20100101  Firefox/28.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:27.3) Gecko/20130101 Firefox/27.3",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:27.0) Gecko/20121011 Firefox/27.0",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:25.0) Gecko/20100101 Firefox/25.0",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.6; rv:25.0) Gecko/20100101 Firefox/25.0",
-            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:24.0) Gecko/20100101 Firefox/24.0",
-            "Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.8; rv:24.0) Gecko/20100101 Firefox/24.0",
-            "Mozilla/5.0 (Windows NT 6.2; rv:22.0) Gecko/20130405 Firefox/23.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:23.0) Gecko/20130406 Firefox/23.0",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:23.0) Gecko/20131011 Firefox/23.0",
-            "Mozilla/5.0 (Windows NT 6.2; rv:22.0) Gecko/20130405 Firefox/22.0",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:22.0) Gecko/20130328 Firefox/22.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:22.0) Gecko/20130405 Firefox/22.0",
-            "Mozilla/5.0 (Microsoft Windows NT 6.2.9200.0); rv:22.0) Gecko/20130405 Firefox/22.0",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/21.0.1",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/21.0.1",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:21.0.0) Gecko/20121011 Firefox/21.0.0",
-            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:21.0) Gecko/20130331 Firefox/21.0",
-            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (X11; Linux i686; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.2; WOW64; rv:21.0) Gecko/20130514 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.2; rv:21.0) Gecko/20130326 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130401 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130331 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130330 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20130401 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20130328 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20130401 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20130331 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 5.0; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.8; rv:21.0) Gecko/20100101 Firefox/21.0",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64;) Gecko/20100101 Firefox/20.0",
-            "Mozilla/5.0 (Windows x86; rv:19.0) Gecko/20100101 Firefox/19.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:6.0) Gecko/20100101 Firefox/19.0",
-            "Mozilla/5.0 (Windows NT 6.1; rv:14.0) Gecko/20100101 Firefox/18.0.1",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:18.0)  Gecko/20100101 Firefox/18.0",
-            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:17.0) Gecko/20100101 Firefox/17.0.6",
-        ],
-        "internetexplorer": [
-            "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; AS; rv:11.0) like Gecko",
-            "Mozilla/5.0 (compatible, MSIE 11, Windows NT 6.3; Trident/7.0;  rv:11.0) like Gecko",
-            "Mozilla/5.0 (compatible; MSIE 10.6; Windows NT 6.1; Trident/5.0; InfoPath.2; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 2.0.50727) 3gpp-gba UNTRUSTED/1.0",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 7.0; InfoPath.3; .NET CLR 3.1.40767; Trident/6.0; en-IN)",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/5.0)",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/4.0; InfoPath.2; SV1; .NET CLR 2.0.50727; WOW64)",
-            "Mozilla/5.0 (compatible; MSIE 10.0; Macintosh; Intel Mac OS X 10_7_3; Trident/6.0)",
-            "Mozilla/4.0 (Compatible; MSIE 8.0; Windows NT 5.2; Trident/6.0)",
-            "Mozilla/4.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/5.0)",
-            "Mozilla/1.22 (compatible; MSIE 10.0; Windows 3.1)",
-            "Mozilla/5.0 (Windows; U; MSIE 9.0; WIndows NT 9.0; en-US))",
-            "Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 7.1; Trident/5.0)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; Media Center PC 6.0; InfoPath.3; MS-RTC LM 8; Zune 4.7)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; Media Center PC 6.0; InfoPath.3; MS-RTC LM 8; Zune 4.7",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 4.0; InfoPath.3; MS-RTC LM 8; .NET4.0C; .NET4.0E)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; chromeframe/12.0.742.112)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 2.0.50727; Media Center PC 6.0)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 2.0.50727; Media Center PC 6.0)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0; .NET CLR 2.0.50727; SLCC2; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 4.0; Tablet PC 2.0; InfoPath.3; .NET4.0C; .NET4.0E)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; yie8)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; InfoPath.2; .NET CLR 1.1.4322; .NET4.0C; Tablet PC 2.0)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; FunWebProducts)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; chromeframe/13.0.782.215)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; chromeframe/11.0.696.57)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0) chromeframe/10.0.648.205",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.1; SV1; .NET CLR 2.8.52393; WOW64; en-US)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0; chromeframe/11.0.696.57)",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/4.0; GTB7.4; InfoPath.3; SV1; .NET CLR 3.1.76908; WOW64; en-US)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.2; SV1; .NET CLR 3.3.69573; WOW64; en-US)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 1.0.3705; .NET CLR 1.1.4322)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; InfoPath.1; SV1; .NET CLR 3.8.36217; WOW64; en-US)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; .NET CLR 2.7.58687; SLCC2; Media Center PC 5.0; Zune 3.4; Tablet PC 3.6; InfoPath.3)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.2; Trident/4.0; Media Center PC 4.0; SLCC1; .NET CLR 3.0.04320)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 1.1.4322)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; InfoPath.2; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 2.0.50727)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; SLCC1; .NET CLR 1.1.4322)",
-            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.0; Trident/4.0; InfoPath.1; SV1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 3.0.04506.30)",
-            "Mozilla/5.0 (compatible; MSIE 7.0; Windows NT 5.0; Trident/4.0; FBSMTWB; .NET CLR 2.0.34861; .NET CLR 3.0.3746.3218; .NET CLR 3.5.33652; msn OptimizedIE8;ENUS)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.2; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; Media Center PC 6.0; InfoPath.2; MS-RTC LM 8)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; Media Center PC 6.0; InfoPath.2; MS-RTC LM 8",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; Media Center PC 6.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET4.0C)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; InfoPath.3; .NET4.0C; .NET4.0E; .NET CLR 3.5.30729; .NET CLR 3.0.30729; MS-RTC LM 8)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; InfoPath.2)",
-            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 3.0)",
-        ],
-        "safari": [
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A",
-            "Mozilla/5.0 (iPad; CPU OS 6_0 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10A5355d Safari/8536.25",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_6_8) AppleWebKit/537.13+ (KHTML, like Gecko) Version/5.1.7 Safari/534.57.2",
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_3) AppleWebKit/534.55.3 (KHTML, like Gecko) Version/5.1.3 Safari/534.53.10",
-            "Mozilla/5.0 (iPad; CPU OS 5_1 like Mac OS X) AppleWebKit/534.46 (KHTML, like Gecko ) Version/5.1 Mobile/9B176 Safari/7534.48.3",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_8; de-at) AppleWebKit/533.21.1 (KHTML, like Gecko) Version/5.0.5 Safari/533.21.1",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; da-dk) AppleWebKit/533.21.1 (KHTML, like Gecko) Version/5.0.5 Safari/533.21.1",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; tr-TR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; ko-KR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; fr-FR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; cs-CZ) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; PPC Mac OS X 10_5_8; zh-cn) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; PPC Mac OS X 10_5_8; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; zh-cn) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; sv-se) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; ko-kr) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; it-it) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; fr-fr) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; es-es) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; en-us) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; en-gb) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; de-de) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; sv-SE) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; de-DE) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; hu-HU) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; de-DE) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ru-RU) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; it-IT) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; en-us) AppleWebKit/534.16+ (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; fr-ch) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_5; de-de) AppleWebKit/534.15+ (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_5; ar) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Android 2.2; Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; zh-HK) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; tr-TR) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; nb-NO) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 6.0; fr-FR) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; zh-TW) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ru-RU) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_5_8; zh-cn) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
-        ],
-    }
+import platform
+
+__all__ = [
+    "Param",
+]
+
+
+class Param:
+    """用于存储项目中需要的参数变量设置"""
+
+    retry_num = 3
+    retry_time_min = 200
+    retry_time_max = 1000
+
+    aiohttp_retry_times_default = 3
+
+    # 部署运行的平台为 win 或 linux
+    IS_WINDOWS = platform.system().lower() == "windows"
+    IS_LINUX = platform.system().lower() == "linux"
+
+    # 动态隧道代理配置示例
+    dynamic_proxy_conf_example = {
+        "proxy": "动态隧道代理地址：***.***.com:*****",
+        "username": "隧道代理用户名",
+        "password": "对应用户的密码",
+    }
+    # 独享代理配置示例
+    exclusive_proxy_conf_example = {
+        "proxy": "独享代理地址：'http://***.com/api/***&num=100&format=json'",
+        "username": "独享代理用户名",
+        "password": "对应用户的密码",
+        "index": "需要返回的独享代理的索引",
+    }
+
+    # aiohttp 配置示例
+    aiohttp_conf_example = {
+        "timeout": 5,
+        "proxy": "127.0.0.1:80",
+        "sleep": 1,
+        "retry_times": 3,
+    }
+
+    charset_collate_map = {
+        # utf8mb4_unicode_ci 也是经常使用的
+        "utf8mb4": "utf8mb4_general_ci",
+        "utf8": "utf8_general_ci",
+        "gbk": "gbk_chinese_ci",
+        "latin1": "latin1_swedish_ci",
+        "utf16": "utf16_general_ci",
+        "utf16le": "utf16le_general_ci",
+        "cp1251": "cp1251_general_ci",
+        "euckr": "euckr_korean_ci",
+        "greek": "greek_general_ci",
+    }
+
+    # 随机请求头列表
+    fake_useragent_dict = {
+        "chrome": [
+            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2228.0 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.1 Safari/537.36",
+            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2227.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2226.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.4; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2225.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2225.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2224.3 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/40.0.2214.93 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2062.124 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.67 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.67 Safari/537.36",
+            "Mozilla/5.0 (X11; OpenBSD i386) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.125 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1944.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.3319.102 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.2309.372 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.2117.157 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.47 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1866.237 Safari/537.36",
+            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.137 Safari/4E423F",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.116 Safari/537.36 Mozilla/5.0 (iPad; U; CPU OS 3_2 like Mac OS X; en-us) AppleWebKit/531.21.10 (KHTML, like Gecko) Version/4.0.4 Mobile/7B334b Safari/531.21.10",
+            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/33.0.1750.517 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1667.0 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1664.3 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/32.0.1664.3 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/31.0.1650.16 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/31.0.1623.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/30.0.1599.17 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.62 Safari/537.36",
+            "Mozilla/5.0 (X11; CrOS i686 4319.74.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.57 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.2 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1468.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1467.0 Safari/537.36",
+            "Mozilla/a/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1464.0 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1500.55 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.90 Safari/537.36",
+            "Mozilla/5.0 (X11; NetBSD) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
+            "Mozilla/5.0 (X11; CrOS i686 3912.101.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.116 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1312.60 Safari/537.17",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_2) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1309.0 Safari/537.17",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.15 (KHTML, like Gecko) Chrome/24.0.1295.0 Safari/537.15",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.14 (KHTML, like Gecko) Chrome/24.0.1292.0 Safari/537.14",
+        ],
+        "opera": [
+            "Opera/9.80 (X11; Linux i686; Ubuntu/14.10) Presto/2.12.388 Version/12.16",
+            "Opera/9.80 (Windows NT 6.0) Presto/2.12.388 Version/12.14",
+            "Mozilla/5.0 (Windows NT 6.0; rv:2.0) Gecko/20100101 Firefox/4.0 Opera 12.14",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0) Opera 12.14",
+            "Opera/12.80 (Windows NT 5.1; U; en) Presto/2.10.289 Version/12.02",
+            "Opera/9.80 (Windows NT 6.1; U; es-ES) Presto/2.9.181 Version/12.00",
+            "Opera/9.80 (Windows NT 5.1; U; zh-sg) Presto/2.9.181 Version/12.00",
+            "Opera/12.0(Windows NT 5.2;U;en)Presto/22.9.168 Version/12.00",
+            "Opera/12.0(Windows NT 5.1;U;en)Presto/22.9.168 Version/12.00",
+            "Mozilla/5.0 (Windows NT 5.1) Gecko/20100101 Firefox/14.0 Opera/12.0",
+            "Opera/9.80 (Windows NT 6.1; WOW64; U; pt) Presto/2.10.229 Version/11.62",
+            "Opera/9.80 (Windows NT 6.0; U; pl) Presto/2.10.229 Version/11.62",
+            "Opera/9.80 (Macintosh; Intel Mac OS X 10.6.8; U; fr) Presto/2.9.168 Version/11.52",
+            "Opera/9.80 (Macintosh; Intel Mac OS X 10.6.8; U; de) Presto/2.9.168 Version/11.52",
+            "Opera/9.80 (Windows NT 5.1; U; en) Presto/2.9.168 Version/11.51",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; de) Opera 11.51",
+            "Opera/9.80 (X11; Linux x86_64; U; fr) Presto/2.9.168 Version/11.50",
+            "Opera/9.80 (X11; Linux i686; U; hu) Presto/2.9.168 Version/11.50",
+            "Opera/9.80 (X11; Linux i686; U; ru) Presto/2.8.131 Version/11.11",
+            "Opera/9.80 (X11; Linux i686; U; es-ES) Presto/2.8.131 Version/11.11",
+            "Mozilla/5.0 (Windows NT 5.1; U; en; rv:1.8.1) Gecko/20061208 Firefox/5.0 Opera 11.11",
+            "Opera/9.80 (X11; Linux x86_64; U; bg) Presto/2.8.131 Version/11.10",
+            "Opera/9.80 (Windows NT 6.0; U; en) Presto/2.8.99 Version/11.10",
+            "Opera/9.80 (Windows NT 5.1; U; zh-tw) Presto/2.8.131 Version/11.10",
+            "Opera/9.80 (Windows NT 6.1; Opera Tablet/15165; U; en) Presto/2.8.149 Version/11.1",
+            "Opera/9.80 (X11; Linux x86_64; U; Ubuntu/10.10 (maverick); pl) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (X11; Linux i686; U; ja) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (X11; Linux i686; U; fr) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.1; U; zh-tw) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.1; U; zh-cn) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.1; U; sv) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.1; U; en-US) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.1; U; cs) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 6.0; U; pl) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 5.2; U; ru) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 5.1; U;) Presto/2.7.62 Version/11.01",
+            "Opera/9.80 (Windows NT 5.1; U; cs) Presto/2.7.62 Version/11.01",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US; rv:1.9.2.13) Gecko/20101213 Opera/9.80 (Windows NT 6.1; U; zh-tw) Presto/2.7.62 Version/11.01",
+            "Mozilla/5.0 (Windows NT 6.1; U; nl; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6 Opera 11.01",
+            "Mozilla/5.0 (Windows NT 6.1; U; de; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6 Opera 11.01",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; de) Opera 11.01",
+            "Opera/9.80 (X11; Linux x86_64; U; pl) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (X11; Linux i686; U; it) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1; U; zh-cn) Presto/2.6.37 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1; U; pl) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1; U; ko) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1; U; fi) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1; U; en-GB) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.1 x64; U; en) Presto/2.7.62 Version/11.00",
+            "Opera/9.80 (Windows NT 6.0; U; en) Presto/2.7.39 Version/11.00",
+        ],
+        "firefox": [
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:40.0) Gecko/20100101 Firefox/40.1",
+            "Mozilla/5.0 (Windows NT 6.3; rv:36.0) Gecko/20100101 Firefox/36.0",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10; rv:33.0) Gecko/20100101 Firefox/33.0",
+            "Mozilla/5.0 (X11; Linux i586; rv:31.0) Gecko/20100101 Firefox/31.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:31.0) Gecko/20130401 Firefox/31.0",
+            "Mozilla/5.0 (Windows NT 5.1; rv:31.0) Gecko/20100101 Firefox/31.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:29.0) Gecko/20120101 Firefox/29.0",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:25.0) Gecko/20100101 Firefox/29.0",
+            "Mozilla/5.0 (X11; OpenBSD amd64; rv:28.0) Gecko/20100101 Firefox/28.0",
+            "Mozilla/5.0 (X11; Linux x86_64; rv:28.0) Gecko/20100101  Firefox/28.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:27.3) Gecko/20130101 Firefox/27.3",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:27.0) Gecko/20121011 Firefox/27.0",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:25.0) Gecko/20100101 Firefox/25.0",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.6; rv:25.0) Gecko/20100101 Firefox/25.0",
+            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:24.0) Gecko/20100101 Firefox/24.0",
+            "Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.8; rv:24.0) Gecko/20100101 Firefox/24.0",
+            "Mozilla/5.0 (Windows NT 6.2; rv:22.0) Gecko/20130405 Firefox/23.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:23.0) Gecko/20130406 Firefox/23.0",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:23.0) Gecko/20131011 Firefox/23.0",
+            "Mozilla/5.0 (Windows NT 6.2; rv:22.0) Gecko/20130405 Firefox/22.0",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:22.0) Gecko/20130328 Firefox/22.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:22.0) Gecko/20130405 Firefox/22.0",
+            "Mozilla/5.0 (Microsoft Windows NT 6.2.9200.0); rv:22.0) Gecko/20130405 Firefox/22.0",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/21.0.1",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/21.0.1",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:21.0.0) Gecko/20121011 Firefox/21.0.0",
+            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:21.0) Gecko/20130331 Firefox/21.0",
+            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (X11; Linux i686; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.2; WOW64; rv:21.0) Gecko/20130514 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.2; rv:21.0) Gecko/20130326 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130401 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130331 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20130330 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20130401 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20130328 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20130401 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20130331 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 5.1; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 5.0; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.8; rv:21.0) Gecko/20100101 Firefox/21.0",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64;) Gecko/20100101 Firefox/20.0",
+            "Mozilla/5.0 (Windows x86; rv:19.0) Gecko/20100101 Firefox/19.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:6.0) Gecko/20100101 Firefox/19.0",
+            "Mozilla/5.0 (Windows NT 6.1; rv:14.0) Gecko/20100101 Firefox/18.0.1",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:18.0)  Gecko/20100101 Firefox/18.0",
+            "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:17.0) Gecko/20100101 Firefox/17.0.6",
+        ],
+        "internetexplorer": [
+            "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; AS; rv:11.0) like Gecko",
+            "Mozilla/5.0 (compatible, MSIE 11, Windows NT 6.3; Trident/7.0;  rv:11.0) like Gecko",
+            "Mozilla/5.0 (compatible; MSIE 10.6; Windows NT 6.1; Trident/5.0; InfoPath.2; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 2.0.50727) 3gpp-gba UNTRUSTED/1.0",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 7.0; InfoPath.3; .NET CLR 3.1.40767; Trident/6.0; en-IN)",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/5.0)",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/4.0; InfoPath.2; SV1; .NET CLR 2.0.50727; WOW64)",
+            "Mozilla/5.0 (compatible; MSIE 10.0; Macintosh; Intel Mac OS X 10_7_3; Trident/6.0)",
+            "Mozilla/4.0 (Compatible; MSIE 8.0; Windows NT 5.2; Trident/6.0)",
+            "Mozilla/4.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/5.0)",
+            "Mozilla/1.22 (compatible; MSIE 10.0; Windows 3.1)",
+            "Mozilla/5.0 (Windows; U; MSIE 9.0; WIndows NT 9.0; en-US))",
+            "Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 7.1; Trident/5.0)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; Media Center PC 6.0; InfoPath.3; MS-RTC LM 8; Zune 4.7)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; Media Center PC 6.0; InfoPath.3; MS-RTC LM 8; Zune 4.7",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 4.0; InfoPath.3; MS-RTC LM 8; .NET4.0C; .NET4.0E)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; chromeframe/12.0.742.112)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 2.0.50727; Media Center PC 6.0)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 2.0.50727; Media Center PC 6.0)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0; .NET CLR 2.0.50727; SLCC2; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 4.0; Tablet PC 2.0; InfoPath.3; .NET4.0C; .NET4.0E)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; yie8)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; InfoPath.2; .NET CLR 1.1.4322; .NET4.0C; Tablet PC 2.0)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; FunWebProducts)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; chromeframe/13.0.782.215)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; chromeframe/11.0.696.57)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0) chromeframe/10.0.648.205",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.1; SV1; .NET CLR 2.8.52393; WOW64; en-US)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0; chromeframe/11.0.696.57)",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/4.0; GTB7.4; InfoPath.3; SV1; .NET CLR 3.1.76908; WOW64; en-US)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.2; SV1; .NET CLR 3.3.69573; WOW64; en-US)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET CLR 1.0.3705; .NET CLR 1.1.4322)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; InfoPath.1; SV1; .NET CLR 3.8.36217; WOW64; en-US)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0; .NET CLR 2.7.58687; SLCC2; Media Center PC 5.0; Zune 3.4; Tablet PC 3.6; InfoPath.3)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.2; Trident/4.0; Media Center PC 4.0; SLCC1; .NET CLR 3.0.04320)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 1.1.4322)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; InfoPath.2; SLCC1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 2.0.50727)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 1.1.4322; .NET CLR 2.0.50727)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.1; SLCC1; .NET CLR 1.1.4322)",
+            "Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 5.0; Trident/4.0; InfoPath.1; SV1; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; .NET CLR 3.0.04506.30)",
+            "Mozilla/5.0 (compatible; MSIE 7.0; Windows NT 5.0; Trident/4.0; FBSMTWB; .NET CLR 2.0.34861; .NET CLR 3.0.3746.3218; .NET CLR 3.5.33652; msn OptimizedIE8;ENUS)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.2; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; Media Center PC 6.0; InfoPath.2; MS-RTC LM 8)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; Media Center PC 6.0; InfoPath.2; MS-RTC LM 8",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; Media Center PC 6.0; .NET CLR 3.5.30729; .NET CLR 3.0.30729; .NET4.0C)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; InfoPath.3; .NET4.0C; .NET4.0E; .NET CLR 3.5.30729; .NET CLR 3.0.30729; MS-RTC LM 8)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; InfoPath.2)",
+            "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; Zune 3.0)",
+        ],
+        "safari": [
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A",
+            "Mozilla/5.0 (iPad; CPU OS 6_0 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10A5355d Safari/8536.25",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_6_8) AppleWebKit/537.13+ (KHTML, like Gecko) Version/5.1.7 Safari/534.57.2",
+            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_3) AppleWebKit/534.55.3 (KHTML, like Gecko) Version/5.1.3 Safari/534.53.10",
+            "Mozilla/5.0 (iPad; CPU OS 5_1 like Mac OS X) AppleWebKit/534.46 (KHTML, like Gecko ) Version/5.1 Mobile/9B176 Safari/7534.48.3",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_8; de-at) AppleWebKit/533.21.1 (KHTML, like Gecko) Version/5.0.5 Safari/533.21.1",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; da-dk) AppleWebKit/533.21.1 (KHTML, like Gecko) Version/5.0.5 Safari/533.21.1",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; tr-TR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; ko-KR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; fr-FR) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; cs-CZ) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; PPC Mac OS X 10_5_8; zh-cn) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; PPC Mac OS X 10_5_8; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; zh-cn) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; sv-se) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; ko-kr) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; ja-jp) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; it-it) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; fr-fr) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; es-es) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; en-us) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; en-gb) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; de-de) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.4 Safari/533.20.27",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; sv-SE) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; de-DE) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; hu-HU) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; de-DE) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ru-RU) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ja-JP) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; it-IT) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US) AppleWebKit/533.20.25 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_7; en-us) AppleWebKit/534.16+ (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_6; fr-ch) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_5; de-de) AppleWebKit/534.15+ (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_6_5; ar) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Android 2.2; Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.3 Safari/533.19.4",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; zh-HK) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; tr-TR) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; nb-NO) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 6.0; fr-FR) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; zh-TW) AppleWebKit/533.19.4 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Windows; U; Windows NT 5.1; ru-RU) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+            "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10_5_8; zh-cn) AppleWebKit/533.18.1 (KHTML, like Gecko) Version/5.0.2 Safari/533.18.5",
+        ],
+    }
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/postgreserrhandle.py` & `ayugespidertools-3.9.8/ayugespidertools/common/postgreserrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.9.8/ayugespidertools/common/sqlformat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,89 @@
-from typing import Any, Dict, Literal, Optional, Tuple, Union
-
-__all__ = [
-    "AboutSql",
-]
-
-SqlModeStr = Literal["and", "or"]
-
-
-class AboutSql:
-    """sql 相关处理: sql 语句的管理方法，
-    这里的 sql 拼接只能做到最简单的逻辑，如果需要灵活或稍复杂的情况，请参考 directsql, python-sql, pypika
-    或 pymilk 等第三方类似功能库的实现方法，以后会再优化此场景
-    """
-
-    @staticmethod
-    def select_generate(
-        db_table: str,
-        key: list,
-        rule: Dict[str, Any],
-        base: SqlModeStr = "and",
-        order_by: Optional[str] = None,
-        limit: Union[bool, int] = False,
-    ) -> Tuple[str, tuple]:
-        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 查询语句（适用于简单情况）
-
-        Args:
-            db_table: 需要查询的表名称
-            key: 需要查询的关键字段
-            rule: 查询需要的规则
-            base: 在有多个查询规则时，选择 "and" 或 "or"，默认 "and"
-            order_by: 排序的 key 值
-            limit: limit 限制，默认无限制（查询所有）；如果需要则指定 int 值即可
-
-        Returns:
-            1). sql: 生成的 sql 语句
-            2). 查询字段的参数名称
-        """
-        select_key = ", ".join(f"`{k}`" for k in key)
-        select_key = select_key.replace("""`count(*)`""", "count(*)")
-        select_key = select_key.replace("""`count(1)`""", "count(1)")
-
-        _base = f" {base} "
-        select_where = _base.join(
-            f"`{k.split('|')[0]}`{k.split('|')[1]}%s" for k in rule
-        )
-
-        _where = f"where {select_where}" if select_where else ""
-        _order_by = f"order by {order_by}" if order_by else ""
-        _limit = f"limit {limit}" if limit else ""
-        sql = f"""select {select_key} from {db_table} {_where} {_order_by} {_limit}"""
-        return sql, tuple(rule.values())
-
-    @staticmethod
-    def insert_generate(db_table: str, data: dict) -> Tuple[str, tuple]:
-        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 插入语句
-
-        Args:
-            db_table: 需要插入的表名称
-            data: 需要插入的关键字段，key: 数据表字段；value: 需插入的参数名
-
-        Returns:
-            1). sql: 生成的 sql 语句
-            2). 新增字段的参数名称
-        """
-        keys = ", ".join(f"`{k}`" for k in data)
-        values = ", ".join(["%s"] * len(data))
-        sql = f"""insert into `{db_table}` ({keys}) values ({values})"""
-        return sql, tuple(data.values())
-
-    @staticmethod
-    def update_generate(
-        db_table: str, data: dict, rule: Dict[str, Any], base: SqlModeStr = "and"
-    ) -> Tuple[str, tuple]:
-        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 更新语句
-
-        Args:
-            db_table: 需要插入的表名称
-            data: 需要更新的 key 和 value 值
-            rule: 更新需要的规则
-            base: 在有多个查询规则时，选择 "and" 或 "or"，默认 "and"
-
-        Returns:
-            1). sql: 生成的 sql 语句
-            2). 更新字段的参数名称
-        """
-        update_set = ", ".join(f"`{k}`=%s" for k in data)
-
-        _base = f" {base} "
-        update_where = _base.join(f"`{k}`=%s" for k in rule)
-        sql = f"""update `{db_table}` set {update_set} where {update_where}"""
-        return sql, tuple(data.values()) + tuple(rule.values())
+from typing import Any, Dict, Literal, Optional, Tuple, Union
+
+__all__ = [
+    "AboutSql",
+]
+
+SqlModeStr = Literal["and", "or"]
+
+
+class AboutSql:
+    """sql 语句的生成方法，只适用简单场景。"""
+
+    @staticmethod
+    def select_generate(
+        db_table: str,
+        key: list,
+        rule: Dict[str, Any],
+        base: SqlModeStr = "and",
+        order_by: Optional[str] = None,
+        limit: Union[bool, int] = False,
+    ) -> Tuple[str, tuple]:
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 查询语句
+
+        Args:
+            db_table: 需要查询的表名称
+            key: 需要查询的关键字段
+            rule: 查询需要的规则
+            base: 多查询条件
+            order_by: 排序的 key 值
+            limit: limit
+
+        Returns:
+            1). sql: 生成的 sql 语句
+            2). 查询字段的参数名称
+        """
+        select_key = ", ".join(f"`{k}`" for k in key)
+        select_key = select_key.replace("""`count(*)`""", "count(*)")
+        select_key = select_key.replace("""`count(1)`""", "count(1)")
+
+        _base = f" {base} "
+        select_where = _base.join(
+            f"`{k.split('|')[0]}`{k.split('|')[1]}%s" for k in rule
+        )
+
+        _where = f"where {select_where}" if select_where else ""
+        _order_by = f"order by {order_by}" if order_by else ""
+        _limit = f"limit {limit}" if limit else ""
+        sql = f"""select {select_key} from {db_table} {_where} {_order_by} {_limit}"""
+        return sql, tuple(rule.values())
+
+    @staticmethod
+    def insert_generate(db_table: str, data: dict) -> Tuple[str, tuple]:
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 插入语句
+
+        Args:
+            db_table: 需要插入的表名称
+            data: 需要插入的关键字段，key: 数据表字段；value: 需插入的参数名
+
+        Returns:
+            1). sql: 生成的 sql 语句
+            2). 新增字段的参数名称
+        """
+        keys = ", ".join(f"`{k}`" for k in data)
+        values = ", ".join(["%s"] * len(data))
+        sql = f"""insert into `{db_table}` ({keys}) values ({values})"""
+        return sql, tuple(data.values())
+
+    @staticmethod
+    def update_generate(
+        db_table: str, data: dict, rule: Dict[str, Any], base: SqlModeStr = "and"
+    ) -> Tuple[str, tuple]:
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 更新语句
+
+        Args:
+            db_table: 需要插入的表名称
+            data: 需要更新的 key 和 value 值
+            rule: 更新需要的规则
+            base: 多查询条件
+
+        Returns:
+            1). sql: 生成的 sql 语句
+            2). 更新字段的参数名称
+        """
+        update_set = ", ".join(f"`{k}`=%s" for k in data)
+
+        _base = f" {base} "
+        update_where = _base.join(f"`{k}`=%s" for k in rule)
+        sql = f"""update `{db_table}` set {update_set} where {update_where}"""
+        return sql, tuple(data.values()) + tuple(rule.values())
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/typevars.py` & `ayugespidertools-3.9.8/ayugespidertools/common/typevars.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,213 +1,212 @@
-# Define your TypeVar here
-import threading
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, List, Literal, NamedTuple, Optional, TypeVar, Union
-
-from sqlalchemy import create_engine
-
-if TYPE_CHECKING:
-    import logging
-
-    from loguru import Logger
-
-    slogT = Union[Logger, logging.LoggerAdapter]
-
-NoneType = type(None)
-I_Str = TypeVar("I_Str", int, str)
-B_Str = TypeVar("B_Str", bytes, str)
-I_Str_N = TypeVar("I_Str_N", int, str, NoneType)
-Str_Lstr = TypeVar("Str_Lstr", str, List[str])
-
-AiohttpRequestMethodStr = Literal[
-    "GET", "POST", "PUT", "DELETE", "HEAD", "OPTIONS", "PATCH"
-]
-authMechanismStr = Literal[
-    "SCRAM-SHA-1", "SCRAM-SHA-256", "MONGODB-CR", "MONGODB-X509", "PLAIN"
-]
-MysqlEngineStr = Literal["InnoDB", "MyISAM", "MEMORY", "NDB", "ARCHIVE"]
-DataItemModeStr = Literal["normal", "namedtuple", "dict"]
-
-
-class DatabaseSingletonMeta(type):
-    _instances = {}
-    _lock = threading.Lock()
-
-    def __call__(cls, engine_url, *args, **kwargs):
-        if engine_url not in cls._instances:
-            with cls._lock:
-                if engine_url not in cls._instances:
-                    instance = super().__call__(engine_url, *args, **kwargs)
-                    cls._instances[engine_url] = instance
-        return cls._instances[engine_url]
-
-
-class DatabaseEngineClass(metaclass=DatabaseSingletonMeta):
-    """database engine 单例模式：同一个 engine_url 只能存在一个实例"""
-
-    def __init__(self, engine_url, *args, **kwargs):
-        self.engine = create_engine(
-            engine_url, pool_pre_ping=True, pool_recycle=3600 * 7, *args, **kwargs
-        )
-
-
-class MysqlConf(NamedTuple):
-    host: str
-    port: int
-    user: str
-    password: str
-    database: str
-    engine: MysqlEngineStr = "InnoDB"
-    charset: str = "utf8mb4"
-    collate: str = "utf8mb4_general_ci"
-    odku_enable: bool = False
-
-
-class MongoDBConf(NamedTuple):
-    host: str = ""
-    port: int = 27017
-    user: str = ""
-    password: str = ""
-    database: Optional[str] = None
-    authsource: Optional[str] = None
-    authMechanism: authMechanismStr = "SCRAM-SHA-1"
-    uri: Optional[str] = None
-
-
-class PostgreSQLConf(NamedTuple):
-    host: str
-    port: int
-    user: str
-    password: str
-    database: Optional[str] = None
-    charset: str = "UTF8"
-
-
-class ESConf(NamedTuple):
-    hosts: str
-    index_class: dict
-    user: Optional[str] = None
-    password: Optional[str] = None
-    init: bool = False
-    verify_certs: bool = False
-    ca_certs: str = None
-    client_cert: str = None
-    client_key: str = None
-    ssl_assert_fingerprint: str = None
-
-
-class OracleConf(NamedTuple):
-    host: str
-    port: int
-    user: str
-    password: str
-    service_name: Optional[str] = None
-    encoding: str = "utf8"
-    thick_lib_dir: Union[bool, str] = False
-
-
-class AiohttpConf(NamedTuple):
-    sleep: int
-    proxy: str
-    proxy_auth: str
-    proxy_headers: dict
-    retry_times: int
-    limit: int
-    ssl: bool
-    verify_ssl: bool
-    limit_per_host: int
-    allow_redirects: bool
-    timeout: Optional[int] = None
-
-
-class AlterItemTable(NamedTuple):
-    """用于描述 AlterItem 中的 table 字段
-
-    Attributes:
-        name: table name
-        notes: table name 的注释
-    """
-
-    name: str
-    notes: str = ""
-
-
-class AlterItem(NamedTuple):
-    new_item: dict
-    notes_dic: dict
-    table: AlterItemTable
-    is_namedtuple: bool = False
-
-
-@dataclass
-class AiohttpRequestArgs:
-    url: Optional[str] = field(default=None)
-    headers: Union[dict, None] = field(default=None)
-    cookies: Union[dict, None] = field(default=None)
-    method: AiohttpRequestMethodStr = field(default="GET")
-    timeout: Union[int, None] = field(default=None)
-    data: Union[dict, str, None] = field(default=None)
-    proxy: Union[str, None] = field(default=None)
-    proxy_auth: Union[str, None] = field(default=None)
-    proxy_headers: Union[dict, None] = field(default=None)
-
-
-class MQConf(NamedTuple):
-    host: str
-    port: int
-    username: str
-    password: str
-    virtualhost: str = "/"
-    heartbeat: int = 0
-    socket_timeout: int = 1
-    queue: Optional[str] = None
-    durable: bool = True
-    exclusive: bool = False
-    auto_delete: bool = False
-    exchange: Optional[str] = None
-    routing_key: Optional[str] = None
-    content_type: str = "text/plain"
-    delivery_mode: int = 1
-    mandatory: bool = True
-
-
-class DynamicProxyConf(NamedTuple):
-    proxy: str
-    username: str
-    password: str
-
-
-class ExclusiveProxyConf(NamedTuple):
-    proxy: str
-    username: str
-    password: str
-    index: int
-
-
-class KafkaConf(NamedTuple):
-    bootstrap_servers: str
-    topic: str
-    key: str
-
-
-class OssConf(NamedTuple):
-    access_key: str
-    access_secret: str
-    endpoint: str
-    bucket: str
-    doc: Optional[str] = None
-    upload_fields_suffix: str = "_file_url"
-    oss_fields_prefix: str = "_"
-    full_link_enable: bool = False
-
-
-class FieldAlreadyExistsError(Exception):
-    def __init__(self, field_name: str):
-        self.field_name = field_name
-        self.message = f"字段 {field_name} 已存在！"
-        super().__init__(self.message)
-
-
-class EmptyKeyError(Exception):
-    def __init__(self):
-        self.message = "字段名不能为空！"
-        super().__init__(self.message)
+# Define your Types here
+import threading
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, List, Literal, NamedTuple, Optional, TypeVar, Union
+
+from sqlalchemy import create_engine
+
+if TYPE_CHECKING:
+    from loguru import Logger
+    from scrapy.utils.log import SpiderLoggerAdapter
+
+    slogT = Union[Logger, SpiderLoggerAdapter]
+
+NoneType = type(None)
+I_Str = TypeVar("I_Str", int, str)
+B_Str = TypeVar("B_Str", bytes, str)
+I_Str_N = TypeVar("I_Str_N", int, str, NoneType)
+Str_Lstr = TypeVar("Str_Lstr", str, List[str])
+
+AiohttpRequestMethodStr = Literal[
+    "GET", "POST", "PUT", "DELETE", "HEAD", "OPTIONS", "PATCH"
+]
+authMechanismStr = Literal[
+    "SCRAM-SHA-1", "SCRAM-SHA-256", "MONGODB-CR", "MONGODB-X509", "PLAIN"
+]
+MysqlEngineStr = Literal["InnoDB", "MyISAM", "MEMORY", "NDB", "ARCHIVE"]
+DataItemModeStr = Literal["normal", "namedtuple", "dict"]
+
+
+class DatabaseSingletonMeta(type):
+    _instances = {}
+    _lock = threading.Lock()
+
+    def __call__(cls, engine_url, *args, **kwargs):
+        if engine_url not in cls._instances:
+            with cls._lock:
+                if engine_url not in cls._instances:
+                    instance = super().__call__(engine_url, *args, **kwargs)
+                    cls._instances[engine_url] = instance
+        return cls._instances[engine_url]
+
+
+class DatabaseEngineClass(metaclass=DatabaseSingletonMeta):
+    """database engine 单例模式：同一个 engine_url 只能存在一个实例"""
+
+    def __init__(self, engine_url, *args, **kwargs):
+        self.engine = create_engine(
+            engine_url, pool_pre_ping=True, pool_recycle=3600 * 7, *args, **kwargs
+        )
+
+
+class MysqlConf(NamedTuple):
+    host: str
+    port: int
+    user: str
+    password: str
+    database: str
+    engine: MysqlEngineStr = "InnoDB"
+    charset: str = "utf8mb4"
+    collate: str = "utf8mb4_general_ci"
+    odku_enable: bool = False
+
+
+class MongoDBConf(NamedTuple):
+    host: str = ""
+    port: int = 27017
+    user: str = ""
+    password: str = ""
+    database: Optional[str] = None
+    authsource: Optional[str] = None
+    authMechanism: authMechanismStr = "SCRAM-SHA-1"
+    uri: Optional[str] = None
+
+
+class PostgreSQLConf(NamedTuple):
+    host: str
+    port: int
+    user: str
+    password: str
+    database: Optional[str] = None
+    charset: str = "UTF8"
+
+
+class ESConf(NamedTuple):
+    hosts: str
+    index_class: dict
+    user: Optional[str] = None
+    password: Optional[str] = None
+    init: bool = False
+    verify_certs: bool = False
+    ca_certs: str = None
+    client_cert: str = None
+    client_key: str = None
+    ssl_assert_fingerprint: str = None
+
+
+class OracleConf(NamedTuple):
+    host: str
+    port: int
+    user: str
+    password: str
+    service_name: Optional[str] = None
+    encoding: str = "utf8"
+    thick_lib_dir: Union[bool, str] = False
+
+
+class AiohttpConf(NamedTuple):
+    sleep: int
+    proxy: str
+    proxy_auth: str
+    proxy_headers: dict
+    retry_times: int
+    limit: int
+    ssl: bool
+    verify_ssl: bool
+    limit_per_host: int
+    allow_redirects: bool
+    timeout: Optional[int] = None
+
+
+class AlterItemTable(NamedTuple):
+    """用于描述 AlterItem 中的 table 字段
+
+    Attributes:
+        name: table name
+        notes: table name 的注释
+    """
+
+    name: str
+    notes: str = ""
+
+
+class AlterItem(NamedTuple):
+    new_item: dict
+    notes_dic: dict
+    table: AlterItemTable
+    is_namedtuple: bool = False
+
+
+@dataclass
+class AiohttpRequestArgs:
+    url: Optional[str] = field(default=None)
+    headers: Union[dict, None] = field(default=None)
+    cookies: Union[dict, None] = field(default=None)
+    method: AiohttpRequestMethodStr = field(default="GET")
+    timeout: Union[int, None] = field(default=None)
+    data: Union[dict, str, None] = field(default=None)
+    proxy: Union[str, None] = field(default=None)
+    proxy_auth: Union[str, None] = field(default=None)
+    proxy_headers: Union[dict, None] = field(default=None)
+
+
+class MQConf(NamedTuple):
+    host: str
+    port: int
+    username: str
+    password: str
+    virtualhost: str = "/"
+    heartbeat: int = 0
+    socket_timeout: int = 1
+    queue: Optional[str] = None
+    durable: bool = True
+    exclusive: bool = False
+    auto_delete: bool = False
+    exchange: Optional[str] = None
+    routing_key: Optional[str] = None
+    content_type: str = "text/plain"
+    delivery_mode: int = 1
+    mandatory: bool = True
+
+
+class DynamicProxyConf(NamedTuple):
+    proxy: str
+    username: str
+    password: str
+
+
+class ExclusiveProxyConf(NamedTuple):
+    proxy: str
+    username: str
+    password: str
+    index: int
+
+
+class KafkaConf(NamedTuple):
+    bootstrap_servers: str
+    topic: str
+    key: str
+
+
+class OssConf(NamedTuple):
+    access_key: str
+    access_secret: str
+    endpoint: str
+    bucket: str
+    doc: Optional[str] = None
+    upload_fields_suffix: str = "_file_url"
+    oss_fields_prefix: str = "_"
+    full_link_enable: bool = False
+
+
+class FieldAlreadyExistsError(Exception):
+    def __init__(self, field_name: str):
+        self.field_name = field_name
+        self.message = f"字段 {field_name} 已存在！"
+        super().__init__(self.message)
+
+
+class EmptyKeyError(Exception):
+    def __init__(self):
+        self.message = "字段名不能为空！"
+        super().__init__(self.message)
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/common/utils.py` & `ayugespidertools-3.9.8/ayugespidertools/common/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,358 +1,346 @@
-import json
-import random
-from functools import lru_cache
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, List, Literal, Optional, Union
-from urllib.parse import urlparse
-
-import requests
-
-from ayugespidertools.common.encryption import EncryptOperation
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
-from ayugespidertools.config import logger
-from ayugespidertools.extras.ext import AppConfManageMixin
-from ayugespidertools.formatdata import DataHandle
-
-__all__ = ["ToolsForAyu"]
-
-if TYPE_CHECKING:
-    from scrapy.http import Response
-    from scrapy.http.headers import Headers
-
-    from ayugespidertools.common.typevars import Str_Lstr
-
-RemoteFormatStr = Literal["json", "hcl", "yaml", "xml"]
-RemoteTypeStr = Literal["consul", "nacos"]
-RemoteConfNameStr = Literal[
-    "mongodb",
-    "mongodb:uri",
-    "mysql",
-    "postgresql",
-    "elasticsearch",
-    "oracle",
-    "oss:ali",
-    "rabbitmq",
-    "kafka",
-    "dynamicproxy",
-    "exclusiveproxy",
-]
-
-
-class ToolsForAyu(AppConfManageMixin):
-    """这里用于存放框架所依赖的方法"""
-
-    @classmethod
-    @lru_cache(maxsize=16)
-    def get_remote_kvs(
-        cls,
-        url: str,
-        remote_type: RemoteTypeStr = "consul",
-        token: Optional[str] = None,
-    ) -> str:
-        """获取远程配置中的 key_values 信息
-
-        Args:
-            url: 获取 kvs 所需的 url
-            remote_type: 配置类型
-            token: consul token or nacos token; nacos 的 token 值直接在 url 中构造即可
-
-        Returns:
-            1). 远程配置中 key_values 的详细信息
-        """
-        headers = {"X-Consul-Token": token} if remote_type == "consul" else None
-        try:
-            r = requests.get(
-                url,
-                headers=headers,
-                verify=False,
-                timeout=(
-                    Param.requests_req_timeout,
-                    Param.requests_res_timeout,
-                ),
-            )
-        except (
-            requests.exceptions.ConnectionError,
-            requests.exceptions.ConnectTimeout,
-        ) as e:
-            raise ValueError(f"请求远程配置 {remote_type} api 超时!") from e
-
-        url_params = urlparse(url).query
-        if remote_type == "consul":
-            if "raw" in url_params:
-                return r.text
-            return EncryptOperation.base64_decode(decode_data=r.json()[0]["Value"])
-        return r.text
-
-    @classmethod
-    def fetch_remote_conf(
-        cls,
-        conf_name: RemoteConfNameStr,
-        url: str,
-        format: RemoteFormatStr = "json",
-        remote_type: RemoteTypeStr = "consul",
-        token: Optional[str] = None,
-    ) -> dict:
-        """获取远程中的项目配置信息
-
-        Args:
-            conf_name: 需要获取的配置
-            token: consul token or nacos token
-            format: 远程配置中的格式，默认为 json 格式
-            remote_type: 配置类型
-            url: 获取远程配置所需的 url
-
-        Returns:
-            1). 远程应用配置中心中的配置信息（key 值为小写）
-        """
-        conf_value = cls.get_remote_kvs(url, remote_type, token)
-        if format == "json":
-            conf_data = json.loads(conf_value)
-        elif format == "xml":
-            conf_data = cls.xml_parser(conf_value)
-        elif format == "yaml":
-            conf_data = cls.yaml_parser(conf_value)
-        elif format == "hcl":
-            conf_data = cls.hcl_parser(conf_value)
-        else:
-            raise ValueError(f"{conf_name} 暂不支持该格式的配置")
-
-        _conf = conf_data.get(conf_name, {})
-        if not _conf:
-            logger.info(f"远程配置 {remote_type} 中未设置 {conf_name}")
-        return _conf
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_css(
-        cls,
-        response: "Response",
-        query: str,
-        get_all: bool = False,
-        return_selector: bool = False,
-    ):
-        """使用 scrapy 的 css 提取信息
-
-        Args:
-            response: scrapy response 或者是 selector 对象
-            query: css 提取的规则
-            get_all: 提取模式，默认：False, 提取符合中的一个
-            return_selector: 是否返回选择器对象
-
-        Returns:
-            1). 提取的内容
-        """
-        if return_selector:
-            return response.css(query)
-        if get_all:
-            return response.css(query).getall()
-        else:
-            return response.css(query).get(default="").strip()
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_xpath(
-        cls,
-        response: "Response",
-        query: str,
-        get_all: bool = False,
-        return_selector: bool = False,
-    ):
-        """使用 scrapy 的 xpath 提取信息
-
-        Args:
-            response: scrapy response 或者是 selector 对象
-            query: css 提取的规则
-            get_all: 提取模式，默认：False, 提取符合中的一个
-            return_selector: 是否返回选择器对象
-
-        Returns:
-            1). 提取的内容
-        """
-        if return_selector:
-            return response.xpath(query)
-        if get_all:
-            return response.xpath(query).getall()
-        else:
-            return response.xpath(query).get(default="").strip()
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_json(cls, json_data: dict, query: Union[str, List[str]]):
-        """scrapy 中提取 json 数据遇到的情况
-
-        Args:
-            json_data: scrapy response 响应内容中的 json 格式数据
-            query: json 提取的规则
-
-        Returns:
-            1). 提取的内容
-        """
-        # 如果输入的提取规则参数的格式为字符；或者参数格式是个列表，但是只含有一个元素的情况时
-        if any(
-            [isinstance(query, str), all([isinstance(query, list), len(query) == 1])]
-        ):
-            if isinstance(query, str):
-                return json_data.get(query, "")
-            return json_data.get(query[0], "")
-
-        # 循环取值时的处理
-        for curr_q in query:
-            # 这里循环时不对 json_data 的类型做判断，如果此时 json_data 类型无 get 方法，不处理
-            json_data = json_data.get(curr_q, "")
-            if not json_data:
-                return json_data
-        return json_data
-
-    @classmethod
-    def extract_with_json_rules(cls, json_data: dict, query_rules: List["Str_Lstr"]):
-        """当提取 json 某个数据时，可以在某些字段中取值，只要返回其中任意一个含有数据的值即可
-
-        Args:
-            json_data: scrapy response 响应内容中的 json 格式数据
-            query_rules: json 提取的规则列表
-
-        Returns:
-            1). 提取的内容
-        """
-        # 先判断层级，最多为 2 层
-        depth_num = ReuseOperation.get_array_depth(query_rules)
-        assert depth_num <= 2, "query_rules 参数错误，请输入深度最多为 2 的参数！"
-
-        for query in query_rules:
-            if extract_res := cls.extract_with_json(json_data=json_data, query=query):
-                return extract_res
-        return ""
-
-    @staticmethod
-    def first_not_none(data_lst: List[Any]) -> Any:
-        """获取列表中第一个不为 None 的值
-
-        Args:
-            data_lst: 数据列表
-
-        Returns:
-            1). 第一个不为 None 的值
-        """
-        _res = [x for x in data_lst if x is not None]
-        return _res[0] if _res else None
-
-    @staticmethod
-    def get_dict_form_scrapy_req_headers(scrapy_headers: "Headers") -> dict:
-        """根据 scrapy request 中的 headers 信息转化为正常的 dict 格式
-
-        Args:
-            scrapy_headers: scrapy 的 request headers 内容
-
-        Returns:
-            1). 转化 dict 后的 headers 内容
-        """
-        return {
-            str(b_key, encoding="utf-8"): str(b_value_list[0], encoding="utf-8")
-            for b_key, b_value_list in dict(scrapy_headers).items()
-        }
-
-    @classmethod
-    def get_data_urls_by_img(cls, mediatype: str, data: Union[bytes, str]) -> str:
-        """根据本地、远程或 bytes 内容的图片生成 Data URLs 格式的数据
-        Data URLs 格式示例:
-            data:image/png;base64,iVB...
-            data:text/html,%3Ch1%3EHello%2C%20World%21%3C%2Fh1%3E
-        关于 Data URLs 更多的描述，其参考文档: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URLs
-
-        Args:
-            mediatype: MIME 类型字符串，例如 'image/jpeg' JPEG 图像文件。
-                如果省略，则默认为 text/plain;charset=US-ASCII
-            data: 用于获取其 base64 编码的二进制数据
-                参数格式可以为全路径图片，或 bytes 内容
-
-        Returns:
-            1). Data URLs 格式数据
-        """
-        assert type(data) in [
-            str,
-            bytes,
-        ], "图片转 Data URLs 的参数 data 需要是全路径 str 或 bytes 数据"
-
-        if isinstance(data, str):
-            data_bytes = Path(data).read_bytes()
-            data_base64_encoded = EncryptOperation.base64_encode(encode_data=data_bytes)
-
-        else:
-            data_base64_encoded = EncryptOperation.base64_encode(encode_data=data)
-        return f"data:image/{mediatype};base64,{data_base64_encoded}"
-
-    @staticmethod
-    def gen_selenium_track(distance):
-        """最简陋的根据缺口距离获取轨迹的方法，以供 selenium 使用
-
-        Args:
-            distance: 滑块缺口的距离
-
-        Returns:
-            tracks_dict:
-                forward_tracks: 往右划的轨迹数组
-                back_tracks: 回退（往左划）的轨迹数组
-        """
-        distance += 20
-        v = 0
-        t = 0.2
-        forward_tracks = []
-        current = 0
-        mid = distance * 3 / 5
-        while current < distance:
-            a = 2 if current < mid else -3
-            s = v * t + 0.5 * a * (t**2)
-            v = v + a * t
-            current += s
-            forward_tracks.append(round(s))
-
-        back_tracks = [-3, -3, -2, -2, -2, -2, -2, -1, -1, -1]
-        return {"forward_tracks": forward_tracks, "back_tracks": back_tracks}
-
-    @staticmethod
-    def gen_tracks(distance):
-        """轨迹生成方法
-
-        Args:
-            distance: 滑块缺口的距离
-
-        Returns:
-            xyt: 轨迹数组
-        """
-        t_list = [random.randint(50, 160)]
-        x_list = [random.randint(5, 11)]
-        y_list = []
-        # 生成x坐标轨迹, 生成t坐标轨迹
-        for j in range(1, distance):
-            x_list.append(x_list[j - 1] + random.randint(2, 4))
-            if x_list[j] > distance:
-                break
-
-        diff = x_list[-1] - distance
-        for j in range(diff):
-            x_list.append(x_list[-1] + random.randint(-2, -1))
-            if x_list[-1] <= distance:
-                x_list[-1] = distance
-                break
-
-        length = len(x_list)
-        # 生成y坐标轨迹
-        for i in range(1, length + 1):
-            if i < int(length * 0.4):
-                y_list.append(0)
-            elif i < int(length * 0.65):
-                y_list.append(-1)
-            elif i < int(length * 0.77):
-                y_list.append(-2)
-            elif i < int(length * 0.95):
-                y_list.append(-3)
-            else:
-                y_list.append(-4)
-            t_list.append(t_list[i - 1] + random.randint(20, 80))
-
-        # 生成t的坐标
-        xyt = list(zip(x_list, y_list, t_list))
-        for j in range(length):
-            xyt[j] = list(xyt[j])
-        return xyt
+import json
+import random
+import urllib.request
+from functools import lru_cache
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, List, Literal, Optional, Union
+from urllib.parse import urlparse
+
+from ayugespidertools.common.encryption import Encrypt
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.config import logger
+from ayugespidertools.extras.ext import AppConfManageMixin
+from ayugespidertools.formatdata import DataHandle
+
+__all__ = ["ToolsForAyu"]
+
+if TYPE_CHECKING:
+    from scrapy.http import Response
+    from scrapy.http.headers import Headers
+
+    from ayugespidertools.common.typevars import Str_Lstr
+
+RemoteFormatStr = Literal["json", "hcl", "yaml", "xml"]
+RemoteTypeStr = Literal["consul", "nacos"]
+RemoteConfNameStr = Literal[
+    "mongodb",
+    "mongodb:uri",
+    "mysql",
+    "postgresql",
+    "elasticsearch",
+    "oracle",
+    "oss:ali",
+    "rabbitmq",
+    "kafka",
+    "dynamicproxy",
+    "exclusiveproxy",
+]
+
+
+class ToolsForAyu(AppConfManageMixin):
+    """这里用于存放框架所依赖的方法"""
+
+    @staticmethod
+    @lru_cache(maxsize=16)
+    def get_remote_kvs(
+        url: str,
+        remote_type: RemoteTypeStr = "consul",
+        token: Optional[str] = None,
+    ) -> str:
+        """获取远程配置中的 key_values 信息
+
+        Args:
+            url: 获取 kvs 所需的 url
+            remote_type: 配置类型
+            token: consul token or nacos token; nacos 的 token 值直接在 url 中构造即可
+
+        Returns:
+            1). 远程配置中 key_values 的详细信息
+        """
+        headers = (
+            {"X-Consul-Token": token}
+            if all([remote_type == "consul", token is not None])
+            else {}
+        )
+        req = urllib.request.Request(url=url, headers=headers)
+        r = urllib.request.urlopen(req)
+        data = r.read().decode(errors="ignore")
+
+        url_params = urlparse(url).query
+        if remote_type == "consul":
+            if "raw" in url_params:
+                return data
+
+            json_data = json.loads(data)
+            return Encrypt.base64_decode(decode_data=json_data[0]["Value"])
+        return data
+
+    @classmethod
+    def fetch_remote_conf(
+        cls,
+        conf_name: RemoteConfNameStr,
+        url: str,
+        format: RemoteFormatStr = "json",
+        remote_type: RemoteTypeStr = "consul",
+        token: Optional[str] = None,
+    ) -> dict:
+        """获取远程中的项目配置信息
+
+        Args:
+            conf_name: 需要获取的配置
+            token: consul token or nacos token
+            format: 远程配置中的格式，默认为 json 格式
+            remote_type: 配置类型
+            url: 获取远程配置所需的 url
+
+        Returns:
+            1). 远程应用配置中心中的配置信息（key 值为小写）
+        """
+        conf_value = cls.get_remote_kvs(url, remote_type, token)
+        if format == "json":
+            conf_data = json.loads(conf_value)
+        elif format == "xml":
+            conf_data = cls.xml_parser(conf_value)
+        elif format == "yaml":
+            conf_data = cls.yaml_parser(conf_value)
+        elif format == "hcl":
+            conf_data = cls.hcl_parser(conf_value)
+        else:
+            raise ValueError(f"{conf_name} 暂不支持该格式的配置")
+
+        _conf = conf_data.get(conf_name, {})
+        if not _conf:
+            logger.info(f"远程配置 {remote_type} 中未设置 {conf_name}")
+        return _conf
+
+    @staticmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_css(
+        response: "Response",
+        query: str,
+        get_all: bool = False,
+        return_selector: bool = False,
+    ):
+        """使用 scrapy 的 css 提取信息
+
+        Args:
+            response: scrapy response 或者是 selector 对象
+            query: css 提取的规则
+            get_all: 提取模式，默认：False, 提取符合中的一个
+            return_selector: 是否返回选择器对象
+
+        Returns:
+            1). 提取的内容
+        """
+        if return_selector:
+            return response.css(query)
+        if get_all:
+            return response.css(query).getall()
+        else:
+            return response.css(query).get(default="").strip()
+
+    @staticmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_xpath(
+        response: "Response",
+        query: str,
+        get_all: bool = False,
+        return_selector: bool = False,
+    ):
+        """使用 scrapy 的 xpath 提取信息
+
+        Args:
+            response: scrapy response 或者是 selector 对象
+            query: css 提取的规则
+            get_all: 提取模式，默认：False, 提取符合中的一个
+            return_selector: 是否返回选择器对象
+
+        Returns:
+            1). 提取的内容
+        """
+        if return_selector:
+            return response.xpath(query)
+        if get_all:
+            return response.xpath(query).getall()
+        else:
+            return response.xpath(query).get(default="").strip()
+
+    @staticmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_json(json_data: dict, query: Union[str, List[str]]):
+        """scrapy 中提取 json 数据遇到的情况
+
+        Args:
+            json_data: scrapy response 响应内容中的 json 格式数据
+            query: json 提取的规则
+
+        Returns:
+            1). 提取的内容
+        """
+        # 如果输入的提取规则参数的格式为字符；或者参数格式是个列表，但是只含有一个元素的情况时
+        if any(
+            [isinstance(query, str), all([isinstance(query, list), len(query) == 1])]
+        ):
+            if isinstance(query, str):
+                return json_data.get(query, "")
+            return json_data.get(query[0], "")
+
+        # 循环取值时的处理
+        for curr_q in query:
+            # 这里循环时不对 json_data 的类型做判断，如果此时 json_data 类型无 get 方法，不处理
+            json_data = json_data.get(curr_q, "")
+            if not json_data:
+                return json_data
+        return json_data
+
+    @classmethod
+    def extract_with_json_rules(cls, json_data: dict, query_rules: List["Str_Lstr"]):
+        """当提取 json 某个数据时，可以在某些字段中取值，只要返回其中任意一个含有数据的值即可
+
+        Args:
+            json_data: scrapy response 响应内容中的 json 格式数据
+            query_rules: json 提取的规则列表
+
+        Returns:
+            1). 提取的内容
+        """
+        depth_num = ReuseOperation.get_array_depth(query_rules)
+        assert depth_num <= 2, "query_rules 参数错误，请输入深度最多为 2 的参数！"
+
+        for query in query_rules:
+            if extract_res := cls.extract_with_json(json_data=json_data, query=query):
+                return extract_res
+        return ""
+
+    @staticmethod
+    def first_not_none(data_lst: List[Any]) -> Any:
+        """获取列表中第一个不为 None 的值
+
+        Args:
+            data_lst: 数据列表
+
+        Returns:
+            1). 第一个不为 None 的值
+        """
+        _res = [x for x in data_lst if x is not None]
+        return _res[0] if _res else None
+
+    @staticmethod
+    def get_dict_form_scrapy_req_headers(scrapy_headers: "Headers") -> dict:
+        """根据 scrapy request 中的 headers 信息转化为正常的 dict 格式
+
+        Args:
+            scrapy_headers: scrapy 的 request headers 内容
+
+        Returns:
+            1). 转化 dict 后的 headers 内容
+        """
+        return {
+            str(b_key, encoding="utf-8"): str(b_value_list[0], encoding="utf-8")
+            for b_key, b_value_list in dict(scrapy_headers).items()
+        }
+
+    @staticmethod
+    def get_data_urls_by_img(mediatype: str, data: Union[bytes, str]) -> str:
+        """根据本地、远程或 bytes 内容的图片生成 Data URLs 格式的数据
+        Data URLs 格式示例:
+            data:image/png;base64,iVB...
+            data:text/html,%3Ch1%3EHello%2C%20World%21%3C%2Fh1%3E
+        关于 Data URLs 更多的描述，其参考文档: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URLs
+
+        Args:
+            mediatype: MIME 类型字符串，例如 'image/jpeg' JPEG 图像文件。
+                如果省略，则默认为 text/plain;charset=US-ASCII
+            data: 用于获取其 base64 编码的二进制数据
+                参数格式可以为全路径图片，或 bytes 内容
+
+        Returns:
+            1). Data URLs 格式数据
+        """
+        assert type(data) in [
+            str,
+            bytes,
+        ], "图片转 Data URLs 的参数 data 需要是全路径 str 或 bytes 数据"
+
+        if isinstance(data, str):
+            data_bytes = Path(data).read_bytes()
+            data_base64_encoded = Encrypt.base64_encode(encode_data=data_bytes)
+
+        else:
+            data_base64_encoded = Encrypt.base64_encode(encode_data=data)
+        return f"data:image/{mediatype};base64,{data_base64_encoded}"
+
+    @staticmethod
+    def gen_selenium_track(distance):
+        """最简陋的根据缺口距离获取轨迹的方法，以供 selenium 使用
+
+        Args:
+            distance: 滑块缺口的距离
+
+        Returns:
+            tracks_dict:
+                forward_tracks: 往右划的轨迹数组
+                back_tracks: 回退（往左划）的轨迹数组
+        """
+        distance += 20
+        v = 0
+        t = 0.2
+        forward_tracks = []
+        current = 0
+        mid = distance * 3 / 5
+        while current < distance:
+            a = 2 if current < mid else -3
+            s = v * t + 0.5 * a * (t**2)
+            v = v + a * t
+            current += s
+            forward_tracks.append(round(s))
+
+        back_tracks = [-3, -3, -2, -2, -2, -2, -2, -1, -1, -1]
+        return {"forward_tracks": forward_tracks, "back_tracks": back_tracks}
+
+    @staticmethod
+    def gen_tracks(distance):
+        """轨迹生成方法
+
+        Args:
+            distance: 滑块缺口的距离
+
+        Returns:
+            xyt: 轨迹数组
+        """
+        t_list = [random.randint(50, 160)]
+        x_list = [random.randint(5, 11)]
+        y_list = []
+        # 生成 x 坐标轨迹, 生成 t 坐标轨迹
+        for j in range(1, distance):
+            x_list.append(x_list[j - 1] + random.randint(2, 4))
+            if x_list[j] > distance:
+                break
+
+        diff = x_list[-1] - distance
+        for j in range(diff):
+            x_list.append(x_list[-1] + random.randint(-2, -1))
+            if x_list[-1] <= distance:
+                x_list[-1] = distance
+                break
+
+        length = len(x_list)
+        # 生成 y 坐标轨迹
+        for i in range(1, length + 1):
+            if i < int(length * 0.4):
+                y_list.append(0)
+            elif i < int(length * 0.65):
+                y_list.append(-1)
+            elif i < int(length * 0.77):
+                y_list.append(-2)
+            elif i < int(length * 0.95):
+                y_list.append(-3)
+            else:
+                y_list.append(-4)
+            t_list.append(t_list[i - 1] + random.randint(20, 80))
+
+        # 生成 t 的坐标
+        xyt = list(zip(x_list, y_list, t_list))
+        for j in range(length):
+            xyt[j] = list(xyt[j])
+        return xyt
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/extras/cvnpil.py` & `ayugespidertools-3.9.8/ayugespidertools/extras/cvnpil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,478 +1,471 @@
-import itertools
-import math
-import random
-from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
-
-try:
-    import cv2
-    import numpy as np
-except ImportError:
-    # pip install ayugespidertools[all]
-    pass
-
-__all__ = ["CvnpilKit", "BezierTrajectory"]
-
-if TYPE_CHECKING:
-    from cv2.typing import MatLike
-
-
-class CvnpilKit:
-    @staticmethod
-    def get_array_dimension(array: Union[frozenset, list, set, tuple]) -> int:
-        """获取 array 的维度
-
-        Args:
-            array: 数组
-
-        Returns:
-            1). 层级数
-        """
-        # 其实直接返回 len(array) 即可
-        return len(np.array(array).shape)
-
-    @staticmethod
-    def read_image_data(
-        img: Union[bytes, str],
-        flags: int = cv2.IMREAD_COLOR,
-    ) -> np.ndarray:
-        """
-        用 opencv 读取图片数据
-        Args:
-            img: 图片参数，类型需要是路径 str 或 bytes 数据
-            flags: 应用颜色通道类型
-
-        Returns:
-            img_cv: opencv 读取背景图片的数据
-        """
-        assert type(img) in [str, bytes], "img 参数需要是路径或 bytes 数据"
-        if isinstance(img, bytes):
-            img_buf = np.frombuffer(img, np.uint8)
-            img_cv = cv2.imdecode(img_buf, cv2.IMREAD_ANYCOLOR)
-        else:
-            # 读取图片，读进来直接是 BGR 格式数据格式在 0~255
-            img_cv = cv2.imread(img, flags)
-        return img_cv
-
-    @classmethod
-    def clear_white(cls, img):
-        """清除图片的空白区域，这里主要清除滑块的空白
-
-        Args:
-            img: 待处理的图片
-
-        Returns:
-            1). 清除图片空白区域的图片
-        """
-        rows, cols, channel = img.shape
-        min_x = 255
-        min_y = 255
-        max_x = 0
-        max_y = 0
-        for x, y in itertools.product(range(1, rows), range(1, cols)):
-            t = set(img[x, y])
-            if len(t) >= 2:
-                if x <= min_x:
-                    min_x = x
-                elif x >= max_x:
-                    max_x = x
-
-                if y <= min_y:
-                    min_y = y
-                elif y >= max_y:
-                    max_y = y
-        return img[min_x:max_x, min_y:max_y]
-
-    @classmethod
-    def image_edge_detection(cls, img):
-        """图像边缘检测处理，识别图片边缘
-
-        Args:
-            img: 需要处理的图片，用于边缘检测使用
-
-        Returns:
-            1). 处理后的图片
-        """
-        return cv2.Canny(img, 100, 200)
-
-    @classmethod
-    def _template_match(
-        cls,
-        bg: "MatLike",
-        slider: "MatLike",
-        out: Optional[str] = None,
-    ) -> int:
-        """模板匹配找出滑块缺口的距离
-
-        Args:
-            bg: 背景图片
-            slider: 缺口(滑块)图片
-            out: 展示图片的存储全路径，会将绘制的图片保存至此
-
-        Returns:
-            tl[0]: 滑块缺口的距离
-        """
-        res = cv2.matchTemplate(bg, slider, cv2.TM_CCOEFF_NORMED)
-        # 寻找最优匹配(一维数组当作向量,用 Mat 定义) 中最小值和最大值的位置
-        min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
-        # 左上角点的坐标
-        tl = max_loc
-
-        # 是否要输出绘制图像
-        if out:
-            # 绘制方框
-            th, tw = slider.shape[:2]
-            # 右下角点的坐标
-            br = (tl[0] + tw, tl[1] + th)
-            cv2.rectangle(bg, tl, br, (0, 0, 255), 2)
-            cv2.imwrite(out, bg)
-        # 返回缺口的X坐标
-        return tl[0]
-
-    @classmethod
-    def discern_gap(
-        cls,
-        bg: Union[str, bytes],
-        slider: Union[str, bytes],
-        out: Optional[str] = None,
-    ):
-        """识别滑块缺口方法
-
-        Args:
-            bg: 带缺口的背景图，可以是全路径图片，也可以是图片的 bytes 数据
-            slider: 滑块图，可以是全路径图片，也可以是图片的 bytes 数据
-            out: 绘制图展示的存储地址，参数格式为图片的全路径
-
-        Returns:
-            1): 滑块缺口横坐标
-        """
-        slider_cv = CvnpilKit.read_image_data(slider)
-        bg_cv = CvnpilKit.read_image_data(bg, cv2.IMREAD_GRAYSCALE)
-        slider_clr = cls.clear_white(slider_cv)
-        slider_clr = cv2.cvtColor(slider_clr, cv2.COLOR_RGB2GRAY)
-        slider_img = cls.image_edge_detection(slider_clr)
-        bg_img = cls.image_edge_detection(bg_cv)
-        slider_img = cv2.cvtColor(slider_img, cv2.COLOR_GRAY2RGB)
-        bg_img = cv2.cvtColor(bg_img, cv2.COLOR_GRAY2RGB)
-        # 输出横坐标, 即滑块在图片上的位置
-        return cls._template_match(bg_img, slider_img, out)
-
-    @classmethod
-    def identify_gap(
-        cls,
-        bg: Union[bytes, str],
-        slider: Union[bytes, str],
-        out: Optional[str] = None,
-    ) -> int:
-        """通过背景图片和缺口图片识别出滑块距离
-
-        Args:
-            bg: 背景图片，可以是图片的全路径，也可以是图片的 bytes 内容
-            slider: 缺口（滑块）图片，可以是图片的全路径，也可以是图片的 bytes 内容
-            out: 输出图片路径，示例：doc/test.jpg；此参数如果为空，则不输出标记后的图片
-
-        Returns:
-            tl[0]: 滑块缺口距离
-        """
-        # 读取图片数据
-        bg_cv = cls.read_image_data(bg)
-        slider_cv = cls.read_image_data(slider, cv2.IMREAD_GRAYSCALE)
-        # 识别图片边缘
-        bg_edge = cv2.Canny(bg_cv, 100, 200)
-        slider_edge = cv2.Canny(slider_cv, 100, 200)
-        # 转换图片格式
-        bg_img = cv2.cvtColor(bg_edge, cv2.COLOR_GRAY2RGB)
-        slider_img = cv2.cvtColor(slider_edge, cv2.COLOR_GRAY2RGB)
-        return cls._template_match(bg_img, slider_img, out)
-
-    @staticmethod
-    def match_gap(bg: Union[str, bytes], slider: Union[str, bytes]):
-        """滑块坐标定位方法
-
-        Args:
-            bg: 1) 带缺口的背景图，全路径; 2) 或者是背景图的 bytes 数据
-            slider: 1） 滑块图，全路径; 2）或者是滑块图的 bytes 数据
-
-        Returns:
-            loc[1][0]: 滑块位置坐标
-        """
-        bg_cv = CvnpilKit.read_image_data(bg, cv2.IMREAD_GRAYSCALE)
-        slider_cv = CvnpilKit.read_image_data(slider, cv2.IMREAD_GRAYSCALE)
-
-        run = 1
-        # 这里的返回值根据不同版本的 open-cv 其返回结果会有不同的个数
-        # w, h, z = slider_cv.shape[::-1]
-        # 在背景图里面查找滑块图的位置
-        res = cv2.matchTemplate(bg_cv, slider_cv, cv2.TM_CCOEFF_NORMED)
-        # 使用二分法查找阈值的精确值
-        lft: float = 0.0
-        rgt: float = 1.0
-        loc: Tuple[np.ndarray[Any, np.dtype[np.signedinteger[Any]]], ...] = ()
-        while run < 20:
-            run += 1
-            threshold = (rgt + lft) / 2
-            if threshold < 0:
-                # 逻辑走到这里，则说明出错了，并未找出目标位置
-                return None
-
-            # 匹配程度大于百分之 threshold 的坐标 x, y
-            loc = np.where(res >= threshold)
-            if len(loc[1]) > 1:
-                rgt += (rgt - lft) / 2
-            elif len(loc[1]) == 1:
-                # 找到目标区域起点x坐标为：loc[1][0]
-                break
-            elif len(loc[1]) < 1:
-                rgt -= (rgt - lft) / 2
-        # 返回 x 坐标
-        return loc[1][0]
-
-    @staticmethod
-    def get_normal_track(space):
-        """通用的根据滑块距离获取轨迹数组方法
-
-        Args:
-            space: 滑块缺口距离
-
-        Returns:
-            tracks_list: 生成的轨迹数组
-        """
-        x = [0, 0]
-        y = [0, 0, 0]
-        z = [0]
-        # x
-        count = np.linspace(-math.pi / 2, math.pi / 2, random.randrange(20, 30))
-        func = list(map(math.sin, count))
-        nx = [i + 1 for i in func]
-        add = random.randrange(10, 15)
-        sadd = space + add
-        x.extend(list(map(lambda x: x * (sadd / 2), nx)))
-        # x.extend(np.linspace(sadd, space, 4 if add > 12 else 3))
-        x.extend(np.linspace(sadd, space, 3 if add > 12 else 2))
-        x = [math.floor(i) for i in x]
-        # y
-        for i in range(len(x) - 2):
-            if y[-1] < 30:
-                y.append(y[-1] + random.choice([0, 0, 1, 1, 2, 2, 1, 2, 0, 0, 3, 3]))
-            else:
-                y.append(
-                    y[-1] + random.choice([0, 0, -1, -1, -2, -2, -1, -2, 0, 0, -3, -3])
-                )
-        # z
-        for i in range(len(x) - 1):
-            # z.append((z[-1] // 100 * 100) + 100 + random.choice([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 2]))
-            z.append(
-                (z[-1] // 100 * 100)
-                + 100
-                + random.choice([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 3])
-            )
-
-        tracks_list = list(map(list, zip(x, y, z)))
-        tracks_list = [x for x in tracks_list if x[0] > 0]
-        return tracks_list
-
-
-class BezierTrajectory:
-    """贝塞尔曲线轨迹生成器
-
-    Examples:
-        >>> bt = BezierTrajectory()
-        >>> gen_data = bt.gen_track(start=[50, 268], end=[367, 485], num=45, order=4, mode=2)
-        >>> track = gen_data["trackArray"]
-    """
-
-    def _generate_control_points(self, track: list):
-        """计算贝塞尔曲线的控制点"""
-        track_len = len(track)
-
-        def calculate_bezier_point(x):
-            t = (x - track[0][0]) / (track[-1][0] - track[0][0])
-            y = np.array([0, 0], dtype=np.float64)
-            for s in range(len(track)):
-                y += track[s] * (
-                    (
-                        math.factorial(track_len - 1)
-                        / (math.factorial(s) * math.factorial(track_len - 1 - s))
-                    )
-                    * math.pow(t, s)
-                    * math.pow((1 - t), track_len - 1 - s)
-                )
-            return y[1]
-
-        return calculate_bezier_point
-
-    def _type(self, mode, x, length):
-        numbers = []
-        pin = (x[1] - x[0]) / length
-        if mode == 0:
-            numbers.extend(i * pin for i in range(length))
-            if pin >= 0:
-                numbers = numbers[::-1]
-        elif mode == 1:
-            for i in range(length):
-                numbers.append(1 * ((i * pin) ** 2))
-            numbers = numbers[::-1]
-        elif mode == 2:
-            for i in range(length):
-                numbers.append(1 * ((i * pin - x[1]) ** 2))
-
-        elif mode == 3:
-            track = [
-                np.array([0, 0]),
-                np.array([(x[1] - x[0]) * 0.8, (x[1] - x[0]) * 0.6]),
-                np.array([x[1] - x[0], 0]),
-            ]
-            fun = self._generate_control_points(track)
-            numbers = [0]
-            numbers.extend(fun(i * pin) + numbers[-1] for i in range(1, length))
-            if pin >= 0:
-                numbers = numbers[::-1]
-        numbers = np.abs(np.array(numbers) - max(numbers))
-        normal_numbers = (
-            (numbers - numbers[numbers.argmin()])
-            / (numbers[numbers.argmax()] - numbers[numbers.argmin()])
-        ) * (x[1] - x[0]) + x[0]
-        normal_numbers[0] = x[0]
-        normal_numbers[-1] = x[1]
-        return normal_numbers
-
-    def simulation(self, start, end, order=1, deviation=0, bias=0.5):
-        """模拟贝塞尔曲线的绘制过程
-
-        Args:
-            start: 开始点的坐标
-            end: 结束点的坐标
-            order: 几阶贝塞尔曲线，越大越复杂
-            deviation: 轨迹上下波动的范围
-            bias: 波动范围的分布位置
-
-        Returns:
-            1). 返回一个字典 equation 对应该曲线的方程，P 对应贝塞尔曲线的影响点
-        """
-        start = np.array(start)
-        end = np.array(end)
-        shake_num = []
-        if order != 1:
-            e = (1 - bias) / (order - 1)
-            shake_num = [[bias + e * i, bias + e * (i + 1)] for i in range(order - 1)]
-
-        track_lst = [start]
-
-        t = random.choice([-1, 1])
-        w = 0
-        for i in shake_num:
-            px1 = start[0] + (end[0] - start[0]) * (
-                random.random() * (i[1] - i[0]) + (i[0])
-            )
-            p = np.array(
-                [px1, self._generate_control_points([start, end])(px1) + t * deviation]
-            )
-            track_lst.append(p)
-            w += 1
-            if w >= 2:
-                w = 0
-                t = -1 * t
-
-        track_lst.append(end)
-        return {
-            "equation": self._generate_control_points(track_lst),
-            "P": np.array(track_lst),
-        }
-
-    def gen_track(
-        self,
-        start: Union[np.ndarray, list],
-        end: Union[np.ndarray, list],
-        num: int,
-        order: int = 1,
-        deviation: int = 0,
-        bias=0.5,
-        mode=0,
-        shake_num=0,
-        yhh=10,
-    ) -> dict:
-        """生成轨迹数组
-
-        Args:
-            start: 开始点的坐标
-            end: 结束点的坐标
-            num: 返回的数组的轨迹点的数量
-            order: 几阶贝塞尔曲线，越大越复杂
-            deviation: 轨迹上下波动的范围
-            bias: 波动范围的分布位置
-            mode: 0 表示均速滑动，1 表示先慢后快，2 表示先快后慢，3 表示先慢中间快后慢
-            shake_num: 在终点来回摆动的次数
-            yhh: 在终点来回摆动的范围
-
-        Returns:
-            1). 返回一个字典 trackArray 对应轨迹数组，P 对应贝塞尔曲线的影响点
-        """
-        s: list = []
-        fun = self.simulation(start, end, order, deviation, bias)
-        w = fun["P"]
-        fun = fun["equation"]
-        if shake_num != 0:
-            track_number = round(num * 0.2 / (shake_num + 1))
-            num -= num * (shake_num + 1)
-
-            x_track_array = self._type(mode, [start[0], end[0]], num)
-            s.extend([i, fun(i)] for i in x_track_array)
-            dq = yhh / shake_num
-            kg = 0
-            ends = np.copy(end)
-            for i in range(shake_num):
-                if kg == 0:
-                    d = np.array(
-                        [
-                            end[0] + (yhh - dq * i),
-                            ((end[1] - start[1]) / (end[0] - start[0]))
-                            * (end[0] + (yhh - dq * i))
-                            + (
-                                end[1]
-                                - ((end[1] - start[1]) / (end[0] - start[0])) * end[0]
-                            ),
-                        ]
-                    )
-                    kg = 1
-                else:
-                    d = np.array(
-                        [
-                            end[0] - (yhh - dq * i),
-                            ((end[1] - start[1]) / (end[0] - start[0]))
-                            * (end[0] - (yhh - dq * i))
-                            + (
-                                end[1]
-                                - ((end[1] - start[1]) / (end[0] - start[0])) * end[0]
-                            ),
-                        ]
-                    )
-                    kg = 0
-                y = self.gen_track(
-                    ends,
-                    d,
-                    track_number,
-                    order=2,
-                    deviation=0,
-                    bias=0.5,
-                    mode=0,
-                    shake_num=0,
-                    yhh=10,
-                )
-                s += list(y["trackArray"])
-                ends = d
-            y = self.gen_track(
-                ends,
-                end,
-                track_number,
-                order=2,
-                deviation=0,
-                bias=0.5,
-                mode=0,
-                shake_num=0,
-                yhh=10,
-            )
-            s += list(y["trackArray"])
-
-        else:
-            x_track_array = self._type(mode, [start[0], end[0]], num)
-            s.extend([i, fun(i)] for i in x_track_array)
-        return {"trackArray": np.array(s), "P": w}
+import itertools
+import math
+import random
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
+
+try:
+    import cv2
+    import numpy as np
+except ImportError:
+    # pip install ayugespidertools[all]
+    pass
+
+__all__ = ["CvnpilKit", "BezierTrajectory"]
+
+if TYPE_CHECKING:
+    from cv2.typing import MatLike
+
+
+class CvnpilKit:
+    @staticmethod
+    def get_array_dimension(array: Union[frozenset, list, set, tuple]) -> int:
+        """获取 array 的维度
+
+        Args:
+            array: 数组
+
+        Returns:
+            1). 层级数
+        """
+        # 其实直接返回 len(array) 即可
+        return len(np.array(array).shape)
+
+    @staticmethod
+    def read_image_data(
+        img: Union[bytes, str],
+        flags: int = cv2.IMREAD_COLOR,
+    ) -> np.ndarray:
+        """
+        用 opencv 读取图片数据
+        Args:
+            img: 图片参数，类型需要是路径 str 或 bytes 数据
+            flags: 应用颜色通道类型
+
+        Returns:
+            img_cv: opencv 读取背景图片的数据
+        """
+        assert type(img) in [str, bytes], "img 参数需要是路径或 bytes 数据"
+        if isinstance(img, bytes):
+            img_buf = np.frombuffer(img, np.uint8)
+            img_cv = cv2.imdecode(img_buf, cv2.IMREAD_ANYCOLOR)
+        else:
+            # 读取图片，读进来直接是 BGR 格式数据格式在 0~255
+            img_cv = cv2.imread(img, flags)
+        return img_cv
+
+    @staticmethod
+    def clear_white(img):
+        """清除图片的空白区域，这里主要清除滑块的空白
+
+        Args:
+            img: 待处理的图片
+
+        Returns:
+            1). 清除图片空白区域的图片
+        """
+        rows, cols, channel = img.shape
+        min_x = 255
+        min_y = 255
+        max_x = 0
+        max_y = 0
+        for x, y in itertools.product(range(1, rows), range(1, cols)):
+            t = set(img[x, y])
+            if len(t) >= 2:
+                if x <= min_x:
+                    min_x = x
+                elif x >= max_x:
+                    max_x = x
+
+                if y <= min_y:
+                    min_y = y
+                elif y >= max_y:
+                    max_y = y
+        return img[min_x:max_x, min_y:max_y]
+
+    @staticmethod
+    def image_edge_detection(img):
+        """图像边缘检测处理，识别图片边缘
+
+        Args:
+            img: 需要处理的图片，用于边缘检测使用
+
+        Returns:
+            1). 处理后的图片
+        """
+        return cv2.Canny(img, 100, 200)
+
+    @staticmethod
+    def _template_match(
+        bg: "MatLike", slider: "MatLike", out: Optional[str] = None
+    ) -> int:
+        """模板匹配找出滑块缺口的距离
+
+        Args:
+            bg: 背景图片
+            slider: 缺口(滑块)图片
+            out: 展示图片的存储全路径，会将绘制的图片保存至此
+
+        Returns:
+            tl[0]: 滑块缺口的距离
+        """
+        res = cv2.matchTemplate(bg, slider, cv2.TM_CCOEFF_NORMED)
+        # 寻找最优匹配(一维数组当作向量,用 Mat 定义) 中最小值和最大值的位置
+        min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
+        # 左上角点的坐标
+        tl = max_loc
+
+        if out:
+            # 绘制方框
+            th, tw = slider.shape[:2]
+            # 右下角点的坐标
+            br = (tl[0] + tw, tl[1] + th)
+            cv2.rectangle(bg, tl, br, (0, 0, 255), 2)
+            cv2.imwrite(out, bg)
+        return tl[0]
+
+    @classmethod
+    def discern_gap(
+        cls,
+        bg: Union[str, bytes],
+        slider: Union[str, bytes],
+        out: Optional[str] = None,
+    ):
+        """识别滑块缺口方法
+
+        Args:
+            bg: 带缺口的背景图，可以是全路径图片，也可以是图片的 bytes 数据
+            slider: 滑块图，可以是全路径图片，也可以是图片的 bytes 数据
+            out: 绘制图展示的存储地址，参数格式为图片的全路径
+
+        Returns:
+            1): 滑块缺口横坐标
+        """
+        slider_cv = CvnpilKit.read_image_data(slider)
+        bg_cv = CvnpilKit.read_image_data(bg, cv2.IMREAD_GRAYSCALE)
+        slider_clr = cls.clear_white(slider_cv)
+        slider_clr = cv2.cvtColor(slider_clr, cv2.COLOR_RGB2GRAY)
+        slider_img = cls.image_edge_detection(slider_clr)
+        bg_img = cls.image_edge_detection(bg_cv)
+        slider_img = cv2.cvtColor(slider_img, cv2.COLOR_GRAY2RGB)
+        bg_img = cv2.cvtColor(bg_img, cv2.COLOR_GRAY2RGB)
+        return cls._template_match(bg_img, slider_img, out)
+
+    @classmethod
+    def identify_gap(
+        cls,
+        bg: Union[bytes, str],
+        slider: Union[bytes, str],
+        out: Optional[str] = None,
+    ) -> int:
+        """通过背景图片和缺口图片识别出滑块距离
+
+        Args:
+            bg: 背景图片，可以是图片的全路径，也可以是图片的 bytes 内容
+            slider: 缺口（滑块）图片，可以是图片的全路径，也可以是图片的 bytes 内容
+            out: 输出图片路径，示例：doc/test.jpg；此参数如果为空，则不输出标记后的图片
+
+        Returns:
+            tl[0]: 滑块缺口距离
+        """
+        # 读取图片数据
+        bg_cv = cls.read_image_data(bg)
+        slider_cv = cls.read_image_data(slider, cv2.IMREAD_GRAYSCALE)
+        # 识别图片边缘
+        bg_edge = cv2.Canny(bg_cv, 100, 200)
+        slider_edge = cv2.Canny(slider_cv, 100, 200)
+        # 转换图片格式
+        bg_img = cv2.cvtColor(bg_edge, cv2.COLOR_GRAY2RGB)
+        slider_img = cv2.cvtColor(slider_edge, cv2.COLOR_GRAY2RGB)
+        return cls._template_match(bg_img, slider_img, out)
+
+    @staticmethod
+    def match_gap(bg: Union[str, bytes], slider: Union[str, bytes]):
+        """滑块坐标定位方法
+
+        Args:
+            bg: 1) 带缺口的背景图，全路径; 2) 或者是背景图的 bytes 数据
+            slider: 1） 滑块图，全路径; 2）或者是滑块图的 bytes 数据
+
+        Returns:
+            loc[1][0]: 滑块位置坐标
+        """
+        bg_cv = CvnpilKit.read_image_data(bg, cv2.IMREAD_GRAYSCALE)
+        slider_cv = CvnpilKit.read_image_data(slider, cv2.IMREAD_GRAYSCALE)
+
+        run = 1
+        # 这里的返回值根据不同版本的 open-cv 其返回结果会有不同的个数
+        # w, h, z = slider_cv.shape[::-1]
+        # 在背景图里面查找滑块图的位置
+        res = cv2.matchTemplate(bg_cv, slider_cv, cv2.TM_CCOEFF_NORMED)
+        # 使用二分法查找阈值的精确值
+        lft: float = 0.0
+        rgt: float = 1.0
+        loc: Tuple[np.ndarray[Any, np.dtype[np.signedinteger[Any]]], ...] = ()
+        while run < 20:
+            run += 1
+            threshold = (rgt + lft) / 2
+            if threshold < 0:
+                # 逻辑走到这里，则说明出错了，并未找出目标位置
+                return None
+
+            # 匹配程度大于百分之 threshold 的坐标 x, y
+            loc = np.where(res >= threshold)
+            if len(loc[1]) > 1:
+                rgt += (rgt - lft) / 2
+            elif len(loc[1]) == 1:
+                # 找到目标区域起点 x 坐标为：loc[1][0]
+                break
+            elif len(loc[1]) < 1:
+                rgt -= (rgt - lft) / 2
+        return loc[1][0]
+
+    @staticmethod
+    def get_normal_track(space):
+        """通用的根据滑块距离获取轨迹数组方法
+
+        Args:
+            space: 滑块缺口距离
+
+        Returns:
+            tracks_list: 生成的轨迹数组
+        """
+        x = [0, 0]
+        y = [0, 0, 0]
+        z = [0]
+        # x
+        count = np.linspace(-math.pi / 2, math.pi / 2, random.randrange(20, 30))
+        func = list(map(math.sin, count))
+        nx = [i + 1 for i in func]
+        add = random.randrange(10, 15)
+        sadd = space + add
+        x.extend(list(map(lambda x: x * (sadd / 2), nx)))
+        # x.extend(np.linspace(sadd, space, 4 if add > 12 else 3))
+        x.extend(np.linspace(sadd, space, 3 if add > 12 else 2))
+        x = [math.floor(i) for i in x]
+        # y
+        for i in range(len(x) - 2):
+            if y[-1] < 30:
+                y.append(y[-1] + random.choice([0, 0, 1, 1, 2, 2, 1, 2, 0, 0, 3, 3]))
+            else:
+                y.append(
+                    y[-1] + random.choice([0, 0, -1, -1, -2, -2, -1, -2, 0, 0, -3, -3])
+                )
+        # z
+        for i in range(len(x) - 1):
+            # z.append((z[-1] // 100 * 100) + 100 + random.choice([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 2]))
+            z.append(
+                (z[-1] // 100 * 100)
+                + 100
+                + random.choice([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 3])
+            )
+
+        tracks_list = list(map(list, zip(x, y, z)))
+        tracks_list = [x for x in tracks_list if x[0] > 0]
+        return tracks_list
+
+
+class BezierTrajectory:
+    """贝塞尔曲线轨迹生成器
+
+    Examples:
+        >>> bt = BezierTrajectory()
+        >>> gen_data = bt.gen_track(start=[50, 268], end=[367, 485], num=45, order=4, mode=2)
+        >>> track = gen_data["trackArray"]
+    """
+
+    def _generate_control_points(self, track: list):
+        """计算贝塞尔曲线的控制点"""
+        track_len = len(track)
+
+        def calculate_bezier_point(x):
+            t = (x - track[0][0]) / (track[-1][0] - track[0][0])
+            y = np.array([0, 0], dtype=np.float64)
+            for s in range(len(track)):
+                y += track[s] * (
+                    (
+                        math.factorial(track_len - 1)
+                        / (math.factorial(s) * math.factorial(track_len - 1 - s))
+                    )
+                    * math.pow(t, s)
+                    * math.pow((1 - t), track_len - 1 - s)
+                )
+            return y[1]
+
+        return calculate_bezier_point
+
+    def _type(self, mode, x, length):
+        numbers = []
+        pin = (x[1] - x[0]) / length
+        if mode == 0:
+            numbers.extend(i * pin for i in range(length))
+            if pin >= 0:
+                numbers = numbers[::-1]
+        elif mode == 1:
+            for i in range(length):
+                numbers.append(1 * ((i * pin) ** 2))
+            numbers = numbers[::-1]
+        elif mode == 2:
+            for i in range(length):
+                numbers.append(1 * ((i * pin - x[1]) ** 2))
+
+        elif mode == 3:
+            track = [
+                np.array([0, 0]),
+                np.array([(x[1] - x[0]) * 0.8, (x[1] - x[0]) * 0.6]),
+                np.array([x[1] - x[0], 0]),
+            ]
+            fun = self._generate_control_points(track)
+            numbers = [0]
+            numbers.extend(fun(i * pin) + numbers[-1] for i in range(1, length))
+            if pin >= 0:
+                numbers = numbers[::-1]
+        numbers = np.abs(np.array(numbers) - max(numbers))
+        normal_numbers = (
+            (numbers - numbers[numbers.argmin()])
+            / (numbers[numbers.argmax()] - numbers[numbers.argmin()])
+        ) * (x[1] - x[0]) + x[0]
+        normal_numbers[0] = x[0]
+        normal_numbers[-1] = x[1]
+        return normal_numbers
+
+    def simulation(self, start, end, order=1, deviation=0, bias=0.5):
+        """模拟贝塞尔曲线的绘制过程
+
+        Args:
+            start: 开始点的坐标
+            end: 结束点的坐标
+            order: 几阶贝塞尔曲线，越大越复杂
+            deviation: 轨迹上下波动的范围
+            bias: 波动范围的分布位置
+
+        Returns:
+            1). 返回一个字典 equation 对应该曲线的方程，P 对应贝塞尔曲线的影响点
+        """
+        start = np.array(start)
+        end = np.array(end)
+        shake_num = []
+        if order != 1:
+            e = (1 - bias) / (order - 1)
+            shake_num = [[bias + e * i, bias + e * (i + 1)] for i in range(order - 1)]
+
+        track_lst = [start]
+
+        t = random.choice([-1, 1])
+        w = 0
+        for i in shake_num:
+            px1 = start[0] + (end[0] - start[0]) * (
+                random.random() * (i[1] - i[0]) + (i[0])
+            )
+            p = np.array(
+                [px1, self._generate_control_points([start, end])(px1) + t * deviation]
+            )
+            track_lst.append(p)
+            w += 1
+            if w >= 2:
+                w = 0
+                t = -1 * t
+
+        track_lst.append(end)
+        return {
+            "equation": self._generate_control_points(track_lst),
+            "P": np.array(track_lst),
+        }
+
+    def gen_track(
+        self,
+        start: Union[np.ndarray, list],
+        end: Union[np.ndarray, list],
+        num: int,
+        order: int = 1,
+        deviation: int = 0,
+        bias=0.5,
+        mode=0,
+        shake_num=0,
+        yhh=10,
+    ) -> dict:
+        """生成轨迹数组
+
+        Args:
+            start: 开始点的坐标
+            end: 结束点的坐标
+            num: 返回的数组的轨迹点的数量
+            order: 几阶贝塞尔曲线，越大越复杂
+            deviation: 轨迹上下波动的范围
+            bias: 波动范围的分布位置
+            mode: 0 表示均速滑动，1 表示先慢后快，2 表示先快后慢，3 表示先慢中间快后慢
+            shake_num: 在终点来回摆动的次数
+            yhh: 在终点来回摆动的范围
+
+        Returns:
+            1). 返回一个字典 trackArray 对应轨迹数组，P 对应贝塞尔曲线的影响点
+        """
+        s: list = []
+        fun = self.simulation(start, end, order, deviation, bias)
+        w = fun["P"]
+        fun = fun["equation"]
+        if shake_num != 0:
+            track_number = round(num * 0.2 / (shake_num + 1))
+            num -= num * (shake_num + 1)
+
+            x_track_array = self._type(mode, [start[0], end[0]], num)
+            s.extend([i, fun(i)] for i in x_track_array)
+            dq = yhh / shake_num
+            kg = 0
+            ends = np.copy(end)
+            for i in range(shake_num):
+                if kg == 0:
+                    d = np.array(
+                        [
+                            end[0] + (yhh - dq * i),
+                            ((end[1] - start[1]) / (end[0] - start[0]))
+                            * (end[0] + (yhh - dq * i))
+                            + (
+                                end[1]
+                                - ((end[1] - start[1]) / (end[0] - start[0])) * end[0]
+                            ),
+                        ]
+                    )
+                    kg = 1
+                else:
+                    d = np.array(
+                        [
+                            end[0] - (yhh - dq * i),
+                            ((end[1] - start[1]) / (end[0] - start[0]))
+                            * (end[0] - (yhh - dq * i))
+                            + (
+                                end[1]
+                                - ((end[1] - start[1]) / (end[0] - start[0])) * end[0]
+                            ),
+                        ]
+                    )
+                    kg = 0
+                y = self.gen_track(
+                    ends,
+                    d,
+                    track_number,
+                    order=2,
+                    deviation=0,
+                    bias=0.5,
+                    mode=0,
+                    shake_num=0,
+                    yhh=10,
+                )
+                s += list(y["trackArray"])
+                ends = d
+            y = self.gen_track(
+                ends,
+                end,
+                track_number,
+                order=2,
+                deviation=0,
+                bias=0.5,
+                mode=0,
+                shake_num=0,
+                yhh=10,
+            )
+            s += list(y["trackArray"])
+
+        else:
+            x_track_array = self._type(mode, [start[0], end[0]], num)
+            s.extend([i, fun(i)] for i in x_track_array)
+        return {"trackArray": np.array(s), "P": w}
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/extras/ext.py` & `ayugespidertools-3.9.8/ayugespidertools/extras/ext.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/extras/oss.py` & `ayugespidertools-3.9.8/ayugespidertools/extras/oss.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import warnings
-from typing import Any, Optional
-
-from retrying import retry
-
-from ayugespidertools.common.params import Param
-
-try:
-    import oss2
-except ImportError:
-    # pip install ayugespidertools[all]
-    pass
-
-warnings.filterwarnings("ignore")
-
-__all__ = [
-    "AliOssBase",
-]
-
-
-class AliOssBase:
-    """阿里云 Oss 对象存储 python sdk 示例
-    其 GitHub 官方文档地址：
-        https://github.com/aliyun/aliyun-oss-python-sdk
-    阿里云官方 oss sdk 文档地址：
-        https://www.alibabacloud.com/help/zh/oss/developer-reference
-    """
-
-    def __init__(
-        self,
-        access_key: str,
-        access_secret: str,
-        endpoint: str,
-        bucket: str,
-        doc: Optional[str] = None,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        """初始化 auth，bucket 等信息
-
-        Args:
-            access_key: 阿里云账号 AccessKey
-            access_secret: 阿里云账号 AccessKey 对应的秘钥
-            endpoint: 填写 Bucket 所在地域对应的 Endpoint；
-                以华东1（杭州）为例，Endpoint 填写为 https://oss-cn-hangzhou.aliyuncs.com
-            bucket: 填写 Bucket 名称，此 oss 项目所属 bucket
-            doc: 需要操作的 oss 文件夹目录，比如 file/img，可选参数
-        """
-        self.endpoint = endpoint
-        self.doc = doc
-        self.auth = oss2.Auth(access_key, access_secret)
-        self.bk = bucket
-        self.bucket = oss2.Bucket(self.auth, f"{self.endpoint}/", bucket)
-        self.headers = {"Connection": "close"}
-
-    @retry(stop_max_attempt_number=Param.retry_num)
-    def put_oss(
-        self,
-        put_bytes: bytes,
-        file: str,
-    ) -> None:
-        """上传单个文件的 bytes 内容
-
-        Args:
-            put_bytes: 需要上传的文件 bytes 内容或链接
-            file: 需要上传的文件的名称
-
-        Returns:
-            None
-        """
-        assert isinstance(put_bytes, bytes), "put_bytes 需要是 bytes 格式"
-
-        oss_file_path = f"{self.doc}/{file}" if self.doc else file
-        self.bucket.put_object(oss_file_path, put_bytes)
-
-    def get_full_link(self, file: str) -> str:
-        """获取文件的完整链接
-
-        Args:
-            file: 当前文件
-
-        Returns:
-            1). 当前文件的完整链接
-        """
-        ep = self.endpoint.replace("https://", "", 1).replace("http://", "", 1)
-        oss_file_path = f"{self.doc}/{file}" if self.doc else file
-        return f"https://{self.bk}.{ep}/{oss_file_path}"
+import warnings
+from typing import Any, Optional
+
+from retrying import retry
+
+from ayugespidertools.common.params import Param
+
+try:
+    import oss2
+except ImportError:
+    # pip install ayugespidertools[all]
+    pass
+
+warnings.filterwarnings("ignore")
+
+__all__ = [
+    "AliOssBase",
+]
+
+
+class AliOssBase:
+    """阿里云 Oss 对象存储 python sdk 示例
+    其 GitHub 官方文档地址：
+        https://github.com/aliyun/aliyun-oss-python-sdk
+    阿里云官方 oss sdk 文档地址：
+        https://www.alibabacloud.com/help/zh/oss/developer-reference
+    """
+
+    def __init__(
+        self,
+        access_key: str,
+        access_secret: str,
+        endpoint: str,
+        bucket: str,
+        doc: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        """初始化 auth，bucket 等信息
+
+        Args:
+            access_key: 阿里云账号 AccessKey
+            access_secret: 阿里云账号 AccessKey 对应的秘钥
+            endpoint: 填写 Bucket 所在地域对应的 Endpoint；
+                以华东1（杭州）为例，Endpoint 填写为 https://oss-cn-hangzhou.aliyuncs.com
+            bucket: 填写 Bucket 名称，此 oss 项目所属 bucket
+            doc: 需要操作的 oss 文件夹目录，比如 file/img，可选参数
+        """
+        self.endpoint = endpoint
+        self.doc = doc
+        self.auth = oss2.Auth(access_key, access_secret)
+        self.bk = bucket
+        self.bucket = oss2.Bucket(self.auth, f"{self.endpoint}/", bucket)
+        self.headers = {"Connection": "close"}
+
+    @retry(stop_max_attempt_number=Param.retry_num)
+    def put_oss(
+        self,
+        put_bytes: bytes,
+        file: str,
+    ) -> None:
+        """上传单个文件的 bytes 内容
+
+        Args:
+            put_bytes: 需要上传的文件 bytes 内容或链接
+            file: 需要上传的文件的名称
+
+        Returns:
+            None
+        """
+        assert isinstance(put_bytes, bytes), "put_bytes 需要是 bytes 格式"
+
+        oss_file_path = f"{self.doc}/{file}" if self.doc else file
+        self.bucket.put_object(oss_file_path, put_bytes)
+
+    def get_full_link(self, file: str) -> str:
+        """获取文件的完整链接
+
+        Args:
+            file: 当前文件
+
+        Returns:
+            1). 当前文件的完整链接
+        """
+        ep = self.endpoint.replace("https://", "", 1).replace("http://", "", 1)
+        oss_file_path = f"{self.doc}/{file}" if self.doc else file
+        return f"https://{self.bk}.{ep}/{oss_file_path}"
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/formatdata.py` & `ayugespidertools-3.9.8/ayugespidertools/formatdata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,209 +1,208 @@
-import datetime
-import re
-import time
-from typing import Optional, Union
-from urllib.parse import urljoin
-
-from w3lib.html import remove_tags, replace_entities
-
-__all__ = [
-    "DataHandle",
-]
-
-
-class DataHandle:
-    """数据处理相关方法"""
-
-    @staticmethod
-    def get_full_url(domain_name: str, deal_url: str) -> str:
-        """根据域名 domain_name 拼接 deal_url 来获得完整链接
-
-        Args:
-            domain_name: 域名链接
-            deal_url: 需要拼接的 url
-
-        Returns:
-            1). 拼接完整的链接
-        """
-        return urljoin(domain_name, deal_url)
-
-    @staticmethod
-    def click_point_deal(decimal: float, decimal_places: int = 2) -> float:
-        """将小数 decimal 保留小数点后 decimal_places 位，结果四舍五入
-
-        Args:
-            decimal: 需要处理的小数
-            decimal_places: 需要保留的小数点位数
-
-        Returns:
-            1). 四舍五入后的小数点
-        """
-        # 先拼接需要保留的位数
-        decimal_deal = f"%.{decimal_places}f"
-        return float(decimal_deal % decimal)
-
-    @staticmethod
-    def judge_utc_time(local_time: str) -> bool:
-        """判断 local_time 是否为 utc 格式的时间
-
-        Args:
-            local_time: 需要判断的时间参数，比如：Thu Jul 21 17:59:44 2022 或 Fri, 22 Jul 2022 01:43:06 +0800 等等
-
-        Returns:
-            1): 是否为 utc 格式的数据
-        """
-        pattern = re.compile(r"""mon|tues|wed|thu|fri|sat|sun""")
-        return bool(pattern.findall(local_time.lower()))
-
-    @staticmethod
-    def judge_include_letter(local_time: str) -> bool:
-        pattern = re.compile(r"""[a-zA-Z]""")
-        return bool(pattern.findall(local_time.lower()))
-
-    @staticmethod
-    def _get_format_t(
-        date_style: str = "",
-        date_is_full: bool = False,
-        specific_date_conn: str = " ",
-        hms_conn: str = ":",
-    ) -> str:
-        """将需要格式化的数据用 date_style 标识来拼接起来，如果 date_is_full 为 True 时，则需要补齐"时分秒"位
-
-        Args:
-            date_style: 将格式化符拼接时需要的标识，比如：-
-            date_is_full: 是否需要完整的时间格式化（即是否需要补齐"时分秒"单位）
-            specific_date_conn: 年月日与时分秒拼接的方式
-            hms_conn: 时分秒拼接的方式
-
-        Returns:
-            1). 最终的格式化拼接结果，比如：%Y-%m-%d %H-%M-%S
-        """
-        # 年月日
-        _y_m_d = ["%Y", "%m", "%d"]
-        _y_m_d_format = date_style.join(_y_m_d)
-
-        if date_is_full:
-            # 时分秒
-            _h_m_s = ["%H", "%M", "%S"]
-            # 时分秒大都为":"连接
-            _h_m_s_format = hms_conn.join(_h_m_s)
-            return specific_date_conn.join([_y_m_d_format, _h_m_s_format])
-        return _y_m_d_format
-
-    @staticmethod
-    def _time_format(date_str: str) -> str:
-        """判断时间是什么格式的，比如：xxxx-xx-xx 或 xxxx.xx.xx
-
-        Args:
-            date_str: 需要判断格式的时间
-
-        Returns:
-            1). 时间格式的标识，比如：-，若没有就返回空字符
-        """
-        format_styles = ["-", ".", "/", "年"]
-        return next(
-            (
-                format_style
-                for format_style in format_styles
-                if format_style in date_str
-            ),
-            "",
-        )
-
-    @classmethod
-    def normal_to_stamp(
-        cls,
-        normal_time: str,
-        _format_t: Optional[str] = None,
-        date_is_full: bool = True,
-        specific_date_conn: str = " ",
-        hms_conn: str = ":",
-    ) -> int:
-        """将网页正常时间转为时间戳
-
-        Args:
-            normal_time: 需要转换的时间
-            _format_t: 时间格式化符，默认不填。除非在英文时间的参数出错时可指定 _format_t 的值
-            date_is_full: 是否包含"时分秒"单位的完整格式
-            specific_date_conn: 年月日与时分秒拼接的方式
-            hms_conn: 时分秒拼接的方式
-
-        Returns:
-            stamp: 返回的时间戳
-        """
-        # 判断 normal_time 是否是特殊模式
-        is_utc_time = cls.judge_utc_time(normal_time)
-        is_letter_time = cls.judge_include_letter(normal_time)
-        # stamp = None
-        if any([is_utc_time, is_letter_time]):
-            # 如果不传递时间的格式符参数
-            if not _format_t:
-                if "," in normal_time:
-                    _format_t = "%a, %d %b %Y %H:%M:%S +0800"
-                else:
-                    _format_t = "%a %b %d %H:%M:%S %Y"
-            standard_time = datetime.datetime.strptime(normal_time, _format_t)
-            stamp = time.mktime(
-                time.strptime(str(standard_time), cls._get_format_t("-", True))
-            )
-
-        else:
-            # 先判断正常时间的格式
-            date_style = cls._time_format(normal_time)
-            # standard_time_format = _get_format_t(date_style, date_is_full).replace('%m', '%b').replace('-', '/')
-            standard_time_format = cls._get_format_t(
-                date_style, date_is_full, specific_date_conn, hms_conn
-            )
-            stamp = time.mktime(time.strptime(normal_time, standard_time_format))
-        return int(stamp)
-
-    @staticmethod
-    def timestamp_to_normal(timestamp: Union[int, str]) -> str:
-        """将时间戳转为正常时间 xxxx-xx-xx xx:xx:xx 的格式
-
-        Args:
-            timestamp: 需要处理的时间格式
-
-        Returns:
-            1). 转换后的时间结果
-        """
-        _timestamp = str(timestamp) if isinstance(timestamp, int) else timestamp
-        timestamp_normal = int(_timestamp[:10])
-        time_array = time.localtime(timestamp_normal)
-        return time.strftime("%Y-%m-%d %H:%M:%S", time_array)
-
-    @staticmethod
-    def remove_all_tags(func):
-        """去除所有标签"""
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            func_res = remove_tags(func_res)
-            return func_res
-
-        return inner
-
-    @staticmethod
-    def normal_display(func):
-        """去除掉网页的注释(将网页中的特殊字符的源码改成正常显示)"""
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            func_res = replace_entities(func_res)
-            return func_res
-
-        return inner
-
-    @staticmethod
-    def simple_deal_for_extract(func):
-        """将 xpath, css 或 json 提取的数据做简单处理；提取的数据若非数组数据，则统一返回字符类型"""
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            if type(func_res) in [str, int, float, bool]:
-                # 这里可添加一些通用的数据处理
-                return str(func_res).strip()
-            else:
-                return func_res
-
-        return inner
+import datetime
+import re
+import time
+from typing import Optional, Union
+from urllib.parse import urljoin
+
+from w3lib.html import remove_tags, replace_entities
+
+__all__ = [
+    "DataHandle",
+]
+
+
+class DataHandle:
+    """数据处理相关方法"""
+
+    @staticmethod
+    def get_full_url(domain_name: str, deal_url: str) -> str:
+        """根据域名 domain_name 拼接 deal_url 来获得完整链接
+
+        Args:
+            domain_name: 域名链接
+            deal_url: 需要拼接的 url
+
+        Returns:
+            1). 拼接完整的链接
+        """
+        return urljoin(domain_name, deal_url)
+
+    @staticmethod
+    def click_point_deal(decimal: float, decimal_places: int = 2) -> float:
+        """将小数 decimal 保留小数点后 decimal_places 位，结果四舍五入
+
+        Args:
+            decimal: 需要处理的小数
+            decimal_places: 需要保留的小数点位数
+
+        Returns:
+            1). 四舍五入后的小数点
+        """
+        decimal_deal = f"%.{decimal_places}f"
+        return float(decimal_deal % decimal)
+
+    @staticmethod
+    def judge_utc_time(local_time: str) -> bool:
+        """判断 local_time 是否为 utc 格式的时间
+
+        Args:
+            local_time: 需要判断的时间参数，比如：Thu Jul 21 17:59:44 2022 或 Fri, 22 Jul 2022 01:43:06 +0800 等等
+
+        Returns:
+            1): 是否为 utc 格式的数据
+        """
+        pattern = re.compile(r"""mon|tues|wed|thu|fri|sat|sun""")
+        return bool(pattern.findall(local_time.lower()))
+
+    @staticmethod
+    def judge_include_letter(local_time: str) -> bool:
+        pattern = re.compile(r"""[a-zA-Z]""")
+        return bool(pattern.findall(local_time.lower()))
+
+    @staticmethod
+    def _get_format_t(
+        date_style: str = "",
+        date_is_full: bool = False,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> str:
+        """将需要格式化的数据用 date_style 标识来拼接起来，如果 date_is_full 为 True 时，则需要补齐"时分秒"位
+
+        Args:
+            date_style: 将格式化符拼接时需要的标识，比如：-
+            date_is_full: 是否需要完整的时间格式化（即是否需要补齐"时分秒"单位）
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            1). 最终的格式化拼接结果，比如：%Y-%m-%d %H-%M-%S
+        """
+        # 年月日
+        _y_m_d = ["%Y", "%m", "%d"]
+        _y_m_d_format = date_style.join(_y_m_d)
+
+        if date_is_full:
+            # 时分秒
+            _h_m_s = ["%H", "%M", "%S"]
+            # 时分秒大都为":"连接
+            _h_m_s_format = hms_conn.join(_h_m_s)
+            return specific_date_conn.join([_y_m_d_format, _h_m_s_format])
+        return _y_m_d_format
+
+    @staticmethod
+    def _time_format(date_str: str) -> str:
+        """判断时间是什么格式的，比如：xxxx-xx-xx 或 xxxx.xx.xx
+
+        Args:
+            date_str: 需要判断格式的时间
+
+        Returns:
+            1). 时间格式的标识，比如：-，若没有就返回空字符
+        """
+        format_styles = ["-", ".", "/", "年"]
+        return next(
+            (
+                format_style
+                for format_style in format_styles
+                if format_style in date_str
+            ),
+            "",
+        )
+
+    @classmethod
+    def normal_to_stamp(
+        cls,
+        normal_time: str,
+        _format_t: Optional[str] = None,
+        date_is_full: bool = True,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> int:
+        """将网页正常时间转为时间戳
+
+        Args:
+            normal_time: 需要转换的时间
+            _format_t: 时间格式化符，默认不填。除非在英文时间的参数出错时可指定 _format_t 的值
+            date_is_full: 是否包含"时分秒"单位的完整格式
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            stamp: 返回的时间戳
+        """
+        # 判断 normal_time 是否是特殊模式
+        is_utc_time = cls.judge_utc_time(normal_time)
+        is_letter_time = cls.judge_include_letter(normal_time)
+        # stamp = None
+        if any([is_utc_time, is_letter_time]):
+            # 如果不传递时间的格式符参数
+            if not _format_t:
+                if "," in normal_time:
+                    _format_t = "%a, %d %b %Y %H:%M:%S +0800"
+                else:
+                    _format_t = "%a %b %d %H:%M:%S %Y"
+            standard_time = datetime.datetime.strptime(normal_time, _format_t)
+            stamp = time.mktime(
+                time.strptime(str(standard_time), cls._get_format_t("-", True))
+            )
+
+        else:
+            # 先判断正常时间的格式
+            date_style = cls._time_format(normal_time)
+            # standard_time_format = _get_format_t(date_style, date_is_full).replace('%m', '%b').replace('-', '/')
+            standard_time_format = cls._get_format_t(
+                date_style, date_is_full, specific_date_conn, hms_conn
+            )
+            stamp = time.mktime(time.strptime(normal_time, standard_time_format))
+        return int(stamp)
+
+    @staticmethod
+    def timestamp_to_normal(timestamp: Union[int, str]) -> str:
+        """将时间戳转为正常时间 xxxx-xx-xx xx:xx:xx 的格式
+
+        Args:
+            timestamp: 需要处理的时间格式
+
+        Returns:
+            1). 转换后的时间结果
+        """
+        _timestamp = str(timestamp) if isinstance(timestamp, int) else timestamp
+        timestamp_normal = int(_timestamp[:10])
+        time_array = time.localtime(timestamp_normal)
+        return time.strftime("%Y-%m-%d %H:%M:%S", time_array)
+
+    @staticmethod
+    def remove_all_tags(func):
+        """去除所有标签"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = remove_tags(func_res)
+            return func_res
+
+        return inner
+
+    @staticmethod
+    def normal_display(func):
+        """去除掉网页的注释(将网页中的特殊字符的源码改成正常显示)"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = replace_entities(func_res)
+            return func_res
+
+        return inner
+
+    @staticmethod
+    def simple_deal_for_extract(func):
+        """将 xpath, css 或 json 提取的数据做简单处理；提取的数据若非数组数据，则统一返回字符类型"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            if type(func_res) in [str, int, float, bool]:
+                # 这里可添加一些通用的数据处理
+                return str(func_res).strip()
+            else:
+                return func_res
+
+        return inner
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/items.py` & `ayugespidertools-3.9.8/ayugespidertools/items.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from abc import ABCMeta
-from collections.abc import MutableMapping
-from dataclasses import dataclass
-from typing import Any, Dict, NamedTuple, Optional, Union
-
-import scrapy
-from scrapy.item import Item
-
-from ayugespidertools.common.typevars import EmptyKeyError, FieldAlreadyExistsError
-
-__all__ = [
-    "DataItem",
-    "AyuItem",
-]
-
-
-class ScrapyItem(Item):
-    """scrapy item 的标准方式"""
-
-    ...
-
-
-class DataItem(NamedTuple):
-    """用于描述 item 中字段
-
-    Attributes:
-        key_value: 参数值
-        notes: 对参数的注释
-    """
-
-    key_value: Any
-    notes: Any = ""
-
-
-class ItemMeta(ABCMeta):
-    def __new__(cls, class_name, bases, attrs):
-        def add_field(self, key: str, value: Any) -> None:
-            """动态添加字段方法
-
-            Args:
-                self: self
-                key: 需要添加的字段名
-                value: 需要添加的字段对应的值
-            """
-            if not key:
-                raise EmptyKeyError()
-            if key in self._AyuItem__fields:
-                raise FieldAlreadyExistsError(key)
-            setattr(self, key, value)
-            self._AyuItem__fields.add(key)
-
-        def asdict(self) -> Dict[str, Any]:
-            """将 AyuItem 转换为 dict"""
-            self._AyuItem__fields.discard("_AyuItem__fields")
-            _item_dict = {key: getattr(self, key) for key in self._AyuItem__fields}
-            return _item_dict
-
-        def asitem(self, assignment: bool = True) -> ScrapyItem:
-            """将 AyuItem 转换为 ScrapyItem
-
-            Args:
-                self: self
-                assignment: 是否将 AyuItem 中的值赋值给 ScrapyItem，默认为 True
-
-            Returns:
-                1). 转换 ScrapyItem 后的实例
-            """
-            item_temp = ScrapyItem()
-            for k, v in self.asdict().items():
-                item_temp.fields[k] = scrapy.Field()
-                if assignment:
-                    item_temp[k] = v
-            return item_temp
-
-        attrs["add_field"] = add_field
-        attrs["asdict"] = asdict
-        attrs["asitem"] = asitem
-        return super().__new__(cls, class_name, bases, attrs)
-
-
-@dataclass
-class AyuItem(MutableMapping, metaclass=ItemMeta):
-    """Used to create AyuItem and add fields dynamically,
-    and provides methods to convert to dict and ScrapyItem.
-
-    Examples:
-        >>> item = AyuItem(
-        ...     _table="ta",
-        ... )
-        >>> # 获取字段
-        >>> item["_table"]
-        'ta'
-        >>>
-        >>> # 添加 / 修改字段，不存在则创建，存在则修改
-        >>> item["_table"] = "tab"
-        >>> item["title"] = "tit"
-        >>> # 也可通过 add_field 添加字段，但不能重复添加相同字段
-        >>> item.add_field("num", 10)
-        >>> [ item["_table"], item["title"], item["num"] ]
-        ['tab', 'tit', 10]
-        >>> item.asdict()
-        {'title': 'tit', '_table': 'tab', 'num': 10}
-        >>> type(item.asitem())
-        <class 'ayugespidertools.items.ScrapyItem'>
-        >>> # 删除字段
-        >>> del item["title"]
-        >>> item
-        {'_table': 'tab', 'num': 10}
-    """
-
-    def __init__(
-        self,
-        _table: Union[DataItem, str],
-        _mongo_update_rule: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        """初始化 AyuItem 实例
-
-        Args:
-            _table: 数据库表名。
-            _mongo_update_rule: MongoDB 存储场景下可能需要的查重条件，默认为 None。
-        """
-        self.__fields = set()
-        if _table:
-            self.__fields.add("_table")
-            setattr(self, "_table", _table)
-        if _mongo_update_rule:
-            self.__fields.add("_mongo_update_rule")
-            setattr(self, "_mongo_update_rule", _mongo_update_rule)
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-            self.__fields.add(key)
-
-    def __getitem__(self, key):
-        return getattr(self, key)
-
-    def __setitem__(self, key, value):
-        if key not in self.__fields:
-            setattr(self, key, value)
-            self.__fields.add(key)
-        else:
-            setattr(self, key, value)
-
-    def __delitem__(self, key):
-        if key not in self.__fields:
-            raise KeyError(f"{key} not found")
-        delattr(self, key)
-        self.__fields.discard(key)
-
-    def __getattr__(self, name):
-        if name in self.__fields:
-            raise AttributeError(f"Try to use item[{name!r}] to get field value")
-        raise AttributeError(name)
-
-    def __setattr__(self, name, value):
-        super().__setattr__(name, value)
-        self.__fields.add(name)
-
-    def __delattr__(self, name):
-        super().__delattr__(name)
-        self.__fields.discard(name)
-
-    def __iter__(self):
-        return iter(self.__fields)
-
-    def __len__(self):
-        return len(self.__fields)
-
-    def __str__(self):
-        # 与下方 __repr__ 一样，不返回 AyuItem(field=data) 的格式
-        return f"{self.asdict()}"
-
-    def __repr__(self):
-        return f"{self.asdict()}"
-
-    def fields(self):
-        self.__fields.discard("_AyuItem__fields")
-        return self.__fields
-
-    def add_field(self, key: str, value: Any) -> None: ...
-
-    def asdict(self) -> Dict[str, Any]: ...
-
-    def asitem(self, assignment: bool = True) -> ScrapyItem: ...
+from abc import ABCMeta
+from collections.abc import MutableMapping
+from dataclasses import dataclass
+from typing import Any, Dict, NamedTuple, Optional, Union
+
+import scrapy
+from scrapy.item import Item
+
+from ayugespidertools.common.typevars import EmptyKeyError, FieldAlreadyExistsError
+
+__all__ = [
+    "DataItem",
+    "AyuItem",
+]
+
+
+class ScrapyItem(Item):
+    """scrapy item 的标准方式"""
+
+    ...
+
+
+class DataItem(NamedTuple):
+    """用于描述 item 中字段
+
+    Attributes:
+        key_value: 参数值
+        notes: 对参数的注释
+    """
+
+    key_value: Any
+    notes: Any = ""
+
+
+class ItemMeta(ABCMeta):
+    def __new__(cls, class_name, bases, attrs):
+        def add_field(self, key: str, value: Any) -> None:
+            """动态添加字段方法
+
+            Args:
+                self: self
+                key: 需要添加的字段名
+                value: 需要添加的字段对应的值
+            """
+            if not key:
+                raise EmptyKeyError()
+            if key in self._AyuItem__fields:
+                raise FieldAlreadyExistsError(key)
+            setattr(self, key, value)
+            self._AyuItem__fields.add(key)
+
+        def asdict(self) -> Dict[str, Any]:
+            """将 AyuItem 转换为 dict"""
+            self._AyuItem__fields.discard("_AyuItem__fields")
+            _item_dict = {key: getattr(self, key) for key in self._AyuItem__fields}
+            return _item_dict
+
+        def asitem(self, assignment: bool = True) -> ScrapyItem:
+            """将 AyuItem 转换为 ScrapyItem
+
+            Args:
+                self: self
+                assignment: 是否将 AyuItem 中的值赋值给 ScrapyItem，默认为 True
+
+            Returns:
+                1). 转换 ScrapyItem 后的实例
+            """
+            item_temp = ScrapyItem()
+            for k, v in self.asdict().items():
+                item_temp.fields[k] = scrapy.Field()
+                if assignment:
+                    item_temp[k] = v
+            return item_temp
+
+        attrs["add_field"] = add_field
+        attrs["asdict"] = asdict
+        attrs["asitem"] = asitem
+        return super().__new__(cls, class_name, bases, attrs)
+
+
+@dataclass
+class AyuItem(MutableMapping, metaclass=ItemMeta):
+    """Used to create AyuItem and add fields dynamically,
+    and provides methods to convert to dict and ScrapyItem.
+
+    Examples:
+        >>> item = AyuItem(
+        ...     _table="ta",
+        ... )
+        >>> # 获取字段
+        >>> item["_table"]
+        'ta'
+        >>>
+        >>> # 添加 / 修改字段，不存在则创建，存在则修改
+        >>> item["_table"] = "tab"
+        >>> item["title"] = "tit"
+        >>> # 也可通过 add_field 添加字段，但不能重复添加相同字段
+        >>> item.add_field("num", 10)
+        >>> [ item["_table"], item["title"], item["num"] ]
+        ['tab', 'tit', 10]
+        >>> item.asdict()
+        {'title': 'tit', '_table': 'tab', 'num': 10}
+        >>> type(item.asitem())
+        <class 'ayugespidertools.items.ScrapyItem'>
+        >>> # 删除字段
+        >>> del item["title"]
+        >>> item
+        {'_table': 'tab', 'num': 10}
+    """
+
+    def __init__(
+        self,
+        _table: Union[DataItem, str],
+        _mongo_update_rule: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ):
+        """初始化 AyuItem 实例
+
+        Args:
+            _table: 数据库表名。
+            _mongo_update_rule: MongoDB 存储场景下可能需要的查重条件，默认为 None。
+        """
+        self.__fields = set()
+        if _table:
+            self.__fields.add("_table")
+            setattr(self, "_table", _table)
+        if _mongo_update_rule:
+            self.__fields.add("_mongo_update_rule")
+            setattr(self, "_mongo_update_rule", _mongo_update_rule)
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+            self.__fields.add(key)
+
+    def __getitem__(self, key):
+        return getattr(self, key)
+
+    def __setitem__(self, key, value):
+        if key not in self.__fields:
+            setattr(self, key, value)
+            self.__fields.add(key)
+        else:
+            setattr(self, key, value)
+
+    def __delitem__(self, key):
+        if key not in self.__fields:
+            raise KeyError(f"{key} not found")
+        delattr(self, key)
+        self.__fields.discard(key)
+
+    def __getattr__(self, name):
+        if name in self.__fields:
+            raise AttributeError(f"Try to use item[{name!r}] to get field value")
+        raise AttributeError(name)
+
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        self.__fields.add(name)
+
+    def __delattr__(self, name):
+        super().__delattr__(name)
+        self.__fields.discard(name)
+
+    def __iter__(self):
+        return iter(self.__fields)
+
+    def __len__(self):
+        return len(self.__fields)
+
+    def __str__(self):
+        # 与下方 __repr__ 一样，不返回 AyuItem(field=data) 的格式
+        return f"{self.asdict()}"
+
+    def __repr__(self):
+        return f"{self.asdict()}"
+
+    def fields(self):
+        self.__fields.discard("_AyuItem__fields")
+        return self.__fields
+
+    def add_field(self, key: str, value: Any) -> None: ...
+
+    def asdict(self) -> Dict[str, Any]: ...
+
+    def asitem(self, assignment: bool = True) -> ScrapyItem: ...
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/middlewares.py` & `ayugespidertools-3.9.8/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.9.8/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/http/request/form.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,44 @@
-import copy
-from dataclasses import asdict
-from typing import (
-    Any,
-    AnyStr,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    Tuple,
-    Union,
-)
-
-from scrapy import Request
-
-from ayugespidertools.common.typevars import AiohttpRequestArgs
-
-__all__ = [
-    "AiohttpRequest",
-]
-
-
-class AiohttpRequest(Request):
-    """为 scrapy 的 Request 对象添加额外的参数"""
-
-    def __init__(
-        self,
-        url: str,
-        callback: Optional[Callable] = None,
-        method: str = "GET",
-        headers: Union[Mapping[AnyStr, Any], Iterable[Tuple[AnyStr, Any]], None] = None,
-        body: Optional[Union[bytes, str]] = None,
-        cookies: Optional[Union[dict, List[dict]]] = None,
-        meta: Optional[Dict[str, Any]] = None,
-        args: Optional[Union[AiohttpRequestArgs, dict]] = None,
-        **kwargs,
-    ) -> None:
-        meta = copy.deepcopy(meta) or {}
-        aiohttp_meta = meta.setdefault("aiohttp", {})
-
-        _args = {"url": url}
-        if isinstance(args, AiohttpRequestArgs):
-            args = asdict(args)
-        _args.update(args or {})
-        _args.update(aiohttp_meta.get("args", {}))
-        aiohttp_meta["args"] = _args
-
-        super(AiohttpRequest, self).__init__(
-            url,
-            callback,
-            method=method,
-            headers=headers,
-            body=body,
-            cookies=cookies,
-            meta=meta,
-            **kwargs,
-        )
+from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Optional, Tuple, Union
+
+from scrapy import FormRequest
+
+from ayugespidertools.scraper.http.request import AiohttpRequest
+
+__all__ = [
+    "AiohttpFormRequest",
+]
+
+if TYPE_CHECKING:
+    from ayugespidertools.common.typevars import AiohttpRequestArgs
+
+FormdataKVType = Tuple[str, Union[str, Iterable[str]]]
+FormdataType = Optional[Union[dict, List[FormdataKVType]]]
+
+
+class AiohttpFormRequest(AiohttpRequest, FormRequest):
+    """使用 aiohttp 发送 FormRequest 请求"""
+
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        callback: Optional[Callable] = None,
+        method: Optional[str] = None,
+        formdata: FormdataType = None,
+        body: Optional[Union[bytes, str]] = None,
+        args: Optional[Union["AiohttpRequestArgs", dict]] = None,
+        **kwargs: Any
+    ) -> None:
+        # First init FormRequest to get url, body and method
+        if formdata:
+            FormRequest.__init__(self, url=url, method=method, formdata=formdata)
+            url, method, body = self.url, self.method, self.body
+        # Then pass all other kwargs to AiohttpRequest
+        AiohttpRequest.__init__(
+            self,
+            url=url,
+            callback=callback,
+            method=method,
+            body=body,
+            args=args,
+            **kwargs
+        )
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-import random
-from typing import TYPE_CHECKING
-
-from scrapy import signals
-
-from ayugespidertools.common.params import Param
-
-__all__ = [
-    "RandomRequestUaMiddleware",
-]
-
-if TYPE_CHECKING:
-    from scrapy import Request
-    from scrapy.crawler import Crawler
-    from typing_extensions import Self
-
-    from ayugespidertools.spiders import AyuSpider
-
-
-class RandomRequestUaMiddleware:
-    """随机请求头中间件"""
-
-    def __init__(self):
-        self.explorer_types = None
-        self.explorer_weights = None
-
-    def get_random_ua_by_weight(self) -> str:
-        # 先按权重取出所需浏览器类型
-        explorer_types = random.choices(
-            self.explorer_types, weights=self.explorer_weights
-        )
-        return random.choice(Param.fake_useragent_dict[explorer_types[0]])
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler") -> "Self":
-        s = cls()
-        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
-        return s
-
-    def spider_opened(self, spider: "AyuSpider") -> None:
-        # 带权重的 ua 列表，这里是根据 fake_useragent 库中的打印信息来规划权重的。
-        ua_arr = [
-            {"explorer": "opera", "weight": 16},
-            {"explorer": "safari", "weight": 32},
-            {"explorer": "internetexplorer", "weight": 41},
-            {"explorer": "firefox", "weight": 124},
-            {"explorer": "chrome", "weight": 772},
-        ]
-        self.explorer_types = [x["explorer"] for x in ua_arr]
-        self.explorer_weights = [x["weight"] for x in ua_arr]
-        spider.slog.info(
-            f"随机请求头中间件 RandomRequestUaMiddleware 已开启，生效脚本为: {spider.name}"
-        )
-
-    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
-        # 根据权重来获取随机请求头 ua 信息
-        request.headers.setdefault(b"User-Agent", self.get_random_ua_by_weight())
+import random
+from typing import TYPE_CHECKING
+
+from scrapy import signals
+
+from ayugespidertools.common.params import Param
+
+__all__ = [
+    "RandomRequestUaMiddleware",
+]
+
+if TYPE_CHECKING:
+    from scrapy import Request
+    from scrapy.crawler import Crawler
+    from typing_extensions import Self
+
+    from ayugespidertools.spiders import AyuSpider
+
+
+class RandomRequestUaMiddleware:
+    """随机请求头中间件"""
+
+    def __init__(self):
+        self.explorer_types = None
+        self.explorer_weights = None
+
+    def get_random_ua_by_weight(self) -> str:
+        explorer_types = random.choices(
+            self.explorer_types, weights=self.explorer_weights
+        )
+        return random.choice(Param.fake_useragent_dict[explorer_types[0]])
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler") -> "Self":
+        s = cls()
+        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
+        return s
+
+    def spider_opened(self, spider: "AyuSpider") -> None:
+        # 带权重的 ua 列表，这里是根据 fake_useragent 库中的打印信息来规划权重的。
+        ua_arr = [
+            {"explorer": "opera", "weight": 16},
+            {"explorer": "safari", "weight": 32},
+            {"explorer": "internetexplorer", "weight": 41},
+            {"explorer": "firefox", "weight": 124},
+            {"explorer": "chrome", "weight": 772},
+        ]
+        self.explorer_types = [x["explorer"] for x in ua_arr]
+        self.explorer_weights = [x["weight"] for x in ua_arr]
+        spider.slog.info(
+            f"随机请求头中间件 RandomRequestUaMiddleware 已开启，生效脚本为: {spider.name}"
+        )
+
+    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
+        request.headers.setdefault(b"User-Agent", self.get_random_ua_by_weight())
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-import asyncio
-from typing import TYPE_CHECKING, Any, Optional, Tuple, TypeVar, Union
-
-import aiohttp
-from itemadapter import ItemAdapter
-from scrapy import signals
-from scrapy.http import HtmlResponse
-from scrapy.utils.python import global_object_name
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import AiohttpConf, AiohttpRequestArgs
-from ayugespidertools.common.utils import ToolsForAyu
-from ayugespidertools.config import logger
-
-__all__ = [
-    "AiohttpDownloaderMiddleware",
-]
-
-if TYPE_CHECKING:
-    from scrapy import Request
-    from scrapy.crawler import Crawler
-    from scrapy.http import Response
-    from scrapy.statscollectors import StatsCollector
-    from typing_extensions import Self
-
-    from ayugespidertools.common.typevars import slogT
-    from ayugespidertools.scraper.http import AiohttpRequest
-    from ayugespidertools.spiders import AyuSpider
-
-    AyuRequest = Union[AiohttpRequest, Request]
-
-ItemAdapterT = TypeVar("ItemAdapterT", bound=ItemAdapter)
-
-
-class AiohttpDownloaderMiddleware:
-    """Downloader middleware handling the requests with aiohttp"""
-
-    session: "aiohttp.ClientSession"
-    priority_adjust: int
-    aiohttp_cfg: AiohttpConf
-    aiohttp_args: dict
-    slog: "slogT"
-
-    def _retry(
-        self,
-        request: "AyuRequest",
-        reason: int,
-        spider: "AyuSpider",
-    ) -> Optional["AyuRequest"]:
-        """重试请求
-
-        Args:
-            request: retry request
-            reason: retry reason
-            spider: AyuSpider
-
-        Returns:
-            1). Optional["AyuRequest"]: 重试的 request 对象
-        """
-        retries = request.meta.get("retry_times", 0) + 1
-        stats = spider.crawler.stats
-        if retries <= self.aiohttp_cfg.retry_times:
-            return self._retry_with_limit(request, retries, reason, stats)
-
-        stats.inc_value("retry/max_reached")
-        logger.error(f"Gave up retrying {request} (failed {retries} times): {reason}")
-        return None
-
-    def _retry_with_limit(
-        self,
-        request: "AyuRequest",
-        retries: int,
-        reason: int,
-        stats: "StatsCollector",
-    ):
-        logger.debug(f"Retrying {request} (failed {retries} times): {reason}")
-        retry_req = request.copy()
-        retry_req.meta["retry_times"] = retries
-        retry_req.dont_filter = True
-        # 优先级逐级降低，以防堆积
-        retry_req.priority = request.priority + self.priority_adjust
-
-        if isinstance(reason, Exception):
-            reason = global_object_name(reason.__class__)
-
-        stats.inc_value("retry/count")
-        stats.inc_value(f"retry/reason_count/{reason}")
-        return retry_req
-
-    def _get_args(self, key: str) -> Any:
-        """根据优先级依次获取不为 None 的请求参数"""
-        data_lst = [
-            self.aiohttp_args.get(key),
-            getattr(self.aiohttp_cfg, key),
-        ]
-        return ToolsForAyu.first_not_none(data_lst=data_lst)
-
-    def spider_opened(self, spider: "AyuSpider") -> None:
-        self.slog = spider.slog
-        settings = spider.crawler.settings
-        # 自定义 aiohttp 全局配置信息，优先级小于 aiohttp_meta 中的配置
-        if local_aiohttp_conf := settings.get("AIOHTTP_CONFIG", {}):
-            # 这里的配置信息如果在 aiohttp_meta 中重复设置，则会更新当前请求的参数
-            self.aiohttp_cfg = AiohttpConf(
-                timeout=settings.get("DOWNLOAD_TIMEOUT"),
-                sleep=local_aiohttp_conf.get("sleep"),
-                proxy=local_aiohttp_conf.get("proxy"),
-                proxy_auth=local_aiohttp_conf.get("proxy_auth"),
-                proxy_headers=local_aiohttp_conf.get("proxy_headers"),
-                retry_times=local_aiohttp_conf.get(
-                    "retry_times", Param.aiohttp_retry_times_default
-                ),
-                limit=local_aiohttp_conf.get("limit", 100),
-                ssl=local_aiohttp_conf.get("ssl", True),
-                verify_ssl=local_aiohttp_conf.get("verify_ssl", True),
-                limit_per_host=local_aiohttp_conf.get("limit_per_host", 0),
-                allow_redirects=local_aiohttp_conf.get("allow_redirects", True),
-            )
-
-            # 这些参数全局生效，不会在 meta 中更新
-            _connector = aiohttp.TCPConnector(
-                ssl=self.aiohttp_cfg.ssl,
-                limit=self.aiohttp_cfg.limit,
-                verify_ssl=self.aiohttp_cfg.verify_ssl,
-                limit_per_host=self.aiohttp_cfg.limit_per_host,
-            )
-            # 超时设置, 若同时配置 AiohttpRequestArgs 的 timeout 参数会更新此值
-            _timeout = aiohttp.ClientTimeout(total=self.aiohttp_cfg.timeout)
-            self.session = aiohttp.ClientSession(connector=_connector, timeout=_timeout)
-            self.priority_adjust = settings.getint("RETRY_PRIORITY_ADJUST")
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler") -> "Self":
-        s = cls()
-        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
-        crawler.signals.connect(s.spider_closed, signal=signals.spider_closed)
-        return s
-
-    async def _request_by_aiohttp(
-        self,
-        aio_request_args: ItemAdapterT,
-    ) -> Tuple[int, str]:
-        """使用 aiohttp 来请求
-
-        Args:
-            aio_request_args: aiohttp 请求参数
-
-        Returns:
-            1). status_code: 状态码
-            2). r_text: 响应内容
-        """
-        try:
-            async with self.session.request(**aio_request_args) as r:
-                status_code = r.status
-                r_text = await r.text(errors="ignore")
-                return status_code, r_text
-        except Exception as e:
-            self.slog.error(f"aiohttp 出现请求错误，Error: {e}")
-            return 504, ""
-
-    async def process_request(
-        self, request: "AyuRequest", spider: "AyuSpider"
-    ) -> Union["AyuRequest", "Response", None]:
-        aiohttp_options = request.meta.get("aiohttp")
-        self.aiohttp_args = aiohttp_options.setdefault("args", {})
-
-        # 设置 url
-        _url = self.aiohttp_args.get("url") or request.url
-        aiohttp_req_args = AiohttpRequestArgs(url=_url)
-
-        # 设置请求方式
-        if _method := self.aiohttp_args.get("method"):
-            aiohttp_req_args.method = _method
-        elif _method := str(request.method).upper():
-            aiohttp_req_args.method = _method  # type: ignore
-        if _method not in {"GET", "POST", "PUT", "DELETE", "HEAD", "OPTIONS", "PATCH"}:
-            logger.error(f"出现未知请求方式 {_method}，请及时查看，默认 GET")
-
-        # 设置请求头信息
-        if _headers_args := self.aiohttp_args.get("headers"):
-            aiohttp_req_args.headers = _headers_args
-        elif _headers_args := ToolsForAyu.get_dict_form_scrapy_req_headers(
-            scrapy_headers=request.headers
-        ):
-            aiohttp_req_args.headers = _headers_args
-
-        # 设置请求 body 参数，GET 情况下和 POST 情况下的请求参数处理
-        if _req_data := self.aiohttp_args.get("data"):
-            aiohttp_req_args.data = _req_data
-        elif req_data_str := str(request.body, encoding="utf-8"):
-            # 如果是 json 字典格式的数据时，则是 scrapy body 传来的 json dumps 参数
-            if ReuseOperation.judge_str_is_json(judge_str=req_data_str):
-                aiohttp_req_args.data = req_data_str
-            # 否则就是传来的字典格式
-            else:
-                req_data_dict = ReuseOperation.get_req_dict_from_scrapy(
-                    req_body_data_str=req_data_str
-                )
-                aiohttp_req_args.data = req_data_dict
-
-        # 设置 proxy
-        if _proxy := self._get_args("proxy"):
-            aiohttp_req_args.proxy = _proxy
-        if _proxy_auth := self._get_args("proxy_auth"):
-            aiohttp_req_args.proxy_auth = _proxy_auth
-        if _proxy_headers := self._get_args("proxy_headers"):
-            aiohttp_req_args.proxy_headers = _proxy_headers
-
-        # 设置 allow_redirects
-        _allow_redirects = self._get_args("allow_redirects")
-        if _allow_redirects is not None:
-            aiohttp_req_args.allow_redirects = _allow_redirects
-
-        # 设置 cookies，优先从 AiohttpRequest 中的 cookies 参数中取值，没有时再从 headers 中取值
-        _ck_args = self.aiohttp_args.get("cookies")
-        aiohttp_cookie_dict = _ck_args if _ck_args is not None else request.cookies
-        if all([not aiohttp_cookie_dict, request.headers.get("Cookie", None)]):
-            headers_cookie_str = str(request.headers.get("Cookie"), encoding="utf-8")
-            aiohttp_cookie_dict = ReuseOperation.get_ck_dict_from_headers(
-                headers_ck_str=headers_cookie_str
-            )
-        aiohttp_req_args.cookies = aiohttp_cookie_dict
-
-        # 超时设置
-        if _timeout := self.aiohttp_args.get("timeout"):
-            aiohttp_req_args.timeout = _timeout
-
-        aio_request_args = ItemAdapter(aiohttp_req_args)
-        status_code, html_content = await self._request_by_aiohttp(
-            aio_request_args=aio_request_args
-        )
-
-        # 请求间隔设置
-        _sleep = self._get_args("sleep")
-        await asyncio.sleep(_sleep)
-
-        if all([status_code == 504, not html_content]):
-            spider.slog.error(f"url: {_url} 返回内容为空，请求超时！")
-            self._retry(request=request, reason=504, spider=spider)
-
-        return HtmlResponse(
-            url=_url,
-            status=status_code,
-            headers=aiohttp_req_args.headers,
-            body=html_content,
-            encoding="utf-8",
-            request=request,
-        )
-
-    async def spider_closed(self, spider: "AyuSpider") -> None:
-        await self.session.close()
+import asyncio
+from typing import TYPE_CHECKING, Any, Optional, Tuple, TypeVar, Union
+
+import aiohttp
+from itemadapter import ItemAdapter
+from scrapy import signals
+from scrapy.http import HtmlResponse
+from scrapy.utils.python import global_object_name
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import AiohttpConf, AiohttpRequestArgs
+from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.config import logger
+
+__all__ = [
+    "AiohttpDownloaderMiddleware",
+]
+
+if TYPE_CHECKING:
+    from scrapy import Request
+    from scrapy.crawler import Crawler
+    from scrapy.http import Response
+    from scrapy.statscollectors import StatsCollector
+    from typing_extensions import Self
+
+    from ayugespidertools.common.typevars import slogT
+    from ayugespidertools.scraper.http import AiohttpRequest
+    from ayugespidertools.spiders import AyuSpider
+
+    AyuRequest = Union[AiohttpRequest, Request]
+
+ItemAdapterT = TypeVar("ItemAdapterT", bound=ItemAdapter)
+
+
+class AiohttpDownloaderMiddleware:
+    """Downloader middleware handling the requests with aiohttp"""
+
+    session: "aiohttp.ClientSession"
+    priority_adjust: int
+    aiohttp_cfg: AiohttpConf
+    aiohttp_args: dict
+    slog: "slogT"
+
+    def _retry(
+        self,
+        request: "AyuRequest",
+        reason: int,
+        spider: "AyuSpider",
+    ) -> Optional["AyuRequest"]:
+        """重试请求
+
+        Args:
+            request: retry request
+            reason: retry reason
+            spider: AyuSpider
+
+        Returns:
+            1). Optional["AyuRequest"]: 重试的 request 对象
+        """
+        retries = request.meta.get("retry_times", 0) + 1
+        stats = spider.crawler.stats
+        if retries <= self.aiohttp_cfg.retry_times:
+            return self._retry_with_limit(request, retries, reason, stats)
+
+        stats.inc_value("retry/max_reached")
+        logger.error(f"Gave up retrying {request} (failed {retries} times): {reason}")
+        return None
+
+    def _retry_with_limit(
+        self,
+        request: "AyuRequest",
+        retries: int,
+        reason: int,
+        stats: "StatsCollector",
+    ):
+        logger.debug(f"Retrying {request} (failed {retries} times): {reason}")
+        retry_req = request.copy()
+        retry_req.meta["retry_times"] = retries
+        retry_req.dont_filter = True
+        # 优先级逐级降低，以防堆积
+        retry_req.priority = request.priority + self.priority_adjust
+
+        if isinstance(reason, Exception):
+            reason = global_object_name(reason.__class__)
+
+        stats.inc_value("retry/count")
+        stats.inc_value(f"retry/reason_count/{reason}")
+        return retry_req
+
+    def _get_args(self, key: str) -> Any:
+        """根据优先级依次获取不为 None 的请求参数"""
+        data_lst = [
+            self.aiohttp_args.get(key),
+            getattr(self.aiohttp_cfg, key),
+        ]
+        return ToolsForAyu.first_not_none(data_lst=data_lst)
+
+    def spider_opened(self, spider: "AyuSpider") -> None:
+        self.slog = spider.slog
+        settings = spider.crawler.settings
+        # 自定义 aiohttp 全局配置信息，优先级小于 aiohttp_meta 中的配置
+        if local_aiohttp_conf := settings.get("AIOHTTP_CONFIG", {}):
+            # 这里的配置信息如果在 aiohttp_meta 中重复设置，则会更新当前请求的参数
+            self.aiohttp_cfg = AiohttpConf(
+                timeout=settings.get("DOWNLOAD_TIMEOUT"),
+                sleep=local_aiohttp_conf.get("sleep"),
+                proxy=local_aiohttp_conf.get("proxy"),
+                proxy_auth=local_aiohttp_conf.get("proxy_auth"),
+                proxy_headers=local_aiohttp_conf.get("proxy_headers"),
+                retry_times=local_aiohttp_conf.get(
+                    "retry_times", Param.aiohttp_retry_times_default
+                ),
+                limit=local_aiohttp_conf.get("limit", 100),
+                ssl=local_aiohttp_conf.get("ssl", True),
+                verify_ssl=local_aiohttp_conf.get("verify_ssl", True),
+                limit_per_host=local_aiohttp_conf.get("limit_per_host", 0),
+                allow_redirects=local_aiohttp_conf.get("allow_redirects", True),
+            )
+
+            # 这些参数全局生效，不会在 meta 中更新
+            _connector = aiohttp.TCPConnector(
+                ssl=self.aiohttp_cfg.ssl,
+                limit=self.aiohttp_cfg.limit,
+                verify_ssl=self.aiohttp_cfg.verify_ssl,
+                limit_per_host=self.aiohttp_cfg.limit_per_host,
+            )
+            # 超时设置, 若同时配置 AiohttpRequestArgs 的 timeout 参数会更新此值
+            _timeout = aiohttp.ClientTimeout(total=self.aiohttp_cfg.timeout)
+            self.session = aiohttp.ClientSession(connector=_connector, timeout=_timeout)
+            self.priority_adjust = settings.getint("RETRY_PRIORITY_ADJUST")
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler") -> "Self":
+        s = cls()
+        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
+        crawler.signals.connect(s.spider_closed, signal=signals.spider_closed)
+        return s
+
+    async def _request_by_aiohttp(
+        self,
+        aio_request_args: ItemAdapterT,
+    ) -> Tuple[int, str]:
+        """使用 aiohttp 来请求
+
+        Args:
+            aio_request_args: aiohttp 请求参数
+
+        Returns:
+            1). status_code: 状态码
+            2). r_text: 响应内容
+        """
+        try:
+            async with self.session.request(**aio_request_args) as r:
+                status_code = r.status
+                r_text = await r.text(errors="ignore")
+                return status_code, r_text
+        except Exception as e:
+            self.slog.error(f"aiohttp 出现请求错误，Error: {e}")
+            return 504, ""
+
+    async def process_request(
+        self, request: "AyuRequest", spider: "AyuSpider"
+    ) -> Union["AyuRequest", "Response", None]:
+        aiohttp_options = request.meta.get("aiohttp")
+        self.aiohttp_args = aiohttp_options.setdefault("args", {})
+
+        # 设置 url
+        _url = self.aiohttp_args.get("url") or request.url
+        aiohttp_req_args = AiohttpRequestArgs(url=_url)
+
+        # 设置请求方式
+        if _method := self.aiohttp_args.get("method"):
+            aiohttp_req_args.method = _method
+        elif _method := str(request.method).upper():
+            aiohttp_req_args.method = _method  # type: ignore
+        if _method not in {"GET", "POST", "PUT", "DELETE", "HEAD", "OPTIONS", "PATCH"}:
+            logger.error(f"出现未知请求方式 {_method}，请及时查看，默认 GET")
+
+        # 设置请求头信息
+        if _headers_args := self.aiohttp_args.get("headers"):
+            aiohttp_req_args.headers = _headers_args
+        elif _headers_args := ToolsForAyu.get_dict_form_scrapy_req_headers(
+            scrapy_headers=request.headers
+        ):
+            aiohttp_req_args.headers = _headers_args
+
+        # 设置请求 body 参数，GET 情况下和 POST 情况下的请求参数处理
+        if _req_data := self.aiohttp_args.get("data"):
+            aiohttp_req_args.data = _req_data
+        elif req_data_str := str(request.body, encoding="utf-8"):
+            # 如果是 json 字典格式的数据时，则是 scrapy body 传来的 json dumps 参数
+            if ReuseOperation.judge_str_is_json(judge_str=req_data_str):
+                aiohttp_req_args.data = req_data_str
+            # 否则就是传来的字典格式
+            else:
+                req_data_dict = ReuseOperation.get_req_dict_from_scrapy(
+                    req_body_data_str=req_data_str
+                )
+                aiohttp_req_args.data = req_data_dict
+
+        # 设置 proxy
+        if _proxy := self._get_args("proxy"):
+            aiohttp_req_args.proxy = _proxy
+        if _proxy_auth := self._get_args("proxy_auth"):
+            aiohttp_req_args.proxy_auth = _proxy_auth
+        if _proxy_headers := self._get_args("proxy_headers"):
+            aiohttp_req_args.proxy_headers = _proxy_headers
+
+        # 设置 allow_redirects
+        _allow_redirects = self._get_args("allow_redirects")
+        if _allow_redirects is not None:
+            aiohttp_req_args.allow_redirects = _allow_redirects
+
+        # 设置 cookies，优先从 AiohttpRequest 中的 cookies 参数中取值，没有时再从 headers 中取值
+        _ck_args = self.aiohttp_args.get("cookies")
+        aiohttp_cookie_dict = _ck_args if _ck_args is not None else request.cookies
+        if all([not aiohttp_cookie_dict, request.headers.get("Cookie", None)]):
+            headers_cookie_str = str(request.headers.get("Cookie"), encoding="utf-8")
+            aiohttp_cookie_dict = ReuseOperation.get_ck_dict_from_headers(
+                headers_ck_str=headers_cookie_str
+            )
+        aiohttp_req_args.cookies = aiohttp_cookie_dict
+
+        # 超时设置
+        if _timeout := self.aiohttp_args.get("timeout"):
+            aiohttp_req_args.timeout = _timeout
+
+        aio_request_args = ItemAdapter(aiohttp_req_args)
+        status_code, html_content = await self._request_by_aiohttp(
+            aio_request_args=aio_request_args
+        )
+
+        # 请求间隔设置
+        _sleep = self._get_args("sleep")
+        await asyncio.sleep(_sleep)
+
+        if all([status_code == 504, not html_content]):
+            spider.slog.error(f"url: {_url} 返回内容为空，请求超时！")
+            self._retry(request=request, reason=504, spider=spider)
+
+        return HtmlResponse(
+            url=_url,
+            status=status_code,
+            headers=aiohttp_req_args.headers,
+            body=html_content,
+            encoding="utf-8",
+            request=request,
+        )
+
+    async def spider_closed(self, spider: "AyuSpider") -> None:
+        await self.session.close()
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-import base64
-from typing import TYPE_CHECKING
-
-from scrapy import signals
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
-
-if TYPE_CHECKING:
-    from scrapy import Request
-    from scrapy.crawler import Crawler
-    from scrapy.settings import Settings
-    from typing_extensions import Self
-
-    from ayugespidertools.spiders import AyuSpider
-
-
-class DynamicProxyDownloaderMiddleware:
-    """动态隧道代理中间件"""
-
-    def __init__(self):
-        self.proxy_url = None
-        self.username = None
-        self.password = None
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler") -> "Self":
-        s = cls()
-        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
-        return s
-
-    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
-        # TODO: 根据权重来随机获取一个账号 DYNAMIC_PROXY_CONFIG
-        # account = ReuseOperation.random_weight(self.account_arr)
-        if request.url.startswith("https://"):
-            request.meta["proxy"] = (
-                f"https://{self.username}:{self.password}@{self.proxy_url}/"
-            )
-        elif request.url.startswith("http://"):
-            request.meta["proxy"] = (
-                f"http://{self.username}:{self.password}@{self.proxy_url}/"
-            )
-        else:
-            spider.slog.info(
-                f"request url: {request.url} error when use proxy middlewares!"
-            )
-
-        # 避免因连接复用导致隧道不能切换 IP
-        request.headers["Connection"] = "close"
-        # 采用 gzip 压缩加速访问
-        request.headers["Accept-Encoding"] = "gzip"
-
-    def spider_opened(self, spider: "AyuSpider") -> None:
-        spider.slog.info(
-            f"动态隧道代理中间件: DynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
-        )
-
-        self.proxy_url = spider.dynamicproxy_conf.proxy
-        self.username = spider.dynamicproxy_conf.username
-        self.password = spider.dynamicproxy_conf.password
-
-
-class AbuDynamicProxyDownloaderMiddleware:
-    """阿布云动态代理 - 隧道验证方式（其实和快代理的写法一致）"""
-
-    def __init__(self, settings: "Settings") -> None:
-        dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
-        # 查看动态隧道代理配置是否符合要求
-        is_match = ReuseOperation.is_dict_meet_min_limit(
-            dict_conf=dynamic_proxy_conf,
-            key_list=["proxy", "username", "password"],
-        )
-        assert (
-            is_match
-        ), f"没有配置动态隧道代理，配置示例为：{Param.dynamic_proxy_conf_example}"
-
-        self.proxy_url = dynamic_proxy_conf["proxy"]
-        self.username = dynamic_proxy_conf["username"]
-        self.password = dynamic_proxy_conf["password"]
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler") -> "Self":
-        s = cls(crawler.settings)
-        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
-        return s
-
-    def spider_opened(self, spider: "AyuSpider") -> None:
-        spider.slog.info(
-            f"阿布云动态隧道代理中间件: AbuDynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
-        )
-
-    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
-        if request.url.startswith("https://"):
-            request.meta["proxy"] = f"https://{self.proxy_url}"
-        elif request.url.startswith("http://"):
-            request.meta["proxy"] = f"http://{self.proxy_url}"
-        else:
-            spider.slog.info(f"request url error: {request.url}")
-
-        proxy_user_pass = f"{self.username}:{self.password}"
-        encoded_user_pass = "Basic " + base64.urlsafe_b64encode(
-            bytes(proxy_user_pass, "ascii")
-        ).decode("utf8")
-        request.headers["Proxy-Authorization"] = encoded_user_pass
+import base64
+from typing import TYPE_CHECKING
+
+from scrapy import signals
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+
+if TYPE_CHECKING:
+    from scrapy import Request
+    from scrapy.crawler import Crawler
+    from scrapy.settings import Settings
+    from typing_extensions import Self
+
+    from ayugespidertools.spiders import AyuSpider
+
+
+class DynamicProxyDownloaderMiddleware:
+    """动态隧道代理中间件"""
+
+    def __init__(self):
+        self.proxy_url = None
+        self.username = None
+        self.password = None
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler") -> "Self":
+        s = cls()
+        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
+        return s
+
+    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
+        if request.url.startswith("https://"):
+            request.meta["proxy"] = (
+                f"https://{self.username}:{self.password}@{self.proxy_url}/"
+            )
+        elif request.url.startswith("http://"):
+            request.meta["proxy"] = (
+                f"http://{self.username}:{self.password}@{self.proxy_url}/"
+            )
+        else:
+            spider.slog.info(
+                f"request url: {request.url} error when use proxy middlewares!"
+            )
+
+        # 避免因连接复用导致隧道不能切换 IP
+        request.headers["Connection"] = "close"
+        # 采用 gzip 压缩加速访问
+        request.headers["Accept-Encoding"] = "gzip"
+
+    def spider_opened(self, spider: "AyuSpider") -> None:
+        spider.slog.info(
+            f"动态隧道代理中间件: DynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
+        )
+
+        self.proxy_url = spider.dynamicproxy_conf.proxy
+        self.username = spider.dynamicproxy_conf.username
+        self.password = spider.dynamicproxy_conf.password
+
+
+class AbuDynamicProxyDownloaderMiddleware:
+    """阿布云动态代理 - 隧道验证方式（其实和快代理的写法一致）"""
+
+    def __init__(self, settings: "Settings") -> None:
+        dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
+        # 查看动态隧道代理配置是否符合要求
+        is_match = ReuseOperation.is_dict_meet_min_limit(
+            dict_conf=dynamic_proxy_conf,
+            key_list=["proxy", "username", "password"],
+        )
+        assert (
+            is_match
+        ), f"没有配置动态隧道代理，配置示例为：{Param.dynamic_proxy_conf_example}"
+
+        self.proxy_url = dynamic_proxy_conf["proxy"]
+        self.username = dynamic_proxy_conf["username"]
+        self.password = dynamic_proxy_conf["password"]
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler") -> "Self":
+        s = cls(crawler.settings)
+        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
+        return s
+
+    def spider_opened(self, spider: "AyuSpider") -> None:
+        spider.slog.info(
+            f"阿布云动态隧道代理中间件: AbuDynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
+        )
+
+    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
+        if request.url.startswith("https://"):
+            request.meta["proxy"] = f"https://{self.proxy_url}"
+        elif request.url.startswith("http://"):
+            request.meta["proxy"] = f"http://{self.proxy_url}"
+        else:
+            spider.slog.info(f"request url error: {request.url}")
+
+        proxy_user_pass = f"{self.username}:{self.password}"
+        encoded_user_pass = "Basic " + base64.urlsafe_b64encode(
+            bytes(proxy_user_pass, "ascii")
+        ).decode("utf8")
+        request.headers["Proxy-Authorization"] = encoded_user_pass
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-import base64
-from typing import TYPE_CHECKING
-
-import requests
-from scrapy import signals
-
-__all__ = [
-    "ExclusiveProxyDownloaderMiddleware",
-]
-
-if TYPE_CHECKING:
-    from scrapy import Request
-    from scrapy.crawler import Crawler
-    from typing_extensions import Self
-
-    from ayugespidertools.spiders import AyuSpider
-
-
-class ExclusiveProxyDownloaderMiddleware:
-    """独享代理中间件"""
-
-    def __init__(self):
-        self.proxy_url = None
-        self.username = None
-        self.password = None
-        self.proxy_index = None
-        # 从 proxy_list 中取出索引为 proxy_index 的值
-        self.proxy = None
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler") -> "Self":
-        s = cls()
-        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
-        return s
-
-    def get_proxy_ip(self, proxy_url: str, index: int) -> str:
-        """获取独享代理接口的索引为 proxy_index 的代理信息"""
-        try:
-            r = requests.get(proxy_url)
-            proxy_list = r.json().get("data").get("proxy_list")
-            proxy_list.sort()
-            if index < len(proxy_list):
-                return proxy_list[index]
-            else:
-                raise IndexError("独享代理取值索引超出范围，请确认独享代理服务情况。")
-
-        except Exception:
-            raise Exception("获取独享代理时失败，请查看独享配置及网络是否正常。")
-
-    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
-        if request.url.startswith("https://"):
-            request.meta["proxy"] = f"https://{self.proxy}"
-        elif request.url.startswith("http://"):
-            request.meta["proxy"] = f"http://{self.proxy}"
-        else:
-            spider.slog.info(f"request url error: {request.url}")
-
-        proxy_user_pass = f"{self.username}:{self.password}"
-        encoded_user_pass = "Basic " + base64.urlsafe_b64encode(
-            bytes(proxy_user_pass, "ascii")
-        ).decode("utf8")
-        request.headers["Proxy-Authorization"] = encoded_user_pass
-
-    def spider_opened(self, spider: "AyuSpider") -> None:
-        spider.slog.info(
-            f"独享代理中间件: ExclusiveProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
-        )
-
-        self.proxy_url = spider.exclusiveproxy_conf.proxy
-        self.username = spider.exclusiveproxy_conf.username
-        self.password = spider.exclusiveproxy_conf.password
-        self.proxy_index = spider.exclusiveproxy_conf.index
-        self.proxy = self.get_proxy_ip(proxy_url=self.proxy_url, index=self.proxy_index)
+import base64
+import json
+import urllib.request
+from typing import TYPE_CHECKING
+
+from scrapy import signals
+
+__all__ = [
+    "ExclusiveProxyDownloaderMiddleware",
+]
+
+if TYPE_CHECKING:
+    from scrapy import Request
+    from scrapy.crawler import Crawler
+    from typing_extensions import Self
+
+    from ayugespidertools.spiders import AyuSpider
+
+
+class ExclusiveProxyDownloaderMiddleware:
+    """独享代理中间件"""
+
+    def __init__(self):
+        self.proxy_url = None
+        self.username = None
+        self.password = None
+        self.proxy_index = None
+        # 从 proxy_list 中取出索引为 proxy_index 的值
+        self.proxy = None
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler") -> "Self":
+        s = cls()
+        crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
+        return s
+
+    def get_proxy_ip(self, proxy_url: str, index: int) -> str:
+        """获取独享代理接口的索引为 proxy_index 的代理信息"""
+        try:
+            r = urllib.request.urlopen(url=proxy_url)
+            content = r.read().decode(errors="ignore")
+            proxy_list = json.loads(content).get("data").get("proxy_list")
+            proxy_list.sort()
+            if index < len(proxy_list):
+                return proxy_list[index]
+            else:
+                raise IndexError("独享代理取值索引超出范围，请确认独享代理服务情况。")
+
+        except Exception:
+            raise Exception("获取独享代理时失败，请查看独享配置及网络是否正常。")
+
+    def process_request(self, request: "Request", spider: "AyuSpider") -> None:
+        if request.url.startswith("https://"):
+            request.meta["proxy"] = f"https://{self.proxy}"
+        elif request.url.startswith("http://"):
+            request.meta["proxy"] = f"http://{self.proxy}"
+        else:
+            spider.slog.info(f"request url error: {request.url}")
+
+        proxy_user_pass = f"{self.username}:{self.password}"
+        encoded_user_pass = "Basic " + base64.urlsafe_b64encode(
+            bytes(proxy_user_pass, "ascii")
+        ).decode("utf8")
+        request.headers["Proxy-Authorization"] = encoded_user_pass
+
+    def spider_opened(self, spider: "AyuSpider") -> None:
+        spider.slog.info(
+            f"独享代理中间件: ExclusiveProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
+        )
+
+        self.proxy_url = spider.exclusiveproxy_conf.proxy
+        self.username = spider.exclusiveproxy_conf.username
+        self.password = spider.exclusiveproxy_conf.password
+        self.proxy_index = spider.exclusiveproxy_conf.index
+        self.proxy = self.get_proxy_ip(proxy_url=self.proxy_url, index=self.proxy_index)
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/es/asynced.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,85 @@
-import asyncio
-from typing import TYPE_CHECKING, Any, Type, Union
-
-from scrapy.utils.defer import deferred_from_coro
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.scraper.pipelines.es import dynamic_es_document
-
-try:
-    from elasticsearch import AsyncElasticsearch
-    from elasticsearch.helpers import async_bulk
-except ImportError:
-    # pip install ayugespidertools[database]
-    pass
-
-__all__ = ["AyuAsyncESPipeline"]
-
-if TYPE_CHECKING:
-    from elasticsearch_dsl import Document
-    from twisted.internet.defer import Deferred
-
-    from ayugespidertools.common.typevars import ESConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-    DocumentType = Union[Type[Document], type]
-
-
-class AyuAsyncESPipeline:
-    es_conf: "ESConf"
-    slog: "slogT"
-    client: "AsyncElasticsearch"
-    es_type: "DocumentType"
-    running_tasks: set
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "es_conf"), "未配置 elasticsearch 连接信息！"
-        self.running_tasks = set()
-        self.es_conf = spider.es_conf
-        _hosts_lst = self.es_conf.hosts.split(",")
-        if any([self.es_conf.user is not None, self.es_conf.password is not None]):
-            http_auth = (self.es_conf.user, self.es_conf.password)
-        else:
-            http_auth = None
-        self.client = AsyncElasticsearch(
-            hosts=_hosts_lst,
-            basic_auth=http_auth,
-            verify_certs=self.es_conf.verify_certs,
-            ca_certs=self.es_conf.ca_certs,
-            client_cert=self.es_conf.client_cert,
-            client_key=self.es_conf.client_key,
-            ssl_assert_fingerprint=self.es_conf.ssl_assert_fingerprint,
-        )
-
-    async def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        alert_item = ReuseOperation.reshape_item(item_dict)
-        if not (new_item := alert_item.new_item):
-            return
-
-        _index = alert_item.table.name
-        if not hasattr(self, "es_type"):
-            fields_define = {k: v.notes for k, v in item_dict.items()}
-            index_define = self.es_conf.index_class
-            index_define["name"] = _index
-            self.es_type = dynamic_es_document("ESType", fields_define, index_define)
-            if self.es_conf.init:
-                self.es_type.init()
-
-        task = asyncio.create_task(self.insert_item(new_item, _index))
-        self.running_tasks.add(task)
-        await task
-        task.add_done_callback(lambda t: self.running_tasks.discard(t))
-        return item
-
-    async def insert_item(self, new_item: dict, index: str) -> None:
-        async def gendata():
-            yield {
-                "_index": index,
-                "doc": new_item,
-            }
-
-        await async_bulk(self.client, gendata())
-
-    async def _close_spider(self):
-        await self.client.close()
-
-    def close_spider(self, spider: "AyuSpider") -> "Deferred":
-        return deferred_from_coro(self._close_spider())
+import warnings
+from typing import TYPE_CHECKING, Any
+
+import pymysql
+
+from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.mysqlerrhandle import Synchronize, deal_mysql_err
+
+# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
+warnings.filterwarnings(
+    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
+)
+
+__all__ = [
+    "AyuMysqlPipeline",
+]
+
+if TYPE_CHECKING:
+    from pymysql.connections import Connection
+    from pymysql.cursors import Cursor
+
+    from ayugespidertools.common.typevars import AlterItem, MysqlConf, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
+    mysql_conf: "MysqlConf"
+    conn: "Connection[Cursor]"
+    slog: "slogT"
+    cursor: "Cursor"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self.conn = self._connect(self.mysql_conf)
+        self.cursor = self.conn.cursor()
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        alter_item = ReuseOperation.reshape_item(item_dict)
+        self.insert_item(alter_item)
+        return item
+
+    def insert_item(self, alter_item: "AlterItem") -> None:
+        """通用插入数据
+
+        Args:
+            alter_item: 经过转变后的 item
+        """
+        if not (new_item := alter_item.new_item):
+            return
+
+        _table_name = alter_item.table.name
+        _table_notes = alter_item.table.notes
+        note_dic = alter_item.notes_dic
+        sql, args = self._get_sql_by_item(
+            table=_table_name,
+            item=new_item,
+            odku_enable=self.mysql_conf.odku_enable,
+        )
+
+        try:
+            self.cursor.execute(sql, args)
+            self.conn.commit()
+        except Exception as e:
+            self.slog.warning(
+                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
+            )
+            self.conn.rollback()
+            deal_mysql_err(
+                Synchronize(),
+                err_msg=str(e),
+                conn=self.conn,
+                cursor=self.cursor,
+                mysql_conf=self.mysql_conf,
+                table=_table_name,
+                table_notes=_table_notes,
+                note_dic=note_dic,
+            )
+            return self.insert_item(alter_item)
+
+    def close_spider(self, spider: "AyuSpider") -> None:
+        self.conn.close()
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import json
-from typing import TYPE_CHECKING, Any, Union
-
-import pika
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.items import AyuItem
-
-__all__ = [
-    "AyuMQPipeline",
-]
-
-if TYPE_CHECKING:
-    from pika.adapters.blocking_connection import BlockingChannel, BlockingConnection
-
-    from ayugespidertools.common.typevars import MQConf
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuMQPipeline:
-    channel: "BlockingChannel"
-    conn: "BlockingConnection"
-
-    @staticmethod
-    def _dict_to_bytes(item: Union[AyuItem, dict]) -> bytes:
-        item_dict = ReuseOperation.item_to_dict(item)
-        item_json_str = json.dumps(item_dict)
-        return bytes(item_json_str, encoding="utf-8")
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "rabbitmq_conf"), "未配置 RabbitMQ 连接信息！"
-        _mq_conf: "MQConf" = spider.rabbitmq_conf
-        mq_conn_param = pika.URLParameters(
-            f"amqp://{_mq_conf.username}:{_mq_conf.password}"
-            f"@{_mq_conf.host}:{_mq_conf.port}/{_mq_conf.virtualhost}"
-            f"?heartbeat={_mq_conf.heartbeat}&socket_timeout={_mq_conf.socket_timeout}"
-        )
-        self.conn = pika.BlockingConnection(parameters=mq_conn_param)
-        self.channel = self.conn.channel()
-        self.channel.queue_declare(
-            queue=_mq_conf.queue,
-            durable=_mq_conf.durable,
-            exclusive=_mq_conf.exclusive,
-            auto_delete=_mq_conf.auto_delete,
-        )
-        self.channel.confirm_delivery()
-
-    def close_spider(self, spider: "AyuSpider") -> None:
-        self.conn.close()
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        self.channel.basic_publish(
-            exchange=spider.rabbitmq_conf.exchange,
-            routing_key=spider.rabbitmq_conf.routing_key,
-            body=self._dict_to_bytes(item),
-            properties=pika.BasicProperties(
-                content_type=spider.rabbitmq_conf.content_type,
-                delivery_mode=spider.rabbitmq_conf.delivery_mode,
-            ),
-            mandatory=True,
-        )
-        return item
+import json
+from typing import TYPE_CHECKING, Any, Union
+
+import pika
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.items import AyuItem
+
+__all__ = [
+    "AyuMQPipeline",
+]
+
+if TYPE_CHECKING:
+    from pika.adapters.blocking_connection import BlockingChannel, BlockingConnection
+
+    from ayugespidertools.common.typevars import MQConf
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuMQPipeline:
+    channel: "BlockingChannel"
+    conn: "BlockingConnection"
+
+    @staticmethod
+    def _dict_to_bytes(item: Union[AyuItem, dict]) -> bytes:
+        item_dict = ReuseOperation.item_to_dict(item)
+        item_json_str = json.dumps(item_dict)
+        return bytes(item_json_str, encoding="utf-8")
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "rabbitmq_conf"), "未配置 RabbitMQ 连接信息！"
+        _mq_conf: "MQConf" = spider.rabbitmq_conf
+        mq_conn_param = pika.URLParameters(
+            f"amqp://{_mq_conf.username}:{_mq_conf.password}"
+            f"@{_mq_conf.host}:{_mq_conf.port}/{_mq_conf.virtualhost}"
+            f"?heartbeat={_mq_conf.heartbeat}&socket_timeout={_mq_conf.socket_timeout}"
+        )
+        self.conn = pika.BlockingConnection(parameters=mq_conn_param)
+        self.channel = self.conn.channel()
+        self.channel.queue_declare(
+            queue=_mq_conf.queue,
+            durable=_mq_conf.durable,
+            exclusive=_mq_conf.exclusive,
+            auto_delete=_mq_conf.auto_delete,
+        )
+        self.channel.confirm_delivery()
+
+    def close_spider(self, spider: "AyuSpider") -> None:
+        self.conn.close()
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        self.channel.basic_publish(
+            exchange=spider.rabbitmq_conf.exchange,
+            routing_key=spider.rabbitmq_conf.routing_key,
+            body=self._dict_to_bytes(item),
+            properties=pika.BasicProperties(
+                content_type=spider.rabbitmq_conf.content_type,
+                delivery_mode=spider.rabbitmq_conf.delivery_mode,
+            ),
+            mandatory=True,
+        )
+        return item
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,65 @@
-import warnings
-from typing import TYPE_CHECKING, Any
-
-import pymysql
-
-from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.mysqlerrhandle import Synchronize, deal_mysql_err
-
-# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
-warnings.filterwarnings(
-    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
-)
-
-__all__ = [
-    "AyuMysqlPipeline",
-]
-
-if TYPE_CHECKING:
-    from pymysql.connections import Connection
-    from pymysql.cursors import Cursor
-
-    from ayugespidertools.common.typevars import AlterItem, MysqlConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
-    mysql_conf: "MysqlConf"
-    conn: "Connection[Cursor]"
-    slog: "slogT"
-    cursor: "Cursor"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.conn = self._connect(self.mysql_conf)
-        self.cursor = self.conn.cursor()
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        alter_item = ReuseOperation.reshape_item(item_dict)
-        self.insert_item(alter_item)
-        return item
-
-    def insert_item(self, alter_item: "AlterItem"):
-        """通用插入数据
-
-        Args:
-            alter_item: 经过转变后的 item
-        """
-        if not (new_item := alter_item.new_item):
-            return
-
-        _table_name = alter_item.table.name
-        _table_notes = alter_item.table.notes
-        note_dic = alter_item.notes_dic
-        sql, args = self._get_sql_by_item(
-            table=_table_name,
-            item=new_item,
-            odku_enable=self.mysql_conf.odku_enable,
-        )
-
-        try:
-            self.cursor.execute(sql, args)
-            self.conn.commit()
-        except Exception as e:
-            self.slog.warning(
-                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
-            )
-            self.conn.rollback()
-            deal_mysql_err(
-                Synchronize(),
-                err_msg=str(e),
-                conn=self.conn,
-                cursor=self.cursor,
-                mysql_conf=self.mysql_conf,
-                table=_table_name,
-                table_notes=_table_notes,
-                note_dic=note_dic,
-            )
-            return self.insert_item(alter_item)
-
-    def close_spider(self, spider: "AyuSpider") -> None:
-        self.conn.close()
+from typing import TYPE_CHECKING, Any
+
+from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.postgreserrhandle import Synchronize, deal_postgres_err
+
+__all__ = ["AyuPostgresPipeline"]
+
+if TYPE_CHECKING:
+    from psycopg.connection import Connection
+    from psycopg.cursor import Cursor
+
+    from ayugespidertools.common.typevars import AlterItem, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuPostgresPipeline(PostgreSQLPipeEnhanceMixin):
+    conn: "Connection"
+    slog: "slogT"
+    cursor: "Cursor"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息！"
+        self.slog = spider.slog
+        self.conn = self._connect(spider.postgres_conf)
+        self.cursor = self.conn.cursor()
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        alter_item = ReuseOperation.reshape_item(item_dict)
+        self.insert_item(alter_item)
+        return item
+
+    def insert_item(self, alter_item: "AlterItem") -> None:
+        if not (new_item := alter_item.new_item):
+            return
+
+        _table_name = alter_item.table.name
+        _table_notes = alter_item.table.notes
+        note_dic = alter_item.notes_dic
+        sql = self._get_sql_by_item(table=_table_name, item=new_item)
+
+        try:
+            self.cursor.execute(sql, tuple(new_item.values()))
+            self.conn.commit()
+
+        except Exception as e:
+            self.slog.warning(
+                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
+            )
+            self.conn.rollback()
+            deal_postgres_err(
+                Synchronize(),
+                err_msg=str(e),
+                conn=self.conn,
+                cursor=self.cursor,
+                table=_table_name,
+                table_notes=_table_notes,
+                note_dic=note_dic,
+            )
+            return self.insert_item(alter_item)
+
+    def close_spider(self, spider: "AyuSpider") -> None:
+        self.cursor.close()
+        self.conn.close()
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-import asyncio
-from typing import TYPE_CHECKING, Any
-
-import aiomysql
-from scrapy.utils.defer import deferred_from_coro
-
-from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-
-__all__ = [
-    "AyuAsyncMysqlPipeline",
-]
-
-if TYPE_CHECKING:
-    from twisted.internet.defer import Deferred
-
-    from ayugespidertools.common.typevars import MysqlConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuAsyncMysqlPipeline(MysqlPipeEnhanceMixin):
-    mysql_conf: "MysqlConf"
-    slog: "slogT"
-    pool: aiomysql.Pool
-    running_tasks: set
-
-    def open_spider(self, spider: "AyuSpider") -> "Deferred":
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-        self.running_tasks = set()
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        return deferred_from_coro(self._open_spider(spider))
-
-    async def _open_spider(self, spider: "AyuSpider") -> None:
-        self.pool = await aiomysql.create_pool(
-            host=self.mysql_conf.host,
-            port=self.mysql_conf.port,
-            user=self.mysql_conf.user,
-            password=self.mysql_conf.password,
-            db=self.mysql_conf.database,
-            charset=self.mysql_conf.charset,
-            cursorclass=aiomysql.DictCursor,
-            autocommit=True,
-        )
-
-    async def insert_item(self, item_dict: dict) -> None:
-        async with self.pool.acquire() as conn:
-            async with conn.cursor() as cursor:
-                alter_item = ReuseOperation.reshape_item(item_dict)
-                new_item = alter_item.new_item
-                sql, args = self._get_sql_by_item(
-                    table=alter_item.table.name,
-                    item=new_item,
-                    odku_enable=self.mysql_conf.odku_enable,
-                )
-                await cursor.execute(sql, args)
-
-    async def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        task = asyncio.create_task(self.insert_item(item_dict))
-        self.running_tasks.add(task)
-        await task
-        task.add_done_callback(lambda t: self.running_tasks.discard(t))
-        return item
-
-    async def _close_spider(self) -> None:
-        await self.pool.wait_closed()
-
-    def close_spider(self, spider: "AyuSpider") -> "Deferred":
-        self.pool.close()
-        return deferred_from_coro(self._close_spider())
+import asyncio
+from typing import TYPE_CHECKING, Any
+
+import aiomysql
+from scrapy.utils.defer import deferred_from_coro
+
+from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+__all__ = [
+    "AyuAsyncMysqlPipeline",
+]
+
+if TYPE_CHECKING:
+    from twisted.internet.defer import Deferred
+
+    from ayugespidertools.common.typevars import MysqlConf
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuAsyncMysqlPipeline(MysqlPipeEnhanceMixin):
+    mysql_conf: "MysqlConf"
+    pool: aiomysql.Pool
+    running_tasks: set
+
+    def open_spider(self, spider: "AyuSpider") -> "Deferred":
+        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+        self.running_tasks = set()
+        self.mysql_conf = spider.mysql_conf
+        return deferred_from_coro(self._open_spider(spider))
+
+    async def _open_spider(self, spider: "AyuSpider") -> None:
+        self.pool = await aiomysql.create_pool(
+            host=self.mysql_conf.host,
+            port=self.mysql_conf.port,
+            user=self.mysql_conf.user,
+            password=self.mysql_conf.password,
+            db=self.mysql_conf.database,
+            charset=self.mysql_conf.charset,
+            cursorclass=aiomysql.DictCursor,
+            autocommit=True,
+        )
+
+    async def insert_item(self, item_dict: dict) -> None:
+        async with self.pool.acquire() as conn:
+            async with conn.cursor() as cursor:
+                alter_item = ReuseOperation.reshape_item(item_dict)
+                new_item = alter_item.new_item
+                sql, args = self._get_sql_by_item(
+                    table=alter_item.table.name,
+                    item=new_item,
+                    odku_enable=self.mysql_conf.odku_enable,
+                )
+                await cursor.execute(sql, args)
+
+    async def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        task = asyncio.create_task(self.insert_item(item_dict))
+        self.running_tasks.add(task)
+        await task
+        task.add_done_callback(lambda t: self.running_tasks.discard(t))
+        return item
+
+    async def _close_spider(self) -> None:
+        await self.pool.wait_closed()
+
+    def close_spider(self, spider: "AyuSpider") -> "Deferred":
+        self.pool.close()
+        return deferred_from_coro(self._close_spider())
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import datetime
-from typing import TYPE_CHECKING, Any, Tuple
-
-from retrying import retry
-
-from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.params import Param
-
-__all__ = [
-    "AyuStatisticsMysqlPipeline",
-]
-
-if TYPE_CHECKING:
-    from pymysql.connections import Connection
-    from pymysql.cursors import Cursor
-
-    from ayugespidertools.common.typevars import MysqlConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuStatisticsMysqlPipeline(MysqlPipeEnhanceMixin):
-    mysql_conf: "MysqlConf"
-    conn: "Connection[Cursor]"
-    slog: "slogT"
-    cursor: "Cursor"
-    crawl_time: "datetime.date"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        self.crawl_time = datetime.date.today()
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.conn = self._connect(self.mysql_conf)
-        self.cursor = self.conn.cursor()
-
-    def table_collection_statistics(
-        self, spider_name: str, database: str, crawl_time: datetime.date
-    ) -> None:
-        """统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
-
-        Args:
-            spider_name: 爬虫脚本名称
-            database: 数据库，保存程序采集记录保存的数据库
-            crawl_time: 采集时间，程序运行时间
-        """
-        sql = f"""
-        select concat(
-        'select "', TABLE_NAME, '", count(id) as num , crawl_time from ', TABLE_SCHEMA, '.', TABLE_NAME,
-        ' where crawl_time = "{crawl_time}"') from information_schema.tables
-        where TABLE_SCHEMA='{database}' and TABLE_NAME in
-        (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
-        """
-        self.cursor.execute(sql)
-        results = self.cursor.fetchall()
-        if sql_list := [row[0] for row in results]:
-            sql_all = " union all ".join(sql_list)
-            self.cursor.execute(sql_all)
-            results = self.cursor.fetchall()
-
-            for row in results:
-                table_statistics = {
-                    "spider_name": spider_name,
-                    "database": database,
-                    "table_name": row[0],
-                    "number": row[1],
-                    "crawl_time": str((row[2] or crawl_time)),
-                }
-                self.insert_table_statistics(table_statistics)
-
-    def insert_table_statistics(
-        self, data: dict, table: str = "table_collection_statistics"
-    ) -> None:
-        """插入统计数据到表中
-
-        Args:
-            data: 需要统计的入库信息
-            table: 存储表的名称
-        """
-        create_table_sql = f"""
-        CREATE TABLE IF NOT EXISTS `{table}` (
-            `id` int(11) NOT NULL AUTO_INCREMENT,
-            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
-            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
-            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',
-            PRIMARY KEY (`id`) USING BTREE
-        ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
-        """
-        self.cursor.execute(create_table_sql)
-
-        sql, args = self._get_sql_by_item(
-            table=table,
-            item=data,
-            odku_enable=self.mysql_conf.odku_enable,
-        )
-        self._log_record(sql=sql, data=args)
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def insert_script_statistics(
-        self, data: dict, table: str = "script_collection_statistics"
-    ) -> None:
-        """存储运行脚本的统计信息
-
-        Args:
-            data: 需要插入的 log 信息
-            table: 存储表的名称
-        """
-        self.cursor.execute(
-            f"""
-                CREATE TABLE IF NOT EXISTS `{table}` (
-                    `id` int(11) NOT NULL AUTO_INCREMENT,
-                    `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-                    `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
-                    `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
-                    `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
-                    `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
-                    `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
-                    `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
-                    `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
-                    `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
-                    `start_time` datetime NOT NULL COMMENT '开始时间',
-                    `finish_time` datetime NOT NULL COMMENT '结束时间',
-                    `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
-                    `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-                    `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
-                    PRIMARY KEY (`id`) USING BTREE
-                    ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
-                """
-        )
-
-        sql, args = self._get_sql_by_item(
-            table=table,
-            item=data,
-            odku_enable=self.mysql_conf.odku_enable,
-        )
-        self._log_record(sql=sql, data=args)
-
-    def _log_record(self, sql: str, data: Tuple) -> None:
-        """执行日志记录的 sql 语句
-
-        Args:
-            sql: sql 语句
-            data: sql 语句中的参数
-        """
-        try:
-            self.cursor.execute(sql, data)
-            self.conn.commit()
-        except Exception as e:
-            self.conn.rollback()
-            self.slog.warning(f"日志记录存储错误: {e}")
-
-    def close_spider(self, spider: "AyuSpider") -> None:
-        log_info = self._get_log_by_spider(spider=spider, crawl_time=self.crawl_time)
-
-        # 运行脚本统计信息
-        self.insert_script_statistics(log_info)
-        self.table_collection_statistics(
-            spider_name=spider.name,
-            database=spider.mysql_conf.database,
-            crawl_time=self.crawl_time,
-        )
-
-        if self.conn:
-            self.conn.close()
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        return item
+import datetime
+from typing import TYPE_CHECKING, Any, Tuple
+
+from retrying import retry
+
+from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.params import Param
+
+__all__ = [
+    "AyuStatisticsMysqlPipeline",
+]
+
+if TYPE_CHECKING:
+    from pymysql.connections import Connection
+    from pymysql.cursors import Cursor
+
+    from ayugespidertools.common.typevars import MysqlConf, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuStatisticsMysqlPipeline(MysqlPipeEnhanceMixin):
+    mysql_conf: "MysqlConf"
+    conn: "Connection[Cursor]"
+    slog: "slogT"
+    cursor: "Cursor"
+    crawl_time: "datetime.date"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        self.crawl_time = datetime.date.today()
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self.conn = self._connect(self.mysql_conf)
+        self.cursor = self.conn.cursor()
+
+    def table_collection_statistics(
+        self, spider_name: str, database: str, crawl_time: datetime.date
+    ) -> None:
+        """统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
+
+        Args:
+            spider_name: 爬虫脚本名称
+            database: 数据库，保存程序采集记录保存的数据库
+            crawl_time: 采集时间，程序运行时间
+        """
+        sql = f"""
+        select concat(
+        'select "', TABLE_NAME, '", count(id) as num , crawl_time from ', TABLE_SCHEMA, '.', TABLE_NAME,
+        ' where crawl_time = "{crawl_time}"') from information_schema.tables
+        where TABLE_SCHEMA='{database}' and TABLE_NAME in
+        (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
+        """
+        self.cursor.execute(sql)
+        results = self.cursor.fetchall()
+        if sql_list := [row[0] for row in results]:
+            sql_all = " union all ".join(sql_list)
+            self.cursor.execute(sql_all)
+            results = self.cursor.fetchall()
+
+            for row in results:
+                table_statistics = {
+                    "spider_name": spider_name,
+                    "database": database,
+                    "table_name": row[0],
+                    "number": row[1],
+                    "crawl_time": str((row[2] or crawl_time)),
+                }
+                self.insert_table_statistics(table_statistics)
+
+    def insert_table_statistics(
+        self, data: dict, table: str = "table_collection_statistics"
+    ) -> None:
+        """插入统计数据到表中
+
+        Args:
+            data: 需要统计的入库信息
+            table: 存储表的名称
+        """
+        create_table_sql = f"""
+        CREATE TABLE IF NOT EXISTS `{table}` (
+            `id` int(11) NOT NULL AUTO_INCREMENT,
+            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
+            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
+            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',
+            PRIMARY KEY (`id`) USING BTREE
+        ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
+        """
+        self.cursor.execute(create_table_sql)
+
+        sql, args = self._get_sql_by_item(
+            table=table,
+            item=data,
+            odku_enable=self.mysql_conf.odku_enable,
+        )
+        self._log_record(sql=sql, data=args)
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def insert_script_statistics(
+        self, data: dict, table: str = "script_collection_statistics"
+    ) -> None:
+        """存储运行脚本的统计信息
+
+        Args:
+            data: 需要插入的 log 信息
+            table: 存储表的名称
+        """
+        self.cursor.execute(
+            f"""
+                CREATE TABLE IF NOT EXISTS `{table}` (
+                    `id` int(11) NOT NULL AUTO_INCREMENT,
+                    `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+                    `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
+                    `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
+                    `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
+                    `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
+                    `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
+                    `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
+                    `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
+                    `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
+                    `start_time` datetime NOT NULL COMMENT '开始时间',
+                    `finish_time` datetime NOT NULL COMMENT '结束时间',
+                    `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
+                    `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+                    `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
+                    PRIMARY KEY (`id`) USING BTREE
+                    ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
+                """
+        )
+
+        sql, args = self._get_sql_by_item(
+            table=table,
+            item=data,
+            odku_enable=self.mysql_conf.odku_enable,
+        )
+        self._log_record(sql=sql, data=args)
+
+    def _log_record(self, sql: str, data: Tuple) -> None:
+        """执行日志记录的 sql 语句
+
+        Args:
+            sql: sql 语句
+            data: sql 语句中的参数
+        """
+        try:
+            self.cursor.execute(sql, data)
+            self.conn.commit()
+        except Exception as e:
+            self.conn.rollback()
+            self.slog.warning(f"日志记录存储错误: {e}")
+
+    def close_spider(self, spider: "AyuSpider") -> None:
+        log_info = self._get_log_by_spider(spider=spider, crawl_time=self.crawl_time)
+
+        # 运行脚本统计信息
+        self.insert_script_statistics(log_info)
+        self.table_collection_statistics(
+            spider_name=spider.name,
+            database=spider.mysql_conf.database,
+            crawl_time=self.crawl_time,
+        )
+
+        if self.conn:
+            self.conn.close()
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        return item
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,90 @@
-from typing import TYPE_CHECKING, Any
-
-from pymysql import cursors
-from twisted.enterprise import adbapi
-
-from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.mysqlerrhandle import TwistedAsynchronous, deal_mysql_err
-
-__all__ = [
-    "AyuTwistedMysqlPipeline",
-]
-
-if TYPE_CHECKING:
-    from ayugespidertools.common.typevars import MysqlConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuTwistedMysqlPipeline(MysqlPipeEnhanceMixin):
-    mysql_conf: "MysqlConf"
-    slog: "slogT"
-    dbpool: "adbapi.ConnectionPool"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。
-        self._connect(self.mysql_conf).close()
-
-        _mysql_conf = {
-            "user": self.mysql_conf.user,
-            "password": self.mysql_conf.password,
-            "host": self.mysql_conf.host,
-            "port": self.mysql_conf.port,
-            "db": self.mysql_conf.database,
-            "charset": self.mysql_conf.charset,
-            "cursorclass": cursors.DictCursor,
-        }
-        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
-        query = self.dbpool.runInteraction(self.db_create)
-        query.addErrback(self.db_create_err)
-
-    def db_create(self, cursor):
-        pass
-
-    def db_create_err(self, failure):
-        self.slog.error(f"创建数据表失败: {failure}")
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        query = self.dbpool.runInteraction(self.db_insert, item_dict)
-        query.addErrback(self.handle_error, item)
-        return item
-
-    def db_insert(self, cursor, item):
-        alter_item = ReuseOperation.reshape_item(item)
-        if not (new_item := alter_item.new_item):
-            return
-
-        _table_name = alter_item.table.name
-        _table_notes = alter_item.table.notes
-        note_dic = alter_item.notes_dic
-        sql, args = self._get_sql_by_item(
-            table=_table_name,
-            item=new_item,
-            odku_enable=self.mysql_conf.odku_enable,
-        )
-
-        try:
-            cursor.execute(sql, args)
-        except Exception as e:
-            self.slog.warning(
-                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
-            )
-            deal_mysql_err(
-                TwistedAsynchronous(),
-                err_msg=str(e),
-                cursor=cursor,
-                mysql_conf=self.mysql_conf,
-                table=_table_name,
-                table_notes=_table_notes,
-                note_dic=note_dic,
-            )
-            return self.db_insert(cursor, item)
-        return item
-
-    def handle_error(self, failure, item):
-        self.slog.error(f"插入数据失败:{failure}, item: {item}")
+from typing import TYPE_CHECKING, Any
+
+from pymysql import cursors
+from twisted.enterprise import adbapi
+
+from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.mysqlerrhandle import TwistedAsynchronous, deal_mysql_err
+
+__all__ = [
+    "AyuTwistedMysqlPipeline",
+]
+
+if TYPE_CHECKING:
+    from twisted.python.failure import Failure
+
+    from ayugespidertools.common.typevars import MysqlConf, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuTwistedMysqlPipeline(MysqlPipeEnhanceMixin):
+    mysql_conf: "MysqlConf"
+    slog: "slogT"
+    dbpool: "adbapi.ConnectionPool"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self._connect(self.mysql_conf).close()
+
+        _mysql_conf = {
+            "user": self.mysql_conf.user,
+            "password": self.mysql_conf.password,
+            "host": self.mysql_conf.host,
+            "port": self.mysql_conf.port,
+            "db": self.mysql_conf.database,
+            "charset": self.mysql_conf.charset,
+            "cursorclass": cursors.DictCursor,
+        }
+        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
+        query = self.dbpool.runInteraction(self.db_create)
+        query.addErrback(self.db_create_err)
+
+    def db_create(self, cursor: Any) -> None:
+        pass
+
+    def db_create_err(self, failure: "Failure") -> None:
+        self.slog.error(f"创建数据表失败: {failure}")
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        query = self.dbpool.runInteraction(self.db_insert, item_dict)
+        query.addErrback(self.handle_error, item)
+        return item
+
+    def db_insert(self, cursor: Any, item: Any) -> Any:
+        alter_item = ReuseOperation.reshape_item(item)
+        if not (new_item := alter_item.new_item):
+            return
+
+        _table_name = alter_item.table.name
+        _table_notes = alter_item.table.notes
+        note_dic = alter_item.notes_dic
+        sql, args = self._get_sql_by_item(
+            table=_table_name,
+            item=new_item,
+            odku_enable=self.mysql_conf.odku_enable,
+        )
+
+        try:
+            cursor.execute(sql, args)
+        except Exception as e:
+            self.slog.warning(
+                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
+            )
+            deal_mysql_err(
+                TwistedAsynchronous(),
+                err_msg=str(e),
+                cursor=cursor,
+                mysql_conf=self.mysql_conf,
+                table=_table_name,
+                table_notes=_table_notes,
+                note_dic=note_dic,
+            )
+            return self.db_insert(cursor, item)
+        return item
+
+    def handle_error(self, failure: "Failure", item: Any) -> None:
+        self.slog.error(f"插入数据失败:{failure}, item: {item}")
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/oracle/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oracle/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-from typing import TYPE_CHECKING, Any
-
-from ayugespidertools.common.expend import OraclePipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-
-__all__ = ["AyuOraclePipeline"]
-
-if TYPE_CHECKING:
-    from oracledb.connection import Connection
-    from oracledb.cursor import Cursor
-
-    from ayugespidertools.common.typevars import AlterItem
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuOraclePipeline(OraclePipeEnhanceMixin):
-    conn: "Connection"
-    cursor: "Cursor"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "oracle_conf"), "未配置 Oracle 连接信息！"
-        self.conn = self._connect(spider.oracle_conf)
-        self.cursor = self.conn.cursor()
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        alter_item = ReuseOperation.reshape_item(item_dict)
-        self.insert_item(alter_item)
-        return item
-
-    def insert_item(self, alter_item: "AlterItem") -> None:
-        """通用插入数据
-
-        Args:
-            alter_item: 经过转变后的 item
-        """
-        if not (new_item := alter_item.new_item):
-            return
-
-        sql = self._get_sql_by_item(table=alter_item.table.name, item=new_item)
-        # no err handing
-        self.cursor.execute(sql, tuple(new_item.values()))
-        self.conn.commit()
-
-    def close_spider(self, spider: "AyuSpider") -> None:
-        self.conn.close()
+from typing import TYPE_CHECKING, Any
+
+from ayugespidertools.common.expend import OraclePipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+__all__ = ["AyuOraclePipeline"]
+
+if TYPE_CHECKING:
+    from oracledb.connection import Connection
+    from oracledb.cursor import Cursor
+
+    from ayugespidertools.common.typevars import AlterItem
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuOraclePipeline(OraclePipeEnhanceMixin):
+    conn: "Connection"
+    cursor: "Cursor"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "oracle_conf"), "未配置 Oracle 连接信息！"
+        self.conn = self._connect(spider.oracle_conf)
+        self.cursor = self.conn.cursor()
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        alter_item = ReuseOperation.reshape_item(item_dict)
+        self.insert_item(alter_item)
+        return item
+
+    def insert_item(self, alter_item: "AlterItem") -> None:
+        """通用插入数据
+
+        Args:
+            alter_item: 经过转变后的 item
+        """
+        if not (new_item := alter_item.new_item):
+            return
+
+        sql = self._get_sql_by_item(table=alter_item.table.name, item=new_item)
+        self.cursor.execute(sql, tuple(new_item.values()))
+        self.conn.commit()
+
+    def close_spider(self, spider: "AyuSpider") -> None:
+        self.conn.close()
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/twisted.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,87 @@
-from typing import TYPE_CHECKING, Any
-
-from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.postgreserrhandle import Synchronize, deal_postgres_err
-
-__all__ = ["AyuPostgresPipeline"]
-
-if TYPE_CHECKING:
-    from psycopg.connection import Connection
-    from psycopg.cursor import Cursor
-
-    from ayugespidertools.common.typevars import AlterItem, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuPostgresPipeline(PostgreSQLPipeEnhanceMixin):
-    conn: "Connection"
-    slog: "slogT"
-    cursor: "Cursor"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息！"
-        self.slog = spider.slog
-        self.conn = self._connect(spider.postgres_conf)
-        self.cursor = self.conn.cursor()
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        alter_item = ReuseOperation.reshape_item(item_dict)
-        self.insert_item(alter_item)
-        return item
-
-    def insert_item(self, alter_item: "AlterItem") -> None:
-        if not (new_item := alter_item.new_item):
-            return
-
-        _table_name = alter_item.table.name
-        _table_notes = alter_item.table.notes
-        note_dic = alter_item.notes_dic
-        sql = self._get_sql_by_item(table=_table_name, item=new_item)
-
-        try:
-            self.cursor.execute(sql, tuple(new_item.values()))
-            self.conn.commit()
-
-        except Exception as e:
-            self.slog.warning(
-                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
-            )
-            self.conn.rollback()
-            deal_postgres_err(
-                Synchronize(),
-                err_msg=str(e),
-                conn=self.conn,
-                cursor=self.cursor,
-                table=_table_name,
-                table_notes=_table_notes,
-                note_dic=note_dic,
-            )
-            return self.insert_item(alter_item)
-
-    def close_spider(self, spider: "AyuSpider") -> None:
-        self.cursor.close()
-        self.conn.close()
+from typing import TYPE_CHECKING, Any
+
+from twisted.enterprise import adbapi
+
+from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.postgreserrhandle import (
+    TwistedAsynchronous,
+    deal_postgres_err,
+)
+
+__all__ = ["AyuTwistedPostgresPipeline"]
+
+if TYPE_CHECKING:
+    from twisted.python.failure import Failure
+
+    from ayugespidertools.common.typevars import PostgreSQLConf, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuTwistedPostgresPipeline(PostgreSQLPipeEnhanceMixin):
+    postgres_conf: "PostgreSQLConf"
+    dbpool: "adbapi.ConnectionPool"
+    slog: "slogT"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息"
+        self.slog = spider.slog
+        self.postgres_conf = spider.postgres_conf
+        self._connect(self.postgres_conf).close()
+
+        _postgres_conf = {
+            "user": self.postgres_conf.user,
+            "password": self.postgres_conf.password,
+            "host": self.postgres_conf.host,
+            "port": self.postgres_conf.port,
+            "dbname": self.postgres_conf.database,
+        }
+        self.dbpool = adbapi.ConnectionPool(
+            "psycopg", cp_reconnect=True, **_postgres_conf
+        )
+        query = self.dbpool.runInteraction(self.db_create)
+        query.addErrback(self.db_create_err)
+
+    def db_create(self, cursor: Any) -> None:
+        pass
+
+    def db_create_err(self, failure: "Failure") -> None:
+        self.slog.error(f"创建数据表失败: {failure}")
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        query = self.dbpool.runInteraction(self.db_insert, item_dict)
+        query.addErrback(self.handle_error, item)
+        return item
+
+    def db_insert(self, cursor: Any, item: Any) -> Any:
+        alter_item = ReuseOperation.reshape_item(item)
+        if not (new_item := alter_item.new_item):
+            return
+
+        _table_name = alter_item.table.name
+        _table_notes = alter_item.table.notes
+        note_dic = alter_item.notes_dic
+        sql = self._get_sql_by_item(table=_table_name, item=new_item)
+
+        try:
+            cursor.execute(sql, tuple(new_item.values()))
+
+        except Exception as e:
+            self.slog.warning(
+                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
+            )
+            cursor.execute("ROLLBACK")
+            deal_postgres_err(
+                TwistedAsynchronous(),
+                err_msg=str(e),
+                cursor=cursor,
+                table=_table_name,
+                table_notes=_table_notes,
+                note_dic=note_dic,
+            )
+            return self.db_insert(cursor, item)
+        return item
+
+    def handle_error(self, failure: "Failure", item: Any) -> None:
+        self.slog.error(f"插入数据失败:{failure}, item: {item}")
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/asynced.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/postgres/asynced.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-from typing import TYPE_CHECKING, Any
-
-from scrapy.utils.defer import deferred_from_coro
-
-from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-
-try:
-    from psycopg_pool import AsyncConnectionPool
-except ImportError:
-    # pip install ayugespidertools[database]
-    pass
-
-__all__ = [
-    "AyuAsyncPostgresPipeline",
-]
-
-if TYPE_CHECKING:
-    from twisted.internet.defer import Deferred
-
-    from ayugespidertools.common.typevars import PostgreSQLConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuAsyncPostgresPipeline(PostgreSQLPipeEnhanceMixin):
-    postgres_conf: "PostgreSQLConf"
-    slog: "slogT"
-    pool: "AsyncConnectionPool"
-    running_tasks: set
-
-    def open_spider(self, spider: "AyuSpider") -> "Deferred":
-        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息！"
-        self.running_tasks = set()
-        self.slog = spider.slog
-        self.postgres_conf = spider.postgres_conf
-        return deferred_from_coro(self._open_spider(spider))
-
-    async def _open_spider(self, spider: "AyuSpider") -> None:
-        self.pool = AsyncConnectionPool(
-            f"dbname={self.postgres_conf.database} "
-            f"user={self.postgres_conf.user} "
-            f"host={self.postgres_conf.host} "
-            f"port={self.postgres_conf.port} "
-            f"password={self.postgres_conf.password}",
-            open=False,
-        )
-        await self.pool.open()
-
-    async def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        async with self.pool.connection() as conn:
-            item_dict = ReuseOperation.item_to_dict(item)
-            alter_item = ReuseOperation.reshape_item(item_dict)
-            new_item = alter_item.new_item
-            sql = self._get_sql_by_item(table=alter_item.table.name, item=new_item)
-            await conn.execute(sql, tuple(new_item.values()))
-        return item
-
-    async def _close_spider(self) -> None:
-        await self.pool.close()
-
-    def close_spider(self, spider: "AyuSpider") -> "Deferred":
-        return deferred_from_coro(self._close_spider())
+from typing import TYPE_CHECKING, Any
+
+from scrapy.utils.defer import deferred_from_coro
+
+from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+try:
+    from psycopg_pool import AsyncConnectionPool
+except ImportError:
+    # pip install ayugespidertools[database]
+    pass
+
+__all__ = [
+    "AyuAsyncPostgresPipeline",
+]
+
+if TYPE_CHECKING:
+    from twisted.internet.defer import Deferred
+
+    from ayugespidertools.common.typevars import PostgreSQLConf
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuAsyncPostgresPipeline(PostgreSQLPipeEnhanceMixin):
+    postgres_conf: "PostgreSQLConf"
+    pool: "AsyncConnectionPool"
+
+    def open_spider(self, spider: "AyuSpider") -> "Deferred":
+        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息！"
+        self.postgres_conf = spider.postgres_conf
+        return deferred_from_coro(self._open_spider(spider))
+
+    async def _open_spider(self, spider: "AyuSpider") -> None:
+        self.pool = AsyncConnectionPool(
+            f"dbname={self.postgres_conf.database} "
+            f"user={self.postgres_conf.user} "
+            f"host={self.postgres_conf.host} "
+            f"port={self.postgres_conf.port} "
+            f"password={self.postgres_conf.password}",
+            open=False,
+        )
+        await self.pool.open()
+
+    async def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        async with self.pool.connection() as conn:
+            item_dict = ReuseOperation.item_to_dict(item)
+            alter_item = ReuseOperation.reshape_item(item_dict)
+            new_item = alter_item.new_item
+            sql = self._get_sql_by_item(table=alter_item.table.name, item=new_item)
+            await conn.execute(sql, tuple(new_item.values()))
+        return item
+
+    async def _close_spider(self) -> None:
+        await self.pool.close()
+
+    def close_spider(self, spider: "AyuSpider") -> "Deferred":
+        return deferred_from_coro(self._close_spider())
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/pipelines/postgres/twisted.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/pipelines/oracle/twisted.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,68 @@
-from typing import TYPE_CHECKING, Any
-
-from twisted.enterprise import adbapi
-
-from ayugespidertools.common.expend import PostgreSQLPipeEnhanceMixin
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.postgreserrhandle import (
-    TwistedAsynchronous,
-    deal_postgres_err,
-)
-
-__all__ = ["AyuTwistedPostgresPipeline"]
-
-if TYPE_CHECKING:
-    from ayugespidertools.common.typevars import PostgreSQLConf, slogT
-    from ayugespidertools.spiders import AyuSpider
-
-
-class AyuTwistedPostgresPipeline(PostgreSQLPipeEnhanceMixin):
-    postgres_conf: "PostgreSQLConf"
-    dbpool: "adbapi.ConnectionPool"
-    slog: "slogT"
-
-    def open_spider(self, spider: "AyuSpider") -> None:
-        assert hasattr(spider, "postgres_conf"), "未配置 PostgreSQL 连接信息"
-        self.slog = spider.slog
-        self.postgres_conf = spider.postgres_conf
-        self._connect(self.postgres_conf).close()
-
-        _postgres_conf = {
-            "user": self.postgres_conf.user,
-            "password": self.postgres_conf.password,
-            "host": self.postgres_conf.host,
-            "port": self.postgres_conf.port,
-            "dbname": self.postgres_conf.database,
-        }
-        self.dbpool = adbapi.ConnectionPool(
-            "psycopg", cp_reconnect=True, **_postgres_conf
-        )
-        query = self.dbpool.runInteraction(self.db_create)
-        query.addErrback(self.db_create_err)
-
-    def db_create(self, cursor):
-        pass
-
-    def db_create_err(self, failure):
-        self.slog.error(f"创建数据表失败: {failure}")
-
-    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
-        item_dict = ReuseOperation.item_to_dict(item)
-        query = self.dbpool.runInteraction(self.db_insert, item_dict)
-        query.addErrback(self.handle_error, item)
-        return item
-
-    def db_insert(self, cursor, item):
-        alter_item = ReuseOperation.reshape_item(item)
-        if not (new_item := alter_item.new_item):
-            return
-
-        _table_name = alter_item.table.name
-        _table_notes = alter_item.table.notes
-        note_dic = alter_item.notes_dic
-        sql = self._get_sql_by_item(table=_table_name, item=new_item)
-
-        try:
-            cursor.execute(sql, tuple(new_item.values()))
-
-        except Exception as e:
-            self.slog.warning(
-                f"Pipe Warn: {e} & Table: {_table_name} & Item: {new_item}"
-            )
-            cursor.execute("ROLLBACK")
-            deal_postgres_err(
-                TwistedAsynchronous(),
-                err_msg=str(e),
-                cursor=cursor,
-                table=_table_name,
-                table_notes=_table_notes,
-                note_dic=note_dic,
-            )
-            return self.db_insert(cursor, item)
-        return item
-
-    def handle_error(self, failure, item):
-        self.slog.error(f"插入数据失败:{failure}, item: {item}")
+from typing import TYPE_CHECKING, Any
+
+from twisted.enterprise import adbapi
+
+from ayugespidertools.common.expend import OraclePipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+__all__ = [
+    "AyuTwistedOraclePipeline",
+]
+
+if TYPE_CHECKING:
+    from oracledb.connection import Connection
+    from twisted.python.failure import Failure
+
+    from ayugespidertools.common.typevars import OracleConf, slogT
+    from ayugespidertools.spiders import AyuSpider
+
+
+class AyuTwistedOraclePipeline(OraclePipeEnhanceMixin):
+    oracle_conf: "OracleConf"
+    slog: "slogT"
+    conn: "Connection"
+    dbpool: "adbapi.ConnectionPool"
+
+    def open_spider(self, spider: "AyuSpider") -> None:
+        assert hasattr(spider, "oracle_conf"), "未配置 Oracle 连接信息！"
+        self.slog = spider.slog
+        self.oracle_conf = spider.oracle_conf
+
+        _oracle_conf = {
+            "user": self.oracle_conf.user,
+            "password": self.oracle_conf.password,
+            "host": self.oracle_conf.host,
+            "port": self.oracle_conf.port,
+            "service_name": self.oracle_conf.service_name,
+            "encoding": self.oracle_conf.encoding,
+            "config_dir": self.oracle_conf.thick_lib_dir or None,
+        }
+        self.dbpool = adbapi.ConnectionPool(
+            "oracledb", cp_reconnect=True, **_oracle_conf
+        )
+        query = self.dbpool.runInteraction(self.db_create)
+        query.addErrback(self.db_create_err)
+
+    def db_create(self, cursor: Any) -> None:
+        pass
+
+    def db_create_err(self, failure: "Failure") -> None:
+        self.slog.error(f"创建数据表失败: {failure}")
+
+    def process_item(self, item: Any, spider: "AyuSpider") -> Any:
+        item_dict = ReuseOperation.item_to_dict(item)
+        query = self.dbpool.runInteraction(self.db_insert, item_dict)
+        query.addErrback(self.handle_error, item)
+        return item
+
+    def db_insert(self, cursor: Any, item: Any) -> Any:
+        alter_item = ReuseOperation.reshape_item(item)
+        if not (new_item := alter_item.new_item):
+            return
+
+        sql = self._get_sql_by_item(table=alter_item.table.name, item=new_item)
+        cursor.execute(sql, tuple(new_item.values()))
+        return item
+
+    def handle_error(self, failure: "Failure", item: Any) -> None:
+        self.slog.error(f"插入数据失败:{failure}, item: {item}")
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.9.8/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,186 +1,185 @@
-import time
-from pathlib import Path
-from typing import TYPE_CHECKING, Any
-
-from scrapy.spiders import Spider
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.spiderconf import (
-    DynamicProxyCreator,
-    ESConfCreator,
-    ExclusiveProxyCreator,
-    KafkaConfCreator,
-    MongoDBConfCreator,
-    MQConfCreator,
-    MysqlConfCreator,
-    OracleConfCreator,
-    OssConfCreator,
-    PostgreSQLConfCreator,
-    get_spider_conf,
-    get_sqlalchemy_conf,
-)
-from ayugespidertools.config import logger
-
-__all__ = [
-    "AyuSpider",
-]
-
-if TYPE_CHECKING:
-    from elasticsearch import Elasticsearch
-    from scrapy.crawler import Crawler
-    from scrapy.settings import BaseSettings
-    from sqlalchemy.engine.base import Connection as SqlalchemyConnectT
-    from sqlalchemy.engine.base import Engine as SqlalchemyEngineT
-    from typing_extensions import Self
-
-    from ayugespidertools.common.typevars import (
-        DynamicProxyConf,
-        ESConf,
-        ExclusiveProxyConf,
-        KafkaConf,
-        MongoDBConf,
-        MQConf,
-        MysqlConf,
-        OracleConf,
-        OssConf,
-        PostgreSQLConf,
-        slogT,
-    )
-
-
-class AyuSpider(Spider):
-    mysql_engine: "SqlalchemyEngineT"
-    mysql_engine_conn: "SqlalchemyConnectT"
-    postgres_engine: "SqlalchemyEngineT"
-    postgres_engine_conn: "SqlalchemyConnectT"
-    oracle_engine: "SqlalchemyEngineT"
-    oracle_engine_conn: "SqlalchemyConnectT"
-    es_engine: "Elasticsearch"
-    es_engine_conn: "Elasticsearch"
-
-    mysql_conf: "MysqlConf"
-    mongodb_conf: "MongoDBConf"
-    postgres_conf: "PostgreSQLConf"
-    es_conf: "ESConf"
-    oracle_conf: "OracleConf"
-    rabbitmq_conf: "MQConf"
-    kafka_conf: "KafkaConf"
-    dynamicproxy_conf: "DynamicProxyConf"
-    exclusiveproxy_conf: "ExclusiveProxyConf"
-    oss_conf: "OssConf"
-
-    SPIDER_TIME: str = time.strftime("%Y-%m-%d", time.localtime())
-
-    @property
-    def slog(self) -> "slogT":
-        """本库的日志管理模块，使用 loguru 来管理日志
-        Note:
-            本配置可与 Scrapy 的 spider.log 同时管理，根据场景可以自行配置。
-        """
-        loguru_enabled = self.crawler.settings.get("LOGURU_ENABLED", True)
-        assert isinstance(loguru_enabled, bool), "loguru_enabled 参数格式需要为 bool"
-
-        return logger if loguru_enabled else super(AyuSpider, self).logger
-
-    @classmethod
-    def update_settings(cls, settings: "BaseSettings") -> None:
-        _normal_settings = {
-            "ROBOTSTXT_OBEY": False,
-            "TELNETCONSOLE_ENABLED": False,
-            "DEPTH_PRIORITY": -1,
-        }
-
-        if not (vit_dir := settings.get("VIT_DIR", None)):
-            logger.warning("settings 中未配置 VIT_DIR，将从默认配置中获取！")
-            exec_path = Path().resolve()
-            _parts = exec_path.parts[-2:]
-            assert len(_parts) >= 2, "执行脚本的路径可能存在问题！"
-            vit_dir = (
-                exec_path / "VIT"
-                if _parts[0] == _parts[1]
-                else exec_path / settings["BOT_NAME"] / "VIT"
-            )
-            _normal_settings["VIT_DIR"] = vit_dir
-
-        # 根据本地配置获取对应的 inner_settings
-        inner_settings = ReuseOperation.fetch_local_conf(
-            vit_dir=vit_dir, inner_settings=_normal_settings
-        )
-        settings.setdict(inner_settings, priority="project")
-        settings.setdict(cls.custom_settings or {}, priority="spider")
-
-    @classmethod
-    def from_crawler(cls, crawler: "Crawler", *args: Any, **kwargs: Any) -> "Self":
-        spider = super(AyuSpider, cls).from_crawler(crawler, *args, **kwargs)
-        _db_engine_enabled = crawler.settings.get("DATABASE_ENGINE_ENABLED", False)
-
-        remote_option = ReuseOperation.get_remote_option(settings=crawler.settings)
-        # 将本地 .conf 或远程（consul, nacos）中对应的配置信息，赋值给 spider 对象
-        if mysql_conf := get_spider_conf(
-            MysqlConfCreator(), crawler.settings, remote_option
-        ):
-            spider.mysql_conf = mysql_conf
-            spider.mysql_engine, spider.mysql_engine_conn = get_sqlalchemy_conf(
-                creator=MysqlConfCreator(),
-                db_conf=mysql_conf,
-                db_engine_enabled=_db_engine_enabled,
-            )
-
-        if mongodb_conf := get_spider_conf(
-            MongoDBConfCreator(), crawler.settings, remote_option
-        ):
-            spider.mongodb_conf = mongodb_conf
-
-        if postgres_conf := get_spider_conf(
-            PostgreSQLConfCreator(), crawler.settings, remote_option
-        ):
-            spider.postgres_conf = postgres_conf
-            spider.postgres_engine, spider.postgres_engine_conn = get_sqlalchemy_conf(
-                creator=PostgreSQLConfCreator(),
-                db_conf=postgres_conf,
-                db_engine_enabled=_db_engine_enabled,
-            )
-
-        if es_conf := get_spider_conf(ESConfCreator(), crawler.settings, remote_option):
-            spider.es_conf = es_conf
-            spider.es_engine = spider.es_engine_conn = get_sqlalchemy_conf(
-                creator=ESConfCreator(),
-                db_conf=es_conf,
-                db_engine_enabled=_db_engine_enabled,
-            )
-
-        if oracle_conf := get_spider_conf(
-            OracleConfCreator(), crawler.settings, remote_option
-        ):
-            spider.oracle_conf = oracle_conf
-            spider.oracle_engine, spider.oracle_engine_conn = get_sqlalchemy_conf(
-                creator=OracleConfCreator(),
-                db_conf=oracle_conf,
-                db_engine_enabled=_db_engine_enabled,
-            )
-
-        if rabbitmq_conf := get_spider_conf(
-            MQConfCreator(), crawler.settings, remote_option
-        ):
-            spider.rabbitmq_conf = rabbitmq_conf
-
-        if kafka_conf := get_spider_conf(
-            KafkaConfCreator(), crawler.settings, remote_option
-        ):
-            spider.kafka_conf = kafka_conf
-
-        if dynamicproxy_conf := get_spider_conf(
-            DynamicProxyCreator(), crawler.settings, remote_option
-        ):
-            spider.dynamicproxy_conf = dynamicproxy_conf
-
-        if exclusiveproxy_conf := get_spider_conf(
-            ExclusiveProxyCreator(), crawler.settings, remote_option
-        ):
-            spider.exclusiveproxy_conf = exclusiveproxy_conf
-
-        if oss_conf := get_spider_conf(
-            OssConfCreator(), crawler.settings, remote_option
-        ):
-            spider.oss_conf = oss_conf
-        return spider
+import time
+from pathlib import Path
+from typing import TYPE_CHECKING, Any
+
+from scrapy.spiders import Spider
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.spiderconf import (
+    DynamicProxyCreator,
+    ESConfCreator,
+    ExclusiveProxyCreator,
+    KafkaConfCreator,
+    MongoDBConfCreator,
+    MQConfCreator,
+    MysqlConfCreator,
+    OracleConfCreator,
+    OssConfCreator,
+    PostgreSQLConfCreator,
+    get_spider_conf,
+    get_sqlalchemy_conf,
+)
+from ayugespidertools.config import logger
+
+__all__ = [
+    "AyuSpider",
+]
+
+if TYPE_CHECKING:
+    from elasticsearch import Elasticsearch
+    from scrapy.crawler import Crawler
+    from scrapy.settings import BaseSettings
+    from sqlalchemy.engine.base import Connection as SqlalchemyConnectT
+    from sqlalchemy.engine.base import Engine as SqlalchemyEngineT
+    from typing_extensions import Self
+
+    from ayugespidertools.common.typevars import (
+        DynamicProxyConf,
+        ESConf,
+        ExclusiveProxyConf,
+        KafkaConf,
+        MongoDBConf,
+        MQConf,
+        MysqlConf,
+        OracleConf,
+        OssConf,
+        PostgreSQLConf,
+        slogT,
+    )
+
+
+class AyuSpider(Spider):
+    mysql_engine: "SqlalchemyEngineT"
+    mysql_engine_conn: "SqlalchemyConnectT"
+    postgres_engine: "SqlalchemyEngineT"
+    postgres_engine_conn: "SqlalchemyConnectT"
+    oracle_engine: "SqlalchemyEngineT"
+    oracle_engine_conn: "SqlalchemyConnectT"
+    es_engine: "Elasticsearch"
+    es_engine_conn: "Elasticsearch"
+
+    mysql_conf: "MysqlConf"
+    mongodb_conf: "MongoDBConf"
+    postgres_conf: "PostgreSQLConf"
+    es_conf: "ESConf"
+    oracle_conf: "OracleConf"
+    rabbitmq_conf: "MQConf"
+    kafka_conf: "KafkaConf"
+    dynamicproxy_conf: "DynamicProxyConf"
+    exclusiveproxy_conf: "ExclusiveProxyConf"
+    oss_conf: "OssConf"
+
+    SPIDER_TIME: str = time.strftime("%Y-%m-%d", time.localtime())
+
+    @property
+    def slog(self) -> "slogT":
+        """本库的日志管理模块，使用 loguru 来管理日志
+        Note:
+            本配置可与 Scrapy 的 spider.log 同时管理，根据场景可以自行配置。
+        """
+        loguru_enabled = self.crawler.settings.get("LOGURU_ENABLED", True)
+        assert isinstance(loguru_enabled, bool), "loguru_enabled 参数格式需要为 bool"
+
+        return logger if loguru_enabled else super(AyuSpider, self).logger
+
+    @classmethod
+    def update_settings(cls, settings: "BaseSettings") -> None:
+        _normal_settings = {
+            "ROBOTSTXT_OBEY": False,
+            "TELNETCONSOLE_ENABLED": False,
+            "DEPTH_PRIORITY": -1,
+        }
+
+        if not (vit_dir := settings.get("VIT_DIR", None)):
+            logger.warning("settings 中未配置 VIT_DIR，将从默认配置中获取！")
+            exec_path = Path().resolve()
+            _parts = exec_path.parts[-2:]
+            assert len(_parts) >= 2, "执行脚本的路径可能存在问题！"
+            vit_dir = (
+                exec_path / "VIT"
+                if _parts[0] == _parts[1]
+                else exec_path / settings["BOT_NAME"] / "VIT"
+            )
+            _normal_settings["VIT_DIR"] = vit_dir
+
+        inner_settings = ReuseOperation.fetch_local_conf(
+            vit_dir=vit_dir, inner_settings=_normal_settings
+        )
+        settings.setdict(inner_settings, priority="project")
+        settings.setdict(cls.custom_settings or {}, priority="spider")
+
+    @classmethod
+    def from_crawler(cls, crawler: "Crawler", *args: Any, **kwargs: Any) -> "Self":
+        spider = super(AyuSpider, cls).from_crawler(crawler, *args, **kwargs)
+        _db_engine_enabled = crawler.settings.get("DATABASE_ENGINE_ENABLED", False)
+
+        remote_option = ReuseOperation.get_remote_option(settings=crawler.settings)
+        # 将本地 .conf 或远程（consul, nacos）中对应的配置信息，赋值给 spider 对象
+        if mysql_conf := get_spider_conf(
+            MysqlConfCreator(), crawler.settings, remote_option
+        ):
+            spider.mysql_conf = mysql_conf
+            spider.mysql_engine, spider.mysql_engine_conn = get_sqlalchemy_conf(
+                creator=MysqlConfCreator(),
+                db_conf=mysql_conf,
+                db_engine_enabled=_db_engine_enabled,
+            )
+
+        if mongodb_conf := get_spider_conf(
+            MongoDBConfCreator(), crawler.settings, remote_option
+        ):
+            spider.mongodb_conf = mongodb_conf
+
+        if postgres_conf := get_spider_conf(
+            PostgreSQLConfCreator(), crawler.settings, remote_option
+        ):
+            spider.postgres_conf = postgres_conf
+            spider.postgres_engine, spider.postgres_engine_conn = get_sqlalchemy_conf(
+                creator=PostgreSQLConfCreator(),
+                db_conf=postgres_conf,
+                db_engine_enabled=_db_engine_enabled,
+            )
+
+        if es_conf := get_spider_conf(ESConfCreator(), crawler.settings, remote_option):
+            spider.es_conf = es_conf
+            spider.es_engine = spider.es_engine_conn = get_sqlalchemy_conf(
+                creator=ESConfCreator(),
+                db_conf=es_conf,
+                db_engine_enabled=_db_engine_enabled,
+            )
+
+        if oracle_conf := get_spider_conf(
+            OracleConfCreator(), crawler.settings, remote_option
+        ):
+            spider.oracle_conf = oracle_conf
+            spider.oracle_engine, spider.oracle_engine_conn = get_sqlalchemy_conf(
+                creator=OracleConfCreator(),
+                db_conf=oracle_conf,
+                db_engine_enabled=_db_engine_enabled,
+            )
+
+        if rabbitmq_conf := get_spider_conf(
+            MQConfCreator(), crawler.settings, remote_option
+        ):
+            spider.rabbitmq_conf = rabbitmq_conf
+
+        if kafka_conf := get_spider_conf(
+            KafkaConfCreator(), crawler.settings, remote_option
+        ):
+            spider.kafka_conf = kafka_conf
+
+        if dynamicproxy_conf := get_spider_conf(
+            DynamicProxyCreator(), crawler.settings, remote_option
+        ):
+            spider.dynamicproxy_conf = dynamicproxy_conf
+
+        if exclusiveproxy_conf := get_spider_conf(
+            ExclusiveProxyCreator(), crawler.settings, remote_option
+        ):
+            spider.exclusiveproxy_conf = exclusiveproxy_conf
+
+        if oss_conf := get_spider_conf(
+            OssConfCreator(), crawler.settings, remote_option
+        ):
+            spider.oss_conf = oss_conf
+        return spider
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.9.8/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.9.7/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.9.8/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from scrapy.spiders import CSVFeedSpider
 
 
 class $classname(CSVFeedSpider):
     name = "$name"
     allowed_domains = ["$domain"]
-    start_urls = ["http://$domain/feed.csv"]
+    start_urls = ["$url"]
     #headers = ["id", "name", "description", "image_link"]
     #delimiter = "\t"
 
     # Do any adaptations you need here
     #def adapt_response(self, response):
     #    return response
```

### Comparing `ayugespidertools-3.9.7/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.9.8/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from scrapy.spiders import XMLFeedSpider
 
 
 class $classname(XMLFeedSpider):
     name = "$name"
     allowed_domains = ["$domain"]
-    start_urls = ["http://$domain/feed.xml"]
+    start_urls = ["$url"]
     iterator = "iternodes"  # you can change this; see the docs
     itertag = "item"  # change it accordingly
 
     def parse_node(self, response, selector):
         item = {}
         #item["url"] = selector.select("url").get()
         #item["name"] = selector.select("name").get()
```

### Comparing `ayugespidertools-3.9.7/pyproject.toml` & `ayugespidertools-3.9.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,177 +1,176 @@
-[tool.poetry]
-name = "AyugeSpiderTools"
-version = "3.9.7"
-description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。"
-authors = ["ayuge <ayugesheng@gmail.com>"]
-maintainers = ["ayuge <ayugesheng@gmail.com>"]
-readme = "README.md"
-packages = [{ include = "ayugespidertools" }]
-repository = "https://github.com/shengchenyang/AyugeSpiderTools"
-documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
-keywords = ["crawler", "scraping", "aiohttp", "asyncio", "scrapy"]
-homepage = "https://www.ayuge.top/mkdocs-material/"
-
-[tool.poetry.dependencies]
-python = "^3.8.1"
-PyMySQL = "^1.0.2"
-loguru = "~0.7.0"
-requests = "^2.28.1"
-Scrapy = "2.11.1"
-retrying = "^1.3.3"
-SQLAlchemy = "^2.0.23"
-DBUtils = "^3.0.2"
-itemadapter = "^0.7.0"
-aiohttp = "~3.9.3"
-aiomysql = "^0.1.1"
-pika = "~1.3.2"
-kafka-python = "2.0.2"
-motor = [
-    { version = "2.5.1", python = "<3.11" },
-    { version = "3.3.0", python = ">=3.11" },
-]
-pymongo = [
-    { version = "^3.12.3", python = "<3.11" },
-    { version = "^4.5.0", python = ">=3.11" },
-]
-mmh3 = { version = "^3.0.0", optional = true }
-pycryptodome = { version = "^3.15.0", optional = true }
-python-hcl2 = { version = "^4.3.0", optional = true }
-pyyaml = { version = "~6.0", optional = true }
-opencv-python = { version = "~4.8.0.74", optional = true }
-Pillow = { version = "^9.2.0", optional = true }
-numpy = [
-    { version = "~1.24.3", python = "<3.9", optional = true },
-    { version = "~1.26.0", python = ">=3.9,<3.13", optional = true },
-]
-psycopg = { version = "^3.1.13", optional = true }
-psycopg-binary = { version = "^3.1.13", optional = true }
-psycopg-pool = { version = "^3.2.0", optional = true }
-oracledb = { version = "^1.4.2", optional = true }
-elasticsearch-dsl = { version = "^8.11.0", optional = true }
-oss2 = { version = "^2.18.4", optional = true }
-
-[tool.poetry.scripts]
-ayuge = "ayugespidertools.utils.cmdline:execute"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
-black = "24.2.0"
-isort = "5.13.2"
-sphinx-rtd-theme = "1.2.0"
-coverage = "^7.2.2"
-tox = "^4.4.8"
-flake8 = "7.0.0"
-testfixtures = "^7.1.0"
-myst-parser = "1.0.0"
-sphinx-markdown-tables = "0.0.17"
-sphinx-hoverxref = "1.3.0"
-sphinx-notfound-page = "0.8.3"
-mypy = "~1.5.1"
-pre-commit = "3.5.0"
-toml = "0.10.2"
-
-[tool.poetry.extras]
-all = [
-    "mmh3", "pycryptodome", "python-hcl2", "pyyaml", "opencv-python", "numpy",
-    "Pillow", "psycopg", "psycopg-binary", "psycopg-pool", "oracledb",
-    "elasticsearch-dsl", "oss2"
-]
-database = [
-    "psycopg", "psycopg-binary", "psycopg-pool", "oracledb", "elasticsearch-dsl"
-]
-
-[[tool.poetry.source]]
-name = "aliyun"
-url = "https://mirrors.aliyun.com/pypi/simple"
-priority = "default"
-
-[[tool.poetry.source]]
-name = "PyPI"
-priority = "primary"
-
-[tool.pytest.ini_options]
-xfail_strict = true
-python_files = "test_*.py __init__.py"
-python_classes = "Test*"
-testpaths = [
-    "tests",
-]
-norecursedirs = ["dist", "build", "docs", "examples"]
-addopts = "--assert=plain --doctest-modules --reactor=asyncio"
-filterwarnings = [
-    "ignore::DeprecationWarning",
-    "ignore:scrapy.downloadermiddlewares.decompression is deprecated",
-    "ignore:Module scrapy.utils.reqser is deprecated",
-    "ignore:typing.re is deprecated",
-    "ignore:typing.io is deprecated"
-]
-
-[tool.coverage.run]
-branch = true
-source = ["ayugespidertools"]
-parallel = true
-omit = [
-    "tests/docs/*",
-    "tests/VIT/*",
-    "tests/conftest.py",
-    "tests/**/__init__.py",
-    "ayugespidertools/**/__init__.py",
-    "ayugespidertools/utils/cmdline.py",
-]
-
-[tool.coverage.report]
-exclude_lines = [
-    "if __name__ == '__main__':",
-    "pragma: no cover",
-    "raise AssertionError",
-    "raise NotImplementedError",
-    "if TYPE_CHECKING:",
-    "__repr__",
-    "__str__",
-]
-precision = 2
-fail_under = 30
-
-[tool.coverage.html]
-directory = "htmlcov"
-
-[tool.coverage.xml]
-output = "coverage.xml"
-
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-python_version = "3.8"
-ignore_missing_imports = true
-disable_error_code = ["attr-defined", "arg-type", "union-attr"]
-
-[[tool.mypy.overrides]]
-module = [
-    "yaml",
-    "toml",
-    "pymysql",
-    "pymysql.connections",
-    "pymysql.cursors",
-    "requests",
-]
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "ayugespidertools.items"
-ignore_errors = "True"
-
-[[tool.mypy.overrides]]
-module = "ayugespidertools.common.typevars"
-ignore_errors = "True"
-
-[[tool.mypy.overrides]]
-module = "tests.mockserver"
-ignore_errors = "True"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "AyugeSpiderTools"
+version = "3.9.8"
+description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。"
+authors = ["ayuge <ayugesheng@gmail.com>"]
+maintainers = ["ayuge <ayugesheng@gmail.com>"]
+readme = "README.md"
+packages = [{ include = "ayugespidertools" }]
+repository = "https://github.com/shengchenyang/AyugeSpiderTools"
+documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
+keywords = ["crawler", "scraping", "scrapy-extension"]
+homepage = "https://www.ayuge.top/mkdocs-material/"
+
+[tool.poetry.dependencies]
+python = "^3.8.1"
+PyMySQL = "^1.0.2"
+loguru = "~0.7.0"
+Scrapy = "2.11.2"
+retrying = "^1.3.3"
+SQLAlchemy = "^2.0.23"
+DBUtils = "^3.0.2"
+itemadapter = "^0.7.0"
+aiohttp = "~3.9.3"
+aiomysql = "^0.1.1"
+pika = "~1.3.2"
+kafka-python = "2.0.2"
+motor = [
+    { version = "2.5.1", python = "<3.11" },
+    { version = "3.3.0", python = ">=3.11" },
+]
+pymongo = [
+    { version = "^3.12.3", python = "<3.11" },
+    { version = "^4.5.0", python = ">=3.11" },
+]
+mmh3 = { version = "^3.0.0", optional = true }
+pycryptodome = { version = "^3.15.0", optional = true }
+python-hcl2 = { version = "^4.3.0", optional = true }
+pyyaml = { version = "~6.0", optional = true }
+opencv-python = { version = "~4.8.0.74", optional = true }
+Pillow = { version = "^9.2.0", optional = true }
+numpy = [
+    { version = "~1.24.3", python = "<3.9", optional = true },
+    { version = "~1.26.0", python = ">=3.9,<3.13", optional = true },
+]
+psycopg = { version = "^3.1.13", optional = true }
+psycopg-binary = { version = "^3.1.13", optional = true }
+psycopg-pool = { version = "^3.2.0", optional = true }
+oracledb = { version = "^1.4.2", optional = true }
+elasticsearch-dsl = { version = "^8.11.0", optional = true }
+oss2 = { version = "^2.18.4", optional = true }
+
+[tool.poetry.scripts]
+ayuge = "ayugespidertools.utils.cmdline:execute"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.3"
+black = "24.2.0"
+isort = "5.13.2"
+sphinx-rtd-theme = "1.2.0"
+coverage = "^7.2.2"
+tox = "^4.4.8"
+flake8 = "7.0.0"
+testfixtures = "^7.1.0"
+myst-parser = "1.0.0"
+sphinx-markdown-tables = "0.0.17"
+sphinx-hoverxref = "1.3.0"
+sphinx-notfound-page = "0.8.3"
+mypy = "~1.5.1"
+pre-commit = "3.5.0"
+toml = "0.10.2"
+
+[tool.poetry.extras]
+all = [
+    "mmh3", "pycryptodome", "python-hcl2", "pyyaml", "opencv-python", "numpy",
+    "Pillow", "psycopg", "psycopg-binary", "psycopg-pool", "oracledb",
+    "elasticsearch-dsl", "oss2"
+]
+database = [
+    "psycopg", "psycopg-binary", "psycopg-pool", "oracledb", "elasticsearch-dsl"
+]
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
+[[tool.poetry.source]]
+name = "aliyun"
+url = "https://mirrors.aliyun.com/pypi/simple"
+priority = "supplemental"
+
+[tool.pytest.ini_options]
+xfail_strict = true
+python_files = "test_*.py __init__.py"
+python_classes = "Test*"
+testpaths = [
+    "tests",
+]
+norecursedirs = ["dist", "build", "docs", "examples"]
+addopts = "--assert=plain --doctest-modules --reactor=asyncio"
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore:scrapy.downloadermiddlewares.decompression is deprecated",
+    "ignore:Module scrapy.utils.reqser is deprecated",
+    "ignore:typing.re is deprecated",
+    "ignore:typing.io is deprecated"
+]
+
+[tool.coverage.run]
+branch = true
+source = ["ayugespidertools"]
+parallel = true
+omit = [
+    "tests/docs/*",
+    "tests/VIT/*",
+    "tests/conftest.py",
+    "tests/**/__init__.py",
+    "ayugespidertools/request.py",
+    "ayugespidertools/**/__init__.py",
+    "ayugespidertools/utils/cmdline.py",
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    "if __name__ == '__main__':",
+    "pragma: no cover",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if TYPE_CHECKING:",
+    "__repr__",
+    "__str__",
+]
+precision = 2
+fail_under = 30
+
+[tool.coverage.html]
+directory = "htmlcov"
+
+[tool.coverage.xml]
+output = "coverage.xml"
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+python_version = "3.8"
+ignore_missing_imports = true
+disable_error_code = ["attr-defined", "arg-type", "union-attr"]
+
+[[tool.mypy.overrides]]
+module = [
+    "yaml",
+    "toml",
+    "pymysql",
+    "pymysql.connections",
+    "pymysql.cursors",
+]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "ayugespidertools.items"
+ignore_errors = "True"
+
+[[tool.mypy.overrides]]
+module = "ayugespidertools.common.typevars"
+ignore_errors = "True"
+
+[[tool.mypy.overrides]]
+module = "tests.mockserver"
+ignore_errors = "True"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ayugespidertools-3.9.7/PKG-INFO` & `ayugespidertools-3.9.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AyugeSpiderTools
-Version: 3.9.7
+Version: 3.9.8
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。
 Home-page: https://www.ayuge.top/mkdocs-material/
-Keywords: crawler,scraping,aiohttp,asyncio,scrapy
+Keywords: crawler,scraping,scrapy-extension
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: database
 Requires-Dist: DBUtils (>=3.0.2,<4.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0) ; extra == "all"
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.23,<3.0.0)
-Requires-Dist: Scrapy (==2.11.1)
+Requires-Dist: Scrapy (==2.11.2)
 Requires-Dist: aiohttp (>=3.9.3,<3.10.0)
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: elasticsearch-dsl (>=8.11.0,<9.0.0) ; extra == "all" or extra == "database"
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
 Requires-Dist: kafka-python (==2.0.2)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0) ; extra == "all"
@@ -40,31 +40,30 @@
 Requires-Dist: psycopg-binary (>=3.1.13,<4.0.0) ; extra == "all" or extra == "database"
 Requires-Dist: psycopg-pool (>=3.2.0,<4.0.0) ; extra == "all" or extra == "database"
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0) ; extra == "all"
 Requires-Dist: pymongo (>=3.12.3,<4.0.0) ; python_version < "3.11"
 Requires-Dist: pymongo (>=4.5.0,<5.0.0) ; python_version >= "3.11"
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0) ; extra == "all"
 Requires-Dist: pyyaml (>=6.0,<6.1) ; extra == "all"
-Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Project-URL: Documentation, https://ayugespidertools.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/shengchenyang/AyugeSpiderTools
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://ayugespidertools.readthedocs.io" target="_blank" rel="noopener noreferrer">
         <img src="./artwork/ayugespidertools-logo.png" alt="ayugespidertools-logo">
     </a>
 </p>
 <hr/>
 
 # AyugeSpiderTools 介绍
 
-![GitHub](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
-![python](https://img.shields.io/badge/python-3.8%2B-blue)
+![license](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
+![python support](https://img.shields.io/badge/python-3.8%2B-blue)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/codeql.yml?branch=main)
 ![Read the Docs](https://img.shields.io/readthedocs/ayugespidertools)
 ![GitHub all releases](https://img.shields.io/github/downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/AyugeSpiderTools?label=pypi%20downloads)
 ![codecov](https://codecov.io/gh/shengchenyang/AyugeSpiderTools/graph/badge.svg?token=1QLOEW2NTI)
 
 **简体中文** | [English](./README_en.md)
@@ -134,15 +133,15 @@
 
 # 运行脚本
 scrapy crawl <spider_name>
 # 注：也可以使用 ayuge crawl <spider_name>
 ```
 
 具体的场景案例请在 [DemoSpider](https://github.com/shengchenyang/DemoSpider)
-项目中查看，也可以在 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中查看教程。 目前已适配以下场景：
+项目中查看，也可以在 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中查看教程。目前已适配以下场景：
 
 ```diff
 + 0).以下场景全支持从 nacos 或 consul 中获取配置，不一一举例。
 
 # 数据存入 Mysql 的场景：
 + 1).demo_one: 从 .conf 中获取 mysql 配置
 + 3).demo_three: 从 consul 中获取 mysql 配置
@@ -192,31 +191,31 @@
 ```
 
 ## 跑通测试
 
 前提：需要在 `tests` 的 `VIT` 目录下创建 `.conf` 文件，已给出示例文件，请填写测试所需内容，然后：
 
 - 可以直接使用 `tox` 来运行测试。
-
 - 本库以 [poetry](https://python-poetry.org/docs/) 开发，那么直接新环境下运行 `poetry install`
   后，手动运行目标测试或 `pytest` 命令来测试等皆可。
 - 也可以使用 `make` 工具，`make start` 然后 `make test` 即可。
 
 ## 你可能在意的事
 
 1. 若你觉得某些场景下的功能实现不太符合你的预期，想要修改或添加自定义功能，比如移除对你无用模块、修改库名等，你可以自行修改后 `build`。
 
-2. 本库主推 `scrapy` 扩展（即增强版的自定义模板）的功能，在使用本库时，理论上并不会影响你 `scrapy`
-   项目及其它组件。
+2. 本库主推 `scrapy` 扩展功能，在使用本库时，不会影响你 `scrapy` 项目及其它组件。
+
+   也就是说，可使用本库开发原生的 `scrapy`，也可用 `scrapy` 的风格来开发，但还是推荐使用 `DemoSpider` 示例中的风格开发。不会对开发者造成过多的迁移成本。
 
 3. 代码测试覆盖率有点低，考虑增加吗？
 
    不考虑，场景所依赖服务太多，且云服务等其它因素导致个人维护成本过高，但不必担心，我会和本地服务的自动化测试结合使用。
 
-4. 如果你想对此项目做出贡献，请参考[pull request 示例](https://ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)。
+4. 如果你想对此项目做出贡献，请参考 [pull request 示例](https://ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)。
 
 ## 构建你的专属库
 
 > 具体内容请以 [poetry 官方文档](https://python-poetry.org/docs/) 为准。
 
 据[你可能在意的事](#你可能在意的事)可知，你可以 `clone`
 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry build`
@@ -227,47 +226,48 @@
 ），确定测试正常了即可 `poetry build` 打包使用。
 
 **希望此项目能在你遇到扩展 scrapy 功能的场景时能对你有所指引。**
 
 ## 功能
 
 - [x] `scrapy` 的扩展功能场景
-    - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
-    - [x] 自定义模板，在 `ayuge startproject <projname>` 和 `ayuge genspider <spidername>` 时生成适合本库的模板文件
-    - [x] 从远程应用管理服务中获取项目配置
-        - [x] 从 `consul` 获取项目配置
-        - [x] 从 `nacos` 获取项目配置（注意：优先级小于 `consul`）
-    - [x] 代理中间件（独享代理、动态隧道代理）
-    - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
-    - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-        - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp`
-          的方式）
-        - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
-    - [x] `Mysql` 存储的场景下适配
-        - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
-    - [x] `MongoDB` 存储场景适配
-    - [x] `PostgreSQL` 存储场景适配
-    - [x] `ElasticSearch` 存储场景适配
-    - [x] `Oracle` 存储场景适配
-    - [x] `oss` 上传场景适配
-    - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
-        - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
-        - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
-    - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
+  - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
+  - [x] 自定义模板，在 `ayuge startproject <projname>` 和 `ayuge genspider <spidername>` 时生成适合本库的模板文件
+  - [x] 从远程应用管理服务中获取项目配置
+    - [x] 从 `consul` 获取项目配置
+    - [x] 从 `nacos` 获取项目配置（注意：优先级小于 `consul`）
+  - [x] 代理中间件（独享代理、动态隧道代理）
+  - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
+  - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
+    - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp`
+      的方式）
+    - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
+  - [x] `Mysql` 存储的场景下适配
+    - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
+  - [x] `MongoDB` 存储场景适配
+  - [x] `PostgreSQL` 存储场景适配
+  - [x] `ElasticSearch` 存储场景适配
+  - [x] `Oracle` 存储场景适配
+  - [x] `oss` 上传场景适配
+  - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
+    - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
+    - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
+  - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
 - [x] 常用开发场景
-    - [x] `sql` 语句拼接，只用于简单场景。已给出优化方向，参考库等信息。
-    - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
-    - [x] 字体反爬还原方法
-        - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
-            - [x] 可以直接在字体文件 `xml`
-              中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
-            - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`
-              ，后再通过各种方式识别。
-    - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等
-    - [x] 添加常用的图片验证码中的处理方法
-        - [x] 滑块缺口距离的识别方法（多种实现方式）
-        - [x] 根据滑块距离生成轨迹数组的方法
-        - [x] 识别点选验证码位置及点击顺序
-        - [x] 图片乱序混淆的还原方法示例
+  - [x] `sql` 语句拼接，只用于简单场景。
+  - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
+  - [x] 字体反爬还原方法
+    - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
+      - [x] 可以直接在字体文件 `xml`
+        中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
+      - [x] 无法找到映射关系的，则一般使用 `ocr` 识别（准确率非百分百），通过 `fontforge` 导出每个映射的 `png`
+        ，后再通过各种方式识别。
+    - [x] 字体反爬部分功能迁移到 `FontMapster` 项目中。
+  - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等
+  - [x] 添加常用的图片验证码中的处理方法
+    - [x] 滑块缺口距离的识别方法（多种实现方式）
+    - [x] 根据滑块距离生成轨迹数组的方法
+    - [x] 识别点选验证码位置及点击顺序
+    - [x] 图片乱序混淆的还原方法示例
 
 注意：功能演示我将放入 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/) 文档中，以防此部分内容过多。
```

#### html2text {}

```diff
@@ -1,50 +1,48 @@
-Metadata-Version: 2.1 Name: AyugeSpiderTools Version: 3.9.7 Summary: scrapy
+Metadata-Version: 2.1 Name: AyugeSpiderTools Version: 3.9.8 Summary: scrapy
 æ©å±åºï¼ç¨äºæ©å± Scrapy åè½æ¥è§£æ¾åæã Home-page: https://
-www.ayuge.top/mkdocs-material/ Keywords:
-crawler,scraping,aiohttp,asyncio,scrapy Author: ayuge Author-email:
-ayugesheng@gmail.com Maintainer: ayuge Maintainer-email: ayugesheng@gmail.com
-Requires-Python: >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
-Provides-Extra: database Requires-Dist: DBUtils (>=3.0.2,<4.0.0) Requires-Dist:
-Pillow (>=9.2.0,<10.0.0) ; extra == "all" Requires-Dist: PyMySQL
-(>=1.0.2,<2.0.0) Requires-Dist: SQLAlchemy (>=2.0.23,<3.0.0) Requires-Dist:
-Scrapy (==2.11.1) Requires-Dist: aiohttp (>=3.9.3,<3.10.0) Requires-Dist:
-aiomysql (>=0.1.1,<0.2.0) Requires-Dist: elasticsearch-dsl (>=8.11.0,<9.0.0) ;
-extra == "all" or extra == "database" Requires-Dist: itemadapter
-(>=0.7.0,<0.8.0) Requires-Dist: kafka-python (==2.0.2) Requires-Dist: loguru
-(>=0.7.0,<0.8.0) Requires-Dist: mmh3 (>=3.0.0,<4.0.0) ; extra == "all"
-Requires-Dist: motor (==2.5.1) ; python_version < "3.11" Requires-Dist: motor
-(==3.3.0) ; python_version >= "3.11" Requires-Dist: numpy (>=1.24.3,<1.25.0) ;
-(python_version < "3.9") and (extra == "all") Requires-Dist: numpy
-(>=1.26.0,<1.27.0) ; (python_version >= "3.9" and python_version < "3.13") and
-(extra == "all") Requires-Dist: opencv-python (>=4.8.0.74,<4.9.0.0) ; extra ==
-"all" Requires-Dist: oracledb (>=1.4.2,<2.0.0) ; extra == "all" or extra ==
-"database" Requires-Dist: oss2 (>=2.18.4,<3.0.0) ; extra == "all" Requires-
-Dist: pika (>=1.3.2,<1.4.0) Requires-Dist: psycopg (>=3.1.13,<4.0.0) ; extra ==
-"all" or extra == "database" Requires-Dist: psycopg-binary (>=3.1.13,<4.0.0) ;
-extra == "all" or extra == "database" Requires-Dist: psycopg-pool
-(>=3.2.0,<4.0.0) ; extra == "all" or extra == "database" Requires-Dist:
-pycryptodome (>=3.15.0,<4.0.0) ; extra == "all" Requires-Dist: pymongo
-(>=3.12.3,<4.0.0) ; python_version < "3.11" Requires-Dist: pymongo
-(>=4.5.0,<5.0.0) ; python_version >= "3.11" Requires-Dist: python-hcl2
-(>=4.3.0,<5.0.0) ; extra == "all" Requires-Dist: pyyaml (>=6.0,<6.1) ; extra ==
-"all" Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: retrying
-(>=1.3.3,<2.0.0) Project-URL: Documentation, https://
-ayugespidertools.readthedocs.io/en/latest/ Project-URL: Repository, https://
-github.com/shengchenyang/AyugeSpiderTools Description-Content-Type: text/
-markdown
+www.ayuge.top/mkdocs-material/ Keywords: crawler,scraping,scrapy-extension
+Author: ayuge Author-email: ayugesheng@gmail.com Maintainer: ayuge Maintainer-
+email: ayugesheng@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Provides-Extra: all Provides-Extra: database Requires-Dist:
+DBUtils (>=3.0.2,<4.0.0) Requires-Dist: Pillow (>=9.2.0,<10.0.0) ; extra ==
+"all" Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) Requires-Dist: SQLAlchemy
+(>=2.0.23,<3.0.0) Requires-Dist: Scrapy (==2.11.2) Requires-Dist: aiohttp
+(>=3.9.3,<3.10.0) Requires-Dist: aiomysql (>=0.1.1,<0.2.0) Requires-Dist:
+elasticsearch-dsl (>=8.11.0,<9.0.0) ; extra == "all" or extra == "database"
+Requires-Dist: itemadapter (>=0.7.0,<0.8.0) Requires-Dist: kafka-python
+(==2.0.2) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: mmh3
+(>=3.0.0,<4.0.0) ; extra == "all" Requires-Dist: motor (==2.5.1) ;
+python_version < "3.11" Requires-Dist: motor (==3.3.0) ; python_version >=
+"3.11" Requires-Dist: numpy (>=1.24.3,<1.25.0) ; (python_version < "3.9") and
+(extra == "all") Requires-Dist: numpy (>=1.26.0,<1.27.0) ; (python_version >=
+"3.9" and python_version < "3.13") and (extra == "all") Requires-Dist: opencv-
+python (>=4.8.0.74,<4.9.0.0) ; extra == "all" Requires-Dist: oracledb
+(>=1.4.2,<2.0.0) ; extra == "all" or extra == "database" Requires-Dist: oss2
+(>=2.18.4,<3.0.0) ; extra == "all" Requires-Dist: pika (>=1.3.2,<1.4.0)
+Requires-Dist: psycopg (>=3.1.13,<4.0.0) ; extra == "all" or extra ==
+"database" Requires-Dist: psycopg-binary (>=3.1.13,<4.0.0) ; extra == "all" or
+extra == "database" Requires-Dist: psycopg-pool (>=3.2.0,<4.0.0) ; extra ==
+"all" or extra == "database" Requires-Dist: pycryptodome (>=3.15.0,<4.0.0) ;
+extra == "all" Requires-Dist: pymongo (>=3.12.3,<4.0.0) ; python_version <
+"3.11" Requires-Dist: pymongo (>=4.5.0,<5.0.0) ; python_version >= "3.11"
+Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0) ; extra == "all" Requires-Dist:
+pyyaml (>=6.0,<6.1) ; extra == "all" Requires-Dist: retrying (>=1.3.3,<2.0.0)
+Project-URL: Documentation, https://ayugespidertools.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/shengchenyang/AyugeSpiderTools
+Description-Content-Type: text/markdown
                             _[_a_y_u_g_e_s_p_i_d_e_r_t_o_o_l_s_-_l_o_g_o_]
 ===============================================================================
-# AyugeSpiderTools ä»ç» ![GitHub](https://img.shields.io/github/license/
-shengchenyang/AyugeSpiderTools) ![python](https://img.shields.io/badge/python-
-3.8%2B-blue) ![GitHub Workflow Status (with branch)](https://img.shields.io/
-github/actions/workflow/status/shengchenyang/AyugeSpiderTools/
+# AyugeSpiderTools ä»ç» ![license](https://img.shields.io/github/license/
+shengchenyang/AyugeSpiderTools) ![python support](https://img.shields.io/badge/
+python-3.8%2B-blue) ![GitHub Workflow Status (with branch)](https://
+img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/
 codeql.yml?branch=main) ![Read the Docs](https://img.shields.io/readthedocs/
 ayugespidertools) ![GitHub all releases](https://img.shields.io/github/
 downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/
 AyugeSpiderTools?label=pypi%20downloads) ![codecov](https://codecov.io/gh/
 shengchenyang/AyugeSpiderTools/graph/badge.svg?token=1QLOEW2NTI)
 **ç®ä½ä¸­æ** | [English](./README_en.md) ## æ¦è¿° >
@@ -75,15 +73,15 @@
 è¿å¥é¡¹ç®æ ¹ç®å½ cd # æ¿æ¢(è¦ç)ä¸ºçå®çéç½® .conf æä»¶ï¼ #
 è¿éæ¯ä¸ºäºæ¼ç¤ºæ¹ä¾¿ï¼æ­£å¸¸æåµæ¯ç´æ¥å¨ VIT ä¸­ç .conf
 æä»¶å¡«ä¸ä½ éè¦çéç½®å³å¯ cp /root/mytemp/.conf DemoSpider/VIT/.conf
 # çæç¬è«èæ¬ ayuge genspider # è¿è¡èæ¬ scrapy crawl #
 æ³¨ï¼ä¹å¯ä»¥ä½¿ç¨ ayuge crawl ``` å·ä½çåºæ¯æ¡ä¾è¯·å¨ [DemoSpider]
 (https://github.com/shengchenyang/DemoSpider) é¡¹ç®ä¸­æ¥çï¼ä¹å¯ä»¥å¨
 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/
-) ææ¡£ä¸­æ¥çæç¨ã ç®åå·²ééä»¥ä¸åºæ¯ï¼ ```diff +
+) ææ¡£ä¸­æ¥çæç¨ãç®åå·²ééä»¥ä¸åºæ¯ï¼ ```diff +
 0).ä»¥ä¸åºæ¯å¨æ¯æä» nacos æ consul
 ä¸­è·åéç½®ï¼ä¸ä¸ä¸ä¸¾ä¾ã # æ°æ®å­å¥ Mysql çåºæ¯ï¼ +
 1).demo_one: ä» .conf ä¸­è·å mysql éç½® + 3).demo_three: ä» consul
 ä¸­è·å mysql éç½® + 21).demo_mysql_nacos: ä» nacos ä¸­è·å mysql éç½®
 + 5).demo_five: Twisted å¼æ­¥å­å¨ç¤ºä¾ + 24).demo_aiomysql: ç»å aiomysql
 å®ç°ç asyncio å¼æ­¥å­å¨ç¤ºä¾ + 13).demo_AyuTurboMysqlPipeline: mysql
 åæ­¥è¿æ¥æ± çç¤ºä¾ # æ°æ®å­å¥ MongoDB çåºæ¯ï¼ + 2).demo_two: ä»
@@ -118,23 +116,26 @@
 å¯ä»¥ç´æ¥ä½¿ç¨ `tox` æ¥è¿è¡æµè¯ã - æ¬åºä»¥ [poetry](https://
 python-poetry.org/docs/) å¼åï¼é£ä¹ç´æ¥æ°ç¯å¢ä¸è¿è¡ `poetry
 install` åï¼æå¨è¿è¡ç®æ æµè¯æ `pytest` å½ä»¤æ¥æµè¯ç­çå¯ã
 - ä¹å¯ä»¥ä½¿ç¨ `make` å·¥å·ï¼`make start` ç¶å `make test` å³å¯ã ##
 ä½ å¯è½å¨æçäº 1.
 è¥ä½ è§å¾æäºåºæ¯ä¸çåè½å®ç°ä¸å¤ªç¬¦åä½ çé¢æï¼æ³è¦ä¿®æ¹ææ·»å èªå®ä¹åè½ï¼æ¯å¦ç§»é¤å¯¹ä½ æ ç¨æ¨¡åãä¿®æ¹åºåç­ï¼ä½ å¯ä»¥èªè¡ä¿®æ¹å
 `build`ã 2. æ¬åºä¸»æ¨ `scrapy`
-æ©å±ï¼å³å¢å¼ºççèªå®ä¹æ¨¡æ¿ï¼çåè½ï¼å¨ä½¿ç¨æ¬åºæ¶ï¼çè®ºä¸å¹¶ä¸ä¼å½±åä½ 
-`scrapy` é¡¹ç®åå¶å®ç»ä»¶ã 3.
+æ©å±åè½ï¼å¨ä½¿ç¨æ¬åºæ¶ï¼ä¸ä¼å½±åä½  `scrapy`
+é¡¹ç®åå¶å®ç»ä»¶ã ä¹å°±æ¯è¯´ï¼å¯ä½¿ç¨æ¬åºå¼ååçç
+`scrapy`ï¼ä¹å¯ç¨ `scrapy` çé£æ ¼æ¥å¼åï¼ä½è¿æ¯æ¨èä½¿ç¨
+`DemoSpider`
+ç¤ºä¾ä¸­çé£æ ¼å¼åãä¸ä¼å¯¹å¼åèé æè¿å¤çè¿ç§»ææ¬ã 3.
 ä»£ç æµè¯è¦ççæç¹ä½ï¼èèå¢å åï¼
 ä¸èèï¼åºæ¯æä¾èµæå¡å¤ªå¤ï¼ä¸äºæå¡ç­å¶å®å ç´ å¯¼è´ä¸ªäººç»´æ¤ææ¬è¿é«ï¼ä½ä¸å¿æå¿ï¼æä¼åæ¬å°æå¡çèªå¨åæµè¯ç»åä½¿ç¨ã
-4. å¦æä½ æ³å¯¹æ­¤é¡¹ç®ååºè´¡ç®ï¼è¯·åè[pull request ç¤ºä¾](https:
-//ayugespidertools.readthedocs.io/en/latest/additional/contribute.html)ã ##
-æå»ºä½ çä¸å±åº > å·ä½åå®¹è¯·ä»¥ [poetry å®æ¹ææ¡£](https://
-python-poetry.org/docs/) ä¸ºåã æ®[ä½ å¯è½å¨æçäº]
-(#ä½ å¯è½å¨æçäº)å¯ç¥ï¼ä½ å¯ä»¥ `clone`
+4. å¦æä½ æ³å¯¹æ­¤é¡¹ç®ååºè´¡ç®ï¼è¯·åè [pull request ç¤ºä¾]
+(https://ayugespidertools.readthedocs.io/en/latest/additional/
+contribute.html)ã ## æå»ºä½ çä¸å±åº > å·ä½åå®¹è¯·ä»¥ [poetry
+å®æ¹ææ¡£](https://python-poetry.org/docs/) ä¸ºåã æ®
+[ä½ å¯è½å¨æçäº](#ä½ å¯è½å¨æçäº)å¯ç¥ï¼ä½ å¯ä»¥ `clone`
 æºç åï¼ä¿®æ¹ä»»ææ¹æ³ï¼æ¯å¦ä½ çé¡¹ç®åºæ¯ä¸å¯è½éè¦å¶å®çæ¥å¿éç½®é»è®¤å¼ï¼ææ·»å å¶å®çé¡¹ç®ç»ææ¨¡æ¿ç­ï¼ï¼ä¿®æ¹å®æå
 `poetry build` æ `make build` å³å¯æåä½¿ç¨ã
 æ¯å¦ä½ å¯è½éè¦æ´æ°ä¾èµåºä¸­ `kafka-python` ä¸ºæ°çæ¬
 `x.x.x`ï¼é£åªé `poetry install` å®è£ç°æä¾èµåï¼å `poetry add
 kafka-python==x.x.x` å®è£ç®æ çæ¬ï¼å°½éä¸è¦ä½¿ç¨ `poetry update
 kafka-python` ï¼ï¼ç¡®å®æµè¯æ­£å¸¸äºå³å¯ `poetry build` æåä½¿ç¨ã
 **å¸ææ­¤é¡¹ç®è½å¨ä½ éå°æ©å± scrapy
@@ -156,24 +157,24 @@
 ç¨æ·åºæ¯ä¸éè¦çæ°æ®åºåæ°æ®è¡¨åå­æ®µæ ¼å¼ï¼è¿æå­æ®µæ³¨é
 - [x] `MongoDB` å­å¨åºæ¯éé - [x] `PostgreSQL` å­å¨åºæ¯éé - [x]
 `ElasticSearch` å­å¨åºæ¯éé - [x] `Oracle` å­å¨åºæ¯éé - [x]
 `oss` ä¸ä¼ åºæ¯éé - [x] `asyncio` è¯­æ³æ¯æä¸ `async`
 ç¬¬ä¸æ¹åºæ¯æç¤ºä¾ - [x] `spider` ä¸­ä½¿ç¨ `asyncio` ç `aiohttp`
 ç¤ºä¾ - [x] `pipeline` ä¸­ä½¿ç¨ `asyncio` ç `aioMysql` ç¤ºä¾ - [x] éæ
 `Kafka`ï¼`RabbitMQ` ç­æ°æ®æ¨éåè½ - [x] å¸¸ç¨å¼ååºæ¯ - [x] `sql`
-è¯­å¥æ¼æ¥ï¼åªç¨äºç®ååºæ¯ãå·²ç»åºä¼åæ¹åï¼åèåºç­ä¿¡æ¯ã
-- [x]
+è¯­å¥æ¼æ¥ï¼åªç¨äºç®ååºæ¯ã - [x]
 æ°æ®æ ¼å¼åå¤çï¼æ¯å¦ï¼å»é¤ç½é¡µæ ç­¾ï¼å»é¤æ æç©ºæ ¼ç­ -
 [x] å­ä½åç¬è¿åæ¹æ³ - [x] åºäº `ttf`ï¼`woff`
 ä¹ç±»çå­ä½æä»¶æ å°ï¼æç»å `css` ç­å®ç° - [x]
 å¯ä»¥ç´æ¥å¨å­ä½æä»¶ `xml` ä¸­æ¾å°æ å°å³ç³»çï¼ä½¿ç¨ [fontforge]
 (https://github.com/fontforge/fontforge/releases) å·¥å·å¯¼åºæ å°å³å¯ã -
 [x] æ æ³æ¾å°æ å°å³ç³»çï¼åä¸è¬ä½¿ç¨ `ocr`
 è¯å«ï¼åç¡®çéç¾åç¾ï¼ï¼éè¿ `fontforge` å¯¼åºæ¯ä¸ªæ å°ç
-`png` ï¼ååéè¿åç§æ¹å¼è¯å«ã - [x] `html`
+`png` ï¼ååéè¿åç§æ¹å¼è¯å«ã - [x]
+å­ä½åç¬é¨ååè½è¿ç§»å° `FontMapster` é¡¹ç®ä¸­ã - [x] `html`
 æ°æ®å¤çï¼å»é¤æ ç­¾ï¼ä¸å¯è§å­ç¬¦ï¼ç¹æ®å­ç¬¦æ¹ææ­£å¸¸æ¾ç¤ºç­
 - [x] æ·»å å¸¸ç¨çå¾çéªè¯ç ä¸­çå¤çæ¹æ³ - [x]
 æ»åç¼ºå£è·ç¦»çè¯å«æ¹æ³ï¼å¤ç§å®ç°æ¹å¼ï¼ - [x]
 æ ¹æ®æ»åè·ç¦»çæè½¨è¿¹æ°ç»çæ¹æ³ - [x]
 è¯å«ç¹ééªè¯ç ä½ç½®åç¹å»é¡ºåº - [x]
 å¾çä¹±åºæ··æ·çè¿åæ¹æ³ç¤ºä¾ æ³¨æï¼åè½æ¼ç¤ºæå°æ¾å¥
 [readthedocs](https://ayugespidertools.readthedocs.io/en/latest/
```

