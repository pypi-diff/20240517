# Comparing `tmp/pixee-0.8.6.tar.gz` & `tmp/pixee-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixee-0.8.6.tar", last modified: Fri May 17 01:18:24 2024, max compression
+gzip compressed data, was "pixee-0.8.7.tar", last modified: Fri May 17 01:18:39 2024, max compression
```

## Comparing `pixee-0.8.6.tar` & `pixee-0.8.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.418028 pixee-0.8.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.394028 pixee-0.8.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.398028 pixee-0.8.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 01:17:52.000000 pixee-0.8.6/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 01:17:52.000000 pixee-0.8.6/.github/workflows/docker_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 01:17:52.000000 pixee-0.8.6/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 01:17:52.000000 pixee-0.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 01:17:52.000000 pixee-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 01:17:52.000000 pixee-0.8.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 01:17:52.000000 pixee-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 01:17:52.000000 pixee-0.8.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:18:24.418028 pixee-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 01:17:52.000000 pixee-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.398028 pixee-0.8.6/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.398028 pixee-0.8.6/ci/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/ci/assets/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/access_token_var.png
--rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/access_token_view.png
--rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/access_tokens.png
--rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/scopes.png
--rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/assets/bitbucket/variables.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/ci/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/bitbucket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/changed_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/bitbucket/pipe.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/ci/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/examples/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/examples/bitbucket-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/ci/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/gitlab/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/gitlab/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/gitlab/ci.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/gitlab/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:17:52.000000 pixee-0.8.6/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 01:17:52.000000 pixee-0.8.6/docker/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.402028 pixee-0.8.6/docker/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-17 01:17:52.000000 pixee-0.8.6/docker/bin/pixee-java-codemods
--rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-17 01:17:52.000000 pixee-0.8.6/docker/bin/pixee-python-codemods
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.414028 pixee-0.8.6/img/
--rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-05-17 01:17:52.000000 pixee-0.8.6/img/dark_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-05-17 01:17:52.000000 pixee-0.8.6/img/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-05-17 01:17:52.000000 pixee-0.8.6/img/light_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-05-17 01:17:52.000000 pixee-0.8.6/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 01:17:52.000000 pixee-0.8.6/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 01:17:52.000000 pixee-0.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:17:52.000000 pixee-0.8.6/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:18:24.418028 pixee-0.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.398028 pixee-0.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.414028 pixee-0.8.6/src/pixee/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-17 01:17:52.000000 pixee-0.8.6/src/pixee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 01:17:52.000000 pixee-0.8.6/src/pixee/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:24.418028 pixee-0.8.6/src/pixee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 01:18:24.000000 pixee-0.8.6/src/pixee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.380762 pixee-0.8.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.356762 pixee-0.8.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.360762 pixee-0.8.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 01:18:23.000000 pixee-0.8.7/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 01:18:23.000000 pixee-0.8.7/.github/workflows/docker_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 01:18:23.000000 pixee-0.8.7/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 01:18:23.000000 pixee-0.8.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 01:18:23.000000 pixee-0.8.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 01:18:23.000000 pixee-0.8.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 01:18:23.000000 pixee-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 01:18:23.000000 pixee-0.8.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:18:39.380762 pixee-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 01:18:23.000000 pixee-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.360762 pixee-0.8.7/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.356762 pixee-0.8.7/ci/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/ci/assets/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/access_token_var.png
+-rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/access_token_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/access_tokens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/scopes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/assets/bitbucket/variables.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/ci/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/bitbucket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/changed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/bitbucket/pipe.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/ci/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/examples/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/examples/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/ci/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/gitlab/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/gitlab/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/gitlab/ci.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/gitlab/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:18:23.000000 pixee-0.8.7/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 01:18:23.000000 pixee-0.8.7/docker/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.364762 pixee-0.8.7/docker/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-17 01:18:23.000000 pixee-0.8.7/docker/bin/pixee-java-codemods
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-17 01:18:23.000000 pixee-0.8.7/docker/bin/pixee-python-codemods
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.376762 pixee-0.8.7/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-05-17 01:18:23.000000 pixee-0.8.7/img/dark_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-05-17 01:18:23.000000 pixee-0.8.7/img/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-05-17 01:18:23.000000 pixee-0.8.7/img/light_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-05-17 01:18:23.000000 pixee-0.8.7/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 01:18:23.000000 pixee-0.8.7/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 01:18:23.000000 pixee-0.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:18:23.000000 pixee-0.8.7/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:18:39.380762 pixee-0.8.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.360762 pixee-0.8.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.376762 pixee-0.8.7/src/pixee/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-17 01:18:23.000000 pixee-0.8.7/src/pixee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 01:18:23.000000 pixee-0.8.7/src/pixee/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:18:39.380762 pixee-0.8.7/src/pixee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 01:18:39.000000 pixee-0.8.7/src/pixee.egg-info/top_level.txt
```

### Comparing `pixee-0.8.6/.github/workflows/deploy_to_pypi.yml` & `pixee-0.8.7/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/.github/workflows/docker_test.yaml` & `pixee-0.8.7/.github/workflows/docker_test.yaml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/.github/workflows/lint.yml` & `pixee-0.8.7/.github/workflows/lint.yml`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
         run: make lint
 
   pre-commit:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
```

