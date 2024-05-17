# Comparing `tmp/dkdc-0.2.8.tar.gz` & `tmp/dkdc-0.4.0.tar.gz`

## Comparing `dkdc-0.2.8.tar` & `dkdc-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,17 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dkdc-0.2.8/config.toml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dkdc-0.2.8/dev-requirements.txt
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 dkdc-0.2.8/eda.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dkdc-0.2.8/justfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/__main__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/cli.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/dkdc.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/math.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/poker.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/resize.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/sql.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/systems.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/testing.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/tools.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/translate.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dkdc-0.2.8/dkdc/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 dkdc-0.2.8/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.2.8/LICENSE
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dkdc-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dkdc-0.2.8/readme.md
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 dkdc-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dkdc-0.4.0/dev-requirements.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dkdc-0.4.0/justfile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dkdc-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/ai.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/cli.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/config.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/defaults.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/image.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/open.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/utils/config.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dkdc-0.4.0/src/dkdc/utils/envvar.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dkdc-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.4.0/LICENSE
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dkdc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dkdc-0.4.0/readme.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 dkdc-0.4.0/PKG-INFO
```

### Comparing `dkdc-0.2.8/justfile` & `dkdc-0.4.0/justfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # Justfile
 
 # load environment variables
 set dotenv-load
 
 # aliases
-alias preview:=app
+alias fmt:=format
 
 # list justfile recipes
 default:
     just --list
 
 # setup
 setup:
-    @pip install -r dev-requirements.txt
+    @uv pip install -r dev-requirements.txt
 
 # build
 build:
     just clean
     @python -m build
 
+# format
+format:
+    @ruff format . || True
+
 # install
 install:
-    @pip install -e '.[all]'
+    @uv pip install -e '.[all]' --reinstall-package dkdc
 
 # uninstall
 uninstall:
-    @pip uninstall dkdc -y
+    @uv pip uninstall dkdc -y
 
 # publish-test
 release-test:
     just build
-    @twine upload --repository testpypi dist/* -u __token__ -p ${PYPI_TEST_KEY}
+    @twine upload --repository testpypi dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
 
 # publish
 release:
     just build
-    @twine upload dist/* -u __token__ -p ${PYPI_KEY}
-
-# streamlit stuff
-app:
-    @streamlit run app.py
+    @twine upload dist/* -u __token__ -p ${PYPI_TOKEN}
 
 # smoke-test
 smoke-test:
-    black --check .
+    ruff format --check .
 
 # clean
 clean:
-    @rm -rf dist || True
-
+    @rm -r dist || True
+
```

### Comparing `dkdc-0.2.8/LICENSE` & `dkdc-0.4.0/LICENSE`

 * *Files identical despite different names*

