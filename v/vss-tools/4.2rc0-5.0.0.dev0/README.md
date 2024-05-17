# Comparing `tmp/vss_tools-4.2rc0.tar.gz` & `tmp/vss_tools-5.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss_tools-4.2rc0.tar", last modified: Fri May 17 13:39:18 2024, max compression
+gzip compressed data, was "vss_tools-5.0.0.dev0.tar", last modified: Thu May  2 13:25:05 2024, max compression
```

## Comparing `vss_tools-4.2rc0.tar` & `vss_tools-5.0.0.dev0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.318427 vss_tools-4.2rc0/
--rw-r--r--   0 erik      (1000) erik      (1000)    16725 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       23 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     2193 2024-05-17 13:39:18.314427 vss_tools-4.2rc0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1797 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/README-PYPI.md
--rw-r--r--   0 erik      (1000) erik      (1000)    13468 2024-05-17 12:51:07.000000 vss_tools-4.2rc0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      252 2024-05-17 12:41:35.000000 vss_tools-4.2rc0/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-17 13:39:18.318427 vss_tools-4.2rc0/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1886 2024-05-17 12:43:41.000000 vss_tools-4.2rc0/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.294427 vss_tools-4.2rc0/vspec/
--rwxr-xr-x   0 erik      (1000) erik      (1000)    37917 2024-05-03 13:37:04.000000 vss_tools-4.2rc0/vspec/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      497 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/loggingconfig.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.298427 vss_tools-4.2rc0/vspec/model/
--rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/model/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    10159 2024-05-17 12:40:57.000000 vss_tools-4.2rc0/vspec/model/constants.py
--rw-r--r--   0 erik      (1000) erik      (1000)      844 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/model/exceptions.py
--rw-r--r--   0 erik      (1000) erik      (1000)    21622 2024-05-17 13:27:55.000000 vss_tools-4.2rc0/vspec/model/vsstree.py
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/py.typed
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.302427 vss_tools-4.2rc0/vspec/utils/
--rw-r--r--   0 erik      (1000) erik      (1000)      850 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/utils/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2799 2024-05-03 12:21:08.000000 vss_tools-4.2rc0/vspec/utils/idgen_utils.py
--rw-r--r--   0 erik      (1000) erik      (1000)      774 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/utils/stringstyle.py
--rw-r--r--   0 erik      (1000) erik      (1000)     7064 2024-05-03 12:21:08.000000 vss_tools-4.2rc0/vspec/utils/vss2id_val.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2163 2024-05-03 13:36:36.000000 vss_tools-4.2rc0/vspec/vspec2vss_config.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    10173 2024-05-17 12:41:35.000000 vss_tools-4.2rc0/vspec/vspec2x.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1346 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vss2x.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.306427 vss_tools-4.2rc0/vspec/vssexporters/
--rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-4.2rc0/vspec/vssexporters/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5057 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2binary.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3424 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2csv.py
--rw-r--r--   0 erik      (1000) erik      (1000)    12374 2024-05-03 13:36:36.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2ddsidl.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3232 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2franca.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5418 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2graphql.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6719 2024-05-17 13:06:58.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2id.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4409 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2json.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6110 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2jsonschema.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     8219 2024-05-17 12:51:07.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2protobuf.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4293 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec/vssexporters/vss2yaml.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      684 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2csv.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      711 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2ddsidl.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      714 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2franca.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      723 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2graphql.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      677 2024-05-03 12:21:19.000000 vss_tools-4.2rc0/vspec2id.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      726 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2jsonschema.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      730 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2protobuf.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-05-03 13:22:47.000000 vss_tools-4.2rc0/vspec2yaml.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-17 13:39:18.314427 vss_tools-4.2rc0/vss_tools.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2193 2024-05-17 13:39:18.000000 vss_tools-4.2rc0/vss_tools.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1045 2024-05-17 13:39:18.000000 vss_tools-4.2rc0/vss_tools.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-17 13:39:18.000000 vss_tools-4.2rc0/vss_tools.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       59 2024-05-17 13:39:18.000000 vss_tools-4.2rc0/vss_tools.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        6 2024-05-17 13:39:18.000000 vss_tools-4.2rc0/vss_tools.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/
+-rw-r--r--   0 erik      (1000) erik      (1000)    16725 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       23 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     2197 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1797 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/README-PYPI.md
+-rw-r--r--   0 erik      (1000) erik      (1000)    13319 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      253 2024-04-30 07:46:11.000000 vss_tools-5.0.0.dev0/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1886 2024-05-02 12:01:50.000000 vss_tools-5.0.0.dev0/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    37003 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      497 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/loggingconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/model/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/model/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9629 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/model/constants.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      844 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/model/exceptions.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    21714 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/model/vsstree.py
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/py.typed
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/utils/
+-rw-r--r--   0 erik      (1000) erik      (1000)      850 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2799 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/idgen_utils.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      774 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/stringstyle.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     7064 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/vss2id_val.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2163 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vspec2vss_config.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    10076 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vspec2x.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1346 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vss2x.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/vssexporters/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5057 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2binary.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3424 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2csv.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12374 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2ddsidl.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3232 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2franca.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5418 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2graphql.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6184 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2id.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4409 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2json.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6110 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     6644 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2protobuf.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4293 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2yaml.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      684 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2csv.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      711 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2ddsidl.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      714 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2franca.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      723 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2graphql.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      677 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec2id.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2json.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      726 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      730 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2protobuf.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2yaml.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vss_tools.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2197 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1045 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       59 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        6 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/top_level.txt
```

### Comparing `vss_tools-4.2rc0/LICENSE` & `vss_tools-5.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/PKG-INFO` & `vss_tools-5.0.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vss-tools
-Version: 4.2rc0
+Version: 5.0.0.dev0
 Summary: COVESA Vehicle Signal Specification tooling.
 Home-page: https://github.com/COVESA/vss-tools
 License: Mozilla Public License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml>=5.1
