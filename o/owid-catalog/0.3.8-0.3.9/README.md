# Comparing `tmp/owid_catalog-0.3.8.tar.gz` & `tmp/owid_catalog-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owid_catalog-0.3.8.tar", max compression
+gzip compressed data, was "owid_catalog-0.3.9.tar", max compression
```

## Comparing `owid_catalog-0.3.8.tar` & `owid_catalog-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1079 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/LICENSE
--rw-r--r--   0        0        0     8866 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/README.md
--rw-r--r--   0        0        0      722 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/__init__.py
--rw-r--r--   0        0        0    14728 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/catalogs.py
--rw-r--r--   0        0        0    11989 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/datasets.py
--rw-r--r--   0        0        0    19770 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/meta.py
--rwxr-xr-x   0        0        0      482 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/processing.py
--rw-r--r--   0        0        0      449 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/properties.py
--rw-r--r--   0        0        0     2991 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/s3_utils.py
--rw-r--r--   0        0        0      532 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/schemas/table.json
--rw-r--r--   0        0        0      527 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/schemas/variable.json
--rw-r--r--   0        0        0    63410 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/tables.py
--rw-r--r--   0        0        0     5592 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/utils.py
--rw-r--r--   0        0        0    27934 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/variables.py
--rw-r--r--   0        0        0     4962 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/owid/catalog/yaml_metadata.py
--rw-r--r--   0        0        0     1418 2023-10-17 14:24:21.273237 owid_catalog-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     9963 1970-01-01 00:00:00.000000 owid_catalog-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/LICENSE
+-rw-r--r--   0        0        0     8923 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/README.md
+-rw-r--r--   0        0        0      811 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/__init__.py
+-rw-r--r--   0        0        0    14728 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/catalogs.py
+-rw-r--r--   0        0        0    12377 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/datasets.py
+-rw-r--r--   0        0        0    19863 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/meta.py
+-rwxr-xr-x   0        0        0      576 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/processing.py
+-rw-r--r--   0        0        0    11727 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/processing_log.py
+-rw-r--r--   0        0        0      449 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/properties.py
+-rw-r--r--   0        0        0     1635 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/s3_utils.py
+-rw-r--r--   0        0        0      532 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/schemas/table.json
+-rw-r--r--   0        0        0      527 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/schemas/variable.json
+-rw-r--r--   0        0        0    61481 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/tables.py
+-rw-r--r--   0        0        0     5592 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/utils.py
+-rw-r--r--   0        0        0    22402 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/variables.py
+-rw-r--r--   0        0        0     4982 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/owid/catalog/yaml_metadata.py
+-rw-r--r--   0        0        0     1274 2024-01-26 09:12:41.204183 owid_catalog-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    10055 1970-01-01 00:00:00.000000 owid_catalog-0.3.9/PKG-INFO
```

### Comparing `owid_catalog-0.3.8/LICENSE` & `owid_catalog-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.8/README.md` & `owid_catalog-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,16 @@
 t = Table.read_csv('/tmp/my_table.csv')
 ```
 
 ## Changelog
 
 - `dev`
 - `v0.3.8`
+  - Switch from isort & black & fake8 to ruff
+- `v0.3.8`
   - Pin dataclasses-json==0.5.8 to fix error with python3.9
 - `v0.3.7`
   - Fix bugs.
   - Improve metadata propagation.
   - Improve metadata YAML file handling, to have common definitions.
   - Remove `DatasetMeta.origins`.
 - `v0.3.6`
```

### Comparing `owid_catalog-0.3.8/owid/catalog/__init__.py` & `owid_catalog-0.3.9/owid/catalog/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     License,
     Origin,
     Source,
     TableMeta,
     VariableMeta,
     VariablePresentationMeta,
 )
