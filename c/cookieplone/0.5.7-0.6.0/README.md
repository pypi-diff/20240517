# Comparing `tmp/cookieplone-0.5.7.tar.gz` & `tmp/cookieplone-0.6.0.tar.gz`

## Comparing `cookieplone-0.5.7.tar` & `cookieplone-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 cookieplone-0.5.7/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.7/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/__main__.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.7/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_git.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.7/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.7/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 cookieplone-0.6.0/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.6.0/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/plone.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.6.0/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/test_filters.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/_resources/plone/dependencies.zcml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/_resources/plone/metadata.xml
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_internal.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_plone.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.6.0/README.md
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cookieplone-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 cookieplone-0.6.0/PKG-INFO
```

### Comparing `cookieplone-0.5.7/.pre-commit-config.yaml` & `cookieplone-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/CHANGES.md` & `cookieplone-0.6.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.6.0 (2024-05-17)
+
+
+### New features:
+
+- Add functions `add_dependency_profile_to_metadata` and `add_dependency_to_zcml` to manipulate Plone files [@ericof] [#25](https://github.com/plone/cookieplone/issues/25)
+
 ## 0.5.7 (2024-05-16)
 
 
 ### Bug fixes:
 
 - Fix usage of `--replay-file` [@ericof] [#23](https://github.com/plone/cookieplone/issues/23)
```

### Comparing `cookieplone-0.5.7/Makefile` & `cookieplone-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/.github/workflows/changelog.yml` & `cookieplone-0.6.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/.github/workflows/main.yml` & `cookieplone-0.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/cli.py` & `cookieplone-0.6.0/cookieplone/cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/data.py` & `cookieplone-0.6.0/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/exceptions.py` & `cookieplone-0.6.0/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/generator.py` & `cookieplone-0.6.0/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/repository.py` & `cookieplone-0.6.0/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/settings.py` & `cookieplone-0.6.0/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/filters/__init__.py` & `cookieplone-0.6.0/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/console.py` & `cookieplone-0.6.0/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/files.py` & `cookieplone-0.6.0/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/git.py` & `cookieplone-0.6.0/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/internal.py` & `cookieplone-0.6.0/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/sanity.py` & `cookieplone-0.6.0/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/validators.py` & `cookieplone-0.6.0/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/versions.py` & `cookieplone-0.6.0/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/cookieplone/utils/commands/__init__.py` & `cookieplone-0.6.0/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/test_cli.py` & `cookieplone-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/test_filters.py` & `cookieplone-0.6.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_commands.py` & `cookieplone-0.6.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_console.py` & `cookieplone-0.6.0/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_files.py` & `cookieplone-0.6.0/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_git.py` & `cookieplone-0.6.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_internal.py` & `cookieplone-0.6.0/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_sanity.py` & `cookieplone-0.6.0/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_validators.py` & `cookieplone-0.6.0/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/tests/utils/test_versions.py` & `cookieplone-0.6.0/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/.gitignore` & `cookieplone-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/LICENSE` & `cookieplone-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/README.md` & `cookieplone-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.7/pyproject.toml` & `cookieplone-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
   "Topic :: Software Development :: Code Generators"
 ]
 dependencies = [
   "cookiecutter==2.6.0",
   "semver==3.0.2",
   "typer==0.12.3",
   "packaging==24.0",
-  "gitpython==3.1.43"
+  "gitpython==3.1.43",
+  "xmltodict==0.13.0",
 ]
 
 [project.scripts]
 cookieplone = 'cookieplone.__main__:main'
 
 [project.urls]
 Documentation = "https://github.com/plone/cookieplone#readme"
```

### Comparing `cookieplone-0.5.7/PKG-INFO` & `cookieplone-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.7
+Version: 0.6.0
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -25,14 +25,15 @@
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.10
 Requires-Dist: cookiecutter==2.6.0
 Requires-Dist: gitpython==3.1.43
 Requires-Dist: packaging==24.0
 Requires-Dist: semver==3.0.2
 Requires-Dist: typer==0.12.3
+Requires-Dist: xmltodict==0.13.0
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">
 </p>
 
 <h1 align="center">
```

