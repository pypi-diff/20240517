# Comparing `tmp/memodules-5.9.2.tar.gz` & `tmp/memodules-5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memodules-5.9.2.tar", last modified: Fri Apr 12 05:32:14 2024, max compression
+gzip compressed data, was "memodules-5.9.3.tar", last modified: Fri Apr 12 05:40:29 2024, max compression
```

## Comparing `memodules-5.9.2.tar` & `memodules-5.9.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.688200 memodules-5.9.2/
--rw-rw-rw-   0        0        0      449 2024-04-12 05:32:14.686207 memodules-5.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.523060 memodules-5.9.2/memodules/
--rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.9.2/memodules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.541606 memodules-5.9.2/memodules/alphabet_to_integer/
--rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.9.2/memodules/alphabet_to_integer/AlphabetToInteger.py
--rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.9.2/memodules/alphabet_to_integer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.544599 memodules-5.9.2/memodules/builtins/
--rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.9.2/memodules/builtins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.551543 memodules-5.9.2/memodules/builtins/tkinter/
--rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.9.2/memodules/builtins/tkinter/Event.py
--rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.9.2/memodules/builtins/tkinter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.558447 memodules-5.9.2/memodules/builtins/tkinter/ttk/
--rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.9.2/memodules/builtins/tkinter/ttk/Event.py
--rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.9.2/memodules/builtins/tkinter/ttk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.564857 memodules-5.9.2/memodules/cr_exchange_lib/
--rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.9.2/memodules/cr_exchange_lib/__init__.py
--rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.9.2/memodules/cr_exchange_lib/crExchangeLib.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.570913 memodules-5.9.2/memodules/cslapp/
--rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.9.2/memodules/cslapp/__init__.py
--rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.9.2/memodules/cslapp/calc_source.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.577528 memodules-5.9.2/memodules/debug_tools/
--rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.9.2/memodules/debug_tools/__init__.py
--rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.9.2/memodules/debug_tools/access_viewer.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.589202 memodules-5.9.2/memodules/decorators/
--rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.9.2/memodules/decorators/PushHF.py
--rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.9.2/memodules/decorators/__init__.py
--rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.9.2/memodules/decorators/debug_dec.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.596179 memodules-5.9.2/memodules/directory/
--rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.9.2/memodules/directory/__init__.py
--rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.9.2/memodules/directory/structure.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.601571 memodules-5.9.2/memodules/e_typing/
--rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.9.2/memodules/e_typing/__init__.py
--rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.9.2/memodules/e_typing/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.608639 memodules-5.9.2/memodules/error_lib/
--rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.9.2/memodules/error_lib/ErrorLib.py
--rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.9.2/memodules/error_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.617296 memodules-5.9.2/memodules/importer/
--rw-rw-rw-   0        0        0      249 2024-04-11 05:41:26.000000 memodules-5.9.2/memodules/importer/__init__.py
--rw-rw-rw-   0        0        0      249 2024-04-11 05:33:20.000000 memodules-5.9.2/memodules/importer/__init__.pyi
--rw-rw-rw-   0        0        0     1418 2024-04-11 06:03:35.000000 memodules-5.9.2/memodules/importer/sqlalchemy.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.628925 memodules-5.9.2/memodules/inicon/
--rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.9.2/memodules/inicon/__init__.py
--rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.9.2/memodules/inicon/inicon.py
--rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.9.2/memodules/inicon/inicon.pyi
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.631915 memodules-5.9.2/memodules/judgment/
--rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.9.2/memodules/judgment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.659453 memodules-5.9.2/memodules/log/
--rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.9.2/memodules/log/Dlog.py
--rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.9.2/memodules/log/Dlog.pyi
--rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.9.2/memodules/log/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.9.2/memodules/log/cprint.py
--rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.9.2/memodules/log/cprint.pyi
--rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.9.2/memodules/log/log.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.670046 memodules-5.9.2/memodules/sandbox/
--rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.9.2/memodules/sandbox/__init__.py
--rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.9.2/memodules/sandbox/sqlalchemy.py
--rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.9.2/memodules/sandbox/sqlalchemy.pyi
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.674069 memodules-5.9.2/memodules/sql_pack/
--rw-rw-rw-   0        0        0     1987 2024-04-12 05:29:16.000000 memodules-5.9.2/memodules/sql_pack/__init__.py
--rw-rw-rw-   0        0        0     2053 2024-04-12 05:31:31.000000 memodules-5.9.2/memodules/sql_pack/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.683217 memodules-5.9.2/memodules/xl_for_python/
--rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.9.2/memodules/xl_for_python/Python_xlTypeLib_Addin.py
--rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.9.2/memodules/xl_for_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:32:14.533332 memodules-5.9.2/memodules.egg-info/
--rw-rw-rw-   0        0        0      449 2024-04-12 05:32:14.000000 memodules-5.9.2/memodules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1545 2024-04-12 05:32:14.000000 memodules-5.9.2/memodules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 05:32:14.000000 memodules-5.9.2/memodules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 05:32:14.000000 memodules-5.9.2/memodules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 05:32:14.688200 memodules-5.9.2/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-04-12 05:32:09.000000 memodules-5.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.310299 memodules-5.9.3/
+-rw-rw-rw-   0        0        0      449 2024-04-12 05:40:29.308320 memodules-5.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.139967 memodules-5.9.3/memodules/
+-rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.9.3/memodules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.156910 memodules-5.9.3/memodules/alphabet_to_integer/
+-rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.9.3/memodules/alphabet_to_integer/AlphabetToInteger.py
+-rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.9.3/memodules/alphabet_to_integer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.159900 memodules-5.9.3/memodules/builtins/
+-rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.9.3/memodules/builtins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.166877 memodules-5.9.3/memodules/builtins/tkinter/
+-rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.9.3/memodules/builtins/tkinter/Event.py
+-rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.9.3/memodules/builtins/tkinter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.173853 memodules-5.9.3/memodules/builtins/tkinter/ttk/
+-rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.9.3/memodules/builtins/tkinter/ttk/Event.py
+-rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.9.3/memodules/builtins/tkinter/ttk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.180830 memodules-5.9.3/memodules/cr_exchange_lib/
+-rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.9.3/memodules/cr_exchange_lib/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.9.3/memodules/cr_exchange_lib/crExchangeLib.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.185813 memodules-5.9.3/memodules/cslapp/
+-rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.9.3/memodules/cslapp/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.9.3/memodules/cslapp/calc_source.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.192790 memodules-5.9.3/memodules/debug_tools/
+-rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.9.3/memodules/debug_tools/__init__.py
+-rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.9.3/memodules/debug_tools/access_viewer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.202757 memodules-5.9.3/memodules/decorators/
+-rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.9.3/memodules/decorators/PushHF.py
+-rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.9.3/memodules/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.9.3/memodules/decorators/debug_dec.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.208737 memodules-5.9.3/memodules/directory/
+-rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.9.3/memodules/directory/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.9.3/memodules/directory/structure.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.223459 memodules-5.9.3/memodules/e_typing/
+-rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.9.3/memodules/e_typing/__init__.py
+-rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.9.3/memodules/e_typing/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.230166 memodules-5.9.3/memodules/error_lib/
+-rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.9.3/memodules/error_lib/ErrorLib.py
+-rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.9.3/memodules/error_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.238539 memodules-5.9.3/memodules/importer/
+-rw-rw-rw-   0        0        0      249 2024-04-11 05:41:26.000000 memodules-5.9.3/memodules/importer/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-04-11 05:33:20.000000 memodules-5.9.3/memodules/importer/__init__.pyi
+-rw-rw-rw-   0        0        0     1418 2024-04-11 06:03:35.000000 memodules-5.9.3/memodules/importer/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.251496 memodules-5.9.3/memodules/inicon/
+-rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.9.3/memodules/inicon/__init__.py
+-rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.9.3/memodules/inicon/inicon.py
+-rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.9.3/memodules/inicon/inicon.pyi
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.255482 memodules-5.9.3/memodules/judgment/
+-rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.9.3/memodules/judgment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.283396 memodules-5.9.3/memodules/log/
+-rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.9.3/memodules/log/Dlog.py
+-rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.9.3/memodules/log/Dlog.pyi
+-rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.9.3/memodules/log/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.9.3/memodules/log/cprint.py
+-rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.9.3/memodules/log/cprint.pyi
+-rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.9.3/memodules/log/log.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.292359 memodules-5.9.3/memodules/sandbox/
+-rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.9.3/memodules/sandbox/__init__.py
+-rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.9.3/memodules/sandbox/sqlalchemy.py
+-rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.9.3/memodules/sandbox/sqlalchemy.pyi
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.297342 memodules-5.9.3/memodules/sql_pack/
+-rw-rw-rw-   0        0        0     2025 2024-04-12 05:38:30.000000 memodules-5.9.3/memodules/sql_pack/__init__.py
+-rw-rw-rw-   0        0        0     2075 2024-04-12 05:40:21.000000 memodules-5.9.3/memodules/sql_pack/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.306312 memodules-5.9.3/memodules/xl_for_python/
+-rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.9.3/memodules/xl_for_python/Python_xlTypeLib_Addin.py
+-rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.9.3/memodules/xl_for_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:40:29.149933 memodules-5.9.3/memodules.egg-info/
+-rw-rw-rw-   0        0        0      449 2024-04-12 05:40:28.000000 memodules-5.9.3/memodules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2024-04-12 05:40:29.000000 memodules-5.9.3/memodules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 05:40:28.000000 memodules-5.9.3/memodules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 05:40:28.000000 memodules-5.9.3/memodules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 05:40:29.310299 memodules-5.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-12 05:37:29.000000 memodules-5.9.3/setup.py
```

### Comparing `memodules-5.9.2/memodules/alphabet_to_integer/AlphabetToInteger.py` & `memodules-5.9.3/memodules/alphabet_to_integer/AlphabetToInteger.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/builtins/tkinter/Event.py` & `memodules-5.9.3/memodules/builtins/tkinter/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/builtins/tkinter/ttk/Event.py` & `memodules-5.9.3/memodules/builtins/tkinter/ttk/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/cr_exchange_lib/crExchangeLib.py` & `memodules-5.9.3/memodules/cr_exchange_lib/crExchangeLib.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/cslapp/calc_source.py` & `memodules-5.9.3/memodules/cslapp/calc_source.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/debug_tools/access_viewer.py` & `memodules-5.9.3/memodules/debug_tools/access_viewer.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/decorators/debug_dec.py` & `memodules-5.9.3/memodules/decorators/debug_dec.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/e_typing/__init__.py` & `memodules-5.9.3/memodules/e_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/e_typing/__init__.pyi` & `memodules-5.9.3/memodules/e_typing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/importer/sqlalchemy.py` & `memodules-5.9.3/memodules/importer/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/inicon/inicon.py` & `memodules-5.9.3/memodules/inicon/inicon.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/inicon/inicon.pyi` & `memodules-5.9.3/memodules/inicon/inicon.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/log/Dlog.py` & `memodules-5.9.3/memodules/log/Dlog.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/log/Dlog.pyi` & `memodules-5.9.3/memodules/log/Dlog.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/log/cprint.py` & `memodules-5.9.3/memodules/log/cprint.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/log/cprint.pyi` & `memodules-5.9.3/memodules/log/cprint.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/log/log.py` & `memodules-5.9.3/memodules/log/log.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/sandbox/sqlalchemy.py` & `memodules-5.9.3/memodules/sandbox/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/sandbox/sqlalchemy.pyi` & `memodules-5.9.3/memodules/sandbox/sqlalchemy.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules/sql_pack/__init__.py` & `memodules-5.9.3/memodules/sql_pack/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,25 +31,26 @@
             result[table_name].append(row)
             if print_to_console: print(row)
     return result
 
 
 def query_gen(session: _Session, table: DeclarativeMeta | None = None,
               *filters: ColumnElement[bool] | BinaryExpression[bool],
-              delete: bool = False):
+              delete=False, commit=False):
     if not delete:
         it = ...
         if filters:
            it = session.query(table).filter(*filters).all
         else:
            it = session.query(table).all
         for item in it():
             yield item
     else:
         def _f():
             result = session.query(table).filter(*filters).first() if filters else session.query(table).first()
             if result:
                 session.delete(result)