+from .processing_log import LogEntry, ProcessingLog
 from .tables import Table
 from .variables import Variable
 
 __all__ = [
     "LocalCatalog",
     "RemoteCatalog",
     "find",
@@ -25,14 +26,16 @@
     "Dataset",
     "Table",
     "Variable",
     "DatasetMeta",
     "TableMeta",
     "VariableMeta",
     "VariablePresentationMeta",
+    "LogEntry",
+    "ProcessingLog",
     "FaqLink",
     "Source",
     "Origin",
     "License",
     "utils",
     "CHANNEL",
     "processing",
```

### Comparing `owid_catalog-0.3.8/owid/catalog/catalogs.py` & `owid_catalog-0.3.9/owid/catalog/catalogs.py`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.8/owid/catalog/datasets.py` & `owid_catalog-0.3.9/owid/catalog/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 import shutil
 import warnings
 from dataclasses import dataclass
 from glob import glob
 from os import environ
 from os.path import join
 from pathlib import Path
-from typing import Any, Iterator, List, Literal, Optional, Union
+from typing import Iterator, List, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 import yaml
+from _hashlib import HASH
 
 from . import tables, utils
 from .meta import SOURCE_EXISTS_OPTIONS, DatasetMeta, TableMeta
+from .processing_log import disable_processing_log
 from .properties import metadata_property
 
 FileFormat = Literal["csv", "feather", "parquet"]
 
 # the formats we can serialise and deserialise; in some cases they
 # will be tried in this order if we don't specify one explicitly
 SUPPORTED_FORMATS: List[FileFormat] = ["feather", "parquet", "csv"]
@@ -59,14 +61,19 @@
         if isinstance(path, Path):
             self.path = path.as_posix()
         else:
             self.path = path
 
         self.metadata = DatasetMeta.load(self._index_file)
 
+    @property
+    def m(self) -> DatasetMeta:
+        """Metadata alias to save typing."""
+        return self.metadata
+
     @classmethod
     def create_empty(cls, path: Union[str, Path], metadata: Optional["DatasetMeta"] = None) -> "Dataset":
         path = Path(path)
 
         if path.is_dir():
             if not (path / "index.json").exists():
                 raise Exception(f"refuse to overwrite non-dataset dir at: {path}")
@@ -174,16 +181,18 @@
             channel, _, _, _ = parts[-4:]
             if channel in CHANNEL.__args__:  # type: ignore
                 self.metadata.channel = channel
 
         self.metadata.save(self._index_file)
 
         # Update the copy of this datasets metadata in every table in the set.
+        # TODO: this entire part should go away and we should make t.metadata.dataset read only
         for table_name in self.table_names:
-            table = self[table_name]
+            with disable_processing_log():
+                table = self[table_name]
             table.metadata.dataset = self.metadata
             table._save_metadata(join(self.path, table.metadata.checked_name + ".meta.json"))
 
     def update_metadata(
         self,
         metadata_path: Path,
         if_source_exists: SOURCE_EXISTS_OPTIONS = "replace",
@@ -204,15 +213,16 @@
             - "fail": raise an exception if origin already exists
         """
         self.metadata.update_from_yaml(metadata_path, if_source_exists=if_source_exists)
 
         with open(metadata_path) as istream:
             metadata = yaml.safe_load(istream)
             for table_name in metadata.get("tables", {}).keys():
-                table = self[table_name]
+                with disable_processing_log():
+                    table = self[table_name]
                 table.update_metadata_from_yaml(metadata_path, table_name, if_origins_exist=if_origins_exist)
                 table._save_metadata(join(self.path, table.metadata.checked_name + ".meta.json"))
 
     def index(self, catalog_path: Path = Path("/")) -> pd.DataFrame:
         """
         Return a DataFrame describing the contents of this dataset, one row per table.
         """
@@ -294,15 +304,15 @@
 for k in DatasetMeta.__dataclass_fields__:
     if hasattr(Dataset, k):
         raise Exception(f'metadata field "{k}" would overwrite a Dataset built-in')
 
     setattr(Dataset, k, metadata_property(k))
 
 
-def checksum_file(filename: str) -> Any:
+def checksum_file(filename: str) -> HASH:
     "Return the MD5 checksum of a given file."
     chunk_size = 2**20  # 1MB
     checksum = hashlib.md5()
     with open(filename, "rb") as istream:
         chunk = istream.read(chunk_size)
         while chunk:
             checksum.update(chunk)
```

### Comparing `owid_catalog-0.3.8/owid/catalog/meta.py` & `owid_catalog-0.3.9/owid/catalog/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pathlib import Path
 from typing import Any, Dict, List, Literal, NewType, Optional, Union
 
 import mistune
 import pandas as pd
 from dataclasses_json import dataclass_json
 
+from .processing_log import ProcessingLog
 from .utils import pruned_json
 
 SOURCE_EXISTS_OPTIONS = Literal["fail", "append", "replace"]
 
 
 YearDateLatest = NewType("YearDateLatest", str)
 
@@ -240,15 +241,15 @@
     # We keep display for the time being as the "less powerful sibling" of grapherConfig below
     display: Optional[Dict[str, Any]] = None
     additional_info: Optional[Dict[str, Any]] = None  # Only used for internal bookkeeping
 
     # How much processing did we do to this data?
     processing_level: Optional[PROCESSING_LEVELS] = None
     # List of processing steps, in the future autogenerated
-    processing_log: List[Dict[str, Any]] = field(default_factory=list)
+    processing_log: ProcessingLog = field(default_factory=ProcessingLog)
 
     presentation: Optional[VariablePresentationMeta] = None
 
     # A short summary of what was done to process this indicator
     description_processing: Optional[str] = None
 
     # This one is the license that we give the data. Normally it will be empty and then it will
@@ -284,17 +285,15 @@
     def _repr_html_(self):
         # Render a nice display of the table metadata
         record = self.to_dict()
         return """
              <h2 style="margin-bottom: 0em"><pre>{}</pre></h2>
              <p style="font-variant: small-caps; font-family: sans-serif; font-size: 1.5em; color: grey; margin-top: -0.2em; margin-bottom: 0.2em">variable meta</p>
              {}
-        """.format(
-            getattr(self, "_name", None), to_html(record)
-        )
+        """.format(getattr(self, "_name", None), to_html(record))
 
     def copy(self, deep=True) -> "VariableMeta":
         """Return a copy of the VariableMeta object."""
         if not deep:
             return dataclasses.replace(self)
         else:
             return _deepcopy_dataclass(self)
@@ -323,14 +322,16 @@
     sources: List[Source] = field(default_factory=list)
     licenses: List[License] = field(default_factory=list)
     is_public: bool = True
     additional_info: Optional[Dict[str, Any]] = None
     version: Optional[str] = None
     # update period in days
     update_period_days: Optional[str] = None
+    # prohibit redistribution (disable chart download)
+    non_redistributable: bool = False
 
     # an md5 checksum of the ingredients used to make this dataset
     source_checksum: Optional[str] = None
 
     def __hash__(self):
         """Hash that uniquely identifies DatasetMeta."""
         return _hash_dataclass(self)
@@ -456,17 +457,15 @@
         # Render a nice display of the table metadata
         record = self.to_dict()
         short_name = record.pop("short_name")
         return """
              <h2 style="margin-bottom: 0em"><pre>{}</pre></h2>
              <p style="font-variant: small-caps; font-family: sans-serif; font-size: 1.5em; color: grey; margin-top: -0.2em; margin-bottom: 0.2em">table meta</p>
              {}
-        """.format(
-            short_name, to_html(record)
-        )
+        """.format(short_name, to_html(record))
 
     def copy(self, deep=True) -> "TableMeta":
         """Return a copy of the TableMeta object."""
         if not deep:
             return dataclasses.replace(self)
         else:
             return _deepcopy_dataclass(self)
```

### Comparing `owid_catalog-0.3.8/owid/catalog/schemas/table.json` & `owid_catalog-0.3.9/owid/catalog/schemas/table.json`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.8/owid/catalog/schemas/variable.json` & `owid_catalog-0.3.9/owid/catalog/schemas/variable.json`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.8/owid/catalog/tables.py` & `owid_catalog-0.3.9/owid/catalog/tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,23 @@
     overload,
 )
 
 import numpy as np
 import pandas as pd
 import pyarrow
 import pyarrow.parquet as pq
