# Comparing `tmp/pyoframe-0.0.4.tar.gz` & `tmp/pyoframe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoframe-0.0.4.tar", last modified: Tue Apr 30 15:00:31 2024, max compression
+gzip compressed data, was "pyoframe-0.0.5.tar", last modified: Fri May 17 09:07:05 2024, max compression
```

## Comparing `pyoframe-0.0.4.tar` & `pyoframe-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:00:31.481448 pyoframe-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-30 15:00:27.000000 pyoframe-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-30 15:00:31.481448 pyoframe-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 15:00:27.000000 pyoframe-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 15:00:27.000000 pyoframe-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:00:31.481448 pyoframe-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:00:31.473447 pyoframe-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:00:31.477448 pyoframe-0.0.4/src/pyoframe/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    32229 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/io_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/model_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-04-30 15:00:27.000000 pyoframe-0.0.4/src/pyoframe/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:00:31.477448 pyoframe-0.0.4/src/pyoframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-30 15:00:31.000000 pyoframe-0.0.4/src/pyoframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 15:00:31.000000 pyoframe-0.0.4/src/pyoframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:00:31.000000 pyoframe-0.0.4/src/pyoframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 15:00:31.000000 pyoframe-0.0.4/src/pyoframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:00:31.000000 pyoframe-0.0.4/src/pyoframe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:00:31.477448 pyoframe-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-30 15:00:27.000000 pyoframe-0.0.4/tests/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-30 15:00:27.000000 pyoframe-0.0.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-30 15:00:27.000000 pyoframe-0.0.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-30 15:00:27.000000 pyoframe-0.0.4/tests/test_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.481773 pyoframe-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 09:07:01.000000 pyoframe-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 09:07:05.481773 pyoframe-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-17 09:07:01.000000 pyoframe-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 09:07:01.000000 pyoframe-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:07:05.481773 pyoframe-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.473773 pyoframe-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/src/pyoframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50583 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/io_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/model_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/user_defined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/src/pyoframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_solver.py
```

### Comparing `pyoframe-0.0.4/LICENSE` & `pyoframe-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.4/PKG-INFO` & `pyoframe-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: pyoframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Blazing fast linear program interface
 Author-email: Bravos Power <dev@bravospower.com>
 Project-URL: Homepage, https://bravos-power.github.io/pyoframe/
 Project-URL: documentation, https://bravos-power.github.io/pyoframe/
 Project-URL: repository, https://github.com/Bravos-Power/pyoframe/
 Project-URL: Issues, https://github.com/Bravos-Power/pyoframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: polars==0.20.13
+Requires-Dist: polars
 Requires-Dist: numpy
 Requires-Dist: pyarrow
 Requires-Dist: pandas
+Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -52,7 +53,13 @@
 ## Contribute
 
 Contributions are welcome! See [`CONTRIBUTE.md`](./CONTRIBUTE.md).
 
 ## Acknowledgments
 
 Martin Staadecker first created this library while working for [Bravos Power](https://www.bravospower.com/) The library takes inspiration from Linopy and Pyomo, two prior libraries for optimization for which we are thankful.
+
+## Troubleshooting Common Errors
+
+### `datatypes of join keys don't match`
+
+Often, this error indicates that two dataframes in your inputs representing the same dimension have different datatypes (e.g. 16bit integer and 64bit integer). This is not allowed and you should ensure for the same dimensions, datatypes are identical.
```

### Comparing `pyoframe-0.0.4/README.md` & `pyoframe-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,13 @@
 ## Contribute
 
 Contributions are welcome! See [`CONTRIBUTE.md`](./CONTRIBUTE.md).
 
 ## Acknowledgments
 
 Martin Staadecker first created this library while working for [Bravos Power](https://www.bravospower.com/) The library takes inspiration from Linopy and Pyomo, two prior libraries for optimization for which we are thankful.
+
+## Troubleshooting Common Errors
+
+### `datatypes of join keys don't match`
+
+Often, this error indicates that two dataframes in your inputs representing the same dimension have different datatypes (e.g. 16bit integer and 64bit integer). This is not allowed and you should ensure for the same dimensions, datatypes are identical.
```

### Comparing `pyoframe-0.0.4/pyproject.toml` & `pyoframe-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoframe"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "Bravos Power", email = "dev@bravospower.com" }]
 description = "Blazing fast linear program interface"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
 ]
-dependencies = ["polars==0.20.13", "numpy", "pyarrow", "pandas"]
+dependencies = ["polars", "numpy", "pyarrow", "pandas", "tqdm"]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
     "isort",
     "pip-tools",
@@ -38,12 +38,18 @@
     "mkdocs-section-index",
     "mkdocs-literate-nav",
 ]
 
 [tool.isort]
 profile = "black"
 
+[tool.coverage.run]
+include = ["src/pyoframe/*"]
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules --ignore=scripts"
+
 [project.urls]
 Homepage = "https://bravos-power.github.io/pyoframe/"
 documentation = "https://bravos-power.github.io/pyoframe/"
 repository = "https://github.com/Bravos-Power/pyoframe/"
 Issues = "https://github.com/Bravos-Power/pyoframe/issues"
