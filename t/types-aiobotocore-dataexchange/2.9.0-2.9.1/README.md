# Comparing `tmp/types-aiobotocore-dataexchange-2.9.0.tar.gz` & `tmp/types-aiobotocore-dataexchange-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dataexchange-2.9.0.tar", last modified: Wed Dec 13 19:59:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-dataexchange-2.9.1.tar", last modified: Thu Jan 18 01:20:29 2024, max compression
```

## Comparing `types-aiobotocore-dataexchange-2.9.0.tar` & `types-aiobotocore-dataexchange-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.461860 types-aiobotocore-dataexchange-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13814 2023-12-13 19:59:03.461860 types-aiobotocore-dataexchange-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:03.461860 types-aiobotocore-dataexchange-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.461860 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24081 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24077 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2023-12-13 19:43:46.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45449 2023-12-13 19:43:47.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45448 2023-12-13 19:43:46.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:45.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.461860 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13814 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:03.000000 types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.089402 types-aiobotocore-dataexchange-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-01-18 01:20:29.089402 types-aiobotocore-dataexchange-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:29.089402 types-aiobotocore-dataexchange-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.089402 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24081 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45448 2024-01-18 01:05:42.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45448 2024-01-18 01:05:41.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:40.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.089402 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:29.000000 types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/LICENSE` & `types-aiobotocore-dataexchange-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/PKG-INFO` & `types-aiobotocore-dataexchange-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dataexchange
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataExchange 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataExchange 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-dataexchange"></a>
 
 # types-aiobotocore-dataexchange
 
 [![PyPI - types-aiobotocore-dataexchange](https://img.shields.io/pypi/v/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dataexchange docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/README.md` & `types-aiobotocore-dataexchange-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dataexchange docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/setup.py` & `types-aiobotocore-dataexchange-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dataexchange",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataExchange 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DataExchange 2.9.1 service generated with"
+        " mypy-boto3-builder 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="aiobotocore dataexchange type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dataexchange": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__init__.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListEventActionsPaginator,
     ListJobsPaginator,
     ListRevisionAssetsPaginator,
 )
 
 Client = DataExchangeClient
 
-
 __all__ = (
     "Client",
     "DataExchangeClient",
     "ListDataSetRevisionsPaginator",
     "ListDataSetsPaginator",
     "ListEventActionsPaginator",
     "ListJobsPaginator",
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__init__.pyi` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/__main__.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataExchange 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DataExchange 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.9.0")
+    print("2.9.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/client.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,37 +60,33 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataExchangeClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class DataExchangeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/)
     """
 
     meta: ClientMeta
@@ -130,15 +126,15 @@
 
     async def create_data_set(
         self,
         *,
         AssetType: AssetTypeType,
         Description: str,
         Name: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         This operation creates a data set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.create_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#create_data_set)
         """
@@ -298,15 +294,15 @@
 
     async def list_jobs(
         self,
         *,
         DataSetId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         This operation lists your jobs sorted by CreatedAt in descending order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#list_jobs)
         """
@@ -348,15 +344,15 @@
         AssetId: str,
         DataSetId: str,
         RevisionId: str,
         Body: str = ...,
         QueryStringParameters: Mapping[str, str] = ...,
         RequestHeaders: Mapping[str, str] = ...,
         Method: str = ...,
-        Path: str = ...
+        Path: str = ...,
     ) -> SendApiAssetResponseTypeDef:
         """
         This operation invokes an API Gateway API asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.send_api_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#send_api_asset)
         """
@@ -365,15 +361,15 @@
         self,
         *,
         DataSetId: str,
         Type: NotificationTypeType,
         Scope: ScopeDetailsTypeDef = ...,
         ClientToken: str = ...,
         Comment: str = ...,
-        Details: NotificationDetailsTypeDef = ...
+        Details: NotificationDetailsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         The type of event associated with the data set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.send_data_set_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#send_data_set_notification)
         """
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/client.pyi` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,31 +62,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("DataExchangeClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class DataExchangeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/)
     """
 
     meta: ClientMeta
@@ -126,15 +129,15 @@
 
     async def create_data_set(
         self,
         *,
         AssetType: AssetTypeType,
         Description: str,
         Name: str,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         This operation creates a data set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.create_data_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#create_data_set)
         """
@@ -294,15 +297,15 @@
 
     async def list_jobs(
         self,
         *,
         DataSetId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         This operation lists your jobs sorted by CreatedAt in descending order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#list_jobs)
         """
@@ -344,15 +347,15 @@
         AssetId: str,
         DataSetId: str,
         RevisionId: str,
         Body: str = ...,
         QueryStringParameters: Mapping[str, str] = ...,
         RequestHeaders: Mapping[str, str] = ...,
         Method: str = ...,
-        Path: str = ...
+        Path: str = ...,
     ) -> SendApiAssetResponseTypeDef:
         """
         This operation invokes an API Gateway API asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.send_api_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#send_api_asset)
         """
@@ -361,15 +364,15 @@
         self,
         *,
         DataSetId: str,
         Type: NotificationTypeType,
         Scope: ScopeDetailsTypeDef = ...,
         ClientToken: str = ...,
         Comment: str = ...,
-        Details: NotificationDetailsTypeDef = ...
+        Details: NotificationDetailsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         The type of event associated with the data set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client.send_data_set_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/client/#send_data_set_notification)
         """
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/literals.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AssetTypeType",
     "CodeType",
     "DatabaseLFTagPolicyPermissionType",
     "JobErrorLimitNameType",
     "JobErrorResourceTypesType",
     "LFPermissionType",
@@ -45,15 +44,14 @@
     "DataExchangeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssetTypeType = Literal[
     "API_GATEWAY_API",
     "LAKE_FORMATION_DATA_PERMISSION",
     "REDSHIFT_DATA_SHARE",
     "S3_DATA_ACCESS",
     "S3_SNAPSHOT",
 ]
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/literals.pyi` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/paginator.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListDataSetRevisionsPaginator",
     "ListDataSetsPaginator",
     "ListEventActionsPaginator",
     "ListJobsPaginator",
     "ListRevisionAssetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -114,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/paginators/#listjobspaginator)
         """
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/paginator.pyi` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/paginators/#listjobspaginator)
         """
 
 class ListRevisionAssetsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/type_defs.py` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApiGatewayApiAssetTypeDef",
     "AssetDestinationEntryTypeDef",
     "RedshiftDataShareAssetTypeDef",
     "S3SnapshotAssetTypeDef",
     "AssetSourceEntryTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange/type_defs.pyi` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/PKG-INFO` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dataexchange
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataExchange 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataExchange 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-dataexchange"></a>
 
 # types-aiobotocore-dataexchange
 
 [![PyPI - types-aiobotocore-dataexchange](https://img.shields.io/pypi/v/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dataexchange docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dataexchange-2.9.0/types_aiobotocore_dataexchange.egg-info/SOURCES.txt` & `types-aiobotocore-dataexchange-2.9.1/types_aiobotocore_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