+import rdata
 import structlog
-from owid.repack import repack_frame
 from pandas._typing import FilePath, ReadCsvBuffer, Scalar  # type: ignore
 from pandas.core.series import Series
 from pandas.util._decorators import rewrite_axis_style_signature
 
+from owid.repack import repack_frame
+
+from . import processing_log as pl
 from . import variables
 from .meta import (
     SOURCE_EXISTS_OPTIONS,
     License,
     Origin,
     Source,
     TableMeta,
@@ -399,27 +402,17 @@
                     value.name = key
                 if value.name == variables.UNNAMED_VARIABLE:
                     # Update the variable name, if it had the unnamed variable tag.
                     # Replace all instances of unnamed variables in the processing log by the actual name of the new
                     # variable.
                     # WARNING: This process assumes that all instances of unnamed variable tag correspond to the new
                     #  variable.
-                    variables.update_variable_name(variable=value, name=key)
+                    value.name = key
                 self._fields[key] = value.metadata
-                # TODO: The only reason why we have to check if variables.PROCESSING_LOG is true is the test
-                #   "test_field_access_can_be_typecast". Consider adapting the test and then remove this check.
-                if variables.PROCESSING_LOG and len(value.metadata.processing_log) > 0:
-                    # If a new variable is added to a table, check its last entry in the processing log.
-                    # If the last variable name is different to the name of the new column, add an entry to the log,
-                    # stating that the variable has changed name (from the old to the current one).
-                    last_variable_name = value.metadata.processing_log[-1]["variable"]
-                    if last_variable_name != key:
-                        value.update_log(
-                            parents=[last_variable_name], operation="rename", variable_name=key, inplace=True
-                        )
+                value.update_log(operation="rename", variable=key)
             else:
                 self._fields[key] = VariableMeta()
 
         if self.DEBUG:
             self.check_metadata()
 
     def equals_table(self, table: "Table") -> bool:
@@ -442,42 +435,43 @@
         old_cols = self.all_columns
         new_table = super().rename(*args, **kwargs)
 
         # __setattr__ on columns has already done its job of renaming
         if inplace:
             new_table = self
         else:
+            assert new_table is not None
             # construct new _fields attribute
             fields = {}
             for old_col, new_col in zip(old_cols, new_table.all_columns):
                 fields[new_col] = self._fields[old_col].copy()
 
             new_table._fields = defaultdict(VariableMeta, fields)
 
+        for old_col, new_col in zip(old_cols, new_table.all_columns):
+            # Update processing log.
+            if old_col != new_col:
+                new_table._fields[new_col].processing_log.add_entry(
+                    variable=new_col,
+                    parents=[self._fields[old_col]],
+                    operation="rename",
+                )
+
         if inplace:
             return None
         else:
             return cast(Table, new_table)
 
     def __setattr__(self, name: str, value) -> None:
         # setting columns must rename them
         if name == "columns":
             for old_col, new_col in zip(self.columns, value):
                 if old_col in self._fields:
                     self._fields[new_col] = self._fields.pop(old_col)
 
-                # Update processing log.
-                if old_col != new_col:
-                    self._fields[new_col].processing_log = variables.add_entry_to_processing_log(
-                        processing_log=self._fields[new_col].processing_log,
-                        variable_name=new_col,
-                        parents=[old_col],
-                        operation="rename",
-                    )
-
         super().__setattr__(name, value)
 
     @property
     def all_columns(self) -> List[str]:
         "Return names of all columns in the dataset, including the index."
         combined: List[str] = filter(None, list(self.index.names) + list(self.columns))  # type: ignore
         return combined
@@ -691,68 +685,82 @@
         for c_old, c_new in columns_map.items():
             # if underscoring didn't change anything, don't add title
             if t[c_new].metadata.title is None and c_old != c_new:
                 t[c_new].metadata.title = c_old
 
         return t
 
-    def dropna(self, *args, **kwargs) -> "Table":
-        tb = super().dropna(*args, **kwargs).copy()
+    def dropna(self, *args, **kwargs) -> Optional["Table"]:
+        tb = super().dropna(*args, **kwargs)
+        # inplace returns None
+        if tb is None:
+            return None
+        tb = tb.copy()
         for column in list(tb.all_columns):
-            tb._fields[column].processing_log = variables.add_entry_to_processing_log(
-                processing_log=tb._fields[column].processing_log,
-                variable_name=column,
-                parents=[column],
+            tb._fields[column].processing_log.add_entry(
+                variable=column,
+                parents=[tb.get_column_or_index(column)],
                 operation="dropna",
             )
 
         return cast("Table", tb)
 
     def update_log(
         self,
         operation: str,
         parents: Optional[List[Any]] = None,
         variable_names: Optional[List[str]] = None,
         comment: Optional[str] = None,
-        inplace: bool = False,
-    ) -> Optional["Table"]:
-        return update_log(
-            table=self,
-            operation=operation,
-            parents=parents,
-            variable_names=variable_names,
-            comment=comment,
-            inplace=inplace,  # type: ignore
-        )
+    ) -> "Table":
+        # Append a new entry to the processing log of the required variables.
+        if variable_names is None:
+            # If no variable is specified, assume all (including index columns).
+            variable_names = list(self.all_columns)
+        for column in variable_names:
+            # If parents is not defined, assume the parents are simply the current variable.
+            _parents = parents or [column]
+            # Update (in place) the processing log of current variable.
+            self._fields[column].processing_log.add_entry(
+                variable=column,
+                parents=_parents,
+                operation=operation,
+                comment=comment,
+            )
+        return self
 
     def amend_log(
         self,
-        operation: str,
-        parents: Optional[List[Any]] = None,
         variable_names: Optional[List[str]] = None,
         comment: Optional[str] = None,
-        entry_num: Optional[int] = -1,
-        inplace: bool = False,
-    ) -> Optional["Table"]:
-        return amend_log(
-            table=self,
-            operation=operation,
-            parents=parents,
-            variable_names=variable_names,
-            comment=comment,
-            entry_num=entry_num,
-            inplace=inplace,
-        )
+        operation: Optional[str] = None,
+    ) -> "Table":
+        """Amend operation or comment of the latest processing log entry."""
+        # Append a new entry to the processing log of the required variables.
+        if variable_names is None:
+            # If no variable is specified, assume all (including index columns).
+            variable_names = list(self.all_columns)
+        for column in variable_names:
+            # Update (in place) the processing log of current variable.
+            self._fields[column].processing_log.amend_entry(
+                operation=operation,
+                comment=comment,
+            )
+        return self
 
     def sort_values(self, by: str, *args, **kwargs) -> "Table":
         tb = super().sort_values(by=by, *args, **kwargs).copy()
         for column in list(tb.all_columns):
