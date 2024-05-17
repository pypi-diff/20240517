# Comparing `tmp/nipype2pydra-0.3.4.tar.gz` & `tmp/nipype2pydra-0.3.5.tar.gz`

## Comparing `nipype2pydra-0.3.4.tar` & `nipype2pydra-0.3.5.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/_version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/exceptions.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/testing.py
--rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/cli/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/cli/base.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/cli/pkg_gen.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/cli/task.py
--rw-r--r--   0        0        0    43825 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/afni-qwarp-only.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/example-packages.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/fastsurfer-only.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/freesurfer-mris-convert-only.yaml
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/freesurfer-only.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/fsl-filmgls-only.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/fsl-only.yaml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/mriqc.yaml
--rw-r--r--   0        0        0    16673 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/nipype-interfaces-to-import.yaml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/qsiprep.yaml
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/README.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/pkg_init.py
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/task/__init__.py
--rw-r--r--   0        0        0    38052 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/task/base.py
--rw-r--r--   0        0        0    16701 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/task/function.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/task/shell_command.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/task/tests/test_task.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/tests/test_pkg_gen.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/nipype2pydra/tests/test_utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/LICENSE
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/README.rst
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 nipype2pydra-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/_version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/exceptions.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/testing.py
+-rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/base.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/pkg_gen.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/cli/task.py
+-rw-r--r--   0        0        0    44133 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/afni-qwarp-only.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/example-packages.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fastsurfer-only.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/freesurfer-mris-convert-only.yaml
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/freesurfer-only.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fsl-filmgls-only.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/fsl-only.yaml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/mriqc.yaml
+-rw-r--r--   0        0        0    16673 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/nipype-interfaces-to-import.yaml
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/qsiprep.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/NOTICE
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/README.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/pkg_init.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/__init__.py
+-rw-r--r--   0        0        0    38808 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/base.py
+-rw-r--r--   0        0        0    16701 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/function.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/shell_command.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/task/tests/test_task.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/tests/test_pkg_gen.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/nipype2pydra/tests/test_utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/README.rst
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 nipype2pydra-0.3.5/PKG-INFO
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/testing.py` & `nipype2pydra-0.3.5/nipype2pydra/testing.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/utils.py` & `nipype2pydra-0.3.5/nipype2pydra/utils.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/cli/pkg_gen.py` & `nipype2pydra-0.3.5/nipype2pydra/cli/pkg_gen.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/cli/task.py` & `nipype2pydra-0.3.5/nipype2pydra/cli/task.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/__init__.py` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
                 )
                 doctests.append(
                     self._fields_stub(
                         "doctest",
                         DocTestGenerator,
                         {
                             "cmdline": cmdline,
-                            "inputs": copy(test_inpts),
+                            "inputs": copy(inpts),
                             "imports": imports,
                             "directive": directive,
                         },
                     )
                 )
                 self.has_doctests = True
         return tests, doctests
@@ -649,14 +649,19 @@
     os.unlink(pkg_dir / "README.md")
     with open(TEMPLATES_DIR / "README.rst") as f:
         readme_rst = f.read()
     readme_rst = readme_rst.replace("=" * 31, "=" * (23 + len(pkg)))
     with open(pkg_dir / "README.rst", "w") as f:
         f.write(readme_rst)
 
+    with open(pkg_dir / "AUTHORS", "w") as f:
+        f.write("# Enter list of names and emails of contributors to this package")
+
+    shutil.copyfile(TEMPLATES_DIR / "NOTICE", pkg_dir / "NOTICE")
+
     fileformat_readme_path = related_pkgs_dir / "fileformats" / "README.rst"
     with open(fileformat_readme_path) as f:
         ff_readme_rst = f.read()
     ff_readme_rst = ff_readme_rst.replace("=" * 29, "=" * (21 + len(pkg)))
     with open(fileformat_readme_path, "w") as f:
         f.write(ff_readme_rst)
 
@@ -674,14 +679,17 @@
     pyproject_toml = pyproject_toml.replace("README.md", "README.rst")
     pyproject_toml = pyproject_toml.replace(
         "test = [\n", 'test = [\n    "nipype2pydra",\n'
     )
     with open(pkg_dir / "pyproject.toml", "w") as f:
         f.write(pyproject_toml)
 
+    for tool_path in (TEMPLATES_DIR / "tools").iterdir():
+        shutil.copyfile(tool_path, pkg_dir / tool_path.name)
+
     # Add "pydra.tasks.<pkg>.auto to gitignore"
     with open(pkg_dir / ".gitignore", "a") as f:
         f.write(f"\n/pydra/tasks/{pkg}/auto" f"\n/pydra/tasks/{pkg}/_version.py\n")
 
     # rename tasks directory
     (pkg_dir / "pydra" / "tasks" / "CHANGEME").rename(pkg_dir / "pydra" / "tasks" / pkg)
     (
@@ -716,15 +724,15 @@
 
     # Replace "CHANGEME" string with pkg name
     for fspath in pkg_dir.glob("**/*"):
         if fspath.is_dir() or fspath.suffix in (".pyc", ".pyo", ".pyd"):
             continue
         with open(fspath) as f:
             contents = f.read()
-        contents = re.sub(r"\bCHANGEME\b", pkg, contents)
+        contents = contents.replace("CHANGEME", pkg)
         with open(fspath, "w") as f:
             f.write(contents)
 
     return pkg_dir
 
 
 def extract_doctest_inputs(
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/freesurfer-only.yaml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/freesurfer-only.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/mriqc.yaml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/mriqc.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/nipype-interfaces-to-import.yaml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/nipype-interfaces-to-import.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/specs/qsiprep.yaml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/specs/qsiprep.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/README.rst` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert.py` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import os.path
 from warnings import warn
 from pathlib import Path
 import shutil
 from importlib import import_module
 import yaml
+from tqdm import tqdm
 import nipype
 import nipype2pydra.utils
 from nipype2pydra.task import get_converter
 
 
 SPECS_DIR = Path(__file__).parent / "specs"
 PKG_ROOT = Path(__file__).parent.parent
@@ -32,15 +33,17 @@
 auto_init = f"# Auto-generated by {__file__}, do not edit as it will be overwritten\n\n"
 
 auto_dir = PKG_ROOT / "pydra" / "tasks" / PKG_NAME / "auto"
 if auto_dir.exists():
     shutil.rmtree(auto_dir)
 
 all_interfaces = []
-for fspath in sorted(SPECS_DIR.glob("**/*.yaml")):
+for fspath in tqdm(
+    sorted(SPECS_DIR.glob("**/*.yaml")), "converting interfaces from Nipype to Pydra"
+):
     with open(fspath) as f:
         spec = yaml.load(f, Loader=yaml.SafeLoader)
 
     rel_pkg_path = str(fspath.parent.relative_to(SPECS_DIR)).replace(os.path.sep, ".")
     if rel_pkg_path == ".":
         rel_pkg_path = fspath.stem
     else:
@@ -66,11 +69,13 @@
 
 nipype_version = "{nipype.__version__.split('.dev')[0]}"
 nipype2pydra_version = "{nipype2pydra.__version__.split('.dev')[0]}"
 post_release = (nipype_version + nipype2pydra_version).replace(".", "")
 """
     )
 
-auto_init += "\n\n__all__ = [\n" + "\n".join(f"    \"{i}\"," for i in all_interfaces) + "\n]\n"
+auto_init += (
+    "\n\n__all__ = [\n" + "\n".join(f'    "{i}",' for i in all_interfaces) + "\n]\n"
+)
 
 with open(PKG_ROOT / "pydra" / "tasks" / PKG_NAME / "auto" / "__init__.py", "w") as f:
     f.write(auto_init)
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/pkg_init.py` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/pkg_init.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -5,39 +5,51 @@
 # https://docs.github.com/en/actions/reference/encrypted-secrets
 
 name: CI/CD
 
 on:
   push:
     branches: [ main, develop ]