### Comparing `pixee-0.8.6/.pre-commit-config.yaml` & `pixee-0.8.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/CONTRIBUTING.md` & `pixee-0.8.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/LICENSE` & `pixee-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/PKG-INFO` & `pixee-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.6
+Version: 0.8.7
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.6/README.md` & `pixee-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/access_token_var.png` & `pixee-0.8.7/ci/assets/bitbucket/access_token_var.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/access_token_view.png` & `pixee-0.8.7/ci/assets/bitbucket/access_token_view.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/access_tokens.png` & `pixee-0.8.7/ci/assets/bitbucket/access_tokens.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/scopes.png` & `pixee-0.8.7/ci/assets/bitbucket/scopes.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/settings.png` & `pixee-0.8.7/ci/assets/bitbucket/settings.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/assets/bitbucket/variables.png` & `pixee-0.8.7/ci/assets/bitbucket/variables.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/bitbucket/README.md` & `pixee-0.8.7/ci/bitbucket/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/bitbucket/bitbucket_client.py` & `pixee-0.8.7/ci/bitbucket/bitbucket_client.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/bitbucket/changed_files.py` & `pixee-0.8.7/ci/bitbucket/changed_files.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/bitbucket/main.py` & `pixee-0.8.7/ci/bitbucket/main.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/bitbucket/pipe.sh` & `pixee-0.8.7/ci/bitbucket/pipe.sh`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/examples/bitbucket-pipelines.yml` & `pixee-0.8.7/ci/examples/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/ci/gitlab/pipeline.py` & `pixee-0.8.7/ci/gitlab/pipeline.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/docker/Dockerfile` & `pixee-0.8.7/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/img/dark_mode_logo.png` & `pixee-0.8.7/img/dark_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/img/demo.gif` & `pixee-0.8.7/img/demo.gif`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/img/light_mode_logo.png` & `pixee-0.8.7/img/light_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/img/logo.png` & `pixee-0.8.7/img/logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/pylintrc` & `pixee-0.8.7/pylintrc`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/pyproject.toml` & `pixee-0.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/src/pixee/cli.py` & `pixee-0.8.7/src/pixee/cli.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/src/pixee/logo.py` & `pixee-0.8.7/src/pixee/logo.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.6/src/pixee.egg-info/PKG-INFO` & `pixee-0.8.7/src/pixee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.6
+Version: 0.8.7
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.6/src/pixee.egg-info/SOURCES.txt` & `pixee-0.8.7/src/pixee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

