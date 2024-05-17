# Comparing `tmp/nipype2pydra-0.3.5.tar.gz` & `tmp/nipype2pydra-0.4.0.tar.gz`

## Comparing `nipype2pydra-0.3.5.tar` & `nipype2pydra-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,59 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/_version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/exceptions.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/testing.py
--rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/base.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/pkg_gen.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/task.py
--rw-r--r--   0        0        0    44133 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/afni-qwarp-only.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/example-packages.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fastsurfer-only.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/freesurfer-mris-convert-only.yaml
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/freesurfer-only.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fsl-filmgls-only.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fsl-only.yaml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/mriqc.yaml
--rw-r--r--   0        0        0    16673 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/nipype-interfaces-to-import.yaml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/qsiprep.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/NOTICE
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/README.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/pkg_init.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/__init__.py
--rw-r--r--   0        0        0    38808 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/base.py
--rw-r--r--   0        0        0    16701 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/function.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/shell_command.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/tests/test_task.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/tests/test_pkg_gen.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/tests/test_utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/LICENSE
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/README.rst
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/_version.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/exceptions.py
+-rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/helpers.py
+-rw-r--r--   0        0        0    40316 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/package.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/testing.py
+-rw-r--r--   0        0        0    45837 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/workflow.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/cli/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/cli/base.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/cli/convert.py
+-rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/cli/pkg_gen.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/__init__.py
+-rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/base.py
+-rw-r--r--   0        0        0    16959 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/function.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/loaders.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/shell_command.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/compute_dvars.yaml
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/non_steady_state_detector_callables.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/tsnr.yaml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/nipype-ports/tsnr_callables.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/interface/tests/test_interface.py
+-rw-r--r--   0        0        0    45492 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/NOTICE
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/README.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/init.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/pkg_gen/tests/test_pkg_gen.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/statements/__init__.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/statements/imports.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/statements/misc.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/statements/utility.py
+-rw-r--r--   0        0        0    31670 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/statements/workflow_build.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/tests/test_package.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/utils/__init__.py
+-rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/utils/misc.py
+-rw-r--r--   0        0        0    23704 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/utils/symbols.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/utils/tests/test_utils_imports.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/nipype2pydra/utils/tests/test_utils_misc.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/README.rst
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    22538 2020-02-02 00:00:00.000000 nipype2pydra-0.4.0/PKG-INFO
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/testing.py` & `nipype2pydra-0.4.0/nipype2pydra/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def test_line_number_of_function():
+def for_testing_line_number_of_function():
     """Test function used to test the detection of a line number of a function."""
     return 1
 
 
 import logging  # noqa: E402
 import asyncio  # noqa: E402
 from pydra.engine.core import Result, TaskBase  # noqa: E402
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/utils.py` & `nipype2pydra-0.4.0/nipype2pydra/utils/symbols.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,637 +1,546 @@
-import traceback
 import typing as ty
-from types import ModuleType
-import sys
 import re
-import os
+import keyword
+import types
 import inspect
 import builtins
-from contextlib import contextmanager
+from operator import attrgetter
+from collections import defaultdict
+from logging import getLogger
+from importlib import import_module
 import attrs
-from pathlib import Path
-from fileformats.core import FileSet
-from .exceptions import UnmatchedParensException
 from nipype.interfaces.base import BaseInterface, TraitedSpec, isdefined, Undefined
 from nipype.interfaces.base import traits_extension
-
-try:
-    from typing import GenericAlias
-except ImportError:
-    from typing import _GenericAlias as GenericAlias
-
-from importlib import import_module
-from logging import getLogger
+from .misc import split_source_into_statements, extract_args
+from ..statements.imports import ImportStatement, parse_imports
 
 
 logger = getLogger("nipype2pydra")
 
 
-INBUILT_NIPYPE_TRAIT_NAMES = [
-    "__all__",
-    "args",
-    "trait_added",
-    "trait_modified",
-    "environ",
-    "output_type",
-]
-
-
-def load_class_or_func(location_str):
-    module_str, name = location_str.split(":")
-    module = import_module(module_str)
-    return getattr(module, name)
-
-
-def show_cli_trace(result):
-    return "".join(traceback.format_exception(*result.exc_info))
-
-
-def import_module_from_path(module_path: ty.Union[ModuleType, Path, str]) -> ModuleType:
-    if isinstance(module_path, ModuleType) or module_path is None:
-        return module_path
-    module_path = Path(module_path).resolve()
-    sys.path.insert(0, str(module_path.parent))
-    try:
-        return import_module(module_path.stem)
-    finally:
-        sys.path.pop(0)
-
-
-@contextmanager
-def set_cwd(path):
-    """Sets the current working directory to `path` and back to original
-    working directory on exit
-
-    Parameters
-    ----------
-    path : str
-        The file system path to set as the current working directory
-    """
-    pwd = os.getcwd()
-    os.chdir(path)
-    try:
-        yield path
-    finally:
-        os.chdir(pwd)
-
-
-@contextmanager
-def add_to_sys_path(path: Path):
-    """Adds the given `path` to the Python system path and then reverts it back to the
-    original value on exit
-
-    Parameters
-    ----------
-    path : str
-        The file system path to add to the system path
-    """
-    sys.path.insert(0, str(path))
-    try:
-        yield sys.path
-    finally:
-        sys.path.pop(0)
-
-
-def is_fileset(tp: type):
-    return (
-        inspect.isclass(tp) and type(tp) is not GenericAlias and issubclass(tp, FileSet)
-    )
-
-
-def to_snake_case(name: str) -> str:
-    """
-    Converts a PascalCase string to a snake_case one
-    """
-    snake_str = ""
-
-    # Loop through each character in the input string
-    for i, char in enumerate(name):
-        # If the current character is uppercase and it's not the first character or
-        # followed by another uppercase character, add an underscore before it and
-        # convert it to lowercase
-        if (
-            i > 0
-            and (char.isupper() or char.isdigit())
-            and (
-                not (name[i - 1].isupper() or name[i - 1].isdigit())
-                or (
-                    (i + 1) < len(name)
-                    and (name[i + 1].islower() or name[i + 1].islower())
-                )
-            )
-        ):
-            snake_str += "_"
-            snake_str += char.lower()
-        else:
-            # Otherwise, just add the character as it is
-            snake_str += char.lower()
-
-    return snake_str
-
-
-def add_exc_note(e, note):
-    """Adds a note to an exception in a Python <3.11 compatible way
-
-    Parameters
-    ----------
-    e : Exception
-        the exception to add the note to
-    note : str
-        the note to add
-
-    Returns
-    -------
-    Exception
-        returns the exception again
-    """
-    if hasattr(e, "add_note"):
-        e.add_note(note)
-    else:
-        e.args = (e.args[0] + "\n" + note,)
-    return e
-
-
-def extract_args(snippet) -> ty.Tuple[str, ty.List[str], str]:
-    """Splits the code snippet at the first opening parenthesis/bracket into a 3-tuple
-    consisting of the preceding text + opening paren/bracket, the arguments/items
-    within the parenthesis/bracket pair, and the closing paren/bracket + trailing text.
-
-    Quotes and escaped characters are handled correctly, and the function can be used
-    to split on either parentheses or brackets. The only limitation is that raw strings
-    are not supported.
-
-    Parameters
-    ----------
-    snippet: str
-        the code snippet to split on the first opening parenthesis/bracket to its matching
-        closing parenthesis/bracket
-
-    Returns
-    -------
-    pre: str
-        the opening parenthesis/bracket and preceding text
-    args: list[str]
-        the arguments supplied to the callable/signature
-    post: str
-        the closing parenthesis/bracket and trailing text
-
-    Raises
-    ------
-    UnmatchedParensException
-        if the first parenthesis/bracket in the snippet is unmatched
-    """
-    splits = re.split(
-        r"(\(|\)|\[|\]|'|\"|\\\(|\\\)|\\\[|\\\]|\\'|\\\")",
-        snippet,
-        flags=re.MULTILINE | re.DOTALL,
-    )
-    quote_types = ["'", '"']
-    pre = "".join(splits[:2])
-    contents = []
-    matching = {")": "(", "]": "["}
-    open = ["(", "["]
-    close = [")", "]"]
-    depth = {p: 0 for p in open}
-    next_item = ""
-    if splits[1] in quote_types:
-        first = None  # which bracket/parens type was opened initially (and signifies)
-        inquote = splits[1]
-    else:
-        first = splits[1]
-        depth[first] += 1  # Open the first bracket/parens type
-        inquote = None
-    for i, s in enumerate(splits[2:], start=2):
-        if not s:
-            continue
-        if s[0] == "\\":
-            next_item += s
-            continue
-        if s in quote_types:
-            if inquote is None:
-                inquote = s
-            elif inquote == s:
-                inquote = None
-            next_item += s
-            continue
-        if inquote:
-            next_item += s
-            continue
-        if s in open:
-            depth[s] += 1
-            next_item += s
-            if first is None:
-                first = s
-                pre += next_item
-                next_item = ""
-        else:
-            if s in close:
-                matching_open = matching[s]
-                depth[matching_open] -= 1
-                if matching_open == first and depth[matching_open] == 0:
-                    if next_item:
-                        contents.append(next_item)
-                    return pre, contents, "".join(splits[i:])
-            if (
-                first
-                and depth[first] == 1
-                and "," in s
-                and all(d == 0 for b, d in depth.items() if b != first)
-            ):
-                parts = [p.strip() for p in s.split(",")]
-                if parts:
-                    next_item += parts[0]
-                    next_item = next_item.strip()
-                    if next_item:
-                        contents.append(next_item)
-                    contents.extend(parts[1:-1])
-                    next_item = parts[-1] if len(parts) > 1 else ""
-                else:
-                    next_item = ""
-            else:
-                next_item += s
-    raise UnmatchedParensException(f"Unmatched parenthesis found in '{snippet}'")
-
-
 @attrs.define
 class UsedSymbols:
     """
     A class to hold the used symbols in a module
 
     Parameters
     -------
-    used_imports : list[str]
+    imports : list[str]
         the import statements that need to be included in the converted file
-    funcs_to_include: list[tuple[str, callable]]
-        list of objects (e.g. classes, functions and variables) that are defined
-        in neighbouring modules that need to be included in the converted file
-        (as opposed of just imported from independent packages) along with the name
-        that they were imported as and therefore should be named as in the converted
-        module
-    used_local_functions: set[callable]
+    local_functions: set[callable]
         locally-defined functions used in the function bodies, or nested functions thereof
-    used_constants: set[tuple[str, str]]
+    local_classes : set[type]
+        like local_functions but classes
+    constants: set[tuple[str, str]]
         constants used in the function bodies, or nested functions thereof, tuples consist
         of the constant name and its definition
+    intra_pkg_funcs: set[tuple[str, callable]]
+        list of functions that are defined in neighbouring modules that need to be
+        included in the converted file (as opposed of just imported from independent
+        packages) along with the name that they were imported as and therefore should
+        be named as in the converted module if they are included inline
+    intra_pkg_classes: list[tuple[str, callable]]
+        like neigh_mod_funcs but classes
+    intra_pkg_constants: set[tuple[str, str, str]]
+        set of all the constants defined within the package that are referenced by the
+        function, (<path of the module>, <constant name>, <local-name>), where
+        the local alias and the definition of the constant
     """
 
+    module_name: str
     imports: ty.Set[str] = attrs.field(factory=set)
-    funcs_to_include: ty.Set[ty.Tuple[str, ty.Callable]] = attrs.field(factory=set)
-    classes_to_include: ty.List[ty.Tuple[str, ty.Callable]] = attrs.field(factory=list)
     local_functions: ty.Set[ty.Callable] = attrs.field(factory=set)
     local_classes: ty.List[type] = attrs.field(factory=list)
     constants: ty.Set[ty.Tuple[str, str]] = attrs.field(factory=set)
+    intra_pkg_funcs: ty.Set[ty.Tuple[str, ty.Callable]] = attrs.field(factory=set)
+    intra_pkg_classes: ty.List[ty.Tuple[str, ty.Callable]] = attrs.field(factory=list)
+    intra_pkg_constants: ty.Set[ty.Tuple[str, str, str]] = attrs.field(factory=set)
 