-    tags: [ '*' ]
   pull_request:
     branches: [ main, develop ]
+  release:
+    types: [published]
   repository_dispatch:
-    types: [create-release]
+    types: [create-post-release]
+
+env:
+  CHANGEME_version: <set-CHANGEME-version-here>
+  CHANGEME_install_dir:  ${{ github.workspace }}/install
 
 jobs:
 
   nipype-conv:
     runs-on: ubuntu-latest
     steps:
+
     - name: Checkout
       uses: actions/checkout@v4
-    - name: Revert version to most recent tag on upstream update
+
+    - name: Revert version to most recent version tag on upstream update
       if: github.event_name == 'repository_dispatch'
-      run: git checkout $(git tag -l | tail -n 1 | awk -F post '{print $1}')    
-    - name: Set up Python ${{ matrix.python-version }}
+      run: git checkout $(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')
+ 
+    - name: Set up Python
       uses: actions/setup-python@v5
+
     - name: Install build dependencies
       run: python -m pip install --upgrade pip
+
     - name: Install requirements
       run: python -m pip install ./related-packages/fileformats -r ./nipype-auto-conv/requirements.txt
+
     - name: Run automatic Nipype > Pydra conversion
       run: ./nipype-auto-conv/generate
-    - uses: actions/upload-artifact@v3
+
+    - uses: actions/upload-artifact@v4
       with:
         name: converted-nipype
         path: pydra/tasks/CHANGEME/auto
 
   devcheck:
     needs: [nipype-conv]
     runs-on: ubuntu-latest
@@ -47,259 +59,348 @@
         pip-flags: ['', '--editable']
         pydra:
         - 'pydra'
         - '--editable git+https://github.com/nipype/pydra.git#egg=pydra'
     steps:
     - name: Checkout
       uses: actions/checkout@v4
-    - name: Revert version to most recent tag on upstream update
+
+    - name: Revert version to most recent version tag on upstream update
       if: github.event_name == 'repository_dispatch'
-      run: git checkout $(git tag -l | tail -n 1 | awk -F post '{print $1}')    
+      run: git checkout $(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')
+
     - name: Download tasks converted from Nipype 
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: converted-nipype
         path: pydra/tasks/CHANGEME/auto
+
     - name: Strip auto package from gitignore so it is included in package
       run: |
         sed -i '/\/pydra\/tasks\/CHANGEME\/auto/d' .gitignore
+        sed -i '/^_version.py/d' .gitignore
+
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install build dependencies
       run: |
         python -m pip install --upgrade pip
+ 
     - name: Install Pydra
       run: |
         pushd $HOME
         pip install ${{ matrix.pydra }}
         popd
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
+
     - name: Install task package
       run: |
-        pip install "./related-packages/fileformats[dev]" "related-packages/fileformats-extras[dev]"
+        pip install ${{ matrix.pip-flags }} "./related-packages/fileformats[dev]"
+        pip install ${{ matrix.pip-flags }} "related-packages/fileformats-extras[dev]"
         pip install ${{ matrix.pip-flags }} ".[dev]"
         python -c "import pydra.tasks.CHANGEME as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import fileformats.medimage_CHANGEME as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import fileformats.extras.medimage_CHANGEME as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
-  
-  fileformats-test:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ['3.8', '3.11']
-    steps:
-    - uses: actions/checkout@v4
-    - name: Revert version to most recent tag on upstream update
-      if: github.event_name == 'repository_dispatch'
-      run: git checkout $(git tag -l | tail -n 1 | awk -F post '{print $1}')
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v5
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install build dependencies
-      run: |
-        python -m pip install --upgrade pip
-    - name: Install task package
-      run: |
-        pip install "./related-packages/fileformats[test]" "./related-packages/fileformats-extras[test]"
-        python -c "import fileformats.medimage_CHANGEME as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
-    - name: Test fileformats with pytest
-      run: |
-        cd ./fileformats
-        pytest -sv --cov fileformats.medimage_CHANGEME --cov fileformats.extras.medimage_CHANGEME --cov-report xml .
 
   test:
-    needs: [nipype-conv, fileformats-test]
-    runs-on: ubuntu-22.04
+    needs: [nipype-conv]
+    runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.8']  # '3.11'
+        python-version: ['3.8', '3.11']
     steps:
+    
     - name: Removed unnecessary tools to free space
       run: |
         sudo rm -rf /usr/share/dotnet
-        sudo rm -rf "$AGENT_TOOLSDIRECTORY"      
-    - name: Get Download cache Key
-      id: cache-key
-      run: echo "::set-output name=key::CHANGEME-linux-ubuntu22_amd64-7.4.1"
-    - name: Cache FreeSurfer
-      uses: actions/cache@v2
-      with:
-        path: $HOME/downloads/CHANGEME
-        key: ${{ steps.cache-key.outputs.key }}
-        restore-keys: |
-          CHANGEME-linux-ubuntu22_amd64-7.4.1
-    - name: Download FreeSurfer
-      if: steps.cache-key.outputs.key != steps.cache-hit.outputs.key
-      run: |
-        mkdir -p $HOME/downloads/CHANGEME
-        curl -s -o $HOME/downloads/CHANGEME/CHANGEME-linux-ubuntu22_amd64-7.4.1.tar.gz https://surfer.nmr.mgh.harvard.edu/pub/dist/CHANGEME/7.4.1/CHANGEME-linux-ubuntu22_amd64-7.4.1.tar.gz
-      shell: bash
-    - name: Install Freesurfer
-      env:
-        FREESURFER_LICENCE: ${{ secrets.FREESURFER_LICENCE }}
-      run: |
-        pushd $HOME/downloads/CHANGEME
-        tar -zxpf CHANGEME-linux-ubuntu22_amd64-7.4.1.tar.gz
-        mv CHANGEME $HOME/
-        popd
-        export FREESURFER_HOME=$HOME/CHANGEME
-        source $FREESURFER_HOME/SetUpFreeSurfer.sh
-        echo $FREESURFER_LICENCE > $FREESURFER_HOME/license.txt
-        export PATH=$FREESURFER_HOME/bin:$PATH
-    - uses: actions/checkout@v4
-    - name: Revert version to most recent tag on upstream update
+        sudo rm -rf "$AGENT_TOOLSDIRECTORY"
+
+    - name: Checkout repo
+      uses: actions/checkout@v4
+
+    - name: Revert version to most recent version tag on Nipype or Nipype2Pydra update
       if: github.event_name == 'repository_dispatch'
-      run: git checkout $(git tag -l | tail -n 1 | awk -F post '{print $1}')
+      run: git checkout $(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')
+
+    - name: Cache CHANGEME Install
+      id: cache-install
+      uses: actions/cache@v4
+      with:
+        path: ${{ env.CHANGEME_install_dir }}
+        key: CHANGEME-${{ env.CHANGEME_version }}-${{ runner.os }}
+
+    - name: Install CHANGEME Package
+      if: steps.cache-install.outputs.cache-hit != 'true'
+      run: |
+        echo "NOT IMPLEMENTED YET (install at CHANGEME_install_dir: $CHANGEME_install_dir)"
+        exit 1  # This is a placeholder, replace this line and the one above with the installation procedure
+        echo "PATH=${{ env.CHANGEME_install_dir }}/bin:$PATH" >> $GITHUB_ENV
+    
     - name: Download tasks converted from Nipype 
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: converted-nipype
         path: pydra/tasks/CHANGEME/auto
+
+    - name: Show the contents of the auto-generated tasks
+      run: tree pydra
+
     - name: Strip auto package from gitignore so it is included in package
       run: |
-        sed -i '/\/src\/pydra\/tasks\/CHANGEME\/auto/d' .gitignore
+        sed -i '/\/pydra\/tasks\/CHANGEME\/auto/d' .gitignore
+
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install build dependencies
       run: |
         python -m pip install --upgrade pip
+
     - name: Install task package
       run: |
         pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
         python -c "import pydra.tasks.CHANGEME as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
+
     - name: Test with pytest
-      run: |
-        pytest -sv --doctest-modules ./pydra/tasks/CHANGEME \
-            --cov pydra.tasks.CHANGEME --cov-report xml
-    - uses: codecov/codecov-action@v3
+      run: >- 
+        pytest -sv
+        ./pydra/tasks/CHANGEME
+        ./related-packages/fileformats
+        ./related-packages/fileformats-extras
+        --cov pydra.tasks.CHANGEME
+        --cov fileformats.medimage_CHANGEME
+        --cov fileformats.extras.medimage_CHANGEME
+        --cov-report xml
+
+    - name: Upload to CodeCov
+      uses: codecov/codecov-action@v3
       if: ${{ always() }}
       with:
-        files: coverage.xml,./fileformats/coverage.xml
+        files: coverage.xml
         name: pydra-CHANGEME
 
+
   deploy-fileformats:
     needs: [devcheck, test]
     runs-on: ubuntu-latest
     steps:
+
     - uses: actions/checkout@v4
       with:
         submodules: recursive
-        fetch-depth: 0 
+        fetch-depth: 0
+
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.11'
+
     - name: Install build tools
       run: python -m pip install build twine
+
     - name: Build source and wheel distributions
       run: python -m build ./related-packages/fileformats
+
     - name: Check distributions
       run: twine check ./related-packages/fileformats/dist/*
+
     - name: Check for PyPI token on tag
       id: deployable
-      if: (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) || github.event_name == 'repository_dispatch'
+      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       env:
         PYPI_API_TOKEN: "${{ secrets.PYPI_FILEFORMATS_API_TOKEN }}"
       run: if [ -n "$PYPI_API_TOKEN" ]; then echo "DEPLOY=true" >> $GITHUB_OUTPUT; fi
+
     - name: Upload to PyPI
       if: steps.deployable.outputs.DEPLOY
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_FILEFORMATS_API_TOKEN }}
         packages-dir: ./related-packages/fileformats/dist 
 
   deploy-fileformats-extras:
     needs: [deploy-fileformats]
     runs-on: ubuntu-latest
     steps:
+
     - uses: actions/checkout@v4
       with:
         submodules: recursive
-        fetch-depth: 0 
+        fetch-depth: 0
+
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.11'
+
     - name: Install build tools
       run: python -m pip install build twine
+
     - name: Build source and wheel distributions
       run: python -m build ./related-packages/fileformats-extras
+
     - name: Check distributions
       run: twine check ./related-packages/fileformats-extras/dist/*
+
     - name: Check for PyPI token on tag
       id: deployable
-      if: (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) || github.event_name == 'repository_dispatch'
+      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       env:
         PYPI_API_TOKEN: "${{ secrets.PYPI_FILEFORMATS_EXTRAS_API_TOKEN }}"
       run: if [ -n "$PYPI_API_TOKEN" ]; then echo "DEPLOY=true" >> $GITHUB_OUTPUT; fi
+
     - name: Upload to PyPI
       if: steps.deployable.outputs.DEPLOY
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_FILEFORMATS_EXTRAS_API_TOKEN }}
         packages-dir: ./related-packages/fileformats-extras/dist 
 
   deploy:
-    needs: [deploy-fileformats-extras]
+    needs: [nipype-conv, test, deploy-fileformats, deploy-fileformats-extras]
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
+
+    - name: Checkout repository
+      uses: actions/checkout@v4
       with:
         submodules: recursive
         fetch-depth: 0
+
+    - name: Set up Git user
+      run: |
+        git config --local user.email "action@github.com"
+        git config --local user.name "GitHub Action"
+
+    - name: Get latest version tag
+      id: latest_tag
+      run: |
+        git fetch --tags
+        echo "TAG=$(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')" >> $GITHUB_OUTPUT
+
+    - name: Revert to latest tag
+      if: github.event_name == 'repository_dispatch'
+      run: git checkout ${{ steps.latest_tag.outputs.TAG }}
+
     - name: Download tasks converted from Nipype 
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: converted-nipype
         path: pydra/tasks/CHANGEME/auto
-    - name: Tag release with a post-release based on Nipype and Nipype2Pydra versions
-      if: github.event_name == 'repository_dispatch'
-      run: |
-        TAG=$(git tag -l | tail -n 1 | awk -F post '{print $1}')
-        POST=$(python -c "from pydra.tasks.CHANGEME.auto._version import *; print(post_release)")
-        git checkout $TAG
-        git add -f pydra/tasks/CHANGEME/auto/_version.py
-        git commit -am"added auto-generated version to make new tag for package version"
-        git tag ${TAG}post${POST}    
+
+    - name: Show the contents of the auto-generated tasks
+      run: tree pydra
+
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.11'
+
     - name: Install build tools
       run: python -m pip install build twine
+
     - name: Strip auto package from gitignore so it is included in package
       run: |
         sed -i '/\/pydra\/tasks\/CHANGEME\/auto/d' .gitignore
+        cat .gitignore
+
+    - name: Install task package to calculate post-release tag
+      run: |
+        pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
+
+    - name: Generate post-release tag based on Nipype and Nipype2Pydra versions
+      id: post_release_tag
+      run: |
+        POST=$(python -c "from pydra.tasks.CHANGEME.auto._version import *; print(post_release)")
+        echo "TAG=${{ steps.latest_tag.outputs.TAG }}post${POST}" >> $GITHUB_OUTPUT
+
+    - name: Add auto directory to git repo
+      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
+      run: |
+        git add pydra/tasks/CHANGEME/auto
+        git commit -am"added auto-generated version to make new tag for package version"
+        git status
+
+    - name: Overwrite the tag of release event with latest commit (i.e. including the auto directory)
+      if: github.event_name == 'release'
+      run: |
+        git tag -d ${{ steps.latest_tag.outputs.TAG }};
+        git tag ${{ steps.latest_tag.outputs.TAG }};
+
+    - name: Tag repo with the post-release
+      if: github.event_name == 'repository_dispatch'
+      run: git tag ${{ steps.post_release_tag.outputs.TAG }}
+
     - name: Build source and wheel distributions
       run: python -m build .
+
     - name: Check distributions
       run: twine check dist/*
-    - uses: actions/upload-artifact@v3
+
+    - uses: actions/upload-artifact@v4
       with:
         name: distributions
         path: dist/
+
     - name: Check for PyPI token on tag
       id: deployable
-      if: (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) || github.event_name == 'repository_dispatch'
+      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       env:
         PYPI_API_TOKEN: "${{ secrets.PYPI_API_TOKEN }}"
       run: if [ -n "$PYPI_API_TOKEN" ]; then echo "DEPLOY=true" >> $GITHUB_OUTPUT; fi
+
     - name: Upload to PyPI
       if: steps.deployable.outputs.DEPLOY
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}   
+        password: ${{ secrets.PYPI_API_TOKEN }}
+
+    - name: Create post-release release for releases triggered by nipype2pydra dispatches
+      if: steps.deployable.outputs.DEPLOY && github.event_name == 'repository_dispatch'
+      uses: actions/create-release@v1
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided by Actions, you do not need to create your own token
+      with:
+        tag_name: ${{ steps.post_release_tag.outputs.TAG }}
+        release_name: Release ${{ steps.post_release_tag.outputs.TAG }}
+        draft: false
+        prerelease: false        
+
+
+  report_progress:
+    needs: [deploy]
+    runs-on: ubuntu-latest
+    steps:
+
+      - name: Generate progress report
+        id: generate-report
+        run: |
+          tools/report_progress.py outputs/progress-report.json
+          echo "progress_report=$(cat outputs/progress-report.json)" >> $GITHUB_OUTPUT
+
+      - name: Report progress to Nipype2Pydra repo
+        if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
+        run: >-
+          curl -XPOST -u "${{ env.POST_RELEASE_PAT }}" -H "Accept: application/vnd.github.everest-preview+json"
+          "https://api.github.com/repos/nipype/pydra-CHANGEME/dispatches"
+          -d '{
+            "event_type": "progress-report",
+            "client_payload": ${{ steps.generate-report.output.progress_report }}
+          }'
+        env:
+          PAT: ${{ env.PROGRESS_REPORT_PAT }}
+
 
 # Deploy on tags if PYPI_API_TOKEN is defined in the repository secrets.
 # Secrets are not accessible in the if: condition [0], so set an output variable [1]
 # [0] https://github.community/t/16928
-# [1] https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#setting-an-output-parameter        
+# [1] https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#setting-an-output-parameter
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml` & `nipype2pydra-0.3.5/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/task/__init__.py` & `nipype2pydra-0.3.5/nipype2pydra/task/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/task/base.py` & `nipype2pydra-0.3.5/nipype2pydra/task/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -907,15 +907,31 @@
                     val = doctest.inputs[nm]
                 except KeyError:
                     if is_fileset(tp):
                         val = f"{tp.__name__}.mock()"
                     else:
                         val = attrs.NOTHING
                 else:
-                    if isinstance(val, str):
+                    if is_fileset(tp):
+                        val = f"{tp.__name__}.mock({val})"
+                    elif ty.get_origin(tp) is list and is_fileset(ty.get_args(tp)[0]):
+                        try:
+                            val = eval(val)
+                        except Exception:
+                            pass
+                        else:
+                            val = (
+                                "["
+                                + ", ".join(
+                                    f'{ty.get_args(tp)[0].__name__}.mock("{v}")'
+                                    for v in val
+                                )
+                                + "]"
+                            )
+                    elif tp is str and not (val.startswith("'") or val.startswith('"')):
                         val = f'"{val}"'
                 if val is None and is_fileset(tp):
                     val = f"{tp.__name__}.mock()"
                 if val is not attrs.NOTHING:
                     doctest_str += f"    >>> task.inputs.{nm} = {val}\n"
             doctest_str += "    >>> task.cmdline\n"
             doctest_str += f"    '{doctest.cmdline}'"
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/task/function.py` & `nipype2pydra-0.3.5/nipype2pydra/task/function.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/task/shell_command.py` & `nipype2pydra-0.3.5/nipype2pydra/task/shell_command.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/nipype2pydra/task/tests/test_task.py` & `nipype2pydra-0.3.5/nipype2pydra/task/tests/test_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from importlib import import_module
 import yaml
 import pytest
 import logging
-from nipype2pydra.utils import show_cli_trace
+import io
+import contextlib
 from traceback import format_exc
 from nipype2pydra.cli.task import task as task_cli
-from nipype2pydra.utils import add_to_sys_path, add_exc_note, INBUILT_NIPYPE_TRAIT_NAMES
+from nipype2pydra.utils import (
+    add_to_sys_path,
+    add_exc_note,
+    INBUILT_NIPYPE_TRAIT_NAMES,
+    show_cli_trace,
+)
 from conftest import EXAMPLE_TASKS_DIR
 
 
 logging.basicConfig(level=logging.INFO)
 
 
 XFAIL_INTERFACES = [
@@ -116,14 +122,31 @@
                     or (
                         n.endswith("_items")
                         and n[: -len("_items")] in nipype_output_names
                     )
                 )
             )
 
+        # Run doctests
+        # logging.info("Running doctests for %s", output_module_path)
+        # with add_to_sys_path(pkg_root):
+        #     with contextlib.redirect_stdout(io.StringIO()) as f:
+        #         exit_code = pytest.main(
+        #             [
+        #                 str(
+        #                     pkg_root.joinpath(
+        #                         *output_module_path.split(".")
+        #                     ).with_suffix(".py")
+        #                 ),
+        #                 "--doctest-modules",
+        #                 "--ignore-glob=test_*.py",
+        #             ]
+        #         )
+
+        # assert not exit_code, f.getvalue()
         # tests_fspath = pkg_root.joinpath(*output_module_path.split(".")).parent / "tests"
 
         # # logging.info("Running generated tests for %s", output_module_path)
         # # # Run generated pytests
         # # with add_to_sys_path(pkg_root):
         # #     result = pytest.main([str(tests_fspath)])
```

### Comparing `nipype2pydra-0.3.4/nipype2pydra/tests/test_utils.py` & `nipype2pydra-0.3.5/nipype2pydra/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/LICENSE` & `nipype2pydra-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/README.rst` & `nipype2pydra-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/pyproject.toml` & `nipype2pydra-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.3.4/PKG-INFO` & `nipype2pydra-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipype2pydra
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tool for converting Nipype tasks and workflows into Pydra syntax
 Project-URL: repository, https://github.com/nipype/nipype2pydra
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