```

### Comparing `vss_tools-4.2rc0/README-PYPI.md` & `vss_tools-5.0.0.dev0/README-PYPI.md`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/README.md` & `vss_tools-5.0.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [vspec2ddsidl.py](vspec2ddsidl.py) | Generating DDS-IDL output | Community Supported   | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2json.py](vspec2json.py) |  Generating JSON output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
 [vspec2yaml.py](vspec2yaml.py) | Generating flattened YAML output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
 [vspec2binary.py](vspec2binary.py) | The binary toolset consists of a tool that translates the VSS YAML specification to the binary file format (see below), and two libraries that provides methods that are likely to be needed by a server that manages the VSS tree, one written in C, and one in Go | Community Supported   | [vspec2binary Documentation](binary/README.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2franca.py](vspec2franca.py) | Parses and expands a VSS and generates a Franca IDL specification | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
 [vspec2c.py](obsolete/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md)                                                                           |
 [vspec2ocf.py](obsolete/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | -                                                                                                                     |
-[vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS tree and generates a Protobuf message definition | Contrib               | [Documentation](docs/vspec2proto.md)                                                                                                                     |
+[vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS and generates a Protobuf specification | Contrib               | -                                                                                                                     |
 [vspec2ttl.py](contrib/vspec2ttl/vspec2ttl.py) | Parses and expands a VSS and generates a TTL specification | Contrib               | -                                                                                                                     |
 [vspec2graphql.py](vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported   | [Documentation](docs/VSS2GRAPHQL.md)                                                                                  |
 [vspec2id.py](vspec2id.py) | Generates and validates static UIDs for a VSS | WIP                   | [vspec2id Documentation](./docs/vspec2id.md)                                                                          |
 
 ## Tool Architecture
 
 All current tools are based on common Python functionality in the `vspec` folder to read, parse and expand a Vehicle Signal Specification files(*.vspec files). As an example, if the standard [VSS root file](https://github.com/COVESA/vehicle_signal_specification/blob/master/spec/VehicleSignalSpecification.vspec) is given as input then the Python tooling will read all included files, do a validation of the content, expand any instances used and create an in-memory representation which then can be used by specialized tools to generate the wanted output.
@@ -70,15 +70,14 @@
 ## Getting started
 
 ## Prerequisites
 
 * If your environment behind a (corporate) proxy, the following environments variables must typically be set: `http_proxy` and `https_proxy` (including authentication e.g., `http://${proxy_username):$(proxy_password)@yourproxy.yourdomain`).
 * If using `apt` and you are behind a proxy, you may also need to configure proxy in `/etc/apt/apt.conf.d/proxy.conf`.
 