-            tb._fields[column].processing_log = variables.add_entry_to_processing_log(
-                processing_log=tb._fields[column].processing_log, variable_name=column, parents=[by], operation="sort"
-            )
+            if isinstance(by, str):
+                parents = [by, column]
+            else:
+                parents = by + [column]
+
+            parent_variables = [tb.get_column_or_index(parent) for parent in parents]
+
+            tb._fields[column].processing_log.add_entry(variable=column, parents=parent_variables, operation="sort")
 
         return cast("Table", tb)
 
     def sum(self, *args, **kwargs) -> variables.Variable:
         variable_name = variables.UNNAMED_VARIABLE
         variable = variables.Variable(super().sum(*args, **kwargs), name=variable_name)
         variable.metadata = variables.combine_variables_metadata(
@@ -769,104 +777,95 @@
         )
 
         return variable
 
     def assign(self, *args, **kwargs) -> "Table":
         return super().assign(*args, **kwargs)  # type: ignore
 
-    def __add__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
-        tb = cast(Table, Table(super().__add__(other=other)).copy_metadata(self))
+    @staticmethod
+    def _update_log(tb: "Table", other: Union[Scalar, Series, variables.Variable, "Table"], operation: str) -> None:
         # The following would have a parents only the scalar, not the scalar and the corresponding variable.
         # tb = update_log(table=tb, operation="+", parents=[other], variable_names=tb.columns)
         # Instead, update the processing log of each variable in the table.
         for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="+", variable_name=column
-            )
+            if isinstance(other, pd.DataFrame):
+                parents = [tb[column], other[column]]
+            else:
+                parents = [tb[column], other]
+            tb[column].update_log(parents=parents, operation=operation)
+
+    def __add__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
+        tb = cast(Table, Table(super().__add__(other=other)).copy_metadata(self))
+        self._update_log(tb, other, "+")
         return tb
 
-    def __iadd__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __iadd__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__add__(other)
 
-    def __sub__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __sub__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__sub__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="-", variable_name=column
-            )
+        self._update_log(tb, other, "-")
         return tb
 
-    def __isub__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __isub__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__sub__(other)
 
-    def __mul__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __mul__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__mul__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="*", variable_name=column
-            )
+        self._update_log(tb, other, "*")
         return tb
 
-    def __imul__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __imul__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__mul__(other)
 
-    def __truediv__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __truediv__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__truediv__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="/", variable_name=column
-            )
+        self._update_log(tb, other, "/")
         return tb
 
-    def __itruediv__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __itruediv__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__truediv__(other)
 
-    def __floordiv__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __floordiv__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__floordiv__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="//", variable_name=column
-            )
+        self._update_log(tb, other, "//")
         return tb
 
-    def __ifloordiv__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __ifloordiv__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__floordiv__(other)
 
-    def __mod__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __mod__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__mod__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="%", variable_name=column
-            )
+        self._update_log(tb, other, "%")
         return tb
 
-    def __imod__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __imod__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__mod__(other)
 
-    def __pow__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __pow__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         tb = cast(Table, Table(super().__pow__(other=other)).copy_metadata(self))
-        for column in tb.columns:
-            tb[column] = variables.update_log(
-                variable=tb[column], parents=[column, other], operation="**", variable_name=column
-            )
+        self._update_log(tb, other, "**")
         return tb
 
