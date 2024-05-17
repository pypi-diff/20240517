# Comparing `tmp/ddeutil_io-0.1.4.tar.gz` & `tmp/ddeutil_io-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.4.tar", last modified: Wed May 15 15:15:06 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.5.tar", last modified: Thu May 16 15:13:30 2024, max compression
```

## Comparing `ddeutil_io-0.1.4.tar` & `ddeutil_io-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_file_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.780377 ddeutil_io-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-16 15:13:30.780377 ddeutil_io-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:13:30.780377 ddeutil_io-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.772377 ddeutil_io-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.772377 ddeutil_io-0.1.5/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.776377 ddeutil_io-0.1.5/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.776377 ddeutil_io-0.1.5/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.776377 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-16 15:13:30.000000 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 15:13:30.000000 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:13:30.000000 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:13:30.000000 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 15:13:30.000000 ddeutil_io-0.1.5/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:13:30.776377 ddeutil_io-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_base_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_base_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-16 15:13:26.000000 ddeutil_io-0.1.5/tests/test_register.py
```

### Comparing `ddeutil_io-0.1.4/LICENSE` & `ddeutil_io-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/PKG-INFO` & `ddeutil_io-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil_io-0.1.4/README.md` & `ddeutil_io-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/pyproject.toml` & `ddeutil_io-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/__base/__init__.py` & `ddeutil_io-0.1.5/src/ddeutil/io/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.5/src/ddeutil/io/__base/__regex.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.5/src/ddeutil/io/__base/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 )
 
 # NOTE: import msgpack
 import yaml
 
 try:
     from yaml import CSafeLoader as SafeLoader
+    from yaml import CUnsafeLoader as UnsafeLoader
 except ImportError:
-    from yaml import SafeLoader
+    from yaml import SafeLoader, UnsafeLoader
 
 from .__regex import RegexConf
 from .utils import search_env, search_env_replace
 
 FileCompressType = Literal["gzip", "gz", "xz", "bz2"]
 DirCompressType = Literal["zip", "rar", "tar", "h5", "hdf5", "fits"]
 