```

### Comparing `pyoframe-0.0.4/src/pyoframe/_arithmetic.py` & `pyoframe-0.0.5/src/pyoframe/_arithmetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 
 from pyoframe.constants import (
     COEF_KEY,
     RESERVED_COL_KEYS,
     VAR_KEY,
     UnmatchedStrategy,
     Config,
+    PyoframeError,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pyoframe.constraints import Expression
-
-
-class PyoframeError(Exception):
-    pass
+    from pyoframe.core import Expression
 
 
 def _add_expressions(*expressions: "Expression") -> "Expression":
     try:
         return _add_expressions_core(*expressions)
     except PyoframeError as error:
         raise PyoframeError(
```

### Comparing `pyoframe-0.0.4/src/pyoframe/constants.py` & `pyoframe-0.0.5/src/pyoframe/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 
 MIT License
 """
 
 from dataclasses import dataclass
 from enum import Enum
 import typing
-from typing import Any, Literal, Optional, Union
+from typing import Literal, Optional, Union
 import polars as pl
 
 
 COEF_KEY = "__coeff"
 VAR_KEY = "__variable_id"
 CONSTRAINT_KEY = "__constraint_id"
 SOLUTION_KEY = "solution"
 DUAL_KEY = "dual"
-NAME_COL = "__name"
+RC_COL = "RC"
+SLACK_COL = "slack"
 
 CONST_TERM = 0
 
 RESERVED_COL_KEYS = (
     COEF_KEY,
     VAR_KEY,
     CONSTRAINT_KEY,
     SOLUTION_KEY,
     DUAL_KEY,
-    NAME_COL,
+    RC_COL,
+    SLACK_COL,
 )
 
 
 class _ConfigMeta(type):
     """Metaclass for Config that stores the default values of all configuration options."""
 
     def __init__(cls, name, bases, dct):
@@ -44,14 +46,17 @@
         }
 
 
 class Config(metaclass=_ConfigMeta):
     disable_unmatched_checks: bool = False
     print_float_precision: Optional[int] = 5
     print_uses_variable_names: bool = True
+    # Number of elements to show when printing a set to the console (additional elements are replaced with ...)
+    print_max_set_elements: int = 50
+    enable_is_duplicated_expression_safety_check: bool = False
 
     @classmethod
     def reset_defaults(cls):
         """
         Resets all configuration options to their default values.
         """
         for key, value in cls._defaults.items():
@@ -61,16 +66,16 @@
 class ConstraintSense(Enum):
     LE = "<="
     GE = ">="
     EQ = "="
 
 
 class ObjSense(Enum):
-    MIN = "minimize"
-    MAX = "maximize"
+    MIN = "min"
+    MAX = "max"
 
 
 class VType(Enum):
     CONTINUOUS = "continuous"
     BINARY = "binary"
     INTEGER = "integer"
 
@@ -79,15 +84,15 @@
     UNSET = "not_set"
     DROP = "drop"
     KEEP = "keep"
 
 
 # This is a hack to get the Literal type for VType
 # See: https://stackoverflow.com/questions/67292470/type-hinting-enum-member-value-in-python
-ObjSenseValue = Literal["minimize", "maximize"]
+ObjSenseValue = Literal["min", "max"]
 VTypeValue = Literal["continuous", "binary", "integer"]
 for enum, type in [(ObjSense, ObjSenseValue), (VType, VTypeValue)]:
     assert set(typing.get_args(type)) == {vtype.value for vtype in enum}
 
 
 class ModelStatus(Enum):
     """
@@ -244,37 +249,35 @@
 class Result:
     """
     Result of the optimization.
     """
 
     status: Status
     solution: Optional[Solution] = None
-    solver_model: Optional[Any] = None
 
     def __repr__(self) -> str:
-        solver_model_string = (
-            "not available" if self.solver_model is None else "available"
-        )
-
         res = (
             f"Status: {self.status.status.value}\n"
             f"Termination condition: {self.status.termination_condition.value}\n"
         )
         if self.solution is not None:
             res += (
                 f"Solution: {len(self.solution.primal)} primals, {len(self.solution.dual) if self.solution.dual is not None else 0} duals\n"
                 f"Objective: {self.solution.objective:.2e}\n"
             )
-        res += f"Solver model: {solver_model_string}\n"
 
         return res
 
     def info(self):
         status = self.status
 
         if status.is_ok:
             if status.termination_condition == TerminationCondition.suboptimal:
                 print(f"Optimization solution is sub-optimal: \n{self}\n")
             else:
                 print(f" Optimization successful: \n{self}\n")
         else:
             print(f"Optimization failed: \n{self}\n")
+
+
+class PyoframeError(Exception):
+    pass
```

### Comparing `pyoframe-0.0.4/src/pyoframe/io.py` & `pyoframe-0.0.5/src/pyoframe/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,93 +2,119 @@
 Module containing all import/export functionalities.
 """
 
 from io import TextIOWrapper
 from tempfile import NamedTemporaryFile
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Optional, TypeVar, Union
+from tqdm import tqdm
 
-from pyoframe.constants import VAR_KEY, Config
-from pyoframe.constraints import Constraint
-from pyoframe.variables import Variable
+from pyoframe.constants import CONST_TERM, VAR_KEY, ObjSense
+from pyoframe.core import Constraint, Variable
 from pyoframe.io_mappers import (
     Base62ConstMapper,
     Base62VarMapper,
     IOMappers,
     Mapper,
     NamedMapper,
+    NamedVariableMapper,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyoframe.model import Model
 
 import polars as pl
 
 
 def objective_to_file(m: "Model", f: TextIOWrapper, var_map):
     """
     Write out the objective of a model to a lp file.
     """
-    assert m.objective is not None, "No objective set."
-
-    f.write(f"{m.objective.sense.value}\n\nobj:\n\n")
-    result = m.objective.to_str(var_map=var_map, include_prefix=False)
-    f.writelines(result)
+    if m.objective is None:
+        return
+    objective_sense = "minimize" if m.sense == ObjSense.MIN else "maximize"
+    f.write(f"{objective_sense}\n\nobj:\n\n")
+    result = m.objective.to_str(
+        var_map=var_map, include_prefix=False, include_const_variable=True
+    )
+    f.write(result)
 
 
 def constraints_to_file(m: "Model", f: TextIOWrapper, var_map, const_map):
-    for constraint in create_section(m.constraints, f, "s.t."):
-        f.writelines(constraint.to_str(var_map=var_map, const_map=const_map) + "\n")
+    for constraint in create_section(
+        tqdm(m.constraints, desc="Writing constraints to file"), f, "s.t."
+    ):
+        f.write(constraint.to_str(var_map=var_map, const_map=const_map) + "\n")
 
 
 def bounds_to_file(m: "Model", f, var_map):
     """
     Write out variables of a model to a lp file.
     """
-    for variable in create_section(m.variables, f, "bounds"):
-        lb = f"{variable.lb:.12g}"
-        ub = f"{variable.ub:.12g}"
+    if (m.objective is not None and m.objective.has_constant) or len(m.variables) != 0:
+        f.write("\n\nbounds\n\n")
+    if m.objective is not None and m.objective.has_constant:
+        const_term_df = pl.DataFrame(
+            {VAR_KEY: [CONST_TERM]}, schema={VAR_KEY: pl.UInt32}
+        )
+        f.write(f"{var_map.apply(const_term_df).item()} = 1\n")
+
+    for variable in tqdm(m.variables, desc="Writing bounds to file"):
+        terms = []
+
+        if variable.lb != 0:
+            terms.append(pl.lit(f"{variable.lb:.12g} <= "))
+
+        terms.append(VAR_KEY)
+
+        if variable.ub != float("inf"):
+            terms.append(pl.lit(f" <= {variable.ub:.12g}"))
+
+        terms.append(pl.lit("\n"))
+
+        if len(terms) < 3:
+            continue
 
         df = (
             var_map.apply(variable.data, to_col=None)
-            .select(
-                pl.concat_str(
-                    pl.lit(f"{lb} <= "), VAR_KEY, pl.lit(f" <= {ub}\n")
-                ).str.concat("")
-            )
+            .select(pl.concat_str(terms).str.concat(""))
             .item()
         )
 
-        f.writelines(df)
+        f.write(df)
 
 
 def binaries_to_file(m: "Model", f, var_map: Mapper):
     """
     Write out binaries of a model to a lp file.
     """
-    for variable in create_section(m.binary_variables, f, "binary"):
+    for variable in create_section(
+        tqdm(m.binary_variables, "Writing binary variables to file"), f, "binary"
+    ):
         lines = (
             var_map.apply(variable.data, to_col=None)
             .select(pl.col(VAR_KEY).str.concat("\n"))
             .item()
         )
-        f.writelines(lines + "\n")
+        f.write(lines + "\n")
 
 
 def integers_to_file(m: "Model", f, var_map: Mapper):
     """
     Write out integers of a model to a lp file.
     """
-    for variable in create_section(m.integer_variables, f, "general"):
+    for variable in create_section(
+        tqdm(m.integer_variables, "Writing integer variables to file"), f, "general"
+    ):
         lines = (
             var_map.apply(variable.data, to_col=None)
             .select(pl.col(VAR_KEY).str.concat("\n"))
             .item()
         )
-        f.writelines(lines + "\n")
+        f.write(lines + "\n")
 
 
 T = TypeVar("T")
 
 
 def create_section(iterable: Iterable[T], f, section_header) -> Iterable[T]:
     wrote = False
@@ -99,15 +125,15 @@
         yield item
 
 
 def get_var_map(m: "Model", use_var_names):
     if use_var_names:
         if m.var_map is not None:
             return m.var_map
-        var_map = NamedMapper(Variable)
+        var_map = NamedVariableMapper(Variable)
     else:
         var_map = Base62VarMapper(Variable)
 
     for v in m.variables:
         var_map.add(v)
     return var_map
 
@@ -140,10 +166,10 @@
 
     with open(file_path, mode="w") as f:
         objective_to_file(m, f, var_map)
         constraints_to_file(m, f, var_map, const_map)
         bounds_to_file(m, f, var_map)
         binaries_to_file(m, f, var_map)
         integers_to_file(m, f, var_map)
-        f.write("end\n")
+        f.write("\nend\n")
 
     return file_path
```

### Comparing `pyoframe-0.0.4/src/pyoframe/io_mappers.py` & `pyoframe-0.0.5/src/pyoframe/io_mappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,87 +5,109 @@
 from dataclasses import dataclass
 import math
 import string
 from abc import ABC, abstractmethod
 
 from typing import TYPE_CHECKING, Optional, Type, Union
 import polars as pl
-from pyoframe.constants import NAME_COL
 from pyoframe.util import concat_dimensions
+from pyoframe.constants import CONST_TERM
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyoframe.model import Variable
-    from pyoframe.constraints import Constraint
-    from pyoframe.util import IdCounterMixin
+    from pyoframe.core import Constraint
+    from pyoframe.util import CountableModelElement
 
 
 @dataclass
 class IOMappers:
     var_map: "Mapper"
     const_map: "Mapper"
 
 
 class Mapper(ABC):
-    def __init__(self, cls: Type["IdCounterMixin"]) -> None:
+
+    NAME_COL = "__name"
+
+    def __init__(self, cls: Type["CountableModelElement"]) -> None:
         self._ID_COL = cls.get_id_column_name()
         self.mapping_registry = pl.DataFrame(
-            {self._ID_COL: [], NAME_COL: []},
-            schema={self._ID_COL: pl.UInt32, NAME_COL: pl.String},
+            {self._ID_COL: [], Mapper.NAME_COL: []},
+            schema={self._ID_COL: pl.UInt32, Mapper.NAME_COL: pl.String},
         )
 
     def add(self, element: Union["Variable", "Constraint"]) -> None:
-        self.mapping_registry = pl.concat(
-            [self.mapping_registry, self._element_to_map(element)]
-        )
+        self._extend_registry(self._element_to_map(element))
+
+    def _extend_registry(self, df: pl.DataFrame) -> None:
+        self.mapping_registry = pl.concat([self.mapping_registry, df])
 
     @abstractmethod
-    def _element_to_map(self, element: "IdCounterMixin") -> pl.DataFrame: ...
+    def _element_to_map(self, element: "CountableModelElement") -> pl.DataFrame: ...
 
     def apply(
         self,
         df: pl.DataFrame,
-        to_col: Optional[str],
+        to_col: Optional[str] = None,
     ) -> pl.DataFrame:
+        if df.height == 0:
+            return df
         result = df.join(
             self.mapping_registry, on=self._ID_COL, how="left", validate="m:1"
         )
         if to_col is None:
             result = result.drop(self._ID_COL)
             to_col = self._ID_COL
-        return result.rename({NAME_COL: to_col})
+        return result.rename({Mapper.NAME_COL: to_col})
 
     def undo(self, df: pl.DataFrame) -> pl.DataFrame:
+        if df.height == 0:
+            return df
+        df = df.rename({self._ID_COL: Mapper.NAME_COL})
         return df.join(
-            self.mapping_registry, on=NAME_COL, how="left", validate="m:1"
-        ).drop(NAME_COL)
+            self.mapping_registry, on=Mapper.NAME_COL, how="left", validate="m:1"
+        ).drop(Mapper.NAME_COL)
 
 
 class NamedMapper(Mapper):
     """
     Maps constraints or variables to a string representation using the object's name and dimensions.
 
     Examples:
 
         >>> import polars as pl
         >>> import pyoframe as pf
-        >>> m = pf.Model()
+        >>> m = pf.Model("min")
         >>> m.foo = pf.Variable(pl.DataFrame({"t": range(4)}))
         >>> pf.sum(m.foo)
         <Expression size=1 dimensions={} terms=4>
         foo[0] + foo[1] + foo[2] + foo[3]
     """
 
     def _element_to_map(self, element) -> pl.DataFrame:
         element_name = element.name  # type: ignore
         assert (
             element_name is not None
         ), "Element must have a name to be used in a named mapping."
         return concat_dimensions(
-            element.ids, keep_dims=False, prefix=element_name, to_col=NAME_COL
+            element.ids, keep_dims=False, prefix=element_name, to_col=Mapper.NAME_COL
+        )
+
+
+class NamedVariableMapper(NamedMapper):
+    CONST_TERM_NAME = "_ONE"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self._extend_registry(
+            pl.DataFrame(
+                {self._ID_COL: [CONST_TERM], self.NAME_COL: [self.CONST_TERM_NAME]},
+                schema={self._ID_COL: pl.UInt32, self.NAME_COL: pl.String},
+            )
         )
 
 
 class Base62Mapper(Mapper, ABC):
     # Mapping between a base 62 character and its integer value
     _CHAR_TABLE = pl.DataFrame(
         {"char": list(string.digits + string.ascii_letters)},
@@ -164,24 +186,24 @@
             .select(pl.concat_str(pl.all()))
             .to_series()
             .str.strip_chars_start(cls._ZERO)
             .replace("", cls._ZERO)
         )
 
     def _element_to_map(self, element) -> pl.DataFrame:
-        return self.apply(element.ids.select(self._ID_COL), to_col=NAME_COL)
+        return self.apply(element.ids.select(self._ID_COL), to_col=Mapper.NAME_COL)
 
 
 class Base62VarMapper(Base62Mapper):
     """
     Examples:
         >>> import polars as pl
         >>> from pyoframe import Model, Variable
         >>> from pyoframe.constants import VAR_KEY
-        >>> m = Model()
+        >>> m = Model("min")
         >>> m.x = Variable(pl.DataFrame({"t": range(1,63)}))
         >>> (m.x.filter(t=11)+1).to_str()
         '[11]: 1  + x[11]'
         >>> (m.x.filter(t=11)+1).to_str(var_map=Base62VarMapper(Variable))
         '[11]: 1  + xb'
 
         >>> Base62VarMapper(Variable).apply(pl.DataFrame({VAR_KEY: []}))
@@ -190,14 +212,23 @@
         │ __variable_id │
         │ ---           │
         │ null          │
         ╞═══════════════╡
         └───────────────┘
     """
 
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        df = pl.DataFrame(
+            {self._ID_COL: [CONST_TERM]},
+            schema={self._ID_COL: pl.UInt32},
+        )
+        df = self.apply(df, to_col=Mapper.NAME_COL)
+        self._extend_registry(df)
+
     @property
     def _prefix(self) -> "str":
         return "x"
 
 
 class Base62ConstMapper(Base62Mapper):
```

### Comparing `pyoframe-0.0.4/src/pyoframe/monkey_patch.py` & `pyoframe-0.0.5/src/pyoframe/monkey_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import polars as pl
-from pyoframe.constraints import SupportsMath
-from pyoframe.constraints import Expression
+from pyoframe.core import SupportsMath
+from pyoframe.core import Expression
 from functools import wraps
 
 from pyoframe.constants import COEF_KEY, CONST_TERM, VAR_KEY
 
 # pyright: reportAttributeAccessIssue=false
```

### Comparing `pyoframe-0.0.4/src/pyoframe/objective.py` & `pyoframe-0.0.5/src/pyoframe/objective.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from typing import Optional, Union
-from pyoframe.constants import ObjSense, ObjSenseValue
-from pyoframe.constraints import SupportsMath, Expression
+from typing import Optional
+from pyoframe.constants import COEF_KEY
+from pyoframe.core import SupportsMath, Expression
 
 
 class Objective(Expression):
     r"""
     Examples:
         >>> from pyoframe import Variable, Model, sum
-        >>> m = Model()
+        >>> m = Model("max")
         >>> m.a = Variable()
         >>> m.b = Variable({"dim1": [1, 2, 3]})
-        >>> m.maximize = m.a + sum("dim1", m.b)
-        >>> m.maximize
+        >>> m.objective = m.a + sum("dim1", m.b)
+        >>> m.objective
         <Objective size=1 dimensions={} terms=4>
-        maximize: a + b[1] + b[2] + b[3]
+        objective: a + b[1] + b[2] + b[3]
     """
 
-    def __init__(
-        self, expr: SupportsMath, sense: Union[ObjSense, ObjSenseValue]
-    ) -> None:
-        self.sense = ObjSense(sense)
-
+    def __init__(self, expr: SupportsMath) -> None:
         expr = expr.to_expr()
-        super().__init__(expr.to_expr().data)
+        super().__init__(expr.data)
         self._model = expr._model
         assert (
             self.dimensions is None
         ), "Objective cannot have dimensions as it must be a single expression"
         self._value: Optional[float] = None
 
     @property
@@ -36,7 +32,14 @@
                 "Objective value is not available before solving the model"
             )
         return self._value
 
     @value.setter
     def value(self, value):
         self._value = value
+
+    @property
+    def has_constant(self):
+        constant_terms = self.constant_terms
+        if len(constant_terms) == 0:
+            return False
+        return constant_terms.get_column(COEF_KEY).item() != 0
```

### Comparing `pyoframe-0.0.4/src/pyoframe/util.py` & `pyoframe-0.0.5/src/pyoframe/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,22 @@
 """
 File containing utility functions and classes.
 """
 
-from abc import abstractmethod, ABC
-from collections import defaultdict
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import Any, Iterable, Optional, Union, List, Dict
+
+from dataclasses import dataclass, field
 
 import polars as pl
 import pandas as pd
+from functools import wraps
 
 from pyoframe.constants import COEF_KEY, CONST_TERM, RESERVED_COL_KEYS, VAR_KEY
 
 
-class IdCounterMixin(ABC):
-    """
-    Provides a method that assigns a unique ID to each row in a DataFrame.
-    IDs start at 1 and go up consecutively. No zero ID is assigned since it is reserved for the constant variable term.
-    IDs are only unique for the subclass since different subclasses have different counters.
-    """
-
-    # Keys are the subclass names and values are the next unasigned ID.
-    _id_counters: Dict[str, int] = defaultdict(lambda: 1)
-
-    @classmethod
-    def _reset_counters(cls):
-        """
-        Resets all the ID counters.
-        This function is called before every unit test to reset the code state.
-        """
-        cls._id_counters = defaultdict(lambda: 1)
-
-    def _assign_ids(self, df: pl.DataFrame) -> pl.DataFrame:
-        """
-        Adds the column `to_column` to the DataFrame `df` with the next batch
-        of unique consecutive IDs.
-        """
-        cls_name = self.__class__.__name__
-        cur_count = self._id_counters[cls_name]
-        id_col_name = self.get_id_column_name()
-
-        if df.height == 0:
-            df = df.with_columns(pl.lit(cur_count).alias(id_col_name))
-        else:
-            df = df.with_columns(
-                pl.int_range(cur_count, cur_count + pl.len()).alias(id_col_name)
-            )
-        df = df.with_columns(pl.col(id_col_name).cast(pl.UInt32))
-        self._id_counters[cls_name] += df.height
-        return df
-
-    @classmethod
-    @abstractmethod
-    def get_id_column_name(cls) -> str:
-        """
-        Returns the name of the column containing the IDs.
-        """
-
-    @property
-    @abstractmethod
-    def ids(self) -> pl.DataFrame:
-        """
-        Returns a dataframe with the IDs and any other relevant columns (i.e. the dimension columns).
-        """
-
-
 def get_obj_repr(obj: object, _props: Iterable[str] = (), **kwargs):
     """
     Helper function to generate __repr__ strings for classes. See usage for examples.
     """
     props = {prop: getattr(obj, prop) for prop in _props}
     props_str = " ".join(f"{k}={v}" for k, v in props.items() if v is not None)
     if props_str:
@@ -265,7 +214,59 @@
             .alias(column_name)
         )
     else:
         df = df.with_columns(pl.col(column_name).cast(pl.Utf8))
     return df.with_columns(pl.concat_str("_sign", column_name).alias(column_name)).drop(
         "_sign"
     )
+
+
+def unwrap_single_values(func):
+    """Decorator for functions that return DataFrames. Returned dataframes with a single value will instead return the value."""
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        if isinstance(result, pl.DataFrame) and result.shape == (1, 1):
+            return result.item()
+        return result
+
+    return wrapper
+
+
+def dataframe_to_tupled_list(
+    df: pl.DataFrame, num_max_elements: Optional[int] = None
+) -> str:
+    """
+    Converts a dataframe into a list of tuples. Used to print a Set to the console. See examples for behaviour.
+
+    Examples:
+        >>> df = pl.DataFrame({"x": [1, 2, 3, 4, 5]})
+        >>> dataframe_to_tupled_list(df)
+        '[1, 2, 3, 4, 5]'
+        >>> dataframe_to_tupled_list(df, 3)
+        '[1, 2, 3, ...]'
+
+        >>> df = pl.DataFrame({"x": [1, 2, 3, 4, 5], "y": [2, 3, 4, 5, 6]})
+        >>> dataframe_to_tupled_list(df, 3)
+        '[(1, 2), (2, 3), (3, 4), ...]'
+    """
+    elipse = False
+    if num_max_elements is not None:
+        if len(df) > num_max_elements:
+            elipse = True
+            df = df.head(num_max_elements)
+
+    res = (row for row in df.iter_rows())
+    if len(df.columns) == 1:
+        res = (row[0] for row in res)
+
+    res = str(list(res))
+    if elipse:
+        res = res[:-1] + ", ...]"
+    return res
+
+
+@dataclass
+class FuncArgs:
+    args: List
+    kwargs: Dict = field(default_factory=dict)
```

### Comparing `pyoframe-0.0.4/src/pyoframe.egg-info/PKG-INFO` & `pyoframe-0.0.5/src/pyoframe.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: pyoframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Blazing fast linear program interface
 Author-email: Bravos Power <dev@bravospower.com>
 Project-URL: Homepage, https://bravos-power.github.io/pyoframe/
 Project-URL: documentation, https://bravos-power.github.io/pyoframe/
 Project-URL: repository, https://github.com/Bravos-Power/pyoframe/
 Project-URL: Issues, https://github.com/Bravos-Power/pyoframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: polars==0.20.13
+Requires-Dist: polars
 Requires-Dist: numpy
 Requires-Dist: pyarrow
 Requires-Dist: pandas
+Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -52,7 +53,13 @@
 ## Contribute
 
 Contributions are welcome! See [`CONTRIBUTE.md`](./CONTRIBUTE.md).
 
 ## Acknowledgments
 
 Martin Staadecker first created this library while working for [Bravos Power](https://www.bravospower.com/) The library takes inspiration from Linopy and Pyomo, two prior libraries for optimization for which we are thankful.
+
+## Troubleshooting Common Errors
+
+### `datatypes of join keys don't match`
+
+Often, this error indicates that two dataframes in your inputs representing the same dimension have different datatypes (e.g. 16bit integer and 64bit integer). This is not allowed and you should ensure for the same dimensions, datatypes are identical.
```

### Comparing `pyoframe-0.0.4/src/pyoframe.egg-info/SOURCES.txt` & `pyoframe-0.0.5/src/pyoframe.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 src/pyoframe/__init__.py
 src/pyoframe/_arithmetic.py
 src/pyoframe/constants.py
-src/pyoframe/constraints.py
+src/pyoframe/core.py
 src/pyoframe/io.py
 src/pyoframe/io_mappers.py
 src/pyoframe/model.py
 src/pyoframe/model_element.py
 src/pyoframe/monkey_patch.py
 src/pyoframe/objective.py
 src/pyoframe/solvers.py
+src/pyoframe/user_defined.py
 src/pyoframe/util.py
-src/pyoframe/variables.py
 src/pyoframe.egg-info/PKG-INFO
 src/pyoframe.egg-info/SOURCES.txt
 src/pyoframe.egg-info/dependency_links.txt
 src/pyoframe.egg-info/requires.txt
 src/pyoframe.egg-info/top_level.txt
 tests/test_arithmetic.py
 tests/test_examples.py
 tests/test_io.py
-tests/test_operations.py
+tests/test_operations.py
+tests/test_solver.py
```

### Comparing `pyoframe-0.0.4/tests/test_arithmetic.py` & `pyoframe-0.0.5/tests/test_arithmetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import re
 import pandas as pd
 import numpy as np
 import pytest
 from pyoframe._arithmetic import PyoframeError
-from pyoframe.constraints import Constraint, Set
 from polars.testing import assert_frame_equal
 import polars as pl
 
-from pyoframe.constants import COEF_KEY, CONST_TERM, VAR_KEY, Config
-from pyoframe import Variable
-from pyoframe.constraints import Expression, sum
+from pyoframe.constants import COEF_KEY, CONST_TERM, VAR_KEY
+from pyoframe import Variable, Model, sum, Set, Config, Expression, VType
 from .util import csvs_to_expr
 
 
 def test_set_multiplication():
     dim1 = [1, 2, 3]
     dim2 = ["a", "b"]
     assert_frame_equal(Set(x=dim1, y=dim2).data, (Set(x=dim1) * Set(y=dim2)).data)
@@ -23,16 +21,24 @@
     dim1 = [1, 2, 3]
     dim2 = ["a", "b"]
     with pytest.raises(AssertionError, match="columns in common"):
         Set(x=dim1) * Set(x=dim2)
 
 
 def test_set_addition():
-    with pytest.raises(ValueError, match="Cannot add two sets"):
-        Set(x=[1, 2, 3]) + Set(x=[1, 2, 3])
+    with pytest.raises(
+        PyoframeError,
+        match=re.escape(
+            "Failed to add sets 'unnamed' and 'unnamed' because dimensions do not match (['x'] != ['y'])"
+        ),
+    ):
+        Set(x=[1, 2, 3]) + Set(y=[2, 3, 4])
+
+    added_set = Set(x=[1, 2, 3]) + Set(x=[2, 3, 4])
+    assert added_set.data.to_dict(as_series=False) == {"x": [1, 2, 3, 4]}
 
 
 def test_multiplication_no_common_dimensions():
     val_1 = pl.DataFrame({"dim1": [1, 2, 3], "value": [1, 2, 3]}).to_expr()
     val_2 = pl.DataFrame({"dim2": ["a", "b"], "value": [1, 2]}).to_expr()
     result = val_1 * val_2
     assert_frame_equal(
@@ -79,17 +85,16 @@
         check_dtype=False,
     )
 
 
 def test_filter_constraint():
     const = pl.DataFrame({"dim1": [1, 2, 3], "value": [1, 2, 3]}).to_expr() >= 0
     result = const.filter(dim1=2)
-    assert isinstance(result, Constraint)
     assert_frame_equal(
-        result.data,
+        result,
         pl.DataFrame({"dim1": [2], COEF_KEY: [2], VAR_KEY: [CONST_TERM]}),
         check_dtype=False,
     )
 
 
 def test_filter_variable():
     v = Variable(pl.DataFrame({"dim1": [1, 2, 3]}))
@@ -111,15 +116,15 @@
         ]
         constraint = 5 <= df.to_expr()
 
         expected_df = pd.DataFrame({"dim1": [1, 2], "value": [1, 2]}).set_index("dim1")[
             "value"
         ]
         expected_constraint = 5 <= expected_df.to_expr()
-        assert constraint == expected_constraint
+        assert str(constraint) == str(expected_constraint)
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
 
 # Matrix of possibilities
 # Has multiple dimensions (dim:yes, no)
@@ -434,7 +439,22 @@
             "Dataframe has unmatched values. If this is intentional, use .drop_unmatched() or .keep_unmatched()"
         ),
     ):
         sum("dim1", expr1 + expr2.keep_unmatched()) + expr3
 
     result = sum("dim1", expr1 + expr2.keep_unmatched()) + expr3.drop_unmatched()
     assert str(result) == "[1]: 10"
+
+
+def test_variable_equals():
+    m = Model("max")
+    index = Set(x=[1, 2, 3])
+    m.Choose = Variable(index, vtype=VType.BINARY)
+    with pytest.raises(
+        AssertionError,
+        match=re.escape("Cannot specify both 'equals' and 'indexing_sets'"),
+    ):
+        m.Choose100 = Variable(index, equals=100 * m.Choose)
+    m.Choose100 = Variable(equals=100 * m.Choose)
+    m.objective = sum(m.Choose100)
+    m.solve(log_to_console=False)
+    assert m.objective.value == 300
```

### Comparing `pyoframe-0.0.4/tests/test_examples.py` & `pyoframe-0.0.5/tests/test_examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from dataclasses import dataclass
 import importlib
 import shutil
 import pytest
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Optional, Tuple, Dict, Any
 
 import polars as pl
 from polars.testing import assert_frame_equal
 
 
 @dataclass
 class Example:
     folder_name: str
     integer_results_only: bool = False
     many_valid_solutions: bool = False
     has_gurobi_version: bool = True
+    check_params: Optional[Dict[str, Any]] = None
 
 
 EXAMPLES = [
     Example("diet_problem"),
-    Example("facility_problem"),
+    Example("facility_problem", check_params={"Method": 2}),
     Example(
         "cutting_stock_problem",
         integer_results_only=True,
         many_valid_solutions=True,
         has_gurobi_version=False,
     ),
 ]
@@ -44,24 +45,30 @@
 
     # Dynamically import the main function of the example
     main_module = importlib.import_module(f"tests.examples.{example.folder_name}.model")
 
     symbolic_solution_file = symbolic_output_dir / "pyoframe-problem.sol"
     dense_solution_file = dense_output_dir / "pyoframe-problem.sol"
 
-    dense_result = main_module.main(
-        input_dir, directory=dense_output_dir, solution_file=dense_solution_file
-    )
-    symbolic_result = main_module.main(
+    symbolic_model = main_module.main(
         input_dir,
         directory=symbolic_output_dir,
         solution_file=symbolic_solution_file,
         use_var_names=True,
     )
-    assert dense_result.objective.value == symbolic_result.objective.value
+    dense_model = main_module.main(
+        input_dir, directory=dense_output_dir, solution_file=dense_solution_file
+    )
+
+    if example.check_params is not None:
+        for param, value in example.check_params.items():
+            assert getattr(dense_model.solver_model.Params, param) == value
+            assert getattr(symbolic_model.solver_model.Params, param) == value
+
+    assert dense_model.objective.value == symbolic_model.objective.value
     check_results_dir_equal(
         expected_output_dir,
         symbolic_output_dir,
         check_solution_equal=not example.many_valid_solutions,
     )
     check_results_dir_equal(
         dense_output_dir,
@@ -130,15 +137,17 @@
     actual_result = parse_gurobi_sol(actual_sol_file)
 
     tol = 1e-8
     for (expected_name, expected_value), (actual_name, actual_value) in zip(
         expected_result, actual_result
     ):
         assert expected_name == actual_name
-        assert expected_value - tol <= actual_value <= expected_value + tol
+        assert (
+            expected_value - tol <= actual_value <= expected_value + tol
+        ), f"Solution file does not match expected values {expected_sol_file}"
 
 
 def parse_gurobi_sol(sol_file_path) -> List[Tuple[str, float]]:
     with open(sol_file_path) as f:
         sol = f.readlines()
     sol = [line.strip() for line in sol]
     sol = [line for line in sol if not (line.startswith("#") or line == "")]
```

### Comparing `pyoframe-0.0.4/tests/test_io.py` & `pyoframe-0.0.5/tests/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pytest
 import polars as pl
-from polars.testing import assert_frame_equal
 
-from pyoframe.variables import Variable
-from pyoframe.constraints import Expression
+from pyoframe.core import Expression, Variable
 
 
 @pytest.fixture
 def expression_with_dimensions():
     df = pl.DataFrame(
         {
             "x": [1, 2, 1, 2],
```

### Comparing `pyoframe-0.0.4/tests/test_operations.py` & `pyoframe-0.0.5/tests/test_operations.py`

 * *Files identical despite different names*

