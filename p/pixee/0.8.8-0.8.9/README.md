# Comparing `tmp/pixee-0.8.8.tar.gz` & `tmp/pixee-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixee-0.8.8.tar", last modified: Fri May 17 01:19:33 2024, max compression
+gzip compressed data, was "pixee-0.8.9.tar", last modified: Fri May 17 01:21:14 2024, max compression
```

## Comparing `pixee-0.8.8.tar` & `pixee-0.8.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.877521 pixee-0.8.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.853520 pixee-0.8.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.857520 pixee-0.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 01:19:17.000000 pixee-0.8.8/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 01:19:17.000000 pixee-0.8.8/.github/workflows/docker_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 01:19:17.000000 pixee-0.8.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 01:19:17.000000 pixee-0.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 01:19:17.000000 pixee-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 01:19:17.000000 pixee-0.8.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 01:19:17.000000 pixee-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 01:19:17.000000 pixee-0.8.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:19:33.873520 pixee-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 01:19:17.000000 pixee-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.857520 pixee-0.8.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.853520 pixee-0.8.8/ci/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.857520 pixee-0.8.8/ci/assets/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/access_token_var.png
--rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/access_token_view.png
--rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/access_tokens.png
--rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/scopes.png
--rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/assets/bitbucket/variables.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.861521 pixee-0.8.8/ci/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/bitbucket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/changed_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/bitbucket/pipe.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.861521 pixee-0.8.8/ci/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/examples/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/examples/bitbucket-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.861521 pixee-0.8.8/ci/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/gitlab/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/gitlab/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/gitlab/ci.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/gitlab/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:19:17.000000 pixee-0.8.8/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.861521 pixee-0.8.8/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 01:19:17.000000 pixee-0.8.8/docker/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.861521 pixee-0.8.8/docker/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-17 01:19:17.000000 pixee-0.8.8/docker/bin/pixee-java-codemods
--rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-17 01:19:17.000000 pixee-0.8.8/docker/bin/pixee-python-codemods
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.873520 pixee-0.8.8/img/
--rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-05-17 01:19:17.000000 pixee-0.8.8/img/dark_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-05-17 01:19:18.000000 pixee-0.8.8/img/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-05-17 01:19:18.000000 pixee-0.8.8/img/light_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-05-17 01:19:18.000000 pixee-0.8.8/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 01:19:18.000000 pixee-0.8.8/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 01:19:18.000000 pixee-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:19:18.000000 pixee-0.8.8/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:19:33.877521 pixee-0.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.853520 pixee-0.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.873520 pixee-0.8.8/src/pixee/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-17 01:19:18.000000 pixee-0.8.8/src/pixee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 01:19:18.000000 pixee-0.8.8/src/pixee/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:19:33.873520 pixee-0.8.8/src/pixee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 01:19:33.000000 pixee-0.8.8/src/pixee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.239918 pixee-0.8.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.211918 pixee-0.8.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.215918 pixee-0.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 01:20:52.000000 pixee-0.8.9/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 01:20:52.000000 pixee-0.8.9/.github/workflows/docker_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 01:20:52.000000 pixee-0.8.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 01:20:52.000000 pixee-0.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 01:20:52.000000 pixee-0.8.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 01:20:52.000000 pixee-0.8.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 01:20:52.000000 pixee-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 01:20:52.000000 pixee-0.8.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:21:14.235918 pixee-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 01:20:52.000000 pixee-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.215918 pixee-0.8.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.215918 pixee-0.8.9/ci/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.219918 pixee-0.8.9/ci/assets/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/access_token_var.png
+-rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/access_token_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/access_tokens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/scopes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/assets/bitbucket/variables.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.219918 pixee-0.8.9/ci/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/bitbucket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/changed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/bitbucket/pipe.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.219918 pixee-0.8.9/ci/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/examples/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/examples/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.223918 pixee-0.8.9/ci/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/gitlab/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/gitlab/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/gitlab/ci.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/gitlab/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:20:52.000000 pixee-0.8.9/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.223918 pixee-0.8.9/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 01:20:52.000000 pixee-0.8.9/docker/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.223918 pixee-0.8.9/docker/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-17 01:20:52.000000 pixee-0.8.9/docker/bin/pixee-java-codemods
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-17 01:20:52.000000 pixee-0.8.9/docker/bin/pixee-python-codemods
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.235918 pixee-0.8.9/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-05-17 01:20:52.000000 pixee-0.8.9/img/dark_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-05-17 01:20:52.000000 pixee-0.8.9/img/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-05-17 01:20:52.000000 pixee-0.8.9/img/light_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-05-17 01:20:52.000000 pixee-0.8.9/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 01:20:52.000000 pixee-0.8.9/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 01:20:52.000000 pixee-0.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:20:52.000000 pixee-0.8.9/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:21:14.239918 pixee-0.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.215918 pixee-0.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.235918 pixee-0.8.9/src/pixee/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-17 01:20:52.000000 pixee-0.8.9/src/pixee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 01:20:52.000000 pixee-0.8.9/src/pixee/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:14.235918 pixee-0.8.9/src/pixee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42802 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 01:21:14.000000 pixee-0.8.9/src/pixee.egg-info/top_level.txt
```

### Comparing `pixee-0.8.8/.github/workflows/deploy_to_pypi.yml` & `pixee-0.8.9/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/.github/workflows/docker_test.yaml` & `pixee-0.8.9/.github/workflows/docker_test.yaml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/.github/workflows/lint.yml` & `pixee-0.8.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/.pre-commit-config.yaml` & `pixee-0.8.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/CONTRIBUTING.md` & `pixee-0.8.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/LICENSE` & `pixee-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/PKG-INFO` & `pixee-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.8
+Version: 0.8.9
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.8/README.md` & `pixee-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/access_token_var.png` & `pixee-0.8.9/ci/assets/bitbucket/access_token_var.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/access_token_view.png` & `pixee-0.8.9/ci/assets/bitbucket/access_token_view.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/access_tokens.png` & `pixee-0.8.9/ci/assets/bitbucket/access_tokens.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/scopes.png` & `pixee-0.8.9/ci/assets/bitbucket/scopes.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/settings.png` & `pixee-0.8.9/ci/assets/bitbucket/settings.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/assets/bitbucket/variables.png` & `pixee-0.8.9/ci/assets/bitbucket/variables.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/bitbucket/README.md` & `pixee-0.8.9/ci/bitbucket/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/bitbucket/bitbucket_client.py` & `pixee-0.8.9/ci/bitbucket/bitbucket_client.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/bitbucket/changed_files.py` & `pixee-0.8.9/ci/bitbucket/changed_files.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/bitbucket/main.py` & `pixee-0.8.9/ci/bitbucket/main.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/bitbucket/pipe.sh` & `pixee-0.8.9/ci/bitbucket/pipe.sh`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/examples/bitbucket-pipelines.yml` & `pixee-0.8.9/ci/examples/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/ci/gitlab/pipeline.py` & `pixee-0.8.9/ci/gitlab/pipeline.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/docker/Dockerfile` & `pixee-0.8.9/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/img/dark_mode_logo.png` & `pixee-0.8.9/img/dark_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/img/demo.gif` & `pixee-0.8.9/img/demo.gif`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/img/light_mode_logo.png` & `pixee-0.8.9/img/light_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/img/logo.png` & `pixee-0.8.9/img/logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/pylintrc` & `pixee-0.8.9/pylintrc`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/pyproject.toml` & `pixee-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/src/pixee/cli.py` & `pixee-0.8.9/src/pixee/cli.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/src/pixee/logo.py` & `pixee-0.8.9/src/pixee/logo.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.8/src/pixee.egg-info/PKG-INFO` & `pixee-0.8.9/src/pixee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.8
+Version: 0.8.9
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.8/src/pixee.egg-info/SOURCES.txt` & `pixee-0.8.9/src/pixee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