-
 ## Environment and Python Version
 
 This repository use the Github `ubuntu-latest` [runner-image](https://github.com/actions/runner-images) for continuous nntegration.
 The Python version used is typically the [default version](https://packages.ubuntu.com/search?keywords=python3) for that Ubuntu release,
 currently Python `3.10.6`.
 Other environments and Python versions may be supported, but are not tested as part of continuous integration or relase testing.
 
@@ -90,16 +89,15 @@
 
 The setup example shown below is based on a fresh minimal install of Ubuntu 22.04.
 
 The first step is to make sure that pyenv and the wanted Python version (in the example 3.10.6) is installed
 
 ```sh
 # Install dependencies, to be able to use curl and build python from source
-sudo apt update
-sudo apt install make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
+sudo apt-get install make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
 
 # Fetch and install pyenv and update variables
 curl https://pyenv.run | bash
 export PYENV_ROOT="$HOME/.pyenv"
 command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
 eval "$(pyenv init -)"
 
@@ -107,28 +105,28 @@
 pyenv install 3.10.6
 ```
 
 Install this project and its dependencies in the local `.venv` folder in this project, then use it (`pipenv shell`):
 
 ```sh
 export PIPENV_VENV_IN_PROJECT=1 # will create a local `.venv` in the project, otherwise uses global location
-sudo apt update && sudo apt install pipenv
+pip install pipenv
 export PATH=/home/${USER}/.local/bin:${PATH}
 pipenv install --dev # install the development dependencies as well
 ```
 
 Then the virtual environment can be started and tested using (`pipenv shell`):
 
 ```sh
 user@ubuntu:~/vss-tools$ pipenv shell
 Launching subshell in virtual environment...
 user@ubuntu:~/vss-tools$  . /home/user/vss-tools/.venv/bin/activate
 (vss-tools) user@ubuntu:~/vss-tools$ ./vspec2yaml.py
 usage: vspec2yaml.py [-h] [-I dir] [-e EXTENDED_ATTRIBUTES] [-s] [--abort-on-unknown-attribute] [--abort-on-name-style] [--format format] [--uuid]
-                     [--no-uuid]  [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
+                     [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
                      [-v version] [--all-idl-features] [--gqlfield GQLFIELD GQLFIELD]
                      <vspec_file> <output_file>
 vspec2yaml.py: error: the following arguments are required: <vspec_file>, <output_file>
 ```
 
 ## Native Setup
 
@@ -136,15 +134,14 @@
 The setup example shown below is based on a fresh minimal install of Ubuntu 22.04.
 
 The first step is to make sure that python and required dependencies are installed. A possible installation flow is shown below.
 
 
 ```sh
 # Install Python, in this case Python 3.10 as that is a version available on the update sites of Ununtu 22.04
-sudo apt update
 sudo apt install python3.10
 
 # For convenience make Python 3.10 available as default Python
 sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.10 100
 
 # Install required dependencies, running pip without sudo means that a user installation will be performed
 sudo apt install pip
@@ -152,28 +149,27 @@
 ```
 
 The environment can be tested by calling one of the tools without arguments, then usage instructions shall be printed similar to below.
 
 ```sh
 user@ubuntu:~/vss-tools$ ./vspec2csv.py
 usage: vspec2csv.py [-h] [-I dir] [-e EXTENDED_ATTRIBUTES] [-s] [--abort-on-unknown-attribute] [--abort-on-name-style] [--format format] [--uuid]
-                    [--no-uuid] [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
+                    [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
                     [-v version] [--all-idl-features] [--gqlfield GQLFIELD GQLFIELD]
                     <vspec_file> <output_file>
 vspec2csv.py: error: the following arguments are required: <vspec_file>, <output_file>
 
 ```
 
 ## Installing additional tools
 
 If you intend to run testcases related to `vspec2protobuf.py` you need to install the protobuf compiler
 
 ```sh
-sudo apt update
-sudo apt install -y golang-go protobuf-compiler
+sudo apt install -y protobuf-compiler
 protoc --version  # Ensure compiler version is 3+
 ```
 
 ## Pre-commit set up
 This repository is set up to use pre-commit hooks. After you clone the project, run `pre-commit install` to install pre-commit into your git hooks. pre-commit will now run on every commit. Every time you clone a project using pre-commit running pre-commit install should always be the first thing you do.
 
 ## Building and installing with Pip
```

### Comparing `vss_tools-4.2rc0/setup.py` & `vss_tools-5.0.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/__init__.py` & `vss_tools-5.0.0.dev0/vspec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -457,31 +457,16 @@
                 if expand_node.name == existing_item.name:
                     # A child with the same name already exists
                     # Typical use-case is that a single instance of this signal has been re-defined in an overlay
                     # Then data from the overlay (for example A.B.Row2.Column2.Sig)
                     # shall have precedence over the expanded instance
                     # This is handled by removing the old node from tree and
                     # instead merging it to the new node
+                    existing_item.parent = None
                     expand_node.merge(existing_item)
-                    # Also make sure that any children already existing are moved or merged to the new tree
-
-                    def merge_children(target_node, input_node):
-                        for existing_child in input_node.children:
-                            found = False
-                            for expanded_child in target_node.children:
-                                if expanded_child.name == existing_child.name:
-                                    expanded_child.merge(existing_child)
-                                    merge_children(expanded_child, existing_child)
-                                    found = True
-                            if not found:
-                                # Totally new node/branch, no need to continue deeper, just take it
-                                existing_child.parent = target_node
-                        input_node.parent = None
-
-                    merge_children(expand_node, existing_item)
                     break
             expand_node.parent = instantiated_branch
         return instantiated_branch
 
     # Checking each node for instances and expand them
     # The walking order makes sure, we do not need to recurse
     for tree_node in PreOrderIter(tree):
@@ -846,29 +831,29 @@
                 new_element,
                 break_on_name_style_violation=break_on_name_style_violation)
 
 
 def merge_elem(base, overlay_element):
     r = Resolver()
     element_name = "/" + overlay_element.qualified_name("/")
+
     if not VSSNode.node_exists(base, element_name):
         # The node in the overlay does not exist, so we connect it
         # print(f"Not exists {overlay_element.qualified_name()} does not exist, creating.")
         new_parent_name = "/" + overlay_element.parent.qualified_name("/")
         new_parent = r.get(base, new_parent_name)
         overlay_element.parent = new_parent
 
     else:
         # else we merge the node. The merge function of VSSNode is not recursive
         # so children in base will not be overwritten
         # print(f"Merging {overlay_element.qualified_name()}")
         other_node: VSSNode = r.get(base, element_name)
         try:
             other_node.merge(overlay_element)
-
         except ImpossibleMergeException as e:
             logging.error(f"Merging impossible: {e}")
             sys.exit(-1)
 
 
 def merge_tree(base: VSSNode, overlay: VSSNode):
     overlay_element: VSSNode
```

### Comparing `vss_tools-4.2rc0/vspec/model/constants.py` & `vss_tools-5.0.0.dev0/vspec/model/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 # SPDX-License-Identifier: MPL-2.0
 
 #
 # Constant Types and Mappings
 #
 # noinspection PyPackageRequirements
 from __future__ import annotations
-import re
 import logging
+import re
 import sys
 from collections import abc
 from collections.abc import Sequence
 from enum import Enum, EnumMeta
 from typing import TextIO, TypeVar
 
 import yaml
 
 NON_ALPHANUMERIC_WORD = re.compile("[^A-Za-z0-9]+")
 
-NON_ALPHANUMERIC_WORD = re.compile('[^A-Za-z0-9]+')
-
 T = TypeVar("T")
 
 
 class VSSUnit(str):
     """String subclass for storing unit information."""
 
     id: str  # Typically abbreviation like "V"
@@ -104,31 +102,14 @@
     def from_str(cls: type[T], value: str) -> T:
         return cls.__reverse_lookup__[value]  # type: ignore[attr-defined]
 
     def values(cls: type[T]) -> Sequence[str]:
         return cls.__values__  # type: ignore[attr-defined]
 
 
-class StringStyle(Enum, metaclass=EnumMetaWithReverseLookup):
-    NONE = "none"
-    CAMEL_CASE = "camelCase"
-    CAMEL_BACK = "camelBack"
-    CAPITAL_CASE = "capitalcase"
-    CONST_CASE = "constcase"
-    LOWER_CASE = "lowercase"
-    PASCAL_CASE = "pascalcase"
-    SENTENCE_CASE = "sentencecase"
-    SNAKE_CASE = "snakecase"
-    SPINAL_CASE = "spinalcase"
-    TITLE_CASE = "titlecase"
-    TRIM_CASE = "trimcase"
-    UPPER_CASE = "uppercase"
-    ALPHANUM_CASE = "alphanumcase"
-
-
 class VSSType(Enum, metaclass=EnumMetaWithReverseLookup):
     BRANCH = "branch"
     ATTRIBUTE = "attribute"
     SENSOR = "sensor"
     ACTUATOR = "actuator"
     STRUCT = "struct"
     PROPERTY = "property"
```

### Comparing `vss_tools-4.2rc0/vspec/model/exceptions.py` & `vss_tools-5.0.0.dev0/vspec/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/model/vsstree.py` & `vss_tools-5.0.0.dev0/vspec/model/vsstree.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         "instances",
         "deprecation",
         "arraysize",
         "comment",
         "$file_name$",
         "fka",
         "delete",
-        "constUID",
     ]
 
     # List of accepted extended attributes. In strict terminate if an attribute is
     # neither in core or extended,
     whitelisted_extended_attributes: List[str] = []
 
     unit: Optional[VSSUnit] = None