-    IGNORE_MODULES = [
+    ALWAYS_OMIT_MODULES = [
         "traits.trait_handlers",  # Old traits module, pre v6.0
+        "nipype.pipeline",
+        "nipype.logging",
+        "nipype.config",
+        "nipype.interfaces.base",
+        "nipype.interfaces.utility",
     ]
 
-    def update(self, other: "UsedSymbols"):
-        self.imports.update(other.imports)
-        self.funcs_to_include.update(other.funcs_to_include)
-        self.funcs_to_include.update((f.__name__, f) for f in other.local_functions)
-        self.classes_to_include.extend(
-            c for c in other.classes_to_include if c not in self.classes_to_include
+    _cache = {}
+
+    symbols_re = re.compile(r"(?<!\"|')\b([a-zA-Z\_][\w\.]*)\b(?!\"|')")
+
+    def update(
+        self,
+        other: "UsedSymbols",
+        absolute_imports: bool = False,
+        to_be_inlined: bool = False,
+    ):
+        if to_be_inlined:
+            self.imports.update(
+                i.absolute() if absolute_imports else i for i in other.imports
+            )
+        self.intra_pkg_funcs.update(other.intra_pkg_funcs)
+        self.intra_pkg_funcs.update((None, f) for f in other.local_functions)
+        self.intra_pkg_classes.extend(
+            c for c in other.intra_pkg_classes if c not in self.intra_pkg_classes
         )
-        self.classes_to_include.extend(
-            (c.__name__, c)
+        self.intra_pkg_classes.extend(
+            (None, c)
             for c in other.local_classes
-            if (c.__name__, c) not in self.classes_to_include
+            if (None, c) not in self.intra_pkg_classes
         )
-        self.constants.update(other.constants)
+        self.intra_pkg_constants.update(
+            (other.module_name, None, c[0]) for c in other.constants
+        )
+        self.intra_pkg_constants.update(other.intra_pkg_constants)
+
+    DEFAULT_FILTERED_CONSTANTS = (
+        Undefined,
+        traits_extension.File,
+        traits_extension.Directory,
+    )
+
+    DEFAULT_FILTERED_FUNCTIONS = (isdefined,)
 
     @classmethod
     def find(
         cls,
-        module,
-        function_bodies: ty.List[str],
+        module: types.ModuleType,
+        function_bodies: ty.List[ty.Union[str, ty.Callable, ty.Type]],
+        collapse_intra_pkg: bool = False,
+        pull_out_inline_imports: bool = True,
+        omit_constants: list = DEFAULT_FILTERED_CONSTANTS,
+        omit_functions: ty.Sequence = DEFAULT_FILTERED_FUNCTIONS,
+        omit_classes: ty.Optional[ty.List[ty.Type]] = None,
+        omit_modules: ty.Optional[ty.List[str]] = None,
+        always_include: ty.Optional[ty.List[str]] = None,
+        translations: ty.Optional[ty.Sequence[ty.Tuple[str, str]]] = None,
+        absolute_imports: bool = False,
     ) -> "UsedSymbols":
-        """Get the imports required for the function body
+        """Get the imports and local functions/classes/constants referenced in the
+        provided function bodies, and those nested within them
 
         Parameters
         ----------
         module: ModuleType
             the module containing the functions to be converted
-        function_bodies: list[str]
-            the source of all functions that need to be checked for used imports
+        function_bodies: list[str | callable | type]
+            the source of all functions/classes (or the functions/classes themselves)
+            that need to be checked for used imports
+        collapse_intra_pkg : bool
+            whether functions and classes defined within the same package, but not the
+            same module, are to be included in the output module or not, i.e. whether
+            the local funcs/classes/constants they referenced need to be included also
+        pull_out_inline_imports : bool, optional
+            whether to pull out imports that are inline in the function bodies
+            or not, by default True
+        omit_constants : list, optional
+            a list of objects to filter out from the used symbols,
+            by default (Undefined, traits_extension.File, traits_extension.Directory)
+        omit_functions : list[type], optional
+            a list of functions to filter out from the used symbols,
+            by default [isdefined]
+        omit_classes : list[type], optional
+            a list of classes (including subclasses) to filter out from the used symbols,
+            by default None
+        always_include : list[str], optional
+            a list of module objects (e.g. functions, classes, etc...) to always include
+            in list of used imports, even if they would be normally filtered out by
+            one of the `omit` clauses, by default None
+        translations : list[tuple[str, str]], optional
+            a list of tuples where the first element is the name of the symbol to be
+            replaced and the second element is the name of the symbol to replace it with,
+            regex supported, by default None
+        absolute_imports : bool, optional
+            whether to convert relative imports to absolute imports, by default False
 
         Returns
         -------
         UsedSymbols
             a class containing the used symbols in the module
         """
-        used = cls()
-        imports = [
-            "import attrs",
-            "from fileformats.generic import File, Directory",
-            "import logging",
-        ]  # attrs is included in imports in case we reference attrs.NOTHING
-        block = ""
+        if omit_classes is None:
+            omit_classes = []
+        if omit_modules is None:
+            omit_modules = []
+        if always_include is None:
+            always_include = []
+        if isinstance(module, str):
+            module = import_module(module)
+        cache_key = (
+            module.__name__,
+            tuple(f.__name__ if not isinstance(f, str) else f for f in function_bodies),
+            collapse_intra_pkg,
+            pull_out_inline_imports,
+            tuple(omit_constants) if omit_constants else None,
+            tuple(omit_functions) if omit_functions else None,
+            tuple(omit_classes) if omit_classes else None,
+            tuple(omit_modules) if omit_modules else None,
+            tuple(always_include) if always_include else None,
+            tuple(translations) if translations else None,
+        )
+        try:
+            return cls._cache[cache_key]
+        except KeyError:
+            pass
+        used = cls(module_name=module.__name__)
+        cls._cache[cache_key] = used
         source_code = inspect.getsource(module)
-        local_functions = get_local_functions(module)
-        local_constants = get_local_constants(module)
-        local_classes = get_local_classes(module)
-        for line in source_code.split("\n"):
-            if block:
-                block += line.strip()
-                if ")" in line:
-                    imports.append(block)
-                    block = ""
-            elif re.match(r"^\s*(from[\w \.]+)?import\b[\w \.\,\(\)]+$", line):
-                if "(" in line and ")" not in line:
-                    block = line.strip()
-                else:
-                    imports.append(line.strip())
-        # extract imported symbols from import statements
-        symbols_re = re.compile(r"(?<!\"|')\b(\w+)\b(?!\"|')")
-        comments_re = re.compile(r"\s*#.*")
+        # Sort local func/classes/consts so they are iterated in a consistent order to
+        # remove stochastic element of traversal and make debugging easier
+        local_functions = sorted(
+            get_local_functions(module), key=attrgetter("__name__")
+        )
+        local_constants = sorted(get_local_constants(module))
+        local_classes = sorted(get_local_classes(module), key=attrgetter("__name__"))
+        module_statements = split_source_into_statements(source_code)
+        imports: ty.List[ImportStatement] = []
+        global_scope = True
+        for stmt in module_statements:
+            if not pull_out_inline_imports:
+                if stmt.startswith("def ") or stmt.startswith("class "):
+                    global_scope = False
+                    continue
+                if not global_scope:
+                    if stmt and not stmt.startswith(" "):
+                        global_scope = True
+                    else:
+                        continue
+            if ImportStatement.matches(stmt):
+                imports.extend(
+                    parse_imports(
+                        stmt,
+                        relative_to=module,
+                        translations=translations,
+                        absolute=absolute_imports,
+                    )
+                )
+        imports = sorted(imports)
+
+        all_src = ""  # All the source code that is searched for symbols
+
         used_symbols = set()
         for function_body in function_bodies:
-            # Strip comments from function body
-            function_body = comments_re.sub("", function_body)
-            used_symbols.update(symbols_re.findall(function_body))
-        # Keep looping through local function source until all local functions and constants
-        # are added to the used symbols
-        new_symbols = True
-        while new_symbols:
-            new_symbols = False
+            if not isinstance(function_body, str):
+                function_body = inspect.getsource(function_body)
+            all_src += "\n\n" + function_body
+            cls._get_symbols(function_body, used_symbols)
+
+        # Keep stepping into nested referenced local function/class sources until all local
+        # functions and constants that are referenced are added to the used symbols
+        prev_num_symbols = -1
+        while len(used_symbols) > prev_num_symbols:
+            prev_num_symbols = len(used_symbols)
             for local_func in local_functions:
                 if (
                     local_func.__name__ in used_symbols
                     and local_func not in used.local_functions
                 ):
                     used.local_functions.add(local_func)
-                    func_body = inspect.getsource(local_func)
-                    func_body = comments_re.sub("", func_body)
-                    local_func_symbols = symbols_re.findall(func_body)
-                    used_symbols.update(local_func_symbols)
-                    new_symbols = True
+                    cls._get_symbols(local_func, used_symbols)
+                    all_src += "\n\n" + inspect.getsource(local_func)
             for local_class in local_classes:
                 if (
                     local_class.__name__ in used_symbols
                     and local_class not in used.local_classes
                 ):
                     if issubclass(local_class, (BaseInterface, TraitedSpec)):
                         continue
                     used.local_classes.append(local_class)
                     class_body = inspect.getsource(local_class)
                     bases = extract_args(class_body)[1]
                     used_symbols.update(bases)
-                    class_body = comments_re.sub("", class_body)
-                    local_class_symbols = symbols_re.findall(class_body)
-                    used_symbols.update(local_class_symbols)
-                    new_symbols = True
+                    cls._get_symbols(class_body, used_symbols)
+                    all_src += "\n\n" + class_body
             for const_name, const_def in local_constants:
                 if (
                     const_name in used_symbols
                     and (const_name, const_def) not in used.constants
                 ):
                     used.constants.add((const_name, const_def))
-                    const_def_symbols = symbols_re.findall(const_def)
-                    used_symbols.update(const_def_symbols)
-                    new_symbols = True
-        used_symbols -= set(cls.SYMBOLS_TO_IGNORE)
-
-        pkg_name = module.__name__.split(".", 1)[0]
-
-        def is_pkg_import(mod_name: str) -> bool:
-            return mod_name.startswith(".") or mod_name.startswith(f"{pkg_name}.")
+                    cls._get_symbols(const_def, used_symbols)
+                    all_src += "\n\n" + const_def
+            used_symbols -= set(cls.SYMBOLS_TO_IGNORE)
+
+        base_pkg = module.__name__.split(".")[0]
+
+        module_omit_re = re.compile(
+            r"^\b("
+            + "|".join(cls.ALWAYS_OMIT_MODULES + [module.__name__] + omit_modules)
+            + r")\b",
+        )
 
         # functions to copy from a relative or nipype module into the output module
         for stmt in imports:
-            stmt = stmt.replace("\n", "")
-            stmt = stmt.replace("(", "")
-            stmt = stmt.replace(")", "")
-            base_stmt, symbol_str = stmt.split("import ")
-            symbol_parts = re.split(r" *, *", symbol_str)
-            split_parts = [re.split(r" +as +", p) for p in symbol_parts]
-            used_parts = [p for p in split_parts if p[-1] in used_symbols]
-            if used_parts:
-                required_stmt = (
-                    base_stmt
-                    + "import "
-                    + ", ".join(" as ".join(p) for p in used_parts)
-                )
-                match = re.match(r"\s*from ([\w\.]+)", base_stmt)
-                import_mod = match.group(1) if match else ""
-                if import_mod in cls.IGNORE_MODULES:
-                    continue
-                if import_mod:
-                    if is_pkg_import(import_mod):
-                        to_include = True
-                        if import_mod.startswith("."):
-                            match = re.match(r"(\.*)(.*)", import_mod)
-                            mod_parts = module.__name__.split(".")
-                            nparents = len(match.group(1))
-                            if Path(module.__file__).stem == "__init__":
-                                nparents -= 1
-                            if nparents:
-                                mod_parts = mod_parts[:-nparents]
-                            mod_name = ".".join(mod_parts)
-                            if match.group(2):
-                                mod_name += "." + match.group(2)
-                        elif import_mod.startswith("nipype."):
-                            mod_name = import_mod
-                        else:
-                            assert False
-                    else:
-                        to_include = False
-                        mod_name = import_mod
-                    mod = import_module(mod_name)
-                    # Filter out any interfaces that have been dragged in
-                    used_parts = [
-                        p
-                        for p in used_parts
-                        if not (
+            stmt = stmt.only_include(used_symbols)
+            # Skip if no required symbols are in the import statement
+            if not stmt:
+                continue
+            # Filter out Nipype-specific objects that aren't relevant in Pydra
+            module_omit = bool(module_omit_re.match(stmt.module_name))
+            if module_omit or omit_classes or omit_functions or omit_constants:
+                to_include = []
+                for imported in stmt.values():
+                    if imported.address in always_include:
+                        to_include.append(imported.local_name)
+                        continue
+                    if module_omit:
+                        continue
+                    try:
+                        obj = imported.object
+                    except ImportError:
+                        logger.warning(
                             (
-                                inspect.isclass(getattr(mod, p[0]))
-                                and issubclass(
-                                    getattr(mod, p[0]), (BaseInterface, TraitedSpec)
-                                )
-                            )
-                            or getattr(mod, p[0])
-                            in (
-                                Undefined,
-                                isdefined,
-                                traits_extension.File,
-                                traits_extension.Directory,
-                            )
+                                "Could not import %s from %s, unable to check whether "
+                                "it is is present in list of classes %s or objects %s "
+                                "to be filtered out"
+                            ),
+                            imported.name,
+                            imported.statement.module_name,
+                            omit_classes,
+                            omit_functions,
                         )
-                    ]
-                    if not used_parts:
+                        to_include.append(imported.local_name)
                         continue
-                    if to_include:
-                        mod_func_bodies = []
-                        for used_part in used_parts:
-                            atr = getattr(mod, used_part[0])
-                            # Check that it is actually a local import
-                            if (
-                                inspect.isfunction(atr) or inspect.isclass(atr)
-                            ) and not is_pkg_import(atr.__module__):
-                                used.imports.add(
-                                    f"from {atr.__module__} import "
-                                    + " as ".join(used_part)
+                    if inspect.isclass(obj):
+                        if omit_classes and issubclass(obj, tuple(omit_classes)):
+                            continue
+                    elif inspect.isfunction(obj):
+                        if omit_functions and obj in omit_functions:
+                            continue
+                    elif imported.address in omit_constants:
+                        continue
+                    to_include.append(imported.local_name)
+                if not to_include:
+                    continue
+                stmt = stmt.only_include(to_include)
+            intra_pkg_objs = defaultdict(set)
+            if stmt.in_package(base_pkg) or (
+                stmt.in_package("nipype") and not stmt.in_package("nipype.interfaces")
+            ):
+
+                for imported in list(stmt.values()):
+                    if not (
+                        imported.in_package(base_pkg) or imported.in_package("nipype")
+                    ) or inspect.isbuiltin(imported.object):
+                        # Case where an object is a nested import from a different package
+                        # which is imported in a chain from a neighbouring module
+                        used.imports.add(
+                            imported.as_independent_statement(resolve=True)
+                        )
+                        stmt.drop(imported)
+                    elif inspect.isfunction(imported.object):
+                        used.intra_pkg_funcs.add((imported.local_name, imported.object))
+                        # Recursively include objects imported in the module
+                        intra_pkg_objs[import_module(imported.object.__module__)].add(
+                            imported.object
+                        )
+                        if collapse_intra_pkg:
+                            stmt.drop(imported)
+                    elif inspect.isclass(imported.object):
+                        class_def = (imported.local_name, imported.object)
+                        # Add the class to the intra_pkg_classes list if it is not
+                        # already there. NB: we can't use a set for intra_pkg_classes
+                        # like we did for functions here because we need to preserve the
+                        # order the classes are defined in the module in case one inherits
+                        # from the other
+                        if class_def not in used.intra_pkg_classes:
+                            used.intra_pkg_classes.append(class_def)
+                        # Recursively include objects imported in the module
+                        intra_pkg_objs[import_module(imported.object.__module__)].add(
+                            imported.object,
+                        )
+                        if collapse_intra_pkg:
+                            stmt.drop(imported)
+                    elif inspect.ismodule(imported.object):
+                        # Skip if the module is the same as the module being converted
+                        if module_omit_re.match(imported.object.__name__):
+                            stmt.drop(imported)
+                            continue
+                        # Findall references to the module's attributes in the source code
+                        # and add them to the list of intra package objects
+                        used_attrs = re.findall(
+                            r"\b" + imported.local_name + r"\.(\w+)\b", all_src
+                        )
+                        for attr_name in used_attrs:
+                            obj = getattr(imported.object, attr_name)
+
+                            if inspect.isfunction(obj):
+                                used.intra_pkg_funcs.add((obj.__name__, obj))
+                                intra_pkg_objs[imported.object.__name__].add(obj)
+                            elif inspect.isclass(obj):
+                                class_def = (obj.__name__, obj)
+                                if class_def not in used.intra_pkg_classes:
+                                    used.intra_pkg_classes.append(class_def)
+                                intra_pkg_objs[imported.object.__name__].add(obj)
+                            else:
+                                used.intra_pkg_constants.add(
+                                    (
+                                        imported.object.__name__,
+                                        attr_name,
+                                        attr_name,
+                                    )
                                 )
-                            elif inspect.isfunction(atr):
-                                used.funcs_to_include.add((used_part[-1], atr))
-                                mod_func_bodies.append(inspect.getsource(atr))
-                            elif inspect.isclass(atr):
-                                if issubclass(atr, BaseInterface):
-                                    # TODO: add warning here
-                                    continue  # Don't include nipype interfaces as it gets silly
-                                # We can't use a set here because we need to preserve the order
-                                class_def = (used_part[-1], atr)
-                                if class_def not in used.classes_to_include:
-                                    used.classes_to_include.append(class_def)
-                                class_body = extract_args(inspect.getsource(atr))[
-                                    2
-                                ].split("\n", 1)[1]
-                                mod_func_bodies.append(class_body)
-                        # Recursively include neighbouring objects imported in the module
-                        if mod is not builtins:
-                            used_in_mod = cls.find(
-                                mod,
-                                function_bodies=mod_func_bodies,
+                                intra_pkg_objs[imported.object.__name__].add(attr_name)
+
+                        if collapse_intra_pkg:
+                            raise NotImplementedError(
+                                f"Cannot inline imported module in statement '{stmt}'"
                             )
-                            used.update(used_in_mod)
                     else:
-                        used.imports.add(required_stmt)
-                else:
-                    used.imports.add(required_stmt)
+                        used.intra_pkg_constants.add(
+                            (
+                                stmt.module_name,
+                                imported.local_name,
+                                imported.name,
+                            )
+                        )
+                        intra_pkg_objs[stmt.module].add(imported.local_name)
+                        if collapse_intra_pkg:
+                            stmt.drop(imported)
+
+            # Recursively include neighbouring objects imported in the module
+            for from_mod, inlined_objs in intra_pkg_objs.items():
+                used_in_mod = cls.find(
+                    from_mod,
+                    function_bodies=inlined_objs,
+                    collapse_intra_pkg=collapse_intra_pkg,
+                    translations=translations,
+                    omit_modules=omit_modules,
+                    omit_classes=omit_classes,
+                    omit_functions=omit_functions,
+                    omit_constants=omit_constants,
+                    always_include=always_include,
+                )
+                used.update(used_in_mod, to_be_inlined=collapse_intra_pkg)
+            if stmt:
+                used.imports.add(stmt)
         return used
 
-    SYMBOLS_TO_IGNORE = ["isdefined"]
+    @classmethod
+    def filter_imports(
+        cls, imports: ty.List[ImportStatement], source_code: str
+    ) -> ty.List[ImportStatement]:
+        """Filter out the imports that are not used in the function bodies"""
+        symbols = set()
+        cls._get_symbols(source_code, symbols)
+        symbols -= set(cls.SYMBOLS_TO_IGNORE)
+        filtered = []
+        for stmt in imports:
+            if stmt.from_:
+                stmt = stmt.only_include(symbols)
+                if stmt:
+                    filtered.append(stmt)
+            elif stmt.sole_imported.local_name in symbols:
+                filtered.append(stmt)
+        return filtered
+
+    def copy(self) -> "UsedSymbols":
+        return attrs.evolve(self)
+
+    @classmethod
+    def _get_symbols(
+        cls, func: ty.Union[str, ty.Callable, ty.Type], symbols: ty.Set[str]
+    ):
+        """Get the symbols used in a function body"""
+        try:
+            fbody = inspect.getsource(func)
+        except TypeError:
+            fbody = func
+        for stmt in split_source_into_statements(fbody):
+            if stmt and not re.match(
+                r"\s*(#|\"|'|from |import |r'|r\"|f'|f\")", stmt
+            ):  # skip comments/docs
+                for sym in cls.symbols_re.findall(stmt):
+                    if "." in sym:
+                        parts = sym.split(".")
+                        symbols.update(
+                            ".".join(parts[: i + 1]) for i in range(len(parts))
+                        )
+                    else:
+                        symbols.add(sym)
+
+    # Nipype-specific names and Python keywords
+    SYMBOLS_TO_IGNORE = ["isdefined"] + keyword.kwlist + list(builtins.__dict__.keys())
+
+    def get_imported_object(self, name: str) -> ty.Any:
+        """Get the object with the given name from used import statements
 
+        Parameters
+        ----------
+        name : str
+            the name of the object to get
+        imports : list[ImportStatement], optional
+            the import statements to search in (used in tests), by default the imports
+            in the used symbols
+
+        Returns
+        -------
+        Any
+            the object with the given name referenced by the given import statements
+        """
+        # Check to see if it isn't an imported module
+        # imported = {
+        #     i.sole_imported.local_name: i.sole_imported.object
+        #     for i in self.imports
+        #     if not i.from_
+        # }
+        all_imported = {}
+        for stmt in self.imports:
+            all_imported.update(stmt.imported)
+        try:
+            return all_imported[name].object
+        except KeyError:
+            pass
+        parts = name.rsplit(".")
+        imported_obj = None
+        for i in range(1, len(parts)):
+            obj_name = ".".join(parts[:-i])
+            try:
+                imported_obj = all_imported[obj_name].object
+            except KeyError:
+                continue
+            else:
+                break
+        if imported_obj is None:
+            raise ImportError(
+                f"Could not find object named {name} in any of the imported modules:\n"
+                + "\n".join(str(i) for i in self.imports)
+            )
+        for part in parts[-i:]:
+            imported_obj = getattr(imported_obj, part)
+        return imported_obj
 
-def get_local_functions(mod):
+
+def get_local_functions(mod) -> ty.List[ty.Callable]:
     """Get the functions defined in the module"""
     functions = []
     for attr_name in dir(mod):
         attr = getattr(mod, attr_name)
         if inspect.isfunction(attr) and attr.__module__ == mod.__name__:
             functions.append(attr)
     return functions
 
 
-def get_local_classes(mod):
+def get_local_classes(mod) -> ty.List[type]:
     """Get the functions defined in the module"""
     classes = []
     for attr_name in dir(mod):
         attr = getattr(mod, attr_name)
         if inspect.isclass(attr) and attr.__module__ == mod.__name__:
             classes.append(attr)
     return classes
 
 
-def get_local_constants(mod):
+def get_local_constants(mod) -> ty.List[ty.Tuple[str, str]]:
     """
     Get the constants defined in the module
     """
     source_code = inspect.getsource(mod)
     source_code = source_code.replace("\\\n", " ")
-    parts = re.split(r"^(\w+) *= *", source_code, flags=re.MULTILINE)
     local_vars = []
-    for attr_name, following in zip(parts[1::2], parts[2::2]):
-        first_line = following.splitlines()[0]
-        if ("(" in first_line and ")" not in first_line) or (
-            "[" in first_line and "]" not in first_line
-        ):
-            pre, args, post = extract_args(following)
-            local_vars.append(
-                (attr_name, pre + re.sub(r"\n *", "", ", ".join(args)) + post[0])
-            )
-        else:
-            local_vars.append((attr_name, first_line))
+    for stmt in split_source_into_statements(source_code):
+        match = re.match(r"^(\w+) *= *(.*)", stmt, flags=re.MULTILINE | re.DOTALL)
+        if match:
+            local_vars.append(tuple(match.groups()))
     return local_vars
-
-
-def cleanup_function_body(function_body: str) -> str:
-    """Ensure 4-space indentation and replace isdefined
-    with the attrs.NOTHING constant
-
-    Parameters
-    ----------
-    function_body: str
-        The source code of the function to process
-    with_signature: bool, optional
-        whether the function signature is included in the source code, by default False
-
-    Returns
-    -------
-    function_body: str
-        The processed source code
-    """
-    if re.match(r"(\s*#.*\n)?(\s*@.*\n)*\s*(def|class)\s+", function_body):
-        with_signature = True
-    else:
-        with_signature = False
-    # Detect the indentation of the source code in src and reduce it to 4 spaces
-    indents = re.findall(r"^( *)[^\s].*\n", function_body, flags=re.MULTILINE)
-    min_indent = min(len(i) for i in indents) if indents else 0
-    indent_reduction = min_indent - (0 if with_signature else 4)
-    assert indent_reduction >= 0, (
-        "Indentation reduction cannot be negative, probably didn't detect signature of "
-        f"method correctly:\n{function_body}"
-    )
-    if indent_reduction:
-        function_body = re.sub(
-            r"^" + " " * indent_reduction, "", function_body, flags=re.MULTILINE
-        )
-    # Other misc replacements
-    # function_body = function_body.replace("LOGGER.", "logger.")
-    parts = re.split(r"not isdefined\b", function_body, flags=re.MULTILINE)
-    new_function_body = parts[0]
-    for part in parts[1:]:
-        pre, args, post = extract_args(part)
-        new_function_body += pre + f"{args[0]} is attrs.NOTHING" + post
-    function_body = new_function_body
-    parts = re.split(r"isdefined\b", function_body, flags=re.MULTILINE)
-    new_function_body = parts[0]
-    for part in parts[1:]:
-        pre, args, post = extract_args(part)
-        assert len(args) == 1, f"Unexpected number of arguments in isdefined: {args}"
-        new_function_body += pre + f"{args[0]} is not attrs.NOTHING" + post
-    function_body = new_function_body
-    function_body = function_body.replace("_Undefined", "attrs.NOTHING")
-    function_body = function_body.replace("Undefined", "attrs.NOTHING")
-    return function_body
-
-
-def insert_args_in_signature(snippet: str, new_args: ty.Iterable[str]) -> str:
-    """Insert the arguments into a function signature
-
-    Parameters
-    ----------
-    snippet: str
-        the function signature to modify
-    new_args: list[str]
-        the arguments to insert into the signature
-
-    Returns
-    -------
-    str
-        the modified function signature
-    """
-    # Split out the argstring from the rest of the code snippet
-    pre, args, post = extract_args(snippet)
-    if "runtime" in args:
-        args.remove("runtime")
-    return pre + ", ".join(args + new_args) + post
-
-
-def get_source_code(func_or_klass: ty.Union[ty.Callable, ty.Type]) -> str:
-    """Get the source code of a function or class, including a comment with the
-    original source location
-    """
-    src = inspect.getsource(func_or_klass)
-    line_number = inspect.getsourcelines(func_or_klass)[1]
-    module = inspect.getmodule(func_or_klass)
-    rel_module_path = os.path.sep.join(
-        module.__name__.split(".")[1:-1] + [Path(module.__file__).name]
-    )
-    install_placeholder = f"<{module.__name__.split('.', 1)[0]}-install>"
-    indent = re.match(r"^(\s*)", src).group(1)
-    comment = (
-        f"{indent}# Original source at L{line_number} of "
-        f"{install_placeholder}{os.path.sep}{rel_module_path}\n"
-    )
-    return comment + src
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/__init__.py` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,33 @@
 import fileformats.core.mixin
 from fileformats.generic import File, Directory
 from fileformats.medimage import Nifti1, NiftiGz, Bval, Bvec
 from fileformats.application import Dicom, Xml
 from fileformats.text import TextFile
 from fileformats.datascience import TextMatrix, DatFile
 import nipype.interfaces.base.core
-from nipype2pydra.task import (
+from nipype.interfaces.base import BaseInterface, TraitedSpec
+from nipype2pydra.package import (  # noqa F401  required to avoid partial import
+    PackageConverter,
+)
+from nipype2pydra.interface import (
     InputsConverter,
     OutputsConverter,
     TestGenerator,
     DocTestGenerator,
 )
 from nipype2pydra.utils import (
     UsedSymbols,
     extract_args,
     get_source_code,
     cleanup_function_body,
     insert_args_in_signature,
     INBUILT_NIPYPE_TRAIT_NAMES,
 )
+from nipype2pydra.statements import parse_imports
 from nipype2pydra.exceptions import UnmatchedParensException
 
 
 TEMPLATES_DIR = Path(__file__).parent.parent / "pkg_gen" / "resources" / "templates"
 
 EXPECTED_FORMATS = [Nifti1, NiftiGz, TextFile, TextMatrix, DatFile, Xml]
 
@@ -102,15 +107,18 @@
     unmatched_formats: ty.List[str] = attrs.field(factory=list)
     ambiguous_formats: ty.List[str] = attrs.field(factory=list)
     pkg_formats: ty.Set[str] = attrs.field(factory=set)
     has_doctests: bool = False
 
     @classmethod
     def parse(
-        cls, nipype_interface: type, pkg: str, base_package: str
+        cls,
+        nipype_interface: type,
+        pkg: str,
+        base_package: str,
     ) -> "NipypeInterface":
         """Generate preamble comments at start of file with args and doc strings"""
 
         doc_string = nipype_interface.__doc__ if nipype_interface.__doc__ else ""
         doc_string = doc_string.replace("\n", "\n# ")
         # Create a preamble at the top of the specificaiton explaining what to do
         preamble = (
@@ -120,18 +128,25 @@
 # Please fill-in/edit the fields below where appropriate
 #
 # Docs
 # ----
 # {doc_string}\n"""
         ).replace("        #", "#")
 
+        base_package = base_package.rstrip(".")
+
+        if base_package:
+            module = nipype_interface.__module__[len(base_package) + 1 :]
+        else:
+            module = nipype_interface.__module__
+
         parsed = cls(
             name=nipype_interface.__name__,
             doc_str=nipype_interface.__doc__ if nipype_interface.__doc__ else "",
-            module=nipype_interface.__module__[len(base_package) + 1 :],
+            module=module,
             pkg=pkg,
             base_package=base_package,
             preamble=preamble,
         )
         # Parse output types and descriptions
         if nipype_interface.output_spec:
             for outpt_name, outpt in nipype_interface.output_spec().traits().items():
@@ -278,18 +293,23 @@
         )
 
         # sort dictionaries by key
         input_types = dict(sorted(input_types.items(), key=itemgetter(0)))
         output_types = dict(sorted(output_types.items(), key=itemgetter(0)))
         output_templates = dict(sorted(output_templates.items(), key=itemgetter(0)))
 
+        if self.base_package:
+            nipype_module = self.base_package + "." + self.module
+        else:
+            nipype_module = self.module
+
         spec_stub = {
             "task_name": self.name,
             "nipype_name": self.name,
-            "nipype_module": self.base_package + "." + self.module,
+            "nipype_module": nipype_module,
             "inputs": self._fields_stub(
                 "inputs",
                 InputsConverter,
                 {
                     "types": {n: type2str(t) for n, t in input_types.items()},
                     "callable_defaults": {
                         n: f"{n}_default" for n in sorted(self.callable_defaults)
@@ -359,19 +379,18 @@
         funcs, classes, imports, consts = get_callable_sources(nipype_interface)
 
         # Write imports to file
         if any(
             re.match(r"\battrs\b", s, flags=re.MULTILINE)
             for s in (list(funcs) + classes)
         ):
-            imports.add("import attrs")
-        obj_imports = set(i for i in imports if i.startswith("from"))
-        mod_imports = imports - obj_imports
-        callables_str += "\n".join(sorted(mod_imports)) + "\n"
-        callables_str += "\n".join(sorted(obj_imports)) + "\n\n"
+            imports.add(parse_imports("import attrs"))
+        callables_str += (
+            "\n".join(str(i.absolute()) for i in sorted(imports) if not i.indent) + "\n"
+        )
 
         # Create separate default function for each input field with genfile, which
         # reference the magic "_gen_filename" method
         for inpt_name, inpt in sorted(nipype_interface.input_spec().traits().items()):
             if inpt.genfile:
                 callables_str += (
                     f"def {inpt_name}_default(inputs):\n"
@@ -398,14 +417,16 @@
 
         # Format the generated code with black
         try:
             callables_str = black.format_file_contents(
                 callables_str, fast=False, mode=black.FileMode()
             )
         except black.parsing.InvalidInput as e:
+            with open(Path("~/Desktop/gen-code.py").expanduser(), "w") as f:
+                f.write(callables_str)
             raise RuntimeError(
                 f"Black could not parse generated code: {e}\n\n{callables_str}"
             )
         return callables_str
 
     def _gen_tests(
         self, doctest_blocks, input_types, output_types, output_templates
@@ -607,41 +628,50 @@
             f.write(response.content)
     else:
         raise RuntimeError(
             f"Could not download the pydra-tasks template at {release_url}"
         )
 
 
-def initialise_task_repo(output_dir, task_template: Path, pkg: str) -> Path:
+def initialise_task_repo(
+    output_dir, task_template: Path, pkg: str, interface_only: bool
+) -> Path:
     """Copy the task template to the output directory and customise it for the given
     package name and return the created package directory"""
 
     pkg_dir = output_dir / f"pydra-{pkg}"
 
     def copy_ignore(_, names):
         return [n for n in names if n in (".git", "__pycache__", ".pytest_cache")]
 
     shutil.copytree(task_template, pkg_dir, ignore=copy_ignore)
 
     # Setup script to auto-convert nipype interfaces
     auto_conv_dir = pkg_dir / "nipype-auto-conv"
     specs_dir = auto_conv_dir / "specs"
     specs_dir.mkdir(parents=True)
-    shutil.copy(TEMPLATES_DIR / "nipype-auto-convert.py", auto_conv_dir / "generate")
+    with open(auto_conv_dir / "generate", "w") as f:
+        f.write(
+            """#!/usr/bin/env bash
+conv_dir=$(dirname $0)
+nipype2pydra convert $conv_dir/specs $conv_dir/.. $@
+"""
+        )
     os.chmod(auto_conv_dir / "generate", 0o755)  # make executable
     shutil.copy(
         TEMPLATES_DIR / "nipype-auto-convert-requirements.txt",
         auto_conv_dir / "requirements.txt",
     )
 
     # Setup GitHub workflows
     gh_workflows_dir = pkg_dir / ".github" / "workflows"
     gh_workflows_dir.mkdir(parents=True, exist_ok=True)
+    ci_cd = "ci-cd-interface.yaml" if interface_only else "ci-cd-workflow.yaml"
     shutil.copy(
-        TEMPLATES_DIR / "gh_workflows" / "ci-cd.yaml",
+        TEMPLATES_DIR / "gh_workflows" / ci_cd,
         gh_workflows_dir / "ci-cd.yaml",
     )
 
     related_pkgs_dir = pkg_dir / "related-packages"
     shutil.copytree(TEMPLATES_DIR / "related-packages", related_pkgs_dir)
     os.rename(related_pkgs_dir / "conftest_.py", related_pkgs_dir / "conftest.py")
 
@@ -686,45 +716,55 @@
     for tool_path in (TEMPLATES_DIR / "tools").iterdir():
         shutil.copyfile(tool_path, pkg_dir / tool_path.name)
 
     # Add "pydra.tasks.<pkg>.auto to gitignore"
     with open(pkg_dir / ".gitignore", "a") as f:
         f.write(f"\n/pydra/tasks/{pkg}/auto" f"\n/pydra/tasks/{pkg}/_version.py\n")
 
+    python_pkg_dir = pkg_dir / "pydra" / "tasks" / pkg
+
     # rename tasks directory
-    (pkg_dir / "pydra" / "tasks" / "CHANGEME").rename(pkg_dir / "pydra" / "tasks" / pkg)
-    (
-        pkg_dir
-        / "related-packages"
-        / "fileformats"
-        / "fileformats"
-        / "medimage_CHANGEME"
-    ).rename(
-        pkg_dir / "related-packages" / "fileformats" / "fileformats" / f"medimage_{pkg}"
-    )
-    (
-        pkg_dir
-        / "related-packages"
-        / "fileformats-extras"
-        / "fileformats"
-        / "extras"
-        / "medimage_CHANGEME"
-    ).rename(
-        pkg_dir
-        / "related-packages"
-        / "fileformats-extras"
-        / "fileformats"
-        / "extras"
-        / f"medimage_{pkg}"
-    )
+    if interface_only:
+        (pkg_dir / "pydra" / "tasks" / "CHANGEME").rename(python_pkg_dir)
+        (
+            pkg_dir
+            / "related-packages"
+            / "fileformats"
+            / "fileformats"
+            / "medimage_CHANGEME"
+        ).rename(
+            pkg_dir
+            / "related-packages"
+            / "fileformats"
+            / "fileformats"
+            / f"medimage_{pkg}"
+        )
+        (
+            pkg_dir
+            / "related-packages"
+            / "fileformats-extras"
+            / "fileformats"
+            / "extras"
+            / "medimage_CHANGEME"
+        ).rename(
+            pkg_dir
+            / "related-packages"
+            / "fileformats-extras"
+            / "fileformats"
+            / "extras"
+            / f"medimage_{pkg}"
+        )
+
+    else:
+        shutil.rmtree(pkg_dir / "pydra" / "tasks" / "CHANGEME")
+        shutil.rmtree(pkg_dir / "related-packages")
+        python_pkg_dir.mkdir(parents=True)
 
     # Add in modified __init__.py
-    shutil.copy(
-        TEMPLATES_DIR / "pkg_init.py", pkg_dir / "pydra" / "tasks" / pkg / "__init__.py"
-    )
+    shutil.copy(TEMPLATES_DIR / "init.py", python_pkg_dir / "__init__.py")
 
     # Replace "CHANGEME" string with pkg name
     for fspath in pkg_dir.glob("**/*"):
         if fspath.is_dir() or fspath.suffix in (".pyc", ".pyo", ".pyd"):
             continue
         with open(fspath) as f:
             contents = f.read()
@@ -1069,23 +1109,25 @@
     # Initialise the source code, imports and constants
     all_funcs = set()
     all_classes = []
     all_imports = set()
     all_constants = set()
     for mod_name, methods in grouped_methods.items():
         mod = import_module(mod_name)
-        used = UsedSymbols.find(mod, methods)
+        used = UsedSymbols.find(mod, methods, omit_classes=(BaseInterface, TraitedSpec))
         all_funcs.update(methods)
         for func in used.local_functions:
             all_funcs.add(cleanup_function_body(get_source_code(func)))
         for klass in used.local_classes:
             klass_src = cleanup_function_body(get_source_code(klass))
             if klass_src not in all_classes:
                 all_classes.append(klass_src)
-        for new_func_name, func in used.funcs_to_include:
+        for new_func_name, func in used.intra_pkg_funcs:
+            if new_func_name is None:
+                continue  # Not referenced directly in this module
             func_src = get_source_code(func)
             location_comment, func_src = func_src.split("\n", 1)
             match = re.match(
                 r"(.*)\bdef *" + func.__name__ + r"(?=\()(.*)$",
                 func_src,
                 re.DOTALL | re.MULTILINE,
             )
@@ -1094,15 +1136,17 @@
                 + "\n"
                 + match.group(1)
                 + "def "
                 + new_func_name
                 + match.group(2)
             )
             all_funcs.add(cleanup_function_body(func_src))
-        for new_klass_name, klass in used.classes_to_include:
+        for new_klass_name, klass in used.intra_pkg_classes:
+            if new_klass_name is None:
+                continue  # Not referenced directly in this module
             klass_src = get_source_code(klass)
             location_comment, klass_src = klass_src.split("\n", 1)
             match = re.match(
                 r"(.*)\bclass *" + klass.__name__ + r"(?=\()(.*)$",
                 klass_src,
                 re.DOTALL | re.MULTILINE,
             )
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/README.rst` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
     - name: Install task package to calculate post-release tag
       run: |
         pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
 
     - name: Generate post-release tag based on Nipype and Nipype2Pydra versions
       id: post_release_tag
       run: |
-        POST=$(python -c "from pydra.tasks.CHANGEME.auto._version import *; print(post_release)")
+        POST=$(python -c "from pydra.tasks.CHANGEME.auto._post_release import post_release; print(post_release)")
         echo "TAG=${{ steps.latest_tag.outputs.TAG }}post${POST}" >> $GITHUB_OUTPUT
 
     - name: Add auto directory to git repo
       if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       run: |
         git add pydra/tasks/CHANGEME/auto
         git commit -am"added auto-generated version to make new tag for package version"
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py` & `nipype2pydra-0.4.0/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/nipype2pydra/task/__init__.py` & `nipype2pydra-0.4.0/nipype2pydra/interface/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-from .function import FunctionTaskConverter
-from .shell_command import ShellCommandTaskConverter
-from importlib import import_module
+from .base import BaseInterfaceConverter
+from .function import FunctionInterfaceConverter
+from .shell_command import ShellCommandInterfaceConverter
 from .base import (
     InputsConverter,
     OutputsConverter,
     TestGenerator,
     DocTestGenerator,
 )
-
-
-def get_converter(nipype_module: str, nipype_name: str, **kwargs):
-    """Loads the appropriate converter for the given nipype interface."""
-    nipype_interface = getattr(import_module(nipype_module), nipype_name)
-
-    if hasattr(nipype_interface, "_cmd"):
-        from .shell_command import ShellCommandTaskConverter as Converter
-    else:
-        from .function import FunctionTaskConverter as Converter
-
-    return Converter(nipype_module=nipype_module, nipype_name=nipype_name, **kwargs)
-
+from .loaders import get_converter
 
 __all__ = [
-    "FunctionTaskConverter",
-    "ShellCommandTaskConverter",
+    "BaseInterfaceConverter",
+    "FunctionInterfaceConverter",
+    "ShellCommandInterfaceConverter",
     "InputsConverter",
     "OutputsConverter",
     "TestGenerator",
     "DocTestGenerator",
     "get_converter",
 ]
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/task/base.py` & `nipype2pydra-0.4.0/nipype2pydra/interface/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,122 +1,46 @@
-import os
 from pathlib import Path
 import typing as ty
 import re
 import logging
 from abc import ABCMeta, abstractmethod
 from importlib import import_module
 from types import ModuleType
 import itertools
 import inspect
-import black
 import traits.trait_types
 import json
+from functools import cached_property
 import attrs
 from attrs.converters import default_if_none
 import nipype.interfaces.base
 from nipype.interfaces.base import traits_extension
 from pydra.engine import specs
 from pydra.engine.helpers import ensure_list
-from ..utils import import_module_from_path, is_fileset, to_snake_case
-from fileformats.core import from_mime
-from fileformats.core.mixin import WithClassifiers
+from ..utils import (
+    import_module_from_path,
+    is_fileset,
+    to_snake_case,
+    UsedSymbols,
+    types_converter,
+    from_dict_converter,
+    unwrap_nested_type,
+)
+from ..statements import (
+    ImportStatement,
+    parse_imports,
+    ExplicitImport,
+    from_list_to_imports,
+)
 from fileformats.generic import File
-
-
-T = ty.TypeVar("T")
+import nipype2pydra.package
 
 logger = logging.getLogger("nipype2pydra")
 
 
-def from_dict_converter(
-    obj: ty.Union[T, dict], klass: ty.Type[T], allow_none=False
-) -> T:
-    if obj is None:
-        if allow_none:
-            converted = None
-        else:
-            converted = klass()
-    elif isinstance(obj, dict):
-        converted = klass(**obj)
-    elif isinstance(obj, klass):
-        converted = obj
-    else:
-        raise TypeError(
-            f"Input must be of type {klass} or dict, not {type(obj)}: {obj}"
-        )
-    return converted
-
-
-def str_to_type(type_str: str) -> type:
-    """Resolve a string representation of a type into a valid type"""
-    if "/" in type_str:
-        tp = from_mime(type_str)
-        try:
-            # If datatype is a field, use its primitive instead
-            tp = tp.primitive  # type: ignore
-        except AttributeError:
-            pass
-    else:
-
-        def resolve_type(type_str: str) -> type:
-            if "." in type_str:
-                parts = type_str.split(".")
-                module = import_module(".".join(parts[:-1]))
-                class_str = parts[-1]
-            else:
-                class_str = type_str
-                module = None
-            match = re.match(r"(\w+)(\[.*\])?", class_str)
-            class_str = match.group(1)
-            if module:
-                t = getattr(module, match.group(1))
-            else:
-                if not re.match(r"^\w+$", class_str):
-                    raise ValueError(f"Cannot parse {class_str} to a type safely")
-                t = eval(class_str)
-            if match.group(2):
-                args = tuple(
-                    resolve_type(arg) for arg in match.group(2)[1:-1].split(",")
-                )
-                t = t.__getitem__(args)
-            return t
-
-        tp = resolve_type(type_str)
-        if not inspect.isclass(tp) and type(tp).__module__ != "typing":
-            raise TypeError(f"Designated type at {type_str} is not a class {tp}")
-    return tp
-
-
-def types_converter(types: ty.Dict[str, ty.Union[str, type]]) -> ty.Dict[str, type]:
-    if types is None:
-        return {}
-    converted = {}
-    for name, tp_or_str in types.items():
-        if isinstance(tp_or_str, str):
-            tp = str_to_type(tp_or_str)
-        converted[name] = tp
-    return converted
-
-
-@attrs.define
-class ImportStatement:
-    module: str
-    name: ty.Optional[str] = None
-    alias: ty.Optional[str] = None
-
-
-def from_list_to_imports(
-    obj: ty.Union[ty.List[ImportStatement], list]
-) -> ty.List[ImportStatement]:
-    if obj is None:
-        return []
-    return [from_dict_converter(t, ImportStatement) for t in obj]
-
-
 @attrs.define
 class SpecConverter:
     omit: ty.List[str] = attrs.field(
         factory=list,
         converter=default_if_none(factory=list),  # type: ignore
         metadata={"help": "fields to omit from the Pydra interface"},
     )
@@ -255,15 +179,15 @@
         factory=dict,
         converter=default_if_none(factory=dict),  # type: ignore
         metadata={
             "help": """values to provide to inputs fields in the task initialisation
                 (if not specified, will try to choose a sensible value)"""
         },
     )
-    imports: ty.List[ImportStatement] = attrs.field(
+    imports: ty.List[ExplicitImport] = attrs.field(
         factory=list,
         converter=from_list_to_imports,
         metadata={
             "help": """list import statements required by the test, with each list item
                 consisting of 'module', 'name', and optionally 'alias' keys"""
         },
     )
@@ -317,15 +241,15 @@
         factory=dict,
         metadata={
             "help": """name-value pairs for inputs to be provided to the doctest.
                 If the field is of file-format type and the value is None, then the
                 '.mock()' method of the corresponding class is used instead."""
         },
     )
-    imports: ty.List[ImportStatement] = attrs.field(
+    imports: ty.List[ExplicitImport] = attrs.field(
         factory=list,
         converter=from_list_to_imports,
         metadata={
             "help": """list import statements required by the test, with each list item
                 consisting of 'module', 'name', and optionally 'alias' keys"""
         },
     )
@@ -357,16 +281,16 @@
     obj: ty.Union[ty.List[DocTestGenerator], list]
 ) -> ty.List[DocTestGenerator]:
     if obj is None:
         return []
     return [from_dict_converter(t, DocTestGenerator) for t in obj]
 
 
-@attrs.define
-class BaseTaskConverter(metaclass=ABCMeta):
+@attrs.define(slots=False)
+class BaseInterfaceConverter(metaclass=ABCMeta):
     """Specifies how the semi-automatic conversion from Nipype to Pydra should
     be performed
 
     Parameters
     ----------
     task_name: str
         name of the Pydra task
@@ -409,14 +333,30 @@
     )
     tests: ty.List[TestGenerator] = attrs.field(  # type: ignore
         factory=list, converter=from_list_to_tests
     )
     doctests: ty.List[DocTestGenerator] = attrs.field(
         factory=list, converter=from_list_to_doctests
     )
+    package: "nipype2pydra.package.PackageConverter" = attrs.field(
+        default=None,
+        metadata={
+            "help": ("the package converter that the workflow is associated with"),
+        },
+    )
+    find_replace: ty.List[ty.Tuple[str, str]] = attrs.field(
+        factory=list,
+        converter=lambda lst: [tuple(i) for i in lst] if lst else [],
+        metadata={
+            "help": (
+                "Generic regular expression substitutions to be run over the code before "
+                "it is processed"
+            ),
+        },
+    )
 
     def __attrs_post_init__(self):
         if self.output_module is None:
             if self.nipype_module.__name__.startswith("nipype.interfaces."):
                 pkg_name = self.nipype_module.__name__.split(".")[2]
                 self.output_module = (
                     f"pydra.tasks.{pkg_name}.auto.{to_snake_case(self.task_name)}"
@@ -438,67 +378,126 @@
         return (
             self.nipype_interface.input_spec()
             if self.nipype_interface.input_spec
             else None
         )
 
     @property
+    def full_address(self):
+        return f"{self.nipype_module.__name__}.{self.nipype_name}"
+
+    @property
     def nipype_output_spec(self) -> nipype.interfaces.base.BaseTraitedSpec:
         return (
             self.nipype_interface.output_spec()
             if self.nipype_interface.output_spec
             else None
         )
 
-    def generate(self, package_root: Path):
-        """creating pydra input/output spec from nipype specs
-        if write is True, a pydra Task class will be written to the file together with tests
-        """
-        input_fields, inp_templates = self.convert_input_fields()
-        output_fields = self.convert_output_spec(fields_from_template=inp_templates)
+    @cached_property
+    def input_fields(self):
+        return self._convert_input_fields[0]
+
+    @cached_property
+    def input_templates(self):
+        return self._convert_input_fields[1]
+
+    @cached_property
+    def output_fields(self):
+        return self.convert_output_spec(fields_from_template=self.input_templates)
+
+    @cached_property
+    def nonstd_types(self):
 
         nonstd_types = set()
 
         def add_nonstd_types(tp):
             if ty.get_origin(tp) in (list, ty.Union):
                 for tp_arg in ty.get_args(tp):
                     add_nonstd_types(tp_arg)
             elif tp.__module__ not in ["builtins", "pathlib", "typing"]:
                 nonstd_types.add(tp)
 
-        for f in input_fields:
+        for f in self.input_fields:
             add_nonstd_types(f[1])
 
-        for f in output_fields:
+        for f in self.output_fields:
             add_nonstd_types(f[1])
+        return nonstd_types
 
-        output_file = (
-            Path(package_root)
-            .joinpath(*self.output_module.split("."))
-            .with_suffix(".py")
+    @property
+    def converted_code(self):
+        return self._converted[0]
+
+    @property
+    def used_symbols(self):
+        return self._converted[1]
+
+    @cached_property
+    def _converted(self):
+        """writing pydra task to the dile based on the input and output spec"""
+
+        return self.generate_code(
+            self.input_fields, self.nonstd_types, self.output_fields
+        )
+
+    def write(
+        self,
+        package_root: Path,
+        already_converted: ty.Set[str] = None,
+        additional_funcs: ty.List[str] = None,
+    ):
+        """creating pydra input/output spec from nipype specs
+        if write is True, a pydra Task class will be written to the file together with tests
+        """
+        if already_converted is None:
+            already_converted = set()
+        if additional_funcs is None:
+            additional_funcs = []
+        if self.full_address in already_converted:
+            return
+
+        self.package.write_to_module(
+            package_root=package_root,
+            module_name=self.output_module,
+            converted_code=self.converted_code,
+            used=self.used_symbols,
+            # inline_intra_pkg=True,
+            find_replace=self.find_replace + self.package.find_replace,
         )
-        testdir = output_file.parent / "tests"
-        testdir.mkdir(parents=True, exist_ok=True)
 
-        self.write_task(
-            output_file,
-            input_fields=input_fields,
-            output_fields=output_fields,
-            nonstd_types=nonstd_types,
+        self.package.write_pkg_inits(
+            package_root,
+            self.output_module,
+            names=[self.task_name],
+            depth=self.package.init_depth,
+            auto_import_depth=self.package.auto_import_init_depth,
+            import_find_replace=self.package.import_find_replace,
+            # + [f.__name__ for f in self.used_symbols.local_functions]
+            # + [c.__name__ for c in self.used_symbols.local_classes],
         )
 
-        filename_test = testdir / f"test_{self.task_name.lower()}.py"
-        # filename_test_run = testdir / f"test_run_{self.task_name.lower()}.py"
-        self.write_tests(
-            filename_test,
-            input_fields=input_fields,
-            nonstd_types=nonstd_types,
+        test_module_fspath = self.package.write_to_module(
+            package_root=package_root,
+            module_name=ImportStatement.join_relative_package(
+                self.output_module, f".tests.test_{self.task_name.lower()}"
+            ),
+            converted_code=self.converted_test_code,
+            used=self.used_symbols_test,
+            inline_intra_pkg=False,
+            find_replace=self.find_replace,
         )
 
-    def convert_input_fields(self):
+        conftest_fspath = test_module_fspath.parent / "conftest.py"
+        if not conftest_fspath.exists():
+            with open(conftest_fspath, "w") as f:
+                f.write(self.CONFTEST)
+
+    @cached_property
+    def _convert_input_fields(self):
         """creating fields list for pydra input spec"""
         pydra_fields_dict = {}
         position_dict = {}
         has_template = []
         for name, fld in self.nipype_input_spec.traits().items():
             if name in self.TRAITS_IRREL:
                 continue
@@ -712,112 +711,81 @@
             repl = f"{name}" if len(keys) == 1 else f"{name}[{i}]"
             match = re.match(r"%([0-9\.]+)f", key)
             if match:
                 repl += ":" + match.group(1)
             new_argstr = new_argstr.replace(key, r"{" + repl + r"}", 1)
         return new_argstr
 
-    def write_task(self, filename, input_fields, nonstd_types, output_fields):
-        """writing pydra task to the dile based on the input and output spec"""
-
-        spec_str = self.generate_task_str(
-            filename, input_fields, nonstd_types, output_fields
-        )
-
-        spec_str = black.format_file_contents(
-            spec_str, fast=False, mode=black.FileMode()
-        )
-
-        # # FIXME: bit of a hack, should make sure that multi-input/output objects
-        # #        are referenced properly without this substitution
-        # spec_str = re.sub(
-        #     r"(?<!specs\.|mport )Multi(Input|Output)", r"specs.Multi\1", spec_str
-        # )
-
-        with open(filename, "w") as f:
-            f.write(spec_str)
-
     @abstractmethod
-    def generate_task_str(self, filename, input_fields, nonstd_types, output_fields):
-        raise NotImplementedError
+    def generate_code(self, input_fields, nonstd_types, output_fields) -> ty.Tuple[
+        str,
+        UsedSymbols,
+    ]:
+        """
+        Returns
+        -------
+        converted_code : str
+            the core converted code for the task
+        used_symbols: UsedSymbols
+            symbols used in the code
+        """
 
     def construct_imports(
-        self, nonstd_types: ty.List[type], spec_str="", base=(), include_task=True
-    ) -> ty.List[str]:
+        self,
+        nonstd_types: ty.List[type],
+        spec_str="",
+        base=(),
+        include_task=True,
+    ) -> ty.List[ImportStatement]:
         """Constructs a list of imports to include at start of file"""
-        stmts: ty.Dict[str, str] = {}
-
-        def add_import(stmt):
-            if stmt == "from nipype import logging":
-                return
-            match = re.match(r".*\s+as\s+(\w+)\s*", stmt)
-            if not match:
-                match = re.match(r".*import\s+([\w\., ]+)\s*$", stmt)
-            if not match:
-                raise ValueError(f"Unrecognised import statment {stmt}")
-            token = match.group(1)
-            try:
-                prev_stmt = stmts[token]
-            except KeyError:
-                pass
-            else:
-                if prev_stmt != stmt:
-                    logger.warning(
-                        f"Cannot add import statement {stmt} as it clashes with "
-                        f"previous import {prev_stmt}"
-                    )
-            stmts[token] = stmt
-
-        for b in base:
-            add_import(b)
+        stmts = parse_imports(base, relative_to=self.output_module)
 
         if re.match(r".*(?<!\w)ty\.", spec_str, flags=re.MULTILINE | re.DOTALL):
-            add_import("import typing as ty")
+            stmts.extend(parse_imports("import typing as ty"))
         if re.match(r".*\bPath\b", spec_str, flags=re.MULTILINE | re.DOTALL):
-            add_import("from pathlib import Path")
+            stmts.extend(parse_imports("from pathlib import Path"))
         if re.match(r".*\blogging\b", spec_str, flags=re.MULTILINE | re.DOTALL):
-            add_import("import logging")
+            stmts.extend(parse_imports("import logging"))
         for test in self.tests:
-            for stmt in test.imports:
-                if "nipype" in stmt.module:
-                    continue
-                if stmt.name is None:
-                    add_import(f"import {stmt.module}")
-                else:
-                    nm = (
-                        stmt.name
-                        if stmt.alias is None
-                        else f"{stmt.name} as {stmt.alias}"
-                    )
-                    add_import(f"from {stmt.module} import {nm}")
-
-        def unwrap_nested_type(t: type) -> ty.List[type]:
-            if issubclass(t, WithClassifiers) and t.is_classified:
-                unwrapped = [t.unclassified]
-                for c in t.classifiers:
-                    unwrapped.extend(unwrap_nested_type(c))
-                return unwrapped
-            return [t]
+            for explicit_import in test.imports:
+                if not explicit_import.module.startswith("nipype"):
+                    stmt = explicit_import.to_statement()
+                    if self.task_name in stmt:
+                        stmt.drop(self.task_name)
+                        if not stmt:
+                            continue
+                    stmts.append(stmt)
 
         for tp in itertools.chain(*(unwrap_nested_type(t) for t in nonstd_types)):
-            add_import(f"from {tp.__module__} import {tp.__name__}")
+            stmts.append(ImportStatement.from_object(tp))
         if include_task:
-            add_import(f"from {self.output_module} import {self.task_name}")
+            stmts.extend(
+                parse_imports(f"from {self.output_module} import {self.task_name}")
+            )
+
+        return ImportStatement.collate(stmts)
 
-        return sorted(stmts.values())
+    @property
+    def converted_test_code(self):
+        return self._converted_test[0]
+
+    @property
+    def used_symbols_test(self):
+        return self._converted_test[1]
 
-    def write_tests(self, filename_test, input_fields, nonstd_types, run=False):
+    @cached_property
+    def _converted_test(self):
         spec_str = ""
         for i, test in enumerate(self.tests, start=1):
             if test.xfail:
                 spec_str += "@pytest.mark.xfail\n"
             # spec_str += f"@pass_after_timeout(seconds={test.timeout})\n"
             spec_str += f"def test_{self.task_name.lower()}_{i}():\n"
             spec_str += f"    task = {self.task_name}()\n"
-            for i, field in enumerate(input_fields):
+            for i, field in enumerate(self.input_fields):
                 nm, tp = field[:2]
                 # Try to get a sensible value for the traits value
                 try:
                     value = test.inputs[nm]
                 except KeyError:
                     pass
                 else:
@@ -866,39 +834,25 @@
             spec_str += "    res = task(plugin=PassAfterTimeoutWorker)\n"
             spec_str += "    print('RESULT: ', res)\n"
             for name, value in test.expected_outputs.items():
                 spec_str += f"    assert res.output.{name} == {value}\n"
             spec_str += "\n\n\n"
 
         imports = self.construct_imports(
-            nonstd_types,
+            self.nonstd_types,
             spec_str,
             base={
                 "import pytest",
                 "from nipype2pydra.testing import PassAfterTimeoutWorker",
             },
         )
-        spec_str = "\n".join(imports) + "\n\n" + spec_str
 
-        try:
-            spec_str_black = black.format_file_contents(
-                spec_str, fast=False, mode=black.FileMode()
-            )
-        except black.parsing.InvalidInput as e:
-            raise RuntimeError(
-                f"Black could not parse generated code: {e}\n\n{spec_str}"
-            )
-
-        with open(filename_test, "w") as f:
-            f.write(spec_str_black)
-
-        conftest_fspath = filename_test.parent / "conftest.py"
-        if not conftest_fspath.exists():
-            with open(conftest_fspath, "w") as f:
-                f.write(self.CONFTEST)
+        return spec_str, UsedSymbols(
+            module_name=self.nipype_module.__name__, imports=imports
+        )
 
     def create_doctests(self, input_fields, nonstd_types):
         """adding doctests to the interfaces"""
         doctest_str = ""
         for doctest in self.doctests:
             doctest_str += f"    >>> task = {self.task_name}()\n"
             for field in input_fields:
@@ -935,15 +889,20 @@
                     doctest_str += f"    >>> task.inputs.{nm} = {val}\n"
             doctest_str += "    >>> task.cmdline\n"
             doctest_str += f"    '{doctest.cmdline}'"
             doctest_str += "\n\n\n"
 
         imports = self.construct_imports(nonstd_types, doctest_str)
         if imports:
-            doctest_str = "    >>> " + "\n    >>> ".join(imports) + "\n\n" + doctest_str
+            doctest_str = (
+                "    >>> "
+                + "\n    >>> ".join(str(i) for i in imports)
+                + "\n\n"
+                + doctest_str
+            )
 
         return "    Examples\n    -------\n\n" + doctest_str
 
     INPUT_KEYS = [
         "allowed_values",
         "argstr",
         "container_path",
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/task/function.py` & `nipype2pydra-0.4.0/nipype2pydra/interface/function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 import typing as ty
 import re
 import inspect
-from operator import attrgetter, itemgetter
+from operator import attrgetter
 from functools import cached_property
 import itertools
+import logging
 import attrs
-from .base import BaseTaskConverter
+from nipype.interfaces.base import BaseInterface, TraitedSpec
+from .base import BaseInterfaceConverter
 from ..utils import (
     extract_args,
     UsedSymbols,
-    get_source_code,
     get_local_functions,
     get_local_constants,
     cleanup_function_body,
     insert_args_in_signature,
 )
 
 
+logger = logging.getLogger("nipype2pydra")
+
+
 @attrs.define(slots=False)
-class FunctionTaskConverter(BaseTaskConverter):
+class FunctionInterfaceConverter(BaseInterfaceConverter):
 
-    def generate_task_str(self, filename, input_fields, nonstd_types, output_fields):
-        """writing pydra task to the dile based on the input and output spec"""
+    def generate_code(self, input_fields, nonstd_types, output_fields) -> ty.Tuple[
+        str,
+        UsedSymbols,
+    ]:
+        """
+        Returns
+        -------
+        converted_code : str
+            the core converted code for the task
+        used_symbols: UsedSymbols
+            symbols used in the code
+        """
 
         base_imports = [
             "import pydra.mark",
             "import logging",
             "from logging import getLogger",
+            "from pydra.engine.task import FunctionTask",
             "import attrs",
         ]
 
         def types_to_names(spec_fields):
             spec_fields_str = []
             for el in spec_fields:
                 el = list(el)
@@ -49,48 +64,59 @@
         output_fields_str = types_to_names(spec_fields=output_fields)
         input_names = [i[0] for i in input_fields]
         output_names = [o[0] for o in output_fields]
         output_type_names = [o[1] for o in output_fields_str]
 
         # Combined src of run_interface and list_outputs
         method_body = inspect.getsource(self.nipype_interface._run_interface).strip()
-        method_body = "\n".join(method_body.split("\n")[1:-1])
+        # Strip out method def and return statement
+        method_lines = method_body.strip().split("\n")[1:]
+        if re.match(r"\s*return", method_lines[-1]):
+            method_lines = method_lines[:-1]
+        method_body = "\n".join(method_lines)
         lo_src = inspect.getsource(self.nipype_interface._list_outputs).strip()
-        lo_lines = lo_src.split("\n")
-        lo_src = "\n".join(lo_lines[1:-1])
-        method_body += lo_src
+        # Strip out method def and return statement
+        lo_lines = lo_src.strip().split("\n")[1:]
+        if re.match(r"\s*(return|raise NotImplementedError)", lo_lines[-1]):
+            lo_lines = lo_lines[:-1]
+        lo_src = "\n".join(lo_lines)
+        method_body += "\n" + lo_src
         method_body = self.process_method_body(method_body, input_names, output_names)
 
         used = UsedSymbols.find(
             self.nipype_module,
             [method_body]
             + [
                 inspect.getsource(f)
                 for f in itertools.chain(
                     self.referenced_local_functions, self.referenced_methods
                 )
             ],
+            omit_classes=self.package.omit_classes + [BaseInterface, TraitedSpec],
+            omit_modules=self.package.omit_modules,
+            omit_functions=self.package.omit_functions,
+            omit_constants=self.package.omit_constants,
+            always_include=self.package.all_explicit,
+            translations=self.package.all_import_translations,
+            absolute_imports=True,
         )
 
-        spec_str = "\n".join(f"{n} = {d}" for n, d in used.constants)
-
-        # Create the spec string
-        spec_str += "\n\n" + self.function_callables()
-        spec_str += "logger = getLogger(__name__)\n\n"
-        spec_str += "@pydra.mark.task\n"
+        spec_str = "@pydra.mark.task\n"
         spec_str += "@pydra.mark.annotate({'return': {"
         spec_str += ", ".join(f"'{n}': {t}" for n, t, _ in output_fields_str)
         spec_str += "}})\n"
         spec_str += f"def {self.task_name}("
         spec_str += ", ".join(f"{i[0]}: {i[1]}" for i in input_fields_str)
-        spec_str += ") -> "
-        if len(output_type_names) > 1:
-            spec_str += "ty.Tuple[" + ", ".join(output_type_names) + "]"
-        else:
-            spec_str += output_type_names[0]
+        spec_str += ")"
+        if output_type_names:
+            spec_str += "-> "
+            if len(output_type_names) > 1:
+                spec_str += "ty.Tuple[" + ", ".join(output_type_names) + "]"
+            else:
+                spec_str += output_type_names[0]
         spec_str += ':\n    """\n'
         spec_str += self.create_doctests(
             input_fields=input_fields, nonstd_types=nonstd_types
         )
         spec_str += '    """\n'
         spec_str += method_body + "\n"
         spec_str += "\n    return {}".format(", ".join(output_names))
@@ -104,52 +130,22 @@
         additional_imports = set()
         for attr, repl, imprt in self.RUNTIME_ATTRS:
             repl_spec_str = spec_str.replace(f"runtime.{attr}", repl)
             if repl_spec_str != spec_str:
                 additional_imports.add(imprt)
                 spec_str = repl_spec_str
 
-        spec_str += "\n\n# Functions defined locally in the original module\n\n"
-
-        for func in sorted(used.local_functions, key=attrgetter("__name__")):
-            spec_str += "\n\n" + cleanup_function_body(
-                get_source_code(func)
-            )
-
-        spec_str += "\n\n# Functions defined in neighbouring modules that have been included inline instead of imported\n\n"
-
-        for func_name, func in sorted(used.funcs_to_include, key=itemgetter(0)):
-            func_src = get_source_code(func)
-            func_src = re.sub(
-                r"^(#[^\n]+\ndef) (\w+)(?=\()",
-                r"\1 " + func_name,
-                func_src,
-                flags=re.MULTILINE,
-            )
-            spec_str += "\n\n" + cleanup_function_body(func_src)
-
-        for klass_name, klass in sorted(used.classes_to_include, key=itemgetter(0)):
-            klass_src = get_source_code(klass)
-            klass_src = re.sub(
-                r"^(#[^\n]+\nclass) (\w+)(?=\()",
-                r"\1 " + klass_name,
-                klass_src,
-                flags=re.MULTILINE,
-            )
-            spec_str += "\n\n" + cleanup_function_body(klass_src)
-
-        imports = self.construct_imports(
+        used.imports = self.construct_imports(
             nonstd_types,
             spec_str,
             include_task=False,
             base=base_imports + list(used.imports) + list(additional_imports),
         )
-        spec_str = "\n".join(imports) + "\n\n" + spec_str
 
-        return spec_str
+        return spec_str, used
 
     def process_method(
         self,
         method: str,
         input_names: ty.List[str],
         output_names: ty.List[str],
         method_args: ty.Dict[str, ty.List[str]] = None,
@@ -167,48 +163,58 @@
         method_body = method_body.split("\n", maxsplit=1)[1]
         method_body = self.process_method_body(method_body, input_names, output_names)
         if self.method_returns.get(method.__name__):
             return_args = self.method_returns[method.__name__]
             method_body = (
                 "    " + " = ".join(return_args) + " = attrs.NOTHING\n" + method_body
             )
-            method_lines = method_body.splitlines()
+            method_lines = method_body.rstrip().splitlines()
             method_body = "\n".join(method_lines[:-1])
             last_line = method_lines[-1]
             if "return" in last_line:
-                method_body += "," + ",".join(return_args)
+                method_body += "\n" + last_line + "," + ",".join(return_args)
             else:
                 method_body += (
                     "\n" + last_line + "\n    return " + ",".join(return_args)
                 )
         return f"{pre.strip()}{', '.join(args)}{return_types}:\n{method_body}"
 
     def process_method_body(
         self, method_body: str, input_names: ty.List[str], output_names: ty.List[str]
     ) -> str:
         # Replace self.inputs.<name> with <name> in the function body
-        input_re = re.compile(r"self\.inputs\.(\w+)")
+        input_re = re.compile(r"self\.inputs\.(\w+)\b(?!\()")
         unrecognised_inputs = set(
             m for m in input_re.findall(method_body) if m not in input_names
         )
-        assert (
-            not unrecognised_inputs
-        ), f"Found the following unrecognised inputs {unrecognised_inputs}"
+        if unrecognised_inputs:
+            logger.warning(
+                "Found the following unrecognised (potentially dynamic) inputs %s in "
+                "'%s' task",
+                unrecognised_inputs,
+                self.task_name,
+            )
         method_body = input_re.sub(r"\1", method_body)
 
         output_re = re.compile(self.return_value + r"\[(?:'|\")(\w+)(?:'|\")\]")
         unrecognised_outputs = set(
             m for m in output_re.findall(method_body) if m not in output_names
         )
-        assert (
-            not unrecognised_outputs
-        ), f"Found the following unrecognised outputs {unrecognised_outputs}"
+        if unrecognised_outputs:
+            logger.warning(
+                "Found the following unrecognised (potentially dynamic) outputs %s in "
+                "'%s' task",
+                unrecognised_outputs,
+                self.task_name,
+            )
         method_body = output_re.sub(r"\1", method_body)
         # Strip initialisation of outputs
-        method_body = re.sub(r"outputs = self.output_spec().*", r"outputs = {}", method_body)
+        method_body = re.sub(
+            r"outputs = self.output_spec().*", r"outputs = {}", method_body
+        )
         # Add args to the function signature of method calls
         method_re = re.compile(r"self\.(\w+)(?=\()", flags=re.MULTILINE | re.DOTALL)
         method_names = [m.__name__ for m in self.referenced_methods]
         unrecognised_methods = set(
             m for m in method_re.findall(method_body) if m not in method_names
         )
         assert (
@@ -216,27 +222,24 @@
         ), f"Found the following unrecognised methods {unrecognised_methods}"
         splits = method_re.split(method_body)
         new_body = splits[0]
         for name, args in zip(splits[1::2], splits[2::2]):
             # Assign additional return values (which were previously saved to member
             # attributes) to new variables from the method call
             if self.method_returns[name]:
-                match = re.match(
-                    r".*\n *([a-zA-Z0-9\,\. ]+ *=)? *$",
-                    new_body,
-                    flags=re.MULTILINE | re.DOTALL,
-                )
+                last_line = new_body.splitlines()[-1]
+                match = re.match(r" *([a-zA-Z0-9\,\.\_ ]+ *=)? *$", last_line)
                 if match:
                     if match.group(1):
                         new_body_lines = new_body.splitlines()
                         new_body = "\n".join(new_body_lines[:-1])
                         last_line = new_body_lines[-1]
                         new_body += "\n" + re.sub(
-                            r"^ *([a-zA-Z0-9\,\. ]+) *= *$",
-                            r"\1, =" + ",".join(self.method_returns[name]),
+                            r"^( *)([a-zA-Z0-9\,\.\_ ]+) *= *$",
+                            r"\1\2, " + ",".join(self.method_returns[name]) + " = ",
                             last_line,
                             flags=re.MULTILINE,
                         )
                     else:
                         new_body += ",".join(self.method_returns[name]) + " = "
                 else:
                     raise NotImplementedError(
@@ -381,21 +384,25 @@
 
     @cached_property
     def local_constants(self):
         return get_local_constants(self.nipype_module)
 
     @cached_property
     def return_value(self):
-        return_line = (
-            inspect.getsource(self.nipype_interface._list_outputs)
-            .strip()
-            .split("\n")[-1]
-        )
-        match = re.match(r"\s*return(.*)", return_line)
-        return match.group(1).strip()
+        def get_return_line(func):
+            return_line = inspect.getsource(func).strip().split("\n")[-1]
+            match = re.match(r"\s*return(.*)", return_line)
+            if not match:
+                raise ValueError("Could not find return line in _list_outputs")
+            return match.group(1).strip()
+
+        try:
+            return get_return_line(self.nipype_interface._list_outputs)
+        except ValueError:
+            return get_return_line(self.nipype_interface._outputs)
 
     @cached_property
     def methods(self):
         """Get the functions defined in the interface"""
         methods = []
         for attr_name in dir(self.nipype_interface):
             if attr_name.startswith("__"):
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/task/shell_command.py` & `nipype2pydra-0.4.0/nipype2pydra/interface/shell_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import re
+import typing as ty
 import attrs
 import inspect
 from copy import copy
-from .base import BaseTaskConverter
+from .base import BaseInterfaceConverter
+from ..utils import UsedSymbols
 from fileformats.core.mixin import WithClassifiers
 from fileformats.generic import File, Directory
 
 
-@attrs.define
-class ShellCommandTaskConverter(BaseTaskConverter):
-    def generate_task_str(self, filename, input_fields, nonstd_types, output_fields):
-        """writing pydra task to the dile based on the input and output spec"""
+@attrs.define(slots=False)
+class ShellCommandInterfaceConverter(BaseInterfaceConverter):
+    def generate_code(self, input_fields, nonstd_types, output_fields) -> ty.Tuple[
+        str,
+        UsedSymbols,
+    ]:
+        """
+        Returns
+        -------
+        converted_code : str
+            the core converted code for the task
+        used_symbols: UsedSymbols
+            symbols used in the code
+        """
 
         base_imports = [
             "from pydra.engine import specs",
         ]
 
         task_base = "ShellCommandTask"
         base_imports.append("from pydra.engine import ShellCommandTask")
@@ -24,40 +36,46 @@
         except AttributeError:
             executable = None
         if not executable:
             executable = self.nipype_interface.cmd
             if not isinstance(executable, str):
                 raise RuntimeError(
                     f"Could not find executable for {self.nipype_interface}, "
-                    "try the FunctionTaskConverter class instead"
+                    "try the FunctionInterfaceConverter class instead"
                 )
 
         def unwrap_field_type(t):
             if issubclass(t, WithClassifiers) and t.is_classified:
-                unwraped_classifiers = ", ".join(unwrap_field_type(c) for c in t.classifiers)
+                unwraped_classifiers = ", ".join(
+                    unwrap_field_type(c) for c in t.classifiers
+                )
                 return f"{t.unclassified.__name__}[{unwraped_classifiers}]"
             return t.__name__
 
         nonstd_types = copy(nonstd_types)
 
         def types_to_names(spec_fields):
             spec_fields_str = []
             for el in spec_fields:
                 el = list(el)
                 field_type = el[1]
-                if inspect.isclass(field_type) and issubclass(field_type, WithClassifiers):
+                if inspect.isclass(field_type) and issubclass(
+                    field_type, WithClassifiers
+                ):
                     field_type_str = unwrap_field_type(field_type)
                 else:
                     field_type_str = str(field_type)
                     if field_type_str.startswith("<class "):
                         field_type_str = el[1].__name__
                     else:
                         # Alter modules in type string to match those that will be imported
                         field_type_str = field_type_str.replace("typing", "ty")
-                        field_type_str = re.sub(r"(\w+\.)+(?<!ty\.)(\w+)", r"\2", field_type_str)
+                        field_type_str = re.sub(
+                            r"(\w+\.)+(?<!ty\.)(\w+)", r"\2", field_type_str
+                        )
                 if field_type_str == "File":
                     nonstd_types.add(File)
                 elif field_type_str == "Directory":
                     nonstd_types.add(Directory)
                 el[1] = "#" + field_type_str + "#"
                 spec_fields_str.append(tuple(el))
             return spec_fields_str
@@ -85,10 +103,12 @@
 
         imports = self.construct_imports(
             nonstd_types,
             spec_str,
             include_task=False,
             base=base_imports,
         )
-        spec_str = "\n".join(imports) + "\n\n" + spec_str
+        # spec_str = "\n".join(str(i) for i in imports) + "\n\n" + spec_str
 
-        return spec_str
+        return spec_str, UsedSymbols(
+            module_name=self.nipype_module.__name__, imports=imports
+        )
```

### Comparing `nipype2pydra-0.3.5/nipype2pydra/task/tests/test_task.py` & `nipype2pydra-0.4.0/nipype2pydra/interface/tests/test_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from importlib import import_module
 import yaml
 import pytest
 import logging
-import io
-import contextlib
 from traceback import format_exc
-from nipype2pydra.cli.task import task as task_cli
 from nipype2pydra.utils import (
     add_to_sys_path,
     add_exc_note,
     INBUILT_NIPYPE_TRAIT_NAMES,
-    show_cli_trace,
 )
-from conftest import EXAMPLE_TASKS_DIR
+from nipype2pydra.package import PackageConverter
+from conftest import EXAMPLE_INTERFACES_DIR
 
 
 logging.basicConfig(level=logging.INFO)
 
 
 XFAIL_INTERFACES = [
     "fsl-prob_track_x2",
@@ -36,64 +33,75 @@
     "fsl-smooth",
     "fsl-merge",
 ]
 
 
 @pytest.fixture(
     params=[
-        str(p.relative_to(EXAMPLE_TASKS_DIR)).replace("/", "-")[:-5]
-        for p in (EXAMPLE_TASKS_DIR).glob("**/*.yaml")
+        str(p.relative_to(EXAMPLE_INTERFACES_DIR)).replace("/", "-")[:-5]
+        for p in (EXAMPLE_INTERFACES_DIR).glob("**/*.yaml")
     ]
 )
-def task_spec_file(request):
-    return EXAMPLE_TASKS_DIR.joinpath(*request.param.split("-")).with_suffix(".yaml")
+def interface_spec_file(request):
+    return EXAMPLE_INTERFACES_DIR.joinpath(*request.param.split("-")).with_suffix(
+        ".yaml"
+    )
 
 
-def test_task_conversion(task_spec_file, cli_runner, work_dir, gen_test_conftest):
+def test_interface_convert(
+    interface_spec_file, cli_runner, work_dir, gen_test_conftest
+):
 
     try:
-        with open(task_spec_file) as f:
-            task_spec = yaml.safe_load(f)
+        with open(interface_spec_file) as f:
+            interface_spec = yaml.safe_load(f)
         pkg_root = work_dir / "src"
         pkg_root.mkdir()
         # shutil.copyfile(gen_test_conftest, pkg_root / "conftest.py")
 
-        output_module_path = f"nipype2pydratest.{task_spec_file.stem.lower()}"
+        pkg_converter = PackageConverter(
+            name="nipype2pydratest."
+            + "_".join(
+                interface_spec["nipype_module"].split(".")
+                + [interface_spec["task_name"]]
+            ),
+            nipype_name=interface_spec["nipype_module"].split(".")[0],
+            interface_only=True,
+        )
 
-        result = cli_runner(
-            task_cli,
-            args=[
-                str(task_spec_file),
-                str(pkg_root),
-                "--output-module",
-                output_module_path,
-                "--callables",
-                str(task_spec_file.parent / (task_spec_file.stem + "_callables.py")),
-            ],
+        converter = pkg_converter.add_interface_from_spec(
+            spec=interface_spec,
+            callables_file=interface_spec_file.parent
+            / (interface_spec_file.stem + "_callables.py"),
         )
 
-        assert result.exit_code == 0, show_cli_trace(result)
+        converter.write(pkg_root)
 
         with add_to_sys_path(pkg_root):
             try:
-                pydra_module = import_module(output_module_path)
+                pydra_module = import_module(converter.output_module)
             except Exception as e:
                 add_exc_note(
                     e,
-                    f"Attempting to import {task_spec['task_name']} from '{output_module_path}'",
+                    f"Attempting to import {interface_spec['task_name']} from '{converter.output_module}'",
                 )
                 raise e
-        pydra_task = getattr(pydra_module, task_spec["task_name"])
+        pydra_task = getattr(pydra_module, interface_spec["task_name"])
         nipype_interface = getattr(
-            import_module(task_spec["nipype_module"]), task_spec["nipype_name"]
+            import_module(interface_spec["nipype_module"]),
+            interface_spec["nipype_name"],
         )
-        assert nipype_interface.__name__ == task_spec["nipype_name"]  # sanity check
+        assert (
+            nipype_interface.__name__ == interface_spec["nipype_name"]
+        )  # sanity check
 
         nipype_input_names = nipype_interface.input_spec().all_trait_names()
-        inputs_omit = task_spec["inputs"]["omit"] if task_spec["inputs"]["omit"] else []
+        inputs_omit = (
+            interface_spec["inputs"]["omit"] if interface_spec["inputs"]["omit"] else []
+        )
 
         assert sorted(
             f[0] for f in pydra_task().input_spec.fields if not f[0].startswith("_")
         ) == sorted(
             n
             for n in nipype_input_names
             if not (
@@ -102,15 +110,17 @@
                 or (n.endswith("_items") and n[: -len("_items")] in nipype_input_names)
             )
         )
 
         if nipype_interface.output_spec:
             nipype_output_names = nipype_interface.output_spec().all_trait_names()
             outputs_omit = (
-                task_spec["outputs"]["omit"] if task_spec["outputs"]["omit"] else []
+                interface_spec["outputs"]["omit"]
+                if interface_spec["outputs"]["omit"]
+                else []
             )
 
             assert sorted(
                 f[0]
                 for f in pydra_task().output_spec.fields
                 if not f[0].startswith("_")
             ) == sorted(
@@ -148,15 +158,15 @@
         # # logging.info("Running generated tests for %s", output_module_path)
         # # # Run generated pytests
         # # with add_to_sys_path(pkg_root):
         # #     result = pytest.main([str(tests_fspath)])
 
         # assert result.value == 0
     except Exception:
-        task_name = task_spec_file.parent.name + "-" + task_spec_file.stem
+        task_name = interface_spec_file.parent.name + "-" + interface_spec_file.stem
         if task_name in XFAIL_INTERFACES or task_name in XFAIL_INTERFACES_IN_COMBINED:
             msg = f"Test for '{task_name}' is expected to fail:\n{format_exc()}"
             if task_name in XFAIL_INTERFACES_IN_COMBINED:
                 msg += (
                     "\nNote that it isn't expected to fail when you run it separately, "
                     "not sure why the interfaces are getting mixed up between tests but "
                     "looks like it comes from another interface"
```

### Comparing `nipype2pydra-0.3.5/LICENSE` & `nipype2pydra-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/README.rst` & `nipype2pydra-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.5/pyproject.toml` & `nipype2pydra-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "pydra",
     "PyYAML>=6.0",
     "fileformats >=0.8",
     "fileformats-medimage >=0.4",
     "fileformats-datascience",
     "requests>=2.31.0",
     "traits",
+    "tqdm",
 ]
 license = { file = "LICENSE" }
 authors = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 maintainers = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 keywords = ["nipype", "data", "pydra", "workflows", "converters"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -46,14 +47,18 @@
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
     "fileformats-medimage-extras",
     "fileformats-medimage-afni",
     "fileformats-medimage-ants",
     "fileformats-medimage-freesurfer",
     "fileformats-medimage-fsl",
+    "niworkflows",
+    "mriqc",
+    "nireports",
+    "nitime",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
```

### Comparing `nipype2pydra-0.3.5/PKG-INFO` & `nipype2pydra-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipype2pydra
-Version: 0.3.5
+Version: 0.4.0
 Summary: Tool for converting Nipype tasks and workflows into Pydra syntax
 Project-URL: repository, https://github.com/nipype/nipype2pydra
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -116,14 +116,15 @@
 Requires-Dist: fileformats-datascience
 Requires-Dist: fileformats-medimage>=0.4
 Requires-Dist: fileformats>=0.8
 Requires-Dist: nipype
 Requires-Dist: pydra
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.31.0
+Requires-Dist: tqdm
 Requires-Dist: traits
 Provides-Extra: dev
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
@@ -137,14 +138,18 @@
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: fileformats-medimage-afni; extra == 'test'
 Requires-Dist: fileformats-medimage-ants; extra == 'test'
 Requires-Dist: fileformats-medimage-extras; extra == 'test'
 Requires-Dist: fileformats-medimage-freesurfer; extra == 'test'
 Requires-Dist: fileformats-medimage-fsl; extra == 'test'
+Requires-Dist: mriqc; extra == 'test'
+Requires-Dist: nireports; extra == 'test'
+Requires-Dist: nitime; extra == 'test'
+Requires-Dist: niworkflows; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 Nipype2Pydra
 ============
```

