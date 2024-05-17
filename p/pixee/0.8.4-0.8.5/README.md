# Comparing `tmp/pixee-0.8.4.tar.gz` & `tmp/pixee-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixee-0.8.4.tar", last modified: Fri Apr 19 01:30:56 2024, max compression
+gzip compressed data, was "pixee-0.8.5.tar", last modified: Fri May 17 01:07:38 2024, max compression
```

## Comparing `pixee-0.8.4.tar` & `pixee-0.8.5.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.786815 pixee-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.762814 pixee-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.766814 pixee-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 01:30:41.000000 pixee-0.8.4/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-19 01:30:41.000000 pixee-0.8.4/.github/workflows/docker_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 01:30:41.000000 pixee-0.8.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 01:30:41.000000 pixee-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 01:30:41.000000 pixee-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 01:30:41.000000 pixee-0.8.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 01:30:41.000000 pixee-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 01:30:41.000000 pixee-0.8.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-04-19 01:30:56.786815 pixee-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 01:30:41.000000 pixee-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.766814 pixee-0.8.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.766814 pixee-0.8.4/ci/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/ci/assets/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/access_token_var.png
--rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/access_token_view.png
--rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/access_tokens.png
--rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/scopes.png
--rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/assets/bitbucket/variables.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/ci/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/bitbucket-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/bitbucket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/bitbucket/pipe.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/ci/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/examples/.gitlab-ci.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/ci/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/gitlab/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/gitlab/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 01:30:41.000000 pixee-0.8.4/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 01:30:41.000000 pixee-0.8.4/docker/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.770814 pixee-0.8.4/docker/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-19 01:30:41.000000 pixee-0.8.4/docker/bin/pixee-java-codemods
--rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-04-19 01:30:41.000000 pixee-0.8.4/docker/bin/pixee-python-codemods
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.782814 pixee-0.8.4/img/
--rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-04-19 01:30:41.000000 pixee-0.8.4/img/dark_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-04-19 01:30:41.000000 pixee-0.8.4/img/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-04-19 01:30:41.000000 pixee-0.8.4/img/light_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-04-19 01:30:41.000000 pixee-0.8.4/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 01:30:41.000000 pixee-0.8.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-19 01:30:41.000000 pixee-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 01:30:41.000000 pixee-0.8.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:30:56.786815 pixee-0.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.766814 pixee-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.782814 pixee-0.8.4/src/pixee/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-19 01:30:41.000000 pixee-0.8.4/src/pixee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-19 01:30:41.000000 pixee-0.8.4/src/pixee/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:30:56.786815 pixee-0.8.4/src/pixee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 01:30:56.000000 pixee-0.8.4/src/pixee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.409490 pixee-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.385490 pixee-0.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.389490 pixee-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 01:06:56.000000 pixee-0.8.5/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 01:06:56.000000 pixee-0.8.5/.github/workflows/docker_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 01:06:56.000000 pixee-0.8.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 01:06:56.000000 pixee-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 01:06:56.000000 pixee-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 01:06:56.000000 pixee-0.8.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 01:06:56.000000 pixee-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 01:06:56.000000 pixee-0.8.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-05-17 01:07:38.409490 pixee-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 01:06:56.000000 pixee-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.389490 pixee-0.8.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.389490 pixee-0.8.5/ci/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.393490 pixee-0.8.5/ci/assets/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/access_token_var.png
+-rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/access_token_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/access_tokens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/scopes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/assets/bitbucket/variables.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.393490 pixee-0.8.5/ci/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/bitbucket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/changed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/bitbucket/pipe.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.393490 pixee-0.8.5/ci/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/examples/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/examples/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.397490 pixee-0.8.5/ci/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/gitlab/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/gitlab/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/gitlab/ci.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/gitlab/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:06:56.000000 pixee-0.8.5/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.397490 pixee-0.8.5/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 01:06:56.000000 pixee-0.8.5/docker/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.397490 pixee-0.8.5/docker/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-05-17 01:06:56.000000 pixee-0.8.5/docker/bin/pixee-java-codemods
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-05-17 01:06:56.000000 pixee-0.8.5/docker/bin/pixee-python-codemods
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.405490 pixee-0.8.5/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-05-17 01:06:56.000000 pixee-0.8.5/img/dark_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-05-17 01:06:56.000000 pixee-0.8.5/img/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-05-17 01:06:56.000000 pixee-0.8.5/img/light_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-05-17 01:06:56.000000 pixee-0.8.5/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 01:06:56.000000 pixee-0.8.5/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 01:06:56.000000 pixee-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:06:56.000000 pixee-0.8.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:07:38.409490 pixee-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.389490 pixee-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.409490 pixee-0.8.5/src/pixee/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-17 01:06:56.000000 pixee-0.8.5/src/pixee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 01:06:56.000000 pixee-0.8.5/src/pixee/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:07:38.409490 pixee-0.8.5/src/pixee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 01:07:38.000000 pixee-0.8.5/src/pixee.egg-info/top_level.txt
```

### Comparing `pixee-0.8.4/.github/workflows/deploy_to_pypi.yml` & `pixee-0.8.5/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/.github/workflows/docker_test.yaml` & `pixee-0.8.5/.github/workflows/docker_test.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: Manual Docker Build and Publish
 
 on:
   workflow_dispatch:  # This enables manual trigger from GitHub UI or API