@@ -87,15 +86,14 @@
     default = ""
 
     instances = None
     expanded = False
     deprecation = ""
     fka = ""
     delete: bool = False
-    constUID: Optional[str] = None
 
     def __deepcopy__(self, memo):
         # Deep copy of source_dict and children needed as overlay or programmatic changes
         # in exporters otherwise risk changing values not only for current instances but also for others
         return VSSNode(
             self.name,
             copy.deepcopy(self.source_dict),
@@ -147,18 +145,21 @@
                 f"Orphan property detected. {self.name} is not defined under a struct"
             )
             sys.exit(-1)
 
         try:
             self.validate_name_style(self.source_dict["$file_name$"])
         except NameStyleValidationException as e:
-            logging.warning(f"Exception: {e}")
+            info_string = str(e)
             if break_on_name_style_violation:
+                logging.warning(info_string)
                 logging.error("You asked for strict checking. Terminating.")
                 sys.exit(-1)
+            else:
+                logging.info(info_string)
 
     def unpack_source_dict(self):
         self.extended_attributes = self.source_dict.copy()
 
         # Clean special cases
         if "children" in self.extended_attributes:
             del self.extended_attributes["children"]
@@ -234,27 +235,28 @@
     def validate_name_style(self, sourcefile):
         """Checks wether this node is adhering to VSS style conventions.
 
         Throws NameStyleValidationException when deviations are detected. A VSS model violating
         this conventions can still be a valid model.
 
         """