@@ -255,49 +256,99 @@
     .. noted::
         - The boolean value in the yaml file
             - true: Y, true, Yes, ON
             - false: n, false, No, off
     """
 
     def read(self, safe: bool = True) -> dict[str, Any]:
-        if safe:
-            with self.open(mode="r") as _r:
-                return yaml.load(_r.read(), SafeLoader)
-        return NotImplementedError
+        with self.open(mode="r") as _r:
+            return yaml.load(_r.read(), (SafeLoader if safe else UnsafeLoader))
 
     def write(self, data: dict[str, Any]) -> None:
         with self.open(mode="w") as _w:
             yaml.dump(data, _w, default_flow_style=False)
 
 
+class YamlFlResolve(YamlFl):
+
+    def read(self, safe: bool = True) -> dict[str, Any]:
+        """Reading Yaml data with does not convert boolean value.
+        Note:
+            Handle top level yaml property ``on``
+            docs: https://github.com/yaml/pyyaml/issues/696
+
+            import re
+            from yaml.resolver import Resolver
+
+            # zap the Resolver class' internal dispatch table
+            Resolver.yaml_implicit_resolvers = {}
+
+            # NOTE: Current Resolver
+            Resolver.add_implicit_resolver(
+                    'tag:yaml.org,2002:bool',
+                    re.compile(r'''^(?:yes|Yes|YES|no|No|NO
+                                |true|True|TRUE|false|False|FALSE
+                                |on|On|ON|off|Off|OFF)$''', re.X),
+                    list('yYnNtTfFoO'))
+
+            # NOTE: The 1.2 bool impl Resolver:
+            Resolver.add_implicit_resolver(
+                    'tag:yaml.org,2002:bool',
+                    re.compile(r'^(?:true|false)$', re.X),
+                    list('tf'))
+        """
+        from yaml.resolver import Resolver
+
+        revert = Resolver.yaml_implicit_resolvers.copy()
+
+        for ch in "OoYyNn":
+            if len(Resolver.yaml_implicit_resolvers[ch]) == 1:
+                del Resolver.yaml_implicit_resolvers[ch]
+            else:
+                Resolver.yaml_implicit_resolvers[ch] = [
+                    x
+                    for x in Resolver.yaml_implicit_resolvers[ch]
+                    if x[0] != "tag:yaml.org,2002:bool"
+                ]
+
+        with self.open(mode="r") as _r:
+            rs: dict[str, Any] = yaml.load(
+                _r.read(), (SafeLoader if safe else UnsafeLoader)
+            )
+            # NOTE: revert resolver when want to use safe load.
+            Resolver.yaml_implicit_resolvers = revert
+            return rs
+
+
 class YamlEnvFl(YamlFl):
     """Yaml object which mapping search environment variable."""
 
     raise_if_not_default: ClassVar[bool] = False
     default: ClassVar[str] = "null"
-    escape: ClassVar[str] = "ESC"
+    escape: ClassVar[str] = "<ESCAPE>"
 
     @staticmethod
     def prepare(x: str) -> str:
         return x
 
     def read(self, safe: bool = True) -> dict[str, Any]:
-        if safe:
-            with self.open(mode="r") as _r:
-                _env_replace: str = search_env_replace(
-                    RegexConf.RE_YAML_COMMENT.sub("", _r.read()),
-                    raise_if_default_not_exists=self.raise_if_not_default,
-                    default=self.default,
-                    escape=self.escape,
-                    caller=self.prepare,
-                )
-                if _result := yaml.load(_env_replace, SafeLoader):
-                    return _result
-                return {}
-        return NotImplementedError
+        with self.open(mode="r") as _r:
+            _env_replace: str = search_env_replace(
+                RegexConf.RE_YAML_COMMENT.sub("", _r.read()),
+                raise_if_default_not_exists=self.raise_if_not_default,
+                default=self.default,
+                escape=self.escape,
+                caller=self.prepare,
+            )
+            if _result := yaml.load(
+                _env_replace,
+                (SafeLoader if safe else UnsafeLoader),
+            ):
+                return _result
+            return {}
 
     def write(self, data: dict[str, Any]) -> None:
         raise NotImplementedError
 
 
 class CsvFl(Fl, FlAbc):
     def read(self) -> list[str]:
```

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.5/src/ddeutil/io/__base/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/config.py` & `ddeutil_io-0.1.5/src/ddeutil/io/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from __future__ import annotations
 
 import abc
 import contextlib
 import inspect
 import json
 import logging
-import os
 import shutil
 import sqlite3
-from collections.abc import Iterator
+from collections.abc import Generator, Iterator
 from datetime import datetime
 from pathlib import Path
+from sqlite3 import Connection
 from typing import (
     Any,
     Optional,
     Union,
 )
 
 from .__base import (
@@ -27,14 +27,17 @@
     JsonFl,
     PathSearch,
     YamlEnvFl,
     rm,
 )
 from .exceptions import ConfigArgumentError
 
+DEFAULT_OPEN_FILE: type[Fl] = YamlEnvFl
+DEFAULT_OPEN_FILE_STG: type[Fl] = JsonFl
+
 
 class ConfABC(abc.ABC):
     """Config Adapter abstract object."""
 
     @abc.abstractmethod
     def load_stage(self, name: str) -> dict:
         raise NotImplementedError
@@ -60,18 +63,18 @@
     def __init__(
         self,
         path: Union[str, Path],
         *,
         compress: Optional[str] = None,
         open_file: Optional[type[Fl]] = None,
         excluded_fmt: Optional[tuple[str]] = None,
-    ):
+    ) -> None:
         self.path: Path = Path(path) if isinstance(path, str) else path
         self.compress: Optional[str] = compress
-        self.open_file: type[Fl] = open_file or YamlEnvFl
+        self.open_file: type[Fl] = open_file or DEFAULT_OPEN_FILE
         self.excluded_fmt: tuple[str] = excluded_fmt or (".json", ".toml")
         if not self.path.exists():
             self.path.mkdir(parents=True)
 
     def load(
         self,
         name: str,
@@ -135,15 +138,15 @@
         path: Path,
         destination: Path,
         *,
         auto_create: bool = True,
     ) -> None:
         """Copy filename to destination path."""
         if auto_create:
-            destination.mkdir(parents=True, exist_ok=True)
+            destination.parent.mkdir(parents=True, exist_ok=True)
         shutil.copy(self.path / path, destination)
 
 
 class ConfFl(BaseConfFl, ConfABC):
     """Config File Loading Object for get data from configuration and stage."""
 
     def __init__(
@@ -163,15 +166,15 @@
         """
         super().__init__(
             path,
             compress=compress,
             open_file=open_file,
             excluded_fmt=excluded_fmt,
         )