-                session.commit()
+                if commit:
+                    session.commit()
             return result
         for item in iter(_f, None):
             yield item
```

### Comparing `memodules-5.9.2/memodules/sql_pack/__init__.pyi` & `memodules-5.9.3/memodules/sql_pack/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 def query_gen[TYPE](session: _Session,
                     table: (EntityType[TYPE]
                             | TypedColumnsClauseRole[TYPE]
                             | TypedColumnClauseArgument[TYPE]
                             | ColumnsClauseArgument[TYPE]
                             | None) = None,
                     *filters: ColumnElement[bool] | BinaryExpression[bool],
-                    delete: bool = False) -> Generator[TYPE, None, None]: ...
+                    delete: bool = False, commit: bool = False) -> Generator[TYPE, None, None]: ...
```

### Comparing `memodules-5.9.2/memodules/xl_for_python/Python_xlTypeLib_Addin.py` & `memodules-5.9.3/memodules/xl_for_python/Python_xlTypeLib_Addin.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/memodules.egg-info/SOURCES.txt` & `memodules-5.9.3/memodules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memodules-5.9.2/setup.py` & `memodules-5.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='memodules',
-    version='5.9.2',
+    version='5.9.3',
     author='mie31',
     author_email='mie.mey.master@icloud.com',
     description='local use functions',
     long_description="We do not consider the use of it by third parties.",
     long_description_content_type="text/plain",
     license="MIT",
     keywords='No redistribution!',
```