+        camel_regexp = re.compile("[A-Z][A-Za-z0-9]*$")
         if (
             self.is_signal()
             and self.datatype == VSSDataType.BOOLEAN
             and not self.name.startswith("Is")
         ):
             raise NameStyleValidationException(
                 (
                     f'Boolean node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
                     'It is recommended that boolean nodes start with "Is".',
                 )
             )
 
-        camel_regexp = re.compile("[A-Z][A-Za-z0-9]*$")
+        camel_regexp = re.compile('[A-Z][A-Za-z0-9]*$')
         # relax camel case requirement for struct properties
         if not self.is_property() and not camel_regexp.match(self.name):
             raise NameStyleValidationException(
                 (
                     f'Node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
                     "It is recommended that node names use camel case, starting with a capital letter, ",
                     "only using letters A-z and numbers 0-9.",
```

### Comparing `vss_tools-4.2rc0/vspec/utils/__init__.py` & `vss_tools-5.0.0.dev0/vspec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/utils/idgen_utils.py` & `vss_tools-5.0.0.dev0/vspec/utils/idgen_utils.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/utils/stringstyle.py` & `vss_tools-5.0.0.dev0/vspec/utils/stringstyle.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/utils/vss2id_val.py` & `vss_tools-5.0.0.dev0/vspec/utils/vss2id_val.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vspec2vss_config.py` & `vss_tools-5.0.0.dev0/vspec/vspec2vss_config.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vspec2x.py` & `vss_tools-5.0.0.dev0/vspec/vspec2x.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,23 +47,20 @@
         if self.vspec2vss_config.extended_attributes_supported:
             parser.add_argument('-e', '--extended-attributes', type=str, default="",
                                 help='Whitelisted extended attributes as comma separated list.')
         parser.add_argument('-s', '--strict', action='store_true',
                             help='Use strict checking: Terminate when anything not covered or not recommended '
                                  'by VSS language or extensions is found.')
         parser.add_argument('--abort-on-unknown-attribute', action='store_true',
-                            help=" Terminate when an unknown attribute is found.")
+                            help="Terminate when an unknown attribute is found.")
         parser.add_argument('--abort-on-name-style', action='store_true',
-                            help=" Terminate naming style not follows recommendations.")
-        # For 4.X always keep uuid even if not considered fo backward compatibility
-        parser.add_argument('--uuid', action='store_true',
-                            help='Include uuid in generated files.')
-        parser.add_argument('--no-uuid', action='store_true',
-                            help='Exclude uuid in generated files.  This is currently the default behavior. ' +
-                            ' This argument is deprecated and will be removed in VSS 5.0')
+                            help="Terminate if name style does not follow VSS standard catalog naming convention.")
+        if self.vspec2vss_config.uuid_supported:
+            parser.add_argument('--uuid', action='store_true',
+                                help='Include uuid in generated files. (Deprecated, will be removed in VSS-tools 6.0)')
         if self.vspec2vss_config.expand_model and self.vspec2vss_config.no_expand_option_supported:
             parser.add_argument('--no-expand', action='store_true',
                                 help='Do not expand tree.')
         parser.add_argument('-o', '--overlays', action='append', metavar='overlays', type=str, default=[],
                             help='Add overlay that will be layered on top of the VSS file in the order they appear.')
         parser.add_argument('-q', '--quantity-file', action='append', metavar='quantity_file', type=str, default=[],
                             help='Quantity file to be used for generation. Argument -q may be used multiple times.')
@@ -104,30 +101,30 @@
         abort_on_namestyle = False
 
         if args.abort_on_unknown_attribute or args.strict:
             abort_on_unknown_attribute = True
         if args.abort_on_name_style or args.strict:
             abort_on_namestyle = True
 
-        if self.vspec2vss_config.extended_attributes_supported:
+        if self.vspec2vss_config.extended_attributes_supported and (len(args.extended_attributes) > 0):
             known_extended_attributes_list = args.extended_attributes.split(",")