-        self.open_file_stg: type[Fl] = open_file_stg or JsonFl
+        self.open_file_stg: type[Fl] = open_file_stg or DEFAULT_OPEN_FILE_STG
 
     def load_stage(
         self,
         path: Union[str, Path],
         *,
         default: Optional[Any] = None,
     ) -> Union[dict[Any, Any], list[Any]]:
@@ -256,40 +259,36 @@
 class BaseConfSQLite:
     """Base Config SQLite object for getting data with SQLite database from
     file storage."""
 
     def __init__(
         self,
         path: Union[str, Path],
-        *,
-        auto_create: bool = True,
-    ):
+    ) -> None:
         self.path: Path = Path(path) if isinstance(path, str) else path
-        if not os.path.exists(self.path):
-            if not auto_create:
-                raise FileNotFoundError(f"Path {path} does not exists.")
-            os.makedirs(self.path, exist_ok=True)
+        if not self.path.exists():
+            self.path.mkdir(parents=True)
 
     @contextlib.contextmanager
-    def connect(self, database: str):
+    def connect(self, database: str) -> Generator[Connection, None, None]:
         """Return SQLite Connection context."""
-        _conn = sqlite3.connect(self.path / database, timeout=3)
+        _conn: Connection = sqlite3.connect(self.path / database, timeout=3)
         _conn.row_factory = self.dict_factory
         try:
             yield _conn
         except sqlite3.Error as err:
             logging.error(err)
             raise ConfigArgumentError(
                 "syntax", f"SQLite syntax error {err}"
             ) from err
         _conn.commit()
         _conn.close()
 
     @staticmethod
-    def dict_factory(cursor, row):
+    def dict_factory(cursor, row) -> dict[str, Any]:
         """Result of dictionary factory.
 
         :note:
             Another logic of dict factory.
 
             - dict(
                 [
@@ -300,14 +299,16 @@
 
             - dict(zip([col[0] for col in cursor.description], row))
         """
         return {col[0]: row[idx] for idx, col in enumerate(cursor.description)}
 
 
 class ConfSQLite(BaseConfSQLite, ConfABC):
+    """Config SQLite Loading Object for get data from configuration and stage."""
+
     def load_stage(
         self,
         table: str,
         default: Optional[dict[Any, Any]] = None,
     ) -> dict[Any, Any]:
         """Return content data from database with table name, default empty
         dict."""
@@ -350,21 +351,20 @@
         table: str,
         data_name: str,
     ) -> None:
         """Remove data by name from table in database with table name."""
         _db, _table = table.rsplit("/", maxsplit=1)
         with self.connect(_db) as conn:
             cur = conn.cursor()
