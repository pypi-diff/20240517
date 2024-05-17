# Comparing `tmp/reqs_cli-0.20240517.1.tar.gz` & `tmp/reqs_cli-0.20240517.2.tar.gz`

## Comparing `reqs_cli-0.20240517.1.tar` & `reqs_cli-0.20240517.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.copier-answers-py.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.coveragerc
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/noxfile.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/readme.md
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/ruff.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.circleci/config.yml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.mise/config.toml
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.mise/tasks/hello
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/ci/.gitignore
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/ci/pytest.ini
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/ci/test-reports/tests.pytests.xml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/mise/config.toml
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/mise/tasks/bootstrap
--rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/mise/tasks/bump
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/base.in
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/base.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/ci.in
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/ci.txt
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/dev.in
--rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/requirements/dev.txt
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/tasks_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/cli.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/config.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/utils.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/__init__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/test_cli.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg1/foo/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg1/requirements/base.in
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg1/requirements/ci.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg1/requirements/dev.in
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg3/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg3/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg4/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg4/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/src/reqs/tests/pkg4/requirements/foo.in
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/.gitignore
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/hatch.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/pyproject.toml
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.1/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.copier-answers-py.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.coveragerc
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/noxfile.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ruff.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.circleci/config.yml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.mise/config.toml
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.mise/tasks/hello
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/.gitignore
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/pytest.ini
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/test-reports/tests.pytests.xml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/config.toml
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/tasks/bootstrap
+-rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/tasks/bump
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/base.in
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/base.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/ci.in
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/ci.txt
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/dev.in
+-rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/dev.txt
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/tasks_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/cli.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/config.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/utils.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/test_cli.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/base.in
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/ci.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/dev.in
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg3/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg3/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/requirements/foo.in
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.gitignore
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/hatch.toml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/pyproject.toml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/readme.md
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/PKG-INFO
```

### Comparing `reqs_cli-0.20240517.1/.pre-commit-config.yaml` & `reqs_cli-0.20240517.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/noxfile.py` & `reqs_cli-0.20240517.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/readme.md` & `reqs_cli-0.20240517.2/readme.md`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/ruff.toml` & `reqs_cli-0.20240517.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/.circleci/config.yml` & `reqs_cli-0.20240517.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/ci/pytest.ini` & `reqs_cli-0.20240517.2/ci/pytest.ini`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/ci/test-reports/tests.pytests.xml` & `reqs_cli-0.20240517.2/ci/test-reports/tests.pytests.xml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/mise/tasks/bump` & `reqs_cli-0.20240517.2/mise/tasks/bump`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/requirements/base.txt` & `reqs_cli-0.20240517.2/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/requirements/ci.txt` & `reqs_cli-0.20240517.2/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/requirements/dev.txt` & `reqs_cli-0.20240517.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/src/reqs/cli.py` & `reqs_cli-0.20240517.2/src/reqs/cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/src/reqs/config.py` & `reqs_cli-0.20240517.2/src/reqs/config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/src/reqs/utils.py` & `reqs_cli-0.20240517.2/src/reqs/utils.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/src/reqs/tests/test_cli.py` & `reqs_cli-0.20240517.2/src/reqs/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/src/reqs/tests/test_config.py` & `reqs_cli-0.20240517.2/src/reqs/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/hatch.toml` & `reqs_cli-0.20240517.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.1/PKG-INFO` & `reqs_cli-0.20240517.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: reqs-cli
-Version: 0.20240517.1
+Version: 0.20240517.2
 Author-email: Randy Syring <randy.syring@level12.io>
 Requires-Dist: build==1.2.1
 Requires-Dist: click==8.1.7
 Requires-Dist: coverage==7.5.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==24.0
 Requires-Dist: pip-tools==7.4.1
@@ -72,7 +72,53 @@
 Requires-Dist: tomlkit==0.12.5; extra == 'dev'
 Requires-Dist: trove-classifiers==2024.4.10; extra == 'dev'
 Requires-Dist: userpath==1.9.2; extra == 'dev'
 Requires-Dist: uv==0.1.44; extra == 'dev'
 Requires-Dist: virtualenv==20.26.2; extra == 'dev'
 Requires-Dist: wheel==0.43.0; extra == 'dev'
 Requires-Dist: zstandard==0.22.0; extra == 'dev'
+Description-Content-Type: text/markdown
+
+reqs
+====
+
+Bootstrap, compile, and sync Python requirements files
+
+# Install
+
+Intended to be used with pipx
+
+- manually & first install: `pipx install -e .../apps/reqs-pkg`; or
+- when developing: `cd .../apps/reqs-pkg;` [`reqs`](../reqs-pkg/) `sync`
+
+
+## Usage
+
+- `reqs bootstrap`: Upgrade pip & install pip-tools
+- `reqs compile`:  Compile .in to .txt when needed (based on file modification times)
+- `reqs sync`: Compile and then update active venv and maybe pipx to match spec
+
+
+# Configuration
+
+Configure using `pyproject.toml`:
+
+
+```toml
+# The options shown are the default values and DO NOT need to be specified
+# if the default is sufficient.
+
+[tool.reqs]
+# Path to the directory containing the .in and .txt requirements files.  Relative to pyproject.toml.
+dpath = 'requirements'
+
+# Use pipx to install an editable version of the project.  True for tools like reqs and env-config
+# that a developer would want available for different projects.  False for most client projects
+# deployed on servers.
+sync_pipx = false
+
+[tool.reqs.depends]
+# Define dependencies between files so `reqs compile` knows when a .in needs to be compiled and
+# what order to use when compiling multiple files.
+'base.in' = ''
+'dev.in' = 'base.txt'
+```
```