-    def __ipow__(self, other: Union[Scalar, Series, variables.Variable]) -> "Table":
+    def __ipow__(self, other: Union[Scalar, Series, variables.Variable, "Table"]) -> "Table":
         return self.__pow__(other)
 
     def sort_index(self, *args, **kwargs) -> "Table":
         return super().sort_index(*args, **kwargs)  # type: ignore
 
     def groupby(self, *args, observed=False, **kwargs) -> "TableGroupBy":
         """Groupby that preserves metadata."""
         if observed is False and args:
             by_list = [args[0]] if isinstance(args[0], str) else args[0]
             for by in by_list:
                 if isinstance(by, str):
-                    by_type = self.dtypes[by] if by in self.dtypes else self.index.dtypes[by]  # type: ignore
+                    try:
+                        by_type = self.dtypes[by] if by in self.dtypes else self.index.dtypes[by]  # type: ignore
+                    except AttributeError:
+                        by_type = by
                 elif isinstance(by, pd.Series):
                     by_type = by.dtype
                 else:
                     by_type = "unknown"
                 if isinstance(by_type, str) and by_type == "category":
                     log.warning(
                         f"You're grouping by categorical variable `{by}` without using observed=True. This may lead to unexpected behaviour."
@@ -892,14 +891,28 @@
         """Rename index."""
         column_idx = list(self.index.names)
         column_idx_new = [renames.get(col, col) for col in column_idx]
         tb = self.reset_index().rename(columns=renames)
         tb = tb.set_index(column_idx_new)
         return tb
 
+    def fillna(self, value, **kwargs) -> "Table":
+        """Usual fillna, but, if the object given to fill values with is a table, transfer its metadata to the filled
+        table."""
+        tb = super().fillna(value, **kwargs)
+
+        if type(value) == type(self):
+            for column in tb.columns:
+                if column in value.columns:
+                    tb._fields[column] = variables.combine_variables_metadata(
+                        variables=[tb[column], value[column]], operation="fillna", name=column
+                    )
+
+        return tb
+
 
 def _create_table(df: pd.DataFrame, metadata: TableMeta, fields: Dict[str, VariableMeta]) -> Table:
     """Create a table with metadata."""
     tb = Table(df, metadata=metadata.copy())
     tb._fields = defaultdict(VariableMeta, fields)
     return tb
 
@@ -928,15 +941,24 @@
             def func(*args, **kwargs):
                 """Apply function and return variable with proper metadata."""
                 df = getattr(self.groupby, name)(*args, **kwargs)
                 if df.ndim == 1:
                     # output is series, e.g. `size` function
                     return df
                 else:
-                    return _create_table(df, self.metadata, self._fields)
+                    tb = _create_table(df, self.metadata, self._fields)
+                    if pl.enabled():
+                        for col in tb.columns:
+                            # parents are grouping columns and grouped one
+                            index_parents = [tb.get_column_or_index(n) for n in tb.index.names]
+                            tb[col].update_log(
+                                operation=f"groupby_{name}",
+                                parents=[tb[col]] + index_parents,
+                            )
+                    return tb
 
             self.__annotations__[name] = Callable[..., "Table"]
             return func
         else:
             self.__annotations__[name] = VariableGroupBy
             return VariableGroupBy(getattr(self.groupby, name), name, self._fields[name])
 
@@ -963,14 +985,23 @@
         df = self.groupby.agg(func, *args, **kwargs)
         tb = _create_table(df, self.metadata, self._fields)
 
         # kwargs rename fields
         for new_col, (col, _) in kwargs.items():
             tb._fields[new_col] = self._fields[col]
 
+        if pl.enabled():
+            for col in tb.columns:
+                # parents are grouping columns and grouped one
+                index_parents = [tb.get_column_or_index("b") for n in tb.index.names]
+                tb[col].update_log(
+                    operation=f"agg_{func}",
+                    parents=[tb[col]] + index_parents,
+                )
+
         return tb
 
 
 class VariableGroupBy:
     def __init__(self, groupby: pd.core.groupby.SeriesGroupBy, name: str, metadata: VariableMeta):
         self.groupby = groupby
         self.metadata = metadata
@@ -1219,20 +1250,21 @@
     # Update variable metadata in the new table.
     for column in table.columns:
         if isinstance(values, str):
             column_name = values
         else:
             column_name = column[0]
         variables_to_combine = [data[column_name]]
-        # "column" is a tuple with all column index levels.
+        # variables_to_combine = _extract_variables(data, columns) + _extract_variables(data, values)
+
         # For now, I assume the only metadata we want to propagate is the one of the upper level.
         # Alternatively, we could combine the metadata of the upper level variable with the metadata of the original
         # variable of all subsequent levels.
         column_metadata = variables.combine_variables_metadata(
-            variables=variables_to_combine, operation="pivot", name=column_name
+            variables=variables_to_combine, operation="pivot", name=column
         )
         # Assign metadata of the original variable in the upper level to the new multiindex column.
         # NOTE: This allows accessing the metadata via, e.g. `table[("level_0", "level_1", "level_2")].metadata`,
         # but not via, e.g. `table["level_0"]["level_1"]["level_2"].metadata`.
         # There may be a way to allow for both.
         table[column].metadata = column_metadata
 
@@ -1260,15 +1292,15 @@
     return table
 
 
 def _add_table_and_variables_metadata_to_table(
     table: Table, metadata: Optional[TableMeta], origin: Optional[Origin]
 ) -> Table:
     if metadata is not None:
-        table.metadata = metadata
+        table.metadata = metadata.copy()
         for column in list(table.all_columns):
             if origin:
                 table._fields[column].origins = [origin]
             else:
                 table._fields[column].sources = metadata.dataset.sources  # type: ignore
             table._fields[column].licenses = metadata.dataset.licenses  # type: ignore
     table = update_processing_logs_when_loading_or_creating_table(table=table)
@@ -1282,119 +1314,138 @@
     origin: Optional[Origin] = None,
     underscore: bool = False,
     *args,
     **kwargs,
 ) -> Table:
     table = Table(pd.read_csv(filepath_or_buffer=filepath_or_buffer, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    if isinstance(filepath_or_buffer, (str, Path)):
-        table = update_log(table=table, operation="load", parents=[filepath_or_buffer])
-    else:
-        log.warning("Currently, the processing log cannot be updated unless you pass a path to read_csv.")
-
     return cast(Table, table)
 
 
 def read_fwf(
     filepath_or_buffer: Union[FilePath, ReadCsvBuffer[bytes], ReadCsvBuffer[str]],
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     *args,
     **kwargs,
 ) -> Table:
     table = Table(pd.read_fwf(filepath_or_buffer=filepath_or_buffer, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    if isinstance(filepath_or_buffer, (str, Path)):
-        table = update_log(table=table, operation="load", parents=[filepath_or_buffer])
-    else:
-        log.warning("Currently, the processing log cannot be updated unless you pass a path to read_fwf.")
-
     return cast(Table, table)
 
 
 def read_feather(
     filepath: Union[str, Path],
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     *args,
     **kwargs,
 ) -> Table:
     table = Table(pd.read_feather(filepath, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    table = update_log(table=table, operation="load", parents=[filepath])
-
     return cast(Table, table)
 
 
 def read_excel(
     io: Union[str, Path],
     *args,
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     **kwargs,
 ) -> Table:
     assert not isinstance(kwargs.get("sheet_name"), list), "Argument 'sheet_name' must be a string or an integer."
     table = Table(pd.read_excel(io=io, *args, **kwargs), underscore=underscore)
-    table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
     # Note: Maybe we should include the sheet name in parents.
-    table = update_log(table=table, operation="load", parents=[io], inplace=False)
-
+    table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
     return cast(Table, table)
 
 
 def read_from_records(
     data: Any,
     *args,
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     **kwargs,
 ):
     table = Table(pd.DataFrame.from_records(data=data, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    # NOTE: Parents could be passed as arguments, or extracted from metadata.
-    table = update_log(table=table, operation="load", parents=["local_data"], inplace=False)
-
     return table
 
 
 def read_from_dict(
     data: Dict[Any, Any],
     *args,
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     **kwargs,
 ) -> Table:
     table = Table(pd.DataFrame.from_dict(data=data, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    # NOTE: Parents could be passed as arguments, or extracted from metadata.
-    table = update_log(table=table, operation="load", parents=["local_data"], inplace=False)
-
     return table
 
 
 def read_json(
     path_or_buf: Union[str, Path, IO[AnyStr]],
     metadata: Optional[TableMeta] = None,
     origin: Optional[Origin] = None,
     underscore: bool = False,
     *args,
     **kwargs,
 ) -> Table:
     table = Table(pd.read_json(path_or_buf=path_or_buf, *args, **kwargs), underscore=underscore)
     table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-    if isinstance(path_or_buf, (str, Path)):
-        table = update_log(table=table, operation="load", parents=[path_or_buf])
-    else:
-        log.warning("Currently, the processing log cannot be updated unless you pass a path to read_json.")
+    return cast(Table, table)
+
+
+def read_stata(
+    filepath_or_buffer: Union[str, Path, IO[AnyStr]],
+    metadata: Optional[TableMeta] = None,
+    origin: Optional[Origin] = None,
+    underscore: bool = False,
+    *args,
+    **kwargs,
+) -> Table:
+    table = Table(pd.read_stata(filepath_or_buffer=filepath_or_buffer, *args, **kwargs), underscore=underscore)
+    table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
+    return cast(Table, table)
+
+
+def read_rda(
+    filepath_or_buffer: Union[str, Path, IO[AnyStr]],
+    table_name: str,
+    metadata: Optional[TableMeta] = None,
+    origin: Optional[Origin] = None,
+    underscore: bool = False,
+) -> Table:
+    parsed = rdata.parser.parse_file(filepath_or_buffer)  # type: ignore
+    converted = rdata.conversion.convert(parsed)
+
+    if table_name not in converted:
+        raise ValueError(f"Table {table_name} not found in RDA file.")
+    table = Table(converted[table_name], underscore=underscore)
+    table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
+    return cast(Table, table)
+
+
+def read_rds(
+    filepath_or_buffer: Union[str, Path, IO[AnyStr]],
+    metadata: Optional[TableMeta] = None,
+    origin: Optional[Origin] = None,
+    underscore: bool = False,
+) -> Table:
+    parsed = rdata.parser.parse_file(filepath_or_buffer, extension="rds")  # type: ignore
+    converted = rdata.conversion.convert(parsed)
 
+    table = Table(converted, underscore=underscore)
+    table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
     return cast(Table, table)
 
 
 class ExcelFile(pd.ExcelFile):
     def __init__(self, *args, metadata: Optional[TableMeta] = None, origin: Optional[Origin] = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.metadata = metadata
@@ -1413,17 +1464,14 @@
         origin = origin or self.origin
 
         # Note: Maybe we should include the sheet name in parents.
         df = super().parse(sheet_name=sheet_name, *args, **kwargs)  # type: ignore
         table = Table(df, underscore=underscore, short_name=str(sheet_name))
         if metadata is not None:
             table = _add_table_and_variables_metadata_to_table(table=table, metadata=metadata, origin=origin)
-        # Note: Maybe we should include the sheet name in parents.
-        table = update_log(table=table, operation="load", parents=[self.io], inplace=False)
-
         return table
 
 
 def update_processing_logs_when_loading_or_creating_table(table: Table) -> Table:
     # Add entry to processing log, specifying that each variable was loaded from this table.
     try:
         # If the table comes from an ETL dataset, generate a URI for the table.
@@ -1431,48 +1479,45 @@
         parents = [table_uri]
         operation = "load"
     except (AssertionError, AttributeError):
         # The table doesn't have an uri, which means it was probably created from scratch.
         parents = []
         operation = "create"
 
-    table = _add_processing_log_entry_to_each_variable(table=table, parents=parents, operation=operation)
+    # Add log entries to all columns
+    for column in list(table.all_columns):
+        pl = table._fields[column].processing_log
+
+        # Clear processing log, we're not keeping log from previous channels. It can always be reconstructed
+        # by concatenating processing log of indicators accross channels.
+        pl.clear()
+        pl.add_entry(
+            variable=column,
+            parents=parents,
+            operation=operation,
+        )
 
     return table
 
 
 def update_processing_logs_when_saving_table(table: Table, path: Union[str, Path]) -> Table:
     # Infer the ETL uri from the path where the table will be saved.
     # Note: If the path does not fit the expected format, the result will be an arbitrary path, but it will not raise an
     # error, as long as path is a Path.
     path = Path(path)
     uri = "/".join(path.absolute().parts[-5:-1] + tuple([path.stem]))
-    table = _add_processing_log_entry_to_each_variable(table=table, parents=[uri], operation="save")
 
-    return table
-
-
-def _add_processing_log_entry_to_each_variable(
-    table: Table, parents: List[Any], operation: variables.OPERATION
-) -> Table:
     # Add a processing log entry to each column, including index columns.
     for column in list(table.all_columns):
-        # New entry to add to the processing log.
-        # Note: The function add_entry_to_processing_log receives the argument variable_name, but in the processing log,
-        # the entry has the field "variable" (for simplicity).
-        log_new_entry = {"variable_name": column, "parents": parents, "operation": operation}
-
-        if log_new_entry not in table._fields[column].processing_log:
-            # If the processing log is not empty but the last entry is identical to the one we want to insert, skip, to
-            # avoid storing the same entry multiple times.
-            # This happens for example when saving tables, given that tables are stored in different formats.
-            # Otherwise, append a new entry to the processing log.
-            table._fields[column].processing_log = variables.add_entry_to_processing_log(
-                processing_log=table._fields[column].processing_log, **log_new_entry
-            )
+        table._fields[column].processing_log.add_entry(
+            target=uri,
+            parents=[table._fields[column]],
+            operation="save",
+            variable=column,
+        )
 
     return table
 
 
 def copy_metadata(from_table: Table, to_table: Table, deep=False) -> Table:
     """Copy metadata from a different table to self."""
     tab = Table(pd.DataFrame.copy(to_table, deep=deep), metadata=from_table.metadata.copy())
@@ -1488,102 +1533,14 @@
         elif k in to_table._fields:
             new_fields[k] = to_table._fields[k]
 
     tab._fields = new_fields
     return tab
 
 
-@overload
-def update_log(
-    table: Table,
-    operation: str,
-    parents: Optional[List[Any]] = None,
-    variable_names: Optional[List[str]] = None,
-    comment: Optional[str] = None,
-    inplace: Literal[True] = True,
-) -> None:
-    ...
-
-
-@overload
-def update_log(
-    table: Table,
-    operation: str,
-    parents: Optional[List[Any]] = None,
-    variable_names: Optional[List[str]] = None,
-    comment: Optional[str] = None,
-    inplace: Literal[False] = False,
-) -> Table:
-    ...
-
-
-def update_log(
-    table: Table,
-    operation: str,
-    parents: Optional[List[Any]] = None,
-    variable_names: Optional[List[str]] = None,
-    comment: Optional[str] = None,
-    inplace: bool = False,
-) -> Optional[Table]:
-    if not inplace:
-        table = table.copy()
-
-    # Append a new entry to the processing log of the required variables.
-    if variable_names is None:
-        # If no variable is specified, assume all (including index columns).
-        variable_names = list(table.all_columns)
-    for column in variable_names:
-        # If parents is not defined, assume the parents are simply the current variable.
-        _parents = parents or [column]
-        # Update (in place) the processing log of current variable.
-        table._fields[column].processing_log = variables.add_entry_to_processing_log(
-            processing_log=table._fields[column].processing_log,
-            variable_name=column,
-            parents=_parents,
-            operation=operation,
-            comment=comment,
-        )
-
-    if not inplace:
-        return table
-
-
-def amend_log(
-    table: Table,
-    operation: str,
-    parents: Optional[List[Any]] = None,
-    variable_names: Optional[List[str]] = None,
-    comment: Optional[str] = None,
-    entry_num: Optional[int] = -1,
-    inplace: bool = False,
-) -> Optional[Table]:
-    if not inplace:
-        table = table.copy()
-
-    # Append a new entry to the processing log of the required variables.
-    if variable_names is None:
-        # If no variable is specified, assume all (including index columns).
-        variable_names = list(table.all_columns)
-    for column in variable_names:
-        # If parents is not defined, assume the parents are simply the current variable.
-        _parents = parents or [column]
-        # Update (in place) the processing log of current variable.
-        table._fields[column].processing_log = variables.amend_entry_in_processing_log(
-            processing_log=table._fields[column].processing_log,
-            variable_name=column,
-            parents=_parents,
-            operation=operation,
-            comment=comment,
-            entry_num=entry_num,
-        )
-
-    if not inplace:
-        return table
-
-
 def get_unique_sources_from_tables(tables: List[Table]) -> List[Source]:
     # Make a list of all sources of all variables in all tables.
     sources = sum([table._fields[column].sources for table in tables for column in list(table.all_columns)], [])
 
     # Get unique array of tuples of source fields (respecting the order).
     return pd.unique(sources).tolist()
 
@@ -1661,7 +1618,15 @@
             for i, ix in enumerate(ixs):
                 new_cols.values[ix] = f"{new_cols[ix]}_{i + 1}"
         elif collision == "ignore":
             pass
         else:
             raise NotImplementedError()
     return new_cols
+
+
+def _extract_variables(t: Table, cols: Optional[Union[List[str], str]]) -> List[variables.Variable]:
+    if not cols:
+        return []
+    if isinstance(cols, str):
+        cols = [cols]
+    return [t[col] for col in cols]  # type: ignore
```

### Comparing `owid_catalog-0.3.8/owid/catalog/utils.py` & `owid_catalog-0.3.9/owid/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.8/pyproject.toml` & `owid_catalog-0.3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 [tool.poetry]
 name = "owid-catalog"
-version = "0.3.8"
+version = "0.3.9"
 description = "Core data types used by OWID for managing data."
 authors = ["Our World in Data <tech@ourworldindata.org>"]
 license = "MIT"
 packages = [{ include = "owid" }]
 readme = "README.md"
 repository = "https://github.com/owid/owid-grapher-py"
 homepage = "https://github.com/owid/owid-grapher-py"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1"
+python = ">=3.8.1, <3.12"
 pandas = ">=1.3.3,<2.0"
 jsonschema = ">=3.2.0"
 pyarrow = ">=10.0.1"
 ipdb = ">=0.13.9"
 requests = ">=2.26.0"
 boto3 = ">=1.21.13"
 Unidecode = ">=1.3.4"
-PyYAML = ">=5.4.1"
+PyYAML = ">=6.0.1"
 structlog = ">=21.5.0"
 owid-repack = ">=0.1.1"
-dynamic-yaml = "^1.3.4"
+dynamic-yaml = "^1.3.5"
 mistune = "^3.0.1"
 # higher version causes error in python 3.9 when running
 # from owid import catalog; catalog.find("global_carbon_budget").sort_values("version", ascending=False).iloc[0].load()
 dataclasses-json = "0.5.8"
+rdata = "0.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.2.5"
 pytest-cov = ">=2.12.1"
-black = "22.3.0"
-flake8 = "6.1.0"
 watchdog = ">=2.1.5"
 argh = ">=0.26.2"
-isort = ">=5.12.0"
 # unpinning those would introduce tons of type errors
 pyright = "1.1.288"
 pandas-stubs = "1.2.0.62"
+ruff = "0.1.6"
 
-
-[tool.isort]
-profile = "black"
-# owid is actually first party library, but we need to stay compatible with ETL
-known_third_party = "owid"
-
-[tool.black]
-line-length = 120
+[tool.ruff]
+extend = "../../pyproject.toml"
 
 [tool.pyright]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `owid_catalog-0.3.8/PKG-INFO` & `owid_catalog-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: owid-catalog
-Version: 0.3.8
+Version: 0.3.9
 Summary: Core data types used by OWID for managing data.
 Home-page: https://github.com/owid/owid-grapher-py
 License: MIT
 Author: Our World in Data
 Author-email: tech@ourworldindata.org
-Requires-Python: >=3.8.1
+Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: PyYAML (>=6.0.1)
 Requires-Dist: Unidecode (>=1.3.4)
 Requires-Dist: boto3 (>=1.21.13)
 Requires-Dist: dataclasses-json (==0.5.8)
-Requires-Dist: dynamic-yaml (>=1.3.4,<2.0.0)
+Requires-Dist: dynamic-yaml (>=1.3.5,<2.0.0)
 Requires-Dist: ipdb (>=0.13.9)
 Requires-Dist: jsonschema (>=3.2.0)
 Requires-Dist: mistune (>=3.0.1,<4.0.0)
 Requires-Dist: owid-repack (>=0.1.1)
 Requires-Dist: pandas (>=1.3.3,<2.0)
 Requires-Dist: pyarrow (>=10.0.1)
+Requires-Dist: rdata (==0.9)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: structlog (>=21.5.0)
 Project-URL: Repository, https://github.com/owid/owid-grapher-py
 Description-Content-Type: text/markdown
 
 [![Build status](https://badge.buildkite.com/66cc67fc572120ca97b9ffff288d5d73cb33e019dd70323053.svg)](https://buildkite.com/our-world-in-data/owid-catalog-unit-tests)
 [![PyPI version](https://badge.fury.io/py/owid-catalog.svg)](https://badge.fury.io/py/owid-catalog)
@@ -242,14 +243,16 @@
 t = Table.read_csv('/tmp/my_table.csv')
 ```
 
 ## Changelog
 
 - `dev`
 - `v0.3.8`
+  - Switch from isort & black & fake8 to ruff
+- `v0.3.8`
   - Pin dataclasses-json==0.5.8 to fix error with python3.9
 - `v0.3.7`
   - Fix bugs.
   - Improve metadata propagation.
   - Improve metadata YAML file handling, to have common definitions.
   - Remove `DatasetMeta.origins`.
 - `v0.3.6`
```