-            if len(known_extended_attributes_list) > 0:
-                vspec.model.vsstree.VSSNode.whitelisted_extended_attributes = known_extended_attributes_list
-                logging.info(f"Known extended attributes: {', '.join(known_extended_attributes_list)}")
+            vspec.model.vsstree.VSSNode.whitelisted_extended_attributes = known_extended_attributes_list
+            logging.info(f"Known extended attributes: {', '.join(known_extended_attributes_list)}")
         else:
             known_extended_attributes_list = list()
 
-        if args.uuid and args.no_uuid:
-            logging.error("Can not use --uuid and --no-uuid at the same time")
-            sys.exit(-1)
-        if args.no_uuid:
-            logging.warning("The argument --no-uuid is deprecated and will be removed in VSS 5.0")
-
         self.vspec2vss_config.generate_uuid = self.vspec2vss_config.uuid_supported and args.uuid
 
+        # Follow up to https://github.com/COVESA/vehicle_signal_specification/pull/721
+        # Deprecate --uuid
+        if self.vspec2vss_config.generate_uuid:
+            logging.warning("The argument --uuid is deprecated and the uuid feature is planned "
+                            "to be removed in VSS-tools 6.0")
+            logging.info("If you need static identifiers consider using the vspec2id tool")
+
         self.vspec2vss_config.expand_model = (self.vspec2vss_config.expand_model and not
                                               (self.vspec2vss_config.no_expand_option_supported and args.no_expand))
 
         vspec.load_quantities(args.vspec_file, args.quantity_file)
         vspec.load_units(args.vspec_file, args.unit_file)
 
         # process data type tree
```

### Comparing `vss_tools-4.2rc0/vspec/vss2x.py` & `vss_tools-5.0.0.dev0/vspec/vss2x.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2binary.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2binary.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2csv.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2csv.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2ddsidl.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2ddsidl.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2franca.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2franca.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2graphql.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2graphql.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2id.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2id.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 
 import yaml
 
 from vspec import load_tree
 from vspec.model.constants import VSSTreeType
 from vspec.model.vsstree import VSSNode
 from vspec.utils import vss2id_val
-from vspec.utils.idgen_utils import (
-    fnv1_32_hash,
-    get_all_keys_values,
-    get_node_identifier_bytes,
-)
+from vspec.utils.idgen_utils import (fnv1_32_hash, get_all_keys_values,
+                                     get_node_identifier_bytes)
 from vspec.vss2x import Vss2X
 from vspec.vspec2vss_config import Vspec2VssConfig
 
 
 def generate_split_id(
     node: VSSNode, id_counter: int, strict_mode: bool
 ) -> Tuple[str, int]:
+
     """Generates static UIDs using 4-byte FNV-1 hash.
 
     @param node: VSSNode that we want to generate a static UID for
     @param id_counter: consecutive numbers counter for amount of nodes
     @param strict_mode: strict mode means case sensitivity for static UID generation
     @return: tuple of hashed string and id counter
     """
