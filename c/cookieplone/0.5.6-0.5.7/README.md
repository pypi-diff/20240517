# Comparing `tmp/cookieplone-0.5.6.tar.gz` & `tmp/cookieplone-0.5.7.tar.gz`

## Comparing `cookieplone-0.5.6.tar` & `cookieplone-0.5.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 cookieplone-0.5.6/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.6/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/__main__.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.6/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_git.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.6/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.6/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 cookieplone-0.5.7/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.7/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.7/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.7/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.7/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.7/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.7/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.7/PKG-INFO
```

### Comparing `cookieplone-0.5.6/.pre-commit-config.yaml` & `cookieplone-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/CHANGES.md` & `cookieplone-0.5.7/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.5.7 (2024-05-16)
+
+
+### Bug fixes:
+
+- Fix usage of `--replay-file` [@ericof] [#23](https://github.com/plone/cookieplone/issues/23)
+
 ## 0.5.6 (2024-05-16)
 
 
 ### Bug fixes:
 
 - Handle in `cookieplone.generator._get_repository_root` the local development of templates containing pre_prompt hooks [@ericof]
```

### Comparing `cookieplone-0.5.6/Makefile` & `cookieplone-0.5.7/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/.github/workflows/changelog.yml` & `cookieplone-0.5.7/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/.github/workflows/main.yml` & `cookieplone-0.5.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/cli.py` & `cookieplone-0.5.7/cookieplone/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cookiecutter.log import configure_logger
 from rich.prompt import Prompt
 
 from cookieplone import data, settings
 from cookieplone.exceptions import GeneratorException
 from cookieplone.generator import generate
 from cookieplone.repository import get_base_repository, get_template_options
-from cookieplone.utils import console, internal
+from cookieplone.utils import console, files, internal
 
 
 def validate_extra_context(value: list[str] | None = None) -> list[str]:
     """Validate extra content follows the correct pattern."""
     if not value:
         return []
     for item in value:
@@ -112,38 +112,43 @@
     ] = None,
     verbose: Annotated[bool, typer.Option("--verbose", "-v")] = False,
 ):
     """Generate a new Plone codebase."""
     if version:
         console.base_print(internal.version_info())
         raise typer.Exit()
+
+    configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
     repository = os.environ.get(settings.REPO_LOCATION)
     if not repository:
         repository = "gh:plone/cookieplone-templates"
 
     repo_path = get_base_repository(repository)
     if not template:
         # Display template options
         template = prompt_for_template(repo_path)
     else:
         console.welcome_screen()
 
-    if replay_file:
-        replay = replay_file
     passwd = os.environ.get(
         settings.REPO_PASSWORD, os.environ.get("COOKIECUTTER_REPO_PASSWORD")
     )
     if not output_dir:
         output_dir = Path().cwd()
-    configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
-    # Annotate extra_context
-    extra_context = parse_extra_content(extra_context)
-    extra_context["__generator_signature"] = internal.signature_md(repo_path)
-    extra_context["__cookieplone_repository_path"] = f"{repo_path}"
-    extra_context["__cookieplone_template"] = f"{template}"
+
+    replay_file = files.resolve_path(replay_file) if replay_file else replay_file
+    if replay_file and replay_file.exists():
+        # Use replay_file
+        replay = replay_file
+    else:
+        # Annotate extra_context
+        extra_context = parse_extra_content(extra_context)
+        extra_context["__generator_signature"] = internal.signature_md(repo_path)
+        extra_context["__cookieplone_repository_path"] = f"{repo_path}"
+        extra_context["__cookieplone_template"] = f"{template}"
     # Run generator
     try:
         generate(
             repository,
             tag,
             no_input,
             extra_context,
@@ -153,18 +158,20 @@
             config_file,
             default_config,
             passwd,
             template,
             skip_if_file_exists,
             keep_project_on_failure,
         )
-    except GeneratorException:
+    except GeneratorException as exc:
+        console.error(exc.message)
         # TODO: Handle error
         raise typer.Exit(1)  # noQA:B904
-    except Exception:
+    except Exception as exc:
+        console.error(exc)
         # TODO: Handle error
         raise typer.Exit(1)  # noQA:B904
 
 
 def main():
     """Run the cli."""
     typer.run(cli)
```

### Comparing `cookieplone-0.5.6/cookieplone/data.py` & `cookieplone-0.5.7/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/exceptions.py` & `cookieplone-0.5.7/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/generator.py` & `cookieplone-0.5.7/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/repository.py` & `cookieplone-0.5.7/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/settings.py` & `cookieplone-0.5.7/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/filters/__init__.py` & `cookieplone-0.5.7/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/console.py` & `cookieplone-0.5.7/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/git.py` & `cookieplone-0.5.7/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/internal.py` & `cookieplone-0.5.7/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/sanity.py` & `cookieplone-0.5.7/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/validators.py` & `cookieplone-0.5.7/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/versions.py` & `cookieplone-0.5.7/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.7/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/test_cli.py` & `cookieplone-0.5.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/test_filters.py` & `cookieplone-0.5.7/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_commands.py` & `cookieplone-0.5.7/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_console.py` & `cookieplone-0.5.7/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_files.py` & `cookieplone-0.5.7/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_git.py` & `cookieplone-0.5.7/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_internal.py` & `cookieplone-0.5.7/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_sanity.py` & `cookieplone-0.5.7/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_validators.py` & `cookieplone-0.5.7/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/tests/utils/test_versions.py` & `cookieplone-0.5.7/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/.gitignore` & `cookieplone-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/LICENSE` & `cookieplone-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/README.md` & `cookieplone-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/pyproject.toml` & `cookieplone-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.6/PKG-INFO` & `cookieplone-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.6
+Version: 0.5.7
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