+  push:
+    branches:
+      - main
 
 jobs:
   build_and_publish:
     runs-on: ubuntu-latest
     steps:
       - name: Check out the repo
         uses: actions/checkout@v4
@@ -44,8 +47,8 @@
           password: ${{ secrets.DOCKERHUB_TOKEN }}
       - name: Build and push Docker image
         uses: docker/build-push-action@v5
         with:
           context: "{{defaultContext}}:docker"
           file: ./Dockerfile
           push: true
-          tags: pixeematt/pixee-cli:latest, pixeematt/pixee-cli:${{ steps.bump-semver.outputs.new_version }}
+          tags: codemodder/pixee-cli:latest, codemodder/pixee-cli:${{ steps.bump-semver.outputs.new_version }}
```

### Comparing `pixee-0.8.4/.github/workflows/lint.yml` & `pixee-0.8.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/.pre-commit-config.yaml` & `pixee-0.8.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/CONTRIBUTING.md` & `pixee-0.8.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/LICENSE` & `pixee-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/PKG-INFO` & `pixee-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.4
+Version: 0.8.5
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.4/README.md` & `pixee-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/access_token_var.png` & `pixee-0.8.5/ci/assets/bitbucket/access_token_var.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/access_token_view.png` & `pixee-0.8.5/ci/assets/bitbucket/access_token_view.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/access_tokens.png` & `pixee-0.8.5/ci/assets/bitbucket/access_tokens.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/scopes.png` & `pixee-0.8.5/ci/assets/bitbucket/scopes.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/settings.png` & `pixee-0.8.5/ci/assets/bitbucket/settings.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/assets/bitbucket/variables.png` & `pixee-0.8.5/ci/assets/bitbucket/variables.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/bitbucket/README.md` & `pixee-0.8.5/ci/bitbucket/README.md`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/bitbucket/bitbucket-pipelines.yml` & `pixee-0.8.5/ci/examples/bitbucket-pipelines.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 image: atlassian/default-image:4
 
+
 pipelines:
   pull-requests:
     '**': # This will run for pull requests targeting any branch
       - step:
           name: "Pixee PR"
           script:
             - echo "Pixee PR run"
```

### Comparing `pixee-0.8.4/ci/bitbucket/bitbucket_client.py` & `pixee-0.8.5/ci/bitbucket/bitbucket_client.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/bitbucket/main.py` & `pixee-0.8.5/ci/bitbucket/main.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/ci/gitlab/pipeline.py` & `pixee-0.8.5/ci/gitlab/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 import json
 import whatthepatch
 import base64
 import secrets
 
 
 # GitLab settings
-gitlab_url = "https://gitlab.com"  # Replace with your GitLab URL
-api_token = os.environ.get("API_TOKEN")
-project_id = os.environ.get("CI_MERGE_REQUEST_PROJECT_ID")
-source_branch = os.environ.get("CI_MERGE_REQUEST_SOURCE_BRANCH_NAME")
+
+gitlab_url = os.environ.get("GITLAB_API_URL", "https://gitlab.com")
+
+api_token = os.environ.get("GITLAB_API_TOKEN_PIXEE")
+project_id = os.environ.get("CI_MERGE_REQUEST_PROJECT_ID") or os.environ.get(
+    "CI_PROJECT_ID"
+)
+source_branch = os.environ.get("CI_MERGE_REQUEST_SOURCE_BRANCH_NAME") or os.environ.get(
+    "CI_COMMIT_REF_NAME"
+)
 new_branch_name = "pixee_" + str(
     secrets.SystemRandom().randint(0, 1000)
 )  # Replace with the desired new branch name
 merge_id = os.environ.get("CI_MERGE_REQUEST_IID")
 
-source_title = os.environ.get("CI_MERGE_REQUEST_TITLE")
+source_title = os.environ.get("CI_MERGE_REQUEST_TITLE") or os.environ.get(
+    "CI_PROJECT_NAME"
+)
 
 
 def main():
