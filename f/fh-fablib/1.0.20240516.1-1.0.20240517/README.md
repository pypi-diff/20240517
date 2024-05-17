# Comparing `tmp/fh_fablib-1.0.20240516.1.tar.gz` & `tmp/fh_fablib-1.0.20240517.tar.gz`

## Comparing `fh_fablib-1.0.20240516.1.tar` & `fh_fablib-1.0.20240517.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/.editorconfig
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21417 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/bumpversion.sh
--rw-r--r--   0        0        0    26871 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/biome.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/LICENSE
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/README.rst
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/pyproject.toml
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/.editorconfig
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21617 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/bumpversion.sh
+-rw-r--r--   0        0        0    27022 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/dotfiles/biome.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517/PKG-INFO
```

### Comparing `fh_fablib-1.0.20240516.1/.pre-commit-config.yaml` & `fh_fablib-1.0.20240517/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/CHANGELOG.rst` & `fh_fablib-1.0.20240517/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+
+1.0.20240517
+~~~~~~~~~~~~
+
+- Improved the ``*.pyc`` deletion stage by skipping potentially big folders
+  which should never contain those files.
+- Skipped freezing more Python packaging libraries.
+
+
 1.0.20240516.1
 ~~~~~~~~~~~~~~
 
 - Added the missing biome configuration.
 
 1.0.20240516
 ~~~~~~~~~~~~
```

### Comparing `fh_fablib-1.0.20240516.1/fh_fablib/__init__.py` & `fh_fablib-1.0.20240517/fh_fablib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa: F401
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20240516.1"
+__version__ = "1.0.20240517"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -413,16 +413,15 @@
 @task
 def freeze(ctx):
     """Freeze the virtualenv's state"""
     run_local(
         ctx,
         '(printf "# AUTOGENERATED, DO NOT EDIT\n\n";'
         "venv/bin/python -m pip freeze -l"
-        # Until Ubuntu gets its act together:
-        ' | grep -vE "(^pkg.resources)"'
+        ' | grep -vE "(^packaging==|^pkg.resources==|^setuptools==|^wheel==)"'
         ") > requirements.txt",
     )
 
 
 @task
 def update(ctx):
     """Update virtualenv and node_modules to match the lockfiles"""
@@ -851,15 +850,19 @@
 
     result = run(conn, "git status --porcelain").stdout.strip()
     if result:
         terminate("Terminating because of uncommitted changes on server")
 
     run(conn, f"git reset --hard origin/{config.branch}")
     run(conn, "git submodule update --init")
-    run(conn, 'find . -name "*.pyc" -delete')
+    skip = "".join(
+        f"-path {path} -prune -o "
+        for path in ["./venv", "./static", "./media", "./.git", "./node_modules"]
+    )
+    run(conn, f'find . {skip} -name "*.pyc" -print | xargs rm')
     _pip_up(conn)
     run(conn, "venv/bin/python -m pip install -r requirements.txt")
     run(conn, "venv/bin/python manage.py migrate")
     run(conn, "venv/bin/python manage.py check --deploy", warn=True)
 
 
 def _deploy_staticfiles(conn):
```

### Comparing `fh_fablib-1.0.20240516.1/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20240517/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20240517/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20240517/fh_fablib/dotfiles/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20240517/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/LICENSE` & `fh_fablib-1.0.20240517/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240516.1/README.rst` & `fh_fablib-1.0.20240517/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240516.1")
+       fl.require("1.0.20240517")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240516.1")
+    fl.require("1.0.20240517")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20240516.1/pyproject.toml` & `fh_fablib-1.0.20240517/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 [project.urls]
 Homepage = "https://github.com/feinheit/fh-fablib/"
 
 [tool.hatch.version]
 path = "fh_fablib/__init__.py"
 
 [tool.ruff]
+fix = true
+show-fixes = true
+target-version = "py39"
+
+[tool.ruff.lint]
 extend-select = [
   # pyflakes, pycodestyle
   "F", "E", "W",
   # mmcabe
   "C90",
   # isort
   "I",
@@ -68,25 +73,22 @@
   # Allow zip() without strict=
   "B905",
   # No line length errors
   "E501",
   # Fabric/invoke do not support keyword-only arguments unfortunately
   "FBT002",
 ]
-fix = true
-show-fixes = true
-target-version = "py39"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 lines-after-imports = 2
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*/migrat*/*" = [
   # Allow using PascalCase model names in migrations
   "N806",
   # Ignore the fact that migration files are invalid module names
   "N999",
 ]
```

### Comparing `fh_fablib-1.0.20240516.1/PKG-INFO` & `fh_fablib-1.0.20240517/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20240516.1
+Version: 1.0.20240517
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240516.1")
+       fl.require("1.0.20240517")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240516.1")
+    fl.require("1.0.20240517")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