-            query: str = f"delete from {_table} where name = '{data_name}';"
-            cur.execute(query)
+            cur.execute(f"delete from {_table} where name = '{data_name}';")
 
     def create(
         self,
         table: str,
-        schemas: Optional[dict] = None,
+        schemas: Optional[dict[str, str]] = None,
     ) -> None:
         """Create table in database."""
         if not schemas:
             raise ConfigArgumentError(
                 "schemas",
                 (
                     f"in `create` method of {self.__class__.__name__} "
@@ -375,38 +375,37 @@
         _db, _table = table.rsplit("/", maxsplit=1)
         with self.connect(_db) as conn:
             cur = conn.cursor()
             cur.execute(f"create table if not exists {_table} ({_schemas})")
 
     @staticmethod
     def prepare_values(
-        values: dict,
+        values: dict[str, Union[str, int, float]],
     ) -> dict[str, Union[str, int, float]]:
         """Return prepare value with dictionary type to string
         to source system.
         """
-        results: dict = values.copy()
+        rs: dict[str, Union[str, int, float]] = values.copy()
         for _ in values:
             if isinstance(values[_], dict):
-                results[_] = json.dumps(values[_])
-        return results
+                rs[_] = json.dumps(values[_])
+        return rs
 
     @staticmethod
     def convert_type(
-        data: dict,
+        data: dict[str, Union[str, int, float]],
         key: Optional[str] = None,
-    ) -> dict:
+    ) -> dict[str, Any]:
         """Return converted value from string to dictionary
         from source system.
         """
         _key: str = key or "data"
-        _results: dict = data.copy()
-        _results[_key] = json.loads(data[_key])
-        return _results
+        rs: dict[str, Any] = data.copy()
+        rs[_key] = json.loads(data[_key])
+        return rs
 
 
 __all__ = (
     "ConfABC",
     "ConfFl",
     "ConfSQLite",
-    "Fl",
 )
```

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.5/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/models.py` & `ddeutil_io-0.1.5/src/ddeutil/io/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -117,25 +117,29 @@
                     ),
                 )
         return value
 
 
 class PathData(BaseModel):
     root: Path = Field(default_factory=Path)
-    data: Path = Field(default="data", validate_default=True)
-    conf: Path = Field(default="conf", validate_default=True)
-    archive: Path = Field(default=".archive", validate_default=True)
+    data: Path = Field(default=None, validate_default=True)
+    conf: Path = Field(default=None, validate_default=True)
+    archive: Path = Field(default=None, validate_default=True)
 
     @field_validator("root", mode="before")
     def prepare_root(cls, v: Union[str, Path]) -> Path:
         return Path(v) if isinstance(v, str) else v
 
     @field_validator("data", "conf", "archive", mode="before")
     def prepare_path_from_str(cls, v, info: ValidationInfo) -> Path:
-        return v if isinstance(v, Path) else (info.data["root"] / v)
+        if v is not None:
+            return Path(v) if isinstance(v, str) else v
+        if info.field_name == "archive":
+            return info.data["root"] / ".archive"
+        return info.data["root"] / info.field_name
 
 
 class FlagData(BaseModel):
     archive: bool = Field(default=False)
     auto_update: bool = Field(default=False)
```

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/register.py` & `ddeutil_io-0.1.5/src/ddeutil/io/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     Naming,
     VerPackage,
     Version,
     make_const,
     make_group,
 )
 
-from .__base import rm
-from .config import ConfFl, Fl
+from .__base import Fl, rm
+from .config import ConfFl
 from .exceptions import ConfigArgumentError, ConfigNotFound
 from .models import Params
 
 METADATA: dict[str, Any] = {}
 
 
 class StageFiles(TypedDict):
@@ -156,60 +156,69 @@
     def __init__(
         self,
         name: str,
         stage: Optional[str] = None,
         *,
         params: Optional[Params] = None,
         loader: Optional[type[Fl]] = None,
+        loader_stg: Optional[type[Fl]] = None,
     ):
         _domain, _name = must_rsplit(concat(name.split()), ":", maxsplit=1)
         super().__init__(name=_name, domain=_domain)
         if not params:
             raise NotImplementedError(
                 "This register instance can not do any actions because config "
                 "param does not set."
             )
         self.stage: str = stage or "base"
         self.loader: Optional[type[Fl]] = loader
+        self.loader_stg: Optional[type[Fl]] = loader_stg
         self.params: Optional[Params] = params
 
         # Load latest version of data from data lake or data store of
         # configuration files
         self.__data: dict[str, Any] = self.pick(stage=self.stage)
         if not self.__data:
             raise ConfigNotFound(
                 f"Config {self.name!r} "
                 f"{f'in domain {self.domain!r} ' if self.domain else ' '}"
                 f"does not exist in stage {self.stage!r}."
             )
 
-        self.meta: dict[str, Any] = METADATA
+        self.meta: dict[str, Any] = METADATA.get(self.fullname, {})
 
         # NOTE:
         #   Compare data from current stage and latest version in metadata.
         self.changed: int = self.compare_data(
             target=self.meta.get(self.stage, {})
         )
 
         # NOTE:
         #   Update metadata if the configuration data does not exist, or
         #   it has any changes.
         if not self.params.engine.flags.auto_update:
-            logging.info("Skip update metadata table/file ...")
+            logging.info("Skip update metadata ...")
         elif self.changed == 99:
             logging.info(
                 f"Configuration data with stage: {self.stage!r} does not "
                 f"exists in metadata ..."
             )
+            # TODO: Create metadata for caching value before compare data next
+            #   time. (It can be table on database or sqlite file.
+            # METADATA.update({"self.fullname": self.__data})
         elif self.changed > 0:
             logging.info(
                 f"Should update metadata because diff level is {self.changed}."
             )
 
-    def __hash__(self):
+        # TODO: Remove this line when develop metadata feature in the next
+        #   release.
+        METADATA.pop(self.fullname, None)
+
+    def __hash__(self) -> int:
         return hash(
             self.fullname
             + self.stage
             + f"{self.timestamp:{self.params.engine.values.dt_fmt}}"
         )
 
     def __str__(self) -> str:
