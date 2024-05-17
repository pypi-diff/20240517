# Comparing `tmp/cookieplone-0.6.0.tar.gz` & `tmp/cookieplone-0.6.1.tar.gz`

## Comparing `cookieplone-0.6.0.tar` & `cookieplone-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 cookieplone-0.6.0/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.6.0/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/__main__.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/plone.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.6.0/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.6.0/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/test_filters.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/_resources/plone/dependencies.zcml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/_resources/plone/metadata.xml
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_internal.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_plone.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.6.0/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.6.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.6.0/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.6.0/README.md
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cookieplone-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 cookieplone-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 cookieplone-0.6.1/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.6.1/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.6.1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/plone.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.6.1/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.6.1/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/test_filters.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/_resources/plone/dependencies.zcml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/_resources/plone/metadata.xml
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_internal.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_plone.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.6.1/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.6.1/README.md
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cookieplone-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 cookieplone-0.6.1/PKG-INFO
```

### Comparing `cookieplone-0.6.0/.pre-commit-config.yaml` & `cookieplone-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/CHANGES.md` & `cookieplone-0.6.1/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.6.1 (2024-05-17)
+
+
+### Bug fixes:
+
+- Small fixes to cookieplone/utils/plone.py functions [@ericof] 
+
 ## 0.6.0 (2024-05-17)
 
 
 ### New features:
 
 - Add functions `add_dependency_profile_to_metadata` and `add_dependency_to_zcml` to manipulate Plone files [@ericof] [#25](https://github.com/plone/cookieplone/issues/25)
```

### Comparing `cookieplone-0.6.0/Makefile` & `cookieplone-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/.github/workflows/changelog.yml` & `cookieplone-0.6.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/.github/workflows/main.yml` & `cookieplone-0.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/cli.py` & `cookieplone-0.6.1/cookieplone/cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/data.py` & `cookieplone-0.6.1/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/exceptions.py` & `cookieplone-0.6.1/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/generator.py` & `cookieplone-0.6.1/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/repository.py` & `cookieplone-0.6.1/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/settings.py` & `cookieplone-0.6.1/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/filters/__init__.py` & `cookieplone-0.6.1/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/console.py` & `cookieplone-0.6.1/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/files.py` & `cookieplone-0.6.1/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/git.py` & `cookieplone-0.6.1/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/internal.py` & `cookieplone-0.6.1/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/sanity.py` & `cookieplone-0.6.1/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/validators.py` & `cookieplone-0.6.1/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/versions.py` & `cookieplone-0.6.1/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/cookieplone/utils/commands/__init__.py` & `cookieplone-0.6.1/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/conftest.py` & `cookieplone-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/test_cli.py` & `cookieplone-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/test_filters.py` & `cookieplone-0.6.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_commands.py` & `cookieplone-0.6.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_console.py` & `cookieplone-0.6.1/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_files.py` & `cookieplone-0.6.1/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_git.py` & `cookieplone-0.6.1/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_internal.py` & `cookieplone-0.6.1/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_plone.py` & `cookieplone-0.6.1/tests/utils/test_plone.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_sanity.py` & `cookieplone-0.6.1/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_validators.py` & `cookieplone-0.6.1/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/tests/utils/test_versions.py` & `cookieplone-0.6.1/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/.gitignore` & `cookieplone-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/LICENSE` & `cookieplone-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/README.md` & `cookieplone-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/pyproject.toml` & `cookieplone-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.0/PKG-INFO` & `cookieplone-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.6.0
+Version: 0.6.1
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