@@ -66,56 +64,43 @@
 
     @param yaml_dict: the to be exported dict
     @param node: parent node of the tree
     @param id_counter: counter for amount of ids
     @param strict_mode: strict mode means case sensitivity for static UID generation
     @return: id_counter, id_counter
     """
-
-    node_id: str
-    if not node.constUID:
-        node_id, id_counter = generate_split_id(node, id_counter, strict_mode)
-        node_id = f"0x{node_id}"
-    else:
-        logging.info(
-            f"Using const ID for {node.qualified_name()}. If you didn't mean "
-            "to do that you can remove it in your vspec / overlay."
-        )
-        node_id = node.constUID
-
-    assert node_id.startswith("0x"), f"Node ID has to begin with '0x': {node_id}"
-    assert len(node_id) == 10, f"Invalid node ID: {node_id}"
+    node_id, id_counter = generate_split_id(node, id_counter, strict_mode)
 
     # check for hash duplicates
     for key, value in get_all_keys_values(yaml_dict):
         if not isinstance(value, dict) and key == "staticUID":
-            if node_id == value:
+            if node_id == value[2:]:
                 logging.fatal(
                     f"There is a small chance that the result of FNV-1 "
                     f"hashes are the same in this case the hash of node "
                     f"'{node.qualified_name()}' is the same as another hash."
                     f"Can you please update it."
                 )
                 # We could add handling of duplicates here
                 sys.exit(-1)
 
     node_path = node.qualified_name()
 
-    yaml_dict[node_path] = {"staticUID": f"{node_id}"}
+    yaml_dict[node_path] = {"staticUID": f"0x{node_id}"}
     yaml_dict[node_path]["description"] = node.description
     yaml_dict[node_path]["type"] = str(node.type.value)
     if node.unit:
         yaml_dict[node_path]["unit"] = str(node.unit.value)
     if node.is_signal() or node.is_property():
         yaml_dict[node_path]["datatype"] = node.data_type_str
     if node.allowed:
         yaml_dict[node_path]["allowed"] = node.allowed
-    if isinstance(node.min, (int, float)):
+    if node.min:
         yaml_dict[node_path]["min"] = node.min
-    if isinstance(node.max, (int, float)):
+    if node.max:
         yaml_dict[node_path]["max"] = node.max
 
     if node.fka:
         yaml_dict[node_path]["fka"] = node.fka
     elif "fka" in node.extended_attributes.keys():
         yaml_dict[node_path]["fka"] = node.extended_attributes["fka"]
 
@@ -132,38 +117,31 @@
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         """Adds command line arguments to a pre-existing argument parser
 
         @param parser: the pre-existing argument parser
         """
         parser.add_argument(
-            "--validate-static-uid",
-            type=str,
-            default="",
-            help="Path to validation file.",
+            "--validate-static-uid", type=str, default="", help="Path to validation file."
         )
         parser.add_argument(
             "--only-validate-no-export",
             action="store_true",
             default=False,
             help="For pytests and pipelines you can skip the export of the vspec file.",
         )
         parser.add_argument(
             "--strict-mode",
             action="store_true",
             help="Strict mode means that the generation of static UIDs is case-sensitive.",
         )
 
-    def generate(
-        self,
-        config: argparse.Namespace,
-        signal_root: VSSNode,
-        vspec2vss_config: Vspec2VssConfig,
-        data_type_root: Optional[VSSNode] = None,
-    ) -> None:
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+
         """Main export function used to generate the output id vspec.
 
         @param config: Command line arguments it was run with
         @param signal_root: root of the signal tree
         @param print_uuid: Not used here but needed by main script
         """
         logging.info("Generating YAML output...")
```

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2json.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2json.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2jsonschema.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2jsonschema.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2protobuf.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2protobuf.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         with open(fp, 'w') as proto_file:
             logging.info(f"Initializing {fp}, package {package_name}")
             proto_file.write("syntax = \"proto3\";\n\n")
             # set up the proto's package
             proto_file.write(f"package {package_name};\n\n")
             self.out_files.add(fp)
 
-    def traverse_data_type_tree(self, tree: VSSNode, static_uid, add_optional):
+    def traverse_data_type_tree(self, tree: VSSNode):
         """
         All structs in a branch are written to a single .proto file.
         The file's base name is same as the branch's name
         The fully qualified path of the type becomes the package.
 
         Example A.B.C.MyType becomes:
         "package A.B.C;
@@ -96,20 +96,20 @@
                 imports = list(set(imports))
                 imports.sort()
                 for importstmt in imports:
                     proto_file.write(f"import \"{importstmt}\";\n")
                 proto_file.write("\n")
 
                 proto_file.write(f"message {type_qn[-1]} {{" + "\n")
-                print_message_body(tree_node.children, proto_file, static_uid, add_optional)
+                print_message_body(tree_node.children, proto_file)
                 proto_file.write("}\n\n")
                 logging.info(f"Wrote {type_qn[-1]} to {fp}")
 
 
-def traverse_signal_tree(tree: VSSNode, proto_file, static_uid, add_optional):
+def traverse_signal_tree(tree: VSSNode, proto_file):
     proto_file.write("syntax = \"proto3\";\n\n")
     tree_node: VSSNode
 
     # get all the import statements for dependent types (structs)
     imports = []
     for c_node in filter(lambda c: c.is_signal() and not c.has_datatype(), PreOrderIter(tree)):
         child_path = c_node.get_datatype().split(PATH_DELIMITER)[:-1]
@@ -123,75 +123,49 @@
     for importstmt in imports:
         proto_file.write(f"import \"{importstmt}\";\n")
     proto_file.write("\n")
 
     # write proto messages to file
     for tree_node in filter(lambda n: n.is_branch(), PreOrderIter(tree)):
         proto_file.write(f"message {tree_node.qualified_name('')} {{" + "\n")
-        print_message_body(tree_node.children, proto_file, static_uid, add_optional)
+        print_message_body(tree_node.children, proto_file)
         proto_file.write("}\n\n")
 
 
-def print_message_body(nodes, proto_file, static_uid, add_optional):
-    usedKeys = {}
+def print_message_body(nodes, proto_file):
     for i, node in enumerate(nodes, 1):
+        data_type = node.qualified_name("")
         if not (node.is_branch() or node.is_struct()):
             dt_val = node.get_datatype()
             data_type = mapped.get(dt_val.strip("[]"), dt_val.strip("[]"))