@@ -359,20 +368,22 @@
         order: Optional[int] = 1,
         reverse: bool = False,
     ) -> dict[str, Any]:
         if (stage is None) or (stage == "base"):
             return ConfFl(
                 path=(self.params.engine.paths.conf / self.domain),
                 open_file=self.loader,
+                open_file_stg=self.loader_stg,
             ).load(name=self.name, order=order)
 
         loading = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=self.params.get_stage(stage).rules.compress,
             open_file=self.loader,
+            open_file_stg=self.loader_stg,
         )
 
         if results := self.__stage_files(stage, loading):
             max_data: list = sorted(
                 results.items(),
                 key=lambda x: (x[1]["parse"],),
                 reverse=reverse,
@@ -390,14 +401,15 @@
         retention: bool = True,
     ) -> Register:
         """Move file to the target stage."""
         loading: ConfFl = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=self.params.get_stage(stage).rules.compress,
             open_file=self.loader,
+            open_file_stg=self.loader_stg,
         )
         if (
             self.compare_data(
                 hash_all(
                     self.pick(stage=stage),
                     exclude=set(self.params.engine.values.excluded),
                 )
@@ -447,35 +459,36 @@
     def purge(self, stage: Optional[str] = None) -> None:
         """Purge configuration files that match with any rules in the stage
         setting.
         """
         _stage: str = stage or self.stage
         if not (_rules := self.params.get_stage(_stage).rules):
             return
-        loading = ConfFl(
+        loading: ConfFl = ConfFl(
             path=self.params.engine.paths.data / stage,
             compress=_rules.compress,
             open_file=self.loader,
+            open_file_stg=self.loader_stg,
         )
-        results: dict = self.__stage_files(_stage, loading)
+        rs: dict[int, StageFiles] = self.__stage_files(_stage, loading)
         max_file: FormatterGroup = max(
-            results.items(),
+            rs.items(),
             key=lambda x: (x[1]["parse"],),
         )[1]["parse"]
 
         upper_bound: Optional[FormatterGroup] = None
         if _rtt_ts := _rules.timestamp:
             upper_bound = max_file.adjust(
                 {"timestamp": relativedelta(**_rtt_ts)}
             )
 
         if upper_bound is not None:
             for _, data in filter(
                 lambda x: x[1]["parse"] < upper_bound,
-                results.items(),
+                rs.items(),
             ):
                 _file: str = data["file"]
                 if self.params.engine.flags.archive:
                     _ac_path: str = (
                         f"{stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
                     )
                     loading.move(
@@ -508,20 +521,22 @@
         :param stage: a stage value that want to remove.
         :type stage: Optional[str]
         """
         _stage: str = stage or self.stage
         assert (
             _stage != "base"
         ), "The remove method can not process on the 'base' stage."
-        loading = ConfFl(
+        loading: ConfFl = ConfFl(
             path=self.params.engine.paths.data / _stage,
             open_file=self.loader,
+            open_file_stg=self.loader_stg,
         )
 
         # Remove all files from the stage.
+        data: StageFiles
         for _, data in self.__stage_files(_stage, loading).items():
             _file: str = data["file"]
             if self.params.engine.flags.archive:
                 _ac_path: str = (
                     f"{_stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
                 )
                 loading.move(
```

### Comparing `ddeutil_io-0.1.4/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.5/src/ddeutil/io/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/src/ddeutil_io.egg-info/PKG-INFO` & `ddeutil_io-0.1.5/src/ddeutil_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil_io-0.1.4/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.5/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 src/ddeutil_io.egg-info/dependency_links.txt
 src/ddeutil_io.egg-info/requires.txt
 src/ddeutil_io.egg-info/top_level.txt
 tests/test_base_csv.py
 tests/test_base_dir.py
 tests/test_base_env.py
 tests/test_base_file.py
-tests/test_base_file_yaml.py
+tests/test_base_yaml.py
 tests/test_config_file.py
 tests/test_config_sqlite.py
 tests/test_models.py
 tests/test_register.py
```

### Comparing `ddeutil_io-0.1.4/tests/test_base_csv.py` & `ddeutil_io-0.1.5/tests/test_base_csv.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/tests/test_base_dir.py` & `ddeutil_io-0.1.5/tests/test_base_dir.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/tests/test_base_env.py` & `ddeutil_io-0.1.5/tests/test_base_env.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/tests/test_base_file.py` & `ddeutil_io-0.1.5/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.4/tests/test_base_file_yaml.py` & `ddeutil_io-0.1.5/tests/test_base_yaml.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,92 @@
 import os
+import shutil
 import unittest
 import warnings
+from collections.abc import Generator
+from pathlib import Path
 from textwrap import dedent
+from typing import Any
 
 import ddeutil.io.__base.files as fl
+import pytest
 import yaml
 
 
-class YamlFileTestCase(unittest.TestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        cls.root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
-            os.sep, "/"
-        )
+@pytest.fixture(scope="module")
+def target_path(test_path) -> Generator[Path, None, None]:
+    target_path: Path = test_path / "base_file_yaml"
+    target_path.mkdir(parents=True, exist_ok=True)
+
+    yield target_path
 
-    def setUp(self) -> None:
-        warnings.simplefilter("ignore", category=ResourceWarning)
-        self.yaml_str: str = dedent(
-            """
-        main_key:
-            sub_key:
-                string: 'test ${DEMO_ENV_VALUE} value'
-                int: 0.001
-                bool: false
-                list: ['i1', 'i2', 'i3']
+    shutil.rmtree(target_path)
+
+
+@pytest.fixture(scope="module")
+def yaml_str_safe() -> str:
+    return dedent(
         """
-        ).strip()
-        self.yaml_data: dict = {
-            "main_key": {
-                "sub_key": {
-                    "string": "test ${DEMO_ENV_VALUE} value",
-                    "int": 0.001,
-                    "bool": False,
-                    "list": ["i1", "i2", "i3"],
-                }
+    main_key:
+        sub_key:
+            string: 'test ${DEMO_ENV_VALUE} value'
+            int: 0.001
+            bool: false
+            list: ['i1', 'i2', 'i3']
+            str2bool: on
+    """
+    ).strip()
+
+
+@pytest.fixture(scope="module")
+def yaml_data_safe() -> dict[str, Any]:
+    return {
+        "main_key": {
+            "sub_key": {
+                "string": "test ${DEMO_ENV_VALUE} value",
+                "int": 0.001,
+                "bool": False,
+                "list": ["i1", "i2", "i3"],
+                "str2bool": True,
             }
         }
+    }
+
+
+def test_write_yaml_file_with_safe(target_path, yaml_str_safe, yaml_data_safe):
+    yaml_path: Path = target_path / "test_write_file.yaml"
+    fl.YamlFl(path=yaml_path).write(yaml_data_safe)
+    assert yaml_path.exists()
+
 
-    def test_write_yaml_file_with_safe_mode(self):
-        yaml_path: str = f"{self.root_path}/test_write_file.yaml"
+def test_read_yaml_resolve_file(target_path, yaml_str_safe, yaml_data_safe):
+    yaml_path: Path = target_path / "test_read_file_resolve.yaml"
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        f.write(yaml_str_safe)
 
-        fl.YamlFl(path=yaml_path).write(self.yaml_data)
+    data = fl.YamlFlResolve(path=yaml_path).read(safe=False)
+    assert "on" == data["main_key"]["sub_key"]["str2bool"]
 
-        self.assertTrue(os.path.exists(yaml_path))
 
-        os.remove(yaml_path)
+def test_read_yaml_file_with_safe(target_path, yaml_str_safe, yaml_data_safe):
+    yaml_path: Path = target_path / "test_read_file_safe.yaml"
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        yaml.dump(yaml.safe_load(yaml_str_safe), f)
 
-    def test_read_yaml_file_with_safe_mode(self):
-        yaml_path: str = f"{self.root_path}/test_read_file.yaml"
+    data = fl.YamlFl(path=yaml_path).read()
+    assert yaml_data_safe == data
 
-        with open(yaml_path, mode="w", encoding="utf-8") as f:
-            yaml.dump(yaml.safe_load(self.yaml_str), f)
 
-        data = fl.YamlFl(path=yaml_path).read()
-        self.assertDictEqual(self.yaml_data, data)
+def test_read_yaml_file(target_path, yaml_str_safe, yaml_data_safe):
+    yaml_path: Path = target_path / "test_read_file.yaml"
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        f.write(yaml_str_safe)
 
-        os.remove(yaml_path)
+    data = fl.YamlFl(path=yaml_path).read(safe=False)
+    assert yaml_data_safe == data
 
 
 class YamlEnvFileTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         cls.root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
             os.sep, "/"
```

### Comparing `ddeutil_io-0.1.4/tests/test_config_file.py` & `ddeutil_io-0.1.5/tests/test_config_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 import shutil
+from collections.abc import Generator
 from pathlib import Path
 
 import ddeutil.io.config as conf
 import pytest
+import yaml
 
 
 @pytest.fixture(scope="module")
-def target_path(test_path) -> Path:
-    return test_path / "conf_file_temp"
+def target_path(test_path) -> Generator[Path, None, None]:
+    tgt_path: Path = test_path / "conf_file_temp"
+    tgt_path.mkdir(exist_ok=True)
+    with open(tgt_path / "test_01_conn.yaml", mode="w") as f:
+        yaml.dump(
+            {
+                "conn_local_file": {
+                    "type": "connection.LocalFileStorage",
+                    "endpoint": "file:///${APP_PATH}/tests/examples/dummy",
+                }
+            },
+            f,
+        )
+    yield tgt_path
+    shutil.rmtree(tgt_path)
 
 
-def test_base_conf_read_file(demo_path, target_path):
-    bcf = conf.BaseConfFl(demo_path)
+def test_base_conf_read_file(target_path):
+    bcf = conf.BaseConfFl(target_path)
 
     assert {
         "alias": "conn_local_file",
         "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == bcf.load(name="conn_local_file")
 
     bcf.move(
-        "demo_01_connections.yaml",
-        destination=target_path / "demo_01_connections.yaml",
+        "test_01_conn.yaml",
+        destination=target_path / "connections/test_01_conn.yaml",
     )
 
     bcf_temp = conf.BaseConfFl(target_path)
     assert {
         "alias": "conn_local_file",
         "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == bcf_temp.load(name="conn_local_file")
 
-    assert (target_path / "demo_01_connections.yaml").exists()
+    assert (target_path / "connections/test_01_conn.yaml").exists()
 
-    if target_path.exists():
-        shutil.rmtree(target_path)
 
-
-def test_conf_read_file(demo_path, target_path):
-    cf = conf.ConfFl(demo_path)
+def test_conf_read_file(target_path):
+    cf = conf.ConfFl(target_path)
     cf.move(
-        path="demo_01_connections.yaml",
-        destination=target_path / "demo_01_connections.yaml",
+        path="test_01_conn.yaml",
+        destination=target_path / "connections/test_01_conn.yaml",
     )
 
-    _stage_path = target_path / "demo_01_connections_stage.json"
+    _stage_path: Path = target_path / "connections/test_01_conn_stage.json"
 
     cf.create(path=_stage_path)
     assert _stage_path.exists()
     cf.save_stage(path=_stage_path, data=cf.load("conn_local_file"))
 
     assert {
         "alias": "conn_local_file",
@@ -68,10 +80,7 @@
     )
 
     assert {
         "alias": "conn_local_file",
         "endpoint": "file:///null/tests/examples/dummy",
         "type": "connection.LocalFileStorage",
     } == cf.load_stage(path=_stage_path)
-
-    if target_path.exists():
-        shutil.rmtree(target_path)
```

### Comparing `ddeutil_io-0.1.4/tests/test_config_sqlite.py` & `ddeutil_io-0.1.5/tests/test_config_sqlite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import shutil
+from collections.abc import Generator
 from pathlib import Path
 
 import ddeutil.io.config as conf
 import pytest
 
 
 @pytest.fixture(scope="module")
-def sqlite_path(test_path) -> Path:
-    return test_path / "conf_sqlite_temp"
+def sqlite_path(test_path) -> Generator[Path, None, None]:
+    sqlite_path: Path = test_path / "conf_sqlite_temp"
 
+    yield sqlite_path
 
-@pytest.fixture(scope="module")
-def demo_path(test_path) -> Path:
-    return test_path / "examples" / "conf" / "demo"
+    if sqlite_path.exists():
+        shutil.rmtree(sqlite_path)
 
 
-def test_base_conf_read_file(demo_path, sqlite_path):
+def test_base_conf_read_file(sqlite_path: Path):
     _schemas: dict[str, str] = {
         "name": "varchar(256) primary key",
         "shortname": "varchar(64) not null",
         "fullname": "varchar(256) not null",
         "data": "json not null",
         "updt": "datetime not null",
         "rtdt": "datetime not null",
@@ -40,11 +41,8 @@
             "updt": "2023-01-01 00:00:00",
             "rtdt": "2023-01-01 00:00:00",
             "author": "unknown",
         },
     }
 
     bc_sql.save_stage(table="demo.db/temp_table", data=_data)
-
     assert _data == bc_sql.load_stage(table="demo.db/temp_table")
-    if sqlite_path.exists():
-        shutil.rmtree(sqlite_path)
```

### Comparing `ddeutil_io-0.1.4/tests/test_models.py` & `ddeutil_io-0.1.5/tests/test_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,45 @@
-import pathlib
+from pathlib import Path
 
 import ddeutil.io.models as md
 
 
+def test_model_path_default(test_path):
+    p = md.PathData.model_validate(
+        {
+            "root": test_path,
+        }
+    )
+    print(p)
+
+
 def test_model_path_data():
     p = md.PathData.model_validate(
         {
-            "data": pathlib.Path("."),
-            "conf": pathlib.Path("."),
-            "archive": pathlib.Path("."),
+            "data": Path("."),
+            "conf": Path("."),
+            "archive": Path("."),
         }
     )
 
     assert {
-        "data": pathlib.Path("."),
-        "conf": pathlib.Path("."),
-        "archive": pathlib.Path("."),
-        "root": pathlib.Path("."),
+        "data": Path("."),
+        "conf": Path("."),
+        "archive": Path("."),
+        "root": Path("."),
     } == p.model_dump()
 
 
 def test_model_path_data_with_root():
     p = md.PathData.model_validate({"root": "./src/"})
     assert {
-        "data": pathlib.Path("./src/data"),
-        "conf": pathlib.Path("./src/conf"),
-        "archive": pathlib.Path("./src/.archive"),
-        "root": pathlib.Path("./src/"),
+        "data": Path("./src/data"),
+        "conf": Path("./src/conf"),
+        "archive": Path("./src/.archive"),
+        "root": Path("./src/"),
     } == p.model_dump()
 
 
 def test_model_rule_data():
     assert {
         "timestamp": {},
         "version": None,
@@ -115,14 +124,14 @@
                 "excluded": ("version", "updt"),
             },
             "flags": {
                 "archive": False,
                 "auto_update": False,
             },
             "paths": {
-                "archive": pathlib.Path(".archive"),
-                "conf": pathlib.Path("conf"),
-                "data": pathlib.Path("data"),
-                "root": pathlib.Path("."),
+                "archive": Path(".archive"),
+                "conf": Path("conf"),
+                "data": Path("data"),
+                "root": Path("."),
             },
         },
     } == params.model_dump()
```

### Comparing `ddeutil_io-0.1.4/tests/test_register.py` & `ddeutil_io-0.1.5/tests/test_register.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,43 @@
+import shutil
+from collections.abc import Generator
 from pathlib import Path
 
 import ddeutil.io.register as rgt
 import pytest
+import yaml
 from ddeutil.io.models import Params
 
 
 @pytest.fixture(scope="module")
-def target_path(test_path) -> Path:
-    return test_path / "conf_file_temp"
+def target_path(test_path) -> Generator[Path, None, None]:
+    tgt_path: Path = test_path / "register_temp"
+    tgt_path.mkdir(exist_ok=True)
+    (tgt_path / "conf/demo").mkdir(parents=True)
+    with open(tgt_path / "conf/demo/test_01_conn.yaml", mode="w") as f:
+        yaml.dump(
+            {
+                "conn_local_file": {
+                    "type": "connection.LocalFileStorage",
+                    "endpoint": "file:///${APP_PATH}/tests/examples/dummy",
+                }
+            },
+            f,
+        )
+    yield tgt_path
+    shutil.rmtree(tgt_path)
 
 
 @pytest.fixture(scope="module")
-def params(test_path, root_path) -> Params:
+def params(target_path, root_path) -> Params:
     return Params.model_validate(
         {
             "engine": {
                 "paths": {
-                    "conf": test_path / "examples/conf",
+                    "conf": target_path / "conf",
                     "data": root_path / "data",
                     "archive": root_path / "/data/.archive",
                 },
                 "flags": {"auto_update": True},
             },
             "stages": {
                 "raw": {"format": "{naming:%s}.{timestamp:%Y%m%d_%H%M%S}"},
```