-    for name, value in os.environ.items():
-        print("{0}: {1}".format(name, value))
-
     filename = str(sys.argv[1])
     # working_dir = os.path.dirname(os.path.abspath(filename))
 
     with open(filename, "r", encoding="utf-8") as file:
         data = json.load(file)
 
     # Initialize GitLab client
@@ -37,14 +42,16 @@
     project = gl.projects.get(project_id)
     branch = project.branches.create({"branch": new_branch_name, "ref": source_branch})
 
     print(f"Created a new branch: {branch.name}")
 
     description = ""
 
+    has_change = False
+
     for result in data["results"]:
         if len(result["changeset"]):
             print(result["summary"])
 
             description = (
                 description
                 + f"""
@@ -68,36 +75,38 @@
                     new_file = whatthepatch.apply_diff(
                         diff, original_file_content, use_patch=True
                     )
                     new_file = "\n".join(new_file[0])
 
                     file.content = new_file
                     file.save(branch=new_branch_name, commit_message=result["summary"])
-                    print(file)
+                    has_change = True
+
                 except Exception as e:
                     print("The error is: ", e)
-
-    new_mr = project.mergerequests.create(
-        {
-            "source_branch": new_branch_name,
-            "target_branch": source_branch,
-            "title": f"Hardening Suggestions for {source_title}",
-            "description": description,
-        }
-    )
-    print(f"Hardening Suggestions for {source_branch}")
-    print(new_mr.web_url)
-
-    merge_request = project.mergerequests.get(merge_id)
-
-    # Add a comment to the merge request
-    merge_request.notes.create(
-        {
-            "body": f"Pixee has created some suggestions in: [Hardening Suggestions for {source_branch}]({new_mr.web_url})"
-        }
-    )
-
-    # print(commit)
+    if has_change:
+        new_mr = project.mergerequests.create(
+            {
+                "source_branch": new_branch_name,
+                "target_branch": source_branch,
+                "title": f"Pixee Hardening Suggestions for {source_title}",
+                "description": description,
+            }
+        )
+        print(f"Hardening Suggestions for {source_branch}")
+        print(new_mr.web_url)
+
+        if merge_id:
+            merge_request = project.mergerequests.get(merge_id)
+
+            # Add a comment to the merge request
+            merge_request.notes.create(
+                {
+                    "body": f"Pixee has created some suggestions in: [Hardening Suggestions for {source_branch}]({new_mr.web_url})"
+                }
+            )
+    else:
+        print("No changes made.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pixee-0.8.4/img/dark_mode_logo.png` & `pixee-0.8.5/img/dark_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/img/demo.gif` & `pixee-0.8.5/img/demo.gif`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/img/light_mode_logo.png` & `pixee-0.8.5/img/light_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/img/logo.png` & `pixee-0.8.5/img/logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/pylintrc` & `pixee-0.8.5/pylintrc`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/pyproject.toml` & `pixee-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/src/pixee/cli.py` & `pixee-0.8.5/src/pixee/cli.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/src/pixee/logo.py` & `pixee-0.8.5/src/pixee/logo.py`

 * *Files identical despite different names*

### Comparing `pixee-0.8.4/src/pixee.egg-info/PKG-INFO` & `pixee-0.8.5/src/pixee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.8.4
+Version: 0.8.5
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pixee-0.8.4/src/pixee.egg-info/SOURCES.txt` & `pixee-0.8.5/src/pixee.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 ci/requirements.txt
 ci/assets/bitbucket/access_token_var.png
 ci/assets/bitbucket/access_token_view.png
 ci/assets/bitbucket/access_tokens.png
 ci/assets/bitbucket/scopes.png
 ci/assets/bitbucket/settings.png
 ci/assets/bitbucket/variables.png
+ci/bitbucket/.dockerignore
 ci/bitbucket/Dockerfile
 ci/bitbucket/README.md
-ci/bitbucket/bitbucket-pipelines.yml
 ci/bitbucket/bitbucket_client.py
+ci/bitbucket/changed_files.py
 ci/bitbucket/main.py
 ci/bitbucket/pipe.sh
 ci/examples/.gitlab-ci.yml
+ci/examples/bitbucket-pipelines.yml
+ci/gitlab/.dockerignore
 ci/gitlab/Dockerfile
+ci/gitlab/ci.sh
 ci/gitlab/pipeline.py
 docker/Dockerfile
 docker/bin/pixee-java-codemods
 docker/bin/pixee-python-codemods
 img/dark_mode_logo.png
 img/demo.gif
 img/light_mode_logo.png
```