-            if dt_val.endswith("[]"):
-                data_type = "repeated " + data_type
-            elif add_optional:
-                data_type = "optional " + data_type
-        else:
-            data_type = node.qualified_name("")
-            if add_optional:
-                data_type = "optional " + data_type
-        if static_uid:
-            if 'staticUID' not in node.extended_attributes:
-                logging.fatal((f"Aborting because {node.qualified_name('.')} does not have the staticUID attribute. "
-                               f"When using the option --static-uid each node must have the attribute staticUID."))
-                sys.exit(-1)
-            fieldNumber = int(int(node.extended_attributes['staticUID'], 0) / 8)
-            if (fieldNumber < 20000 and fieldNumber >= 19000):
-                logging.fatal('''Aborting because field number {fieldNumber} for signal {node.name} is in
-                reservered range between 19000 and 20000. Consider changing the signal to alter the staticUID.''')
-                sys.exit(-1)
-            if fieldNumber in usedKeys:
-                logging.fatal((f"Aborting, due to collision for fieldNumber {fieldNumber}. "
-                               f"It is used by {node.qualified_name('.')} and {usedKeys[fieldNumber]}. "
-                               "Consider changing the signals to alter the staticUID."))
-                proto_file.truncate(0)
-                sys.exit(-1)
-            else:
-                usedKeys[fieldNumber] = node.qualified_name('.')
-        else:
-            fieldNumber = i
-        proto_file.write(f"  {data_type} {node.name} = {fieldNumber};" + "\n")
+            data_type = ("repeated " if dt_val.endswith("[]") else "") + data_type
+        proto_file.write(f"  {data_type} {node.name} = {i};" + "\n")
 
 
 class Vss2Protobuf(Vss2X):
 
     def __init__(self, vspec2vss_config: Vspec2VssConfig):
         vspec2vss_config.no_expand_option_supported = False
         vspec2vss_config.uuid_supported = False
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument('--static-uid', action='store_true',
-                            help=" Expect staticUID attribute in the vspec input and use it as field number.")
-        parser.add_argument('--add-optional', action='store_true',
-                            help=" Set each field to optional.")
+        parser.add_argument('--json-all-extended-attributes', action='store_true',
+                            help="Generate all extended attributes found in the model "
+                                 "(default is generating only those given by the -e/--extended-attributes parameter).")
+        parser.add_argument('--json-pretty', action='store_true',
+                            help=" Pretty print JSON output.")
 
     def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
                  data_type_root: Optional[VSSNode] = None) -> None:
         logging.info("Generating protobuf output...")
         if data_type_root is not None:
             if config.types_output_file is not None:
                 fp = Path(config.types_output_file)
                 exporter_path = Path(os.path.dirname(fp))
             else:
                 exporter_path = Path(Path.cwd())
             logging.debug(f"Will use {exporter_path} for type exports")
             exporter = ProtoExporter(exporter_path)
-            exporter.traverse_data_type_tree(data_type_root, config.static_uid, config.add_optional)
+            exporter.traverse_data_type_tree(data_type_root)
 
         with open(config.output_file, 'w') as f:
-            traverse_signal_tree(signal_root, f, config.static_uid, config.add_optional)
+            traverse_signal_tree(signal_root, f)
```

### Comparing `vss_tools-4.2rc0/vspec/vssexporters/vss2yaml.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2yaml.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2csv.py` & `vss_tools-5.0.0.dev0/vspec2csv.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2ddsidl.py` & `vss_tools-5.0.0.dev0/vspec2ddsidl.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2franca.py` & `vss_tools-5.0.0.dev0/vspec2franca.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2graphql.py` & `vss_tools-5.0.0.dev0/vspec2graphql.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2id.py` & `vss_tools-5.0.0.dev0/vspec2id.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2json.py` & `vss_tools-5.0.0.dev0/vspec2json.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2jsonschema.py` & `vss_tools-5.0.0.dev0/vspec2jsonschema.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2protobuf.py` & `vss_tools-5.0.0.dev0/vspec2protobuf.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vspec2yaml.py` & `vss_tools-5.0.0.dev0/vspec2yaml.py`

 * *Files identical despite different names*

### Comparing `vss_tools-4.2rc0/vss_tools.egg-info/PKG-INFO` & `vss_tools-5.0.0.dev0/vss_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vss-tools
-Version: 4.2rc0
+Version: 5.0.0.dev0
 Summary: COVESA Vehicle Signal Specification tooling.
 Home-page: https://github.com/COVESA/vss-tools
 License: Mozilla Public License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml>=5.1
```

### Comparing `vss_tools-4.2rc0/vss_tools.egg-info/SOURCES.txt` & `vss_tools-5.0.0.dev0/vss_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

