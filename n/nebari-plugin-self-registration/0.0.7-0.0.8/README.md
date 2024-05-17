# Comparing `tmp/nebari_plugin_self_registration-0.0.7.tar.gz` & `tmp/nebari_plugin_self_registration-0.0.8.tar.gz`

## Comparing `nebari_plugin_self_registration-0.0.7.tar` & `nebari_plugin_self_registration-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,56 @@
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.github/workflows/publish-docker-image.yaml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/.dockerignore
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/Dockerfile
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/requirements.txt
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/job.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/main.py
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/static/logo.png
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/static/styles.css
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/templates/index.html
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/docker/app/templates/success.html
--rw-r--r--   0        0        0   203481 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/account-confirm.png
--rw-r--r--   0        0        0   143215 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/account-register.png
--rw-r--r--   0        0        0    97043 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/nebari-splash.png
--rw-r--r--   0        0        0   215778 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/verify-email.png
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/images/welcome-nebari.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__about__.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/outputs.tf
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/variables.tf
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/versions.tf
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/__init__.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/README.md
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.github/workflows/publish-docker-image.yaml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0   203481 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/account-confirm.png
+-rw-r--r--   0        0        0   143215 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/account-register.png
+-rw-r--r--   0        0        0    97043 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/nebari-splash.png
+-rw-r--r--   0        0        0   215778 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/verify-email.png
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/welcome-nebari.png
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/.dockerignore
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/Dockerfile
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/Dockerfile.local
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/config.sample.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/requirements.txt
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/run.sh
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/job.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/main.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/theme.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/static/favicon.ico
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/static/logo.svg
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/base.html
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/index.html
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/styles.css
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/success.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__about__.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__init__.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/outputs.tf
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/variables.tf
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/versions.tf
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/README.md
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/PKG-INFO
```

### Comparing `nebari_plugin_self_registration-0.0.7/.github/workflows/publish-docker-image.yaml` & `nebari_plugin_self_registration-0.0.8/.github/workflows/publish-docker-image.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 name: Publish Docker Image
 
 on:
   push:
-    branches: ['main']
+    branches: ["main"]
     paths:
-      - docker/**
+      - self-registration/**
   pull_request:
     paths:
-      - docker/**
+      - self-registration/**
 
 env:
   REGISTRY: ghcr.io
   IMAGE_NAME: ${{ github.repository }}
 
 jobs:
   push:
@@ -22,22 +22,22 @@
     steps:
       - uses: actions/checkout@v3
       - name: Set lower case image name
         run: echo "IMAGE_LC=${IMAGE_NAME,,}" >>${GITHUB_ENV}
       - name: Set the timestamp for version
         run: echo "VERSION=$(date +'%Y%m%d-%H%M')" >> ${GITHUB_ENV}
       - name: Build image
-        run: docker build docker --file docker/Dockerfile --tag $IMAGE_LC --label "runnumber=${GITHUB_RUN_ID}"
+        run: docker build self-registration --file self-registration/Dockerfile --tag $IMAGE_LC --label "runnumber=${GITHUB_RUN_ID}"
       - name: Log in to registry
         run: echo "${{ secrets.GITHUB_TOKEN }}" | docker login $REGISTRY -u $ --password-stdin
       - name: Push image
         run: |
           IMAGE_ID=ghcr.io/$IMAGE_LC
           IMAGE_ID=$(echo $IMAGE_ID | tr '[A-Z]' '[a-z]')
 
           [[ "${{ github.ref }}" == "refs/tags/"* ]] && VERSION=$(echo $VERSION | sed -e 's/^v//')
 
           [ "$VERSION" == "main" ] && VERSION=latest
           echo IMAGE_ID=$IMAGE_ID
           echo VERSION=$VERSION
           docker tag $IMAGE_LC $IMAGE_ID:$VERSION
-          docker push $IMAGE_ID:$VERSION
+          docker push $IMAGE_ID:$VERSION
```

### Comparing `nebari_plugin_self_registration-0.0.7/.github/workflows/publish-pypi.yaml` & `nebari_plugin_self_registration-0.0.8/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/docker/app/job.py` & `nebari_plugin_self_registration-0.0.8/self-registration/app/job.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/docker/app/main.py` & `nebari_plugin_self_registration-0.0.8/self-registration/app/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,85 @@
-from datetime import datetime, timedelta
-from fastapi import FastAPI, Form, Request, APIRouter
-from fastapi.templating import Jinja2Templates
-from fastapi.staticfiles import StaticFiles
-import string
-import re
+import os
 import random
+import re
+import string
+from datetime import datetime, timedelta
+
 import yaml
+from fastapi import APIRouter, FastAPI, Form, Request
+from fastapi.staticfiles import StaticFiles
+from fastapi.templating import Jinja2Templates
 from keycloak import KeycloakAdmin, KeycloakConnectionError, KeycloakGetError
+from theme import DEFAULT_THEME
+
 
 class UserExistsException(Exception):
     pass
 
+
 # Manual context URL.  Must be prepended to all paths in app and templates.
 url_prefix = "/registration"
 
 app = FastAPI()
 
-app.mount(url_prefix+"/static", StaticFiles(directory="static"), name="static")
+app.mount(url_prefix + "/static", StaticFiles(directory="static"), name="static")
 templates = Jinja2Templates(directory="templates")
 
-file_path = "/mnt/config.yaml"
-with open(file_path, "r") as file:
-    config = yaml.safe_load(file)
+mount_path = "/mnt/config.yaml"
+app_path = "/app/config.yaml"
+if os.path.exists(mount_path):
+    with open(mount_path) as file:
+        config = yaml.safe_load(file)
+elif os.path.exists(app_path):
+    with open(app_path) as file:
+        config = yaml.safe_load(file)
+else:
+    config = {}
+
 
 def check_email_domain(email):
     approved_domains = config.get("approved_domains", [])
     for domain in approved_domains:
         # Replace wildcard with its regex equivalent
-        pattern = domain.replace('*', '.*')
+        pattern = domain.replace("*", ".*")
         if re.search(f"@{pattern}$", email):
             return True
     return False
 
+
 def create_keycloak_user(email, expiration_days=7):
     # Random password generator
     def generate_random_password(length=12):
         characters = string.ascii_letters + string.digits + string.punctuation
-        return ''.join(random.choice(characters) for i in range(length))
+        return "".join(random.choice(characters) for i in range(length))
 
     try:
         keycloak_admin = KeycloakAdmin(
             server_url=config["keycloak"]["server_url"],
             realm_name=config["keycloak"]["realm_name"],
             client_id=config["keycloak"]["client_id"],
             client_secret_key=config["keycloak"]["client_secret"],
             user_realm_name=config["keycloak"]["realm_name"],
             verify=True,
         )
     except KeycloakConnectionError:
         return email, False, None
 
-
     # Check if the user already exists
     user_id = keycloak_admin.get_user_id(email)
     if user_id:
-        raise UserExistsException("A user with this email address already exists. Contact the administrator if you need to recover your account.")
+        raise UserExistsException(
+            "A user with this email address already exists. Contact the administrator if you need to recover your account."
+        )
 
     # Calculate account expiration as Unix timestamp
     expiration_date = datetime.utcnow() + timedelta(days=expiration_days)
 
     # Format expiration timestamp as a human-readable string
-    date_format="%Y-%m-%d %H:%M:%S"
+    date_format = "%Y-%m-%d %H:%M:%S"
     formatted_expiration_date = expiration_date.strftime(date_format)
 
     # Create a new user
     user_data = {
         "username": email,
         "email": email,
         "enabled": True,
@@ -75,14 +90,15 @@
     user_id = keycloak_admin.create_user(user_data)
 
     # Set a random temporary password
     temporary_password = generate_random_password()
     keycloak_admin.set_user_password(user_id, temporary_password, temporary=True)
     return keycloak_admin.get_user(user_id), temporary_password, expiration_date
 
+
 # Function to assign a user to a group
 def assign_user_to_group(user, group_name):
     try:
         keycloak_admin = KeycloakAdmin(
             server_url=config["keycloak"]["server_url"],
             realm_name=config["keycloak"]["realm_name"],
             client_id=config["keycloak"]["client_id"],
@@ -93,46 +109,105 @@
     except KeycloakConnectionError:
         return False
 
     # Get group
     try:
         group = keycloak_admin.get_group_by_path(group_name)
     except KeycloakGetError:
-        return False # Fail if Keycloak group throws exception finding group
+        return False  # Fail if Keycloak group throws exception finding group
     if not group:
         return False  # Also fail if Keycloak admin doesn't throw exception but group is still missing
 
     # Assign the user to the group
     keycloak_admin.group_user_add(user["id"], group["id"])
-    
+
     return True
 
+
+def get_theme():
+    theme = config.get("theme", {})
+    if theme:
+        return {**DEFAULT_THEME, **theme}
+    else:
+        return DEFAULT_THEME
+
+
+def get_template_context(request: Request, error_message: str = None):
+    if (error_message is None) or (error_message == ""):
+        return {
+            "url_prefix": url_prefix,
+            "request": request,
+            "registration_message": config.get("registration_message", None),
+            **get_theme(),
+        }
+    else:
+        return {
+            "url_prefix": url_prefix,
+            "request": request,
+            "registration_message": config.get("registration_message", None),
+            "error_message": error_message,
+            **get_theme(),
+        }
+
+
 @app.get(url_prefix)
 def read_root(request: Request):
-    return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request})
+    return templates.TemplateResponse("index.html", get_template_context(request))
+
 
 @app.post(url_prefix + "/validate/")
 async def validate_submission(request: Request, email: str = Form(...), coupon_code: str = Form(...)):
     if coupon_code in config.get("coupons", []):
         if check_email_domain(email):
-            
+
             # Create the user in Keycloak
             try:
-                user, temporary_password, expiration_date = create_keycloak_user(email, config.get("account_expiration_days", None))
+                user, temporary_password, expiration_date = create_keycloak_user(
+                    email, config.get("account_expiration_days", None)
+                )
             except UserExistsException as e:
-                return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request, "error_message": str(e)})
-            
+                return templates.TemplateResponse("index.html", get_template_context(request, str(e)))
+
             # Assign user to group
             if user:
                 success = assign_user_to_group(user, config.get("registration_group", None))
 
                 if success:
-                    return templates.TemplateResponse("success.html", {"url_prefix": url_prefix, "request": request, "email": email, "temporary_password": temporary_password, "user_id": user["id"], "expiration_date": expiration_date.strftime("%m-%d-%Y")})
+                    return templates.TemplateResponse(
+                        "success.html",
+                        {
+                            "url_prefix": url_prefix,
+                            "request": request,
+                            "email": email,
+                            "temporary_password": temporary_password,
+                            "user_id": user["id"],
+                            "expiration_date": expiration_date.strftime("%m-%d-%Y"),
+                            **get_theme(),
+                        },
+                    )
                 else:
-                    return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request, "error_message": "Your user was registered but could not be granted access to JupyterLab environments.  Please contact support for assistance."})
+                    return templates.TemplateResponse(
+                        "index.html",
+                        get_template_context(
+                            request,
+                            "User created but could not be assigned to JupyterLab group.  Please contact support for assistance.",
+                        ),
+                    )
             else:
-                return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request, "error_message": "Unable to create user.  Please try again later."})
+                return templates.TemplateResponse(
+                    "index.html",
+                    get_template_context(request, "Unable to create user.  Please try again later."),
+                )
 
         else:
-            return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request, "error_message": "Access to the platform is limited to accounts created with pre-approved email domains. The email address you provided when registering your account uses a domain that's not currently approved. Please contact the system administrator to request access."})
+            return templates.TemplateResponse(
+                "index.html",
+                get_template_context(
+                    request,
+                    "Access to the platform is limited to accounts created with pre-approved email domains. The email address you provided when registering your account uses a domain that's not currently approved. Please contact the system administrator to request access.",
+                ),
+            )
     else:
-        return templates.TemplateResponse("index.html", {"url_prefix": url_prefix, "request": request, "error_message": "Invalid coupon code. Please try again."})
+        return templates.TemplateResponse(
+            "index.html",
+            get_template_context(request, "Invalid coupon code. Please try again."),
+        )
```

### Comparing `nebari_plugin_self_registration-0.0.7/docker/app/templates/success.html` & `nebari_plugin_self_registration-0.0.8/self-registration/app/templates/success.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,56 @@
-<!DOCTYPE html>
-<html>
-  <head>
-    <title>Self Registration</title>
-    <script src="https://cdn.tailwindcss.com"></script>
-    <link href="{{ url_prefix }}/static/styles.css" rel="stylesheet" />
-    <link
-      rel="stylesheet"
-      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
-      integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
-      crossorigin="anonymous"
-      referrerpolicy="no-referrer"
-    />
-    <script>
-      function handleCopy() {
-        // Copy to clipboard only works in secure context
-        if (window.isSecureContext) {
-          var copyText = document.getElementById("newPassword").textContent;
-          navigator.clipboard.writeText(copyText);
+{% extends "base.html" %} {% block head %}
+<link
+  rel="stylesheet"
+  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
+  integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
+  crossorigin="anonymous"
+  referrerpolicy="no-referrer"
+/>
+<script>
+  function handleCopy() {
+    // Copy to clipboard only works in secure context
+    if (window.isSecureContext) {
+      var copyText = document.getElementById("newPassword").textContent;
+      navigator.clipboard.writeText(copyText);
 
-          var copyMessage = document.getElementById("copyMessage");
-          copyMessage.style.visibility = "visible";
-        }
-      }
-    </script>
-  </head>
-  <body>
-    <header class="flex content-center">
-      <img src="{{ url_prefix }}/static/logo.png" alt="logo" />
-    </header>
-    <div class="container flex justify-start">
-      <div class="confirmation">
-        <h1 class="mb-8">Account Confirmation</h1>
-        <div class="mb-6">
-          Congratulations! Your account has been successfully created! Your
-          account will expire automatically on
-          <span class="font-bold">{{ expiration_date }}</span>.
-        </div>
-        <div class="mb-6">
-          Your temporary password for
-          <span class="font-bold">{{ email }}</span> is:
-        </div>
-        <div class="password-box flex justify-between">
-          <span id="newPassword" class="password-content flex justify-start"
-            >{{ temporary_password }}</span
-          >
-          <button
-            id="copyButton"
-            class="copy-btn flex justify-end"
-            onclick="handleCopy()"
-          >
-            <i class="fa-regular fa-clipboard"></i>
-          </button>
-        </div>
-        <div id="copyMessage" class="text-sm mb-6" style="visibility: hidden">
-          Password copied successfully!
-        </div>
-        <div class="mb-8">
-          Please copy the password and log in, after which you will be asked to
-          set a new password. Please note, this temporary password cannot be
-          recovered.
-        </div>
-        <div class="w-[180px]">
-          <a href="/" class="btn btn-primary">Login</a>
-        </div>
-      </div>
-    </div>
-  </body>
-</html>
+      var copyMessage = document.getElementById("copyMessage");
+      copyMessage.style.visibility = "visible";
+    }
+  }
+</script>
+{% endblock %} {% block content %}
+<div class="confirmation">
+  <h1 class="mb-8">Account Confirmation</h1>
+  <div class="mb-6">
+    Congratulations! Your account has been successfully created! Your account
+    will expire automatically on
+    <span class="font-bold">{{ expiration_date }}</span>.
+  </div>
+  <div class="mb-6">
+    Your temporary password for
+    <span class="font-bold">{{ email }}</span> is:
+  </div>
+  <div class="password-box flex justify-between">
+    <span id="newPassword" class="password-content flex justify-start"
+      >{{ temporary_password }}</span
+    >
+    <button
+      id="copyButton"
+      class="copy-btn flex justify-end"
+      onclick="handleCopy()"
+    >
+      <i class="fa-regular fa-clipboard"></i>
+    </button>
+  </div>
+  <div id="copyMessage" class="text-sm mb-6" style="visibility: hidden">
+    Password copied successfully!
+  </div>
+  <div class="mb-8">
+    Please copy the password and log in, after which you will be asked to set a
+    new password. Please note, this temporary password cannot be recovered.
+  </div>
+  <div class="w-[180px]">
+    <a href="/" class="btn btn-primary">Login</a>
+  </div>
+</div>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-[logo]
+{% extends "base.html" %} {% block head %}
+{% endblock %} {% block content %}
 ************ AAccccoouunntt CCoonnffiirrmmaattiioonn ************
 Congratulations! Your account has been successfully created! Your account will
 expire automatically on {{ expiration_date }}.
 Your temporary password for {{ email }} is:
 {{ temporary_password }}
 Password copied successfully!
 Please copy the password and log in, after which you will be asked to set a new
 password. Please note, this temporary password cannot be recovered.
 _L_o_g_i_n
+{% endblock %}
```

### Comparing `nebari_plugin_self_registration-0.0.7/images/account-confirm.png` & `nebari_plugin_self_registration-0.0.8/images/account-confirm.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/images/account-register.png` & `nebari_plugin_self_registration-0.0.8/images/account-register.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/images/nebari-splash.png` & `nebari_plugin_self_registration-0.0.8/images/nebari-splash.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/images/verify-email.png` & `nebari_plugin_self_registration-0.0.8/images/verify-email.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/images/welcome-nebari.png` & `nebari_plugin_self_registration-0.0.8/images/welcome-nebari.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/__init__.py` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import inspect
 import sys
 import time
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Union
 
-from nebari.schema import Base
 from _nebari.stages.base import NebariTerraformStage
+from _nebari.stages.tf_objects import NebariKubernetesProvider, NebariTerraformState
 from nebari.hookspecs import NebariStage, hookimpl
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
-from _nebari.stages.tf_objects import (
-    NebariKubernetesProvider,
-    NebariTerraformState,
-)
+from nebari.schema import Base
 
 NUM_ATTEMPTS = 10
 TIMEOUT = 10
 
 CLIENT_NAME = "self-registration"
 
+
 class SelfRegistrationAffinitySelectorConfig(Base):
     default: str
     app: Optional[str] = ""
     job: Optional[str] = ""
 
-class SelfRegistrationConfig(Base):
+
+class SelfRegistrationAffinityConfig(Base):
     enabled: Optional[bool] = True
     selector: Union[SelfRegistrationAffinitySelectorConfig, str] = "general"
 
+
 class SelfRegistrationConfig(Base):
     name: Optional[str] = "self-registration"
     namespace: Optional[str] = None
     values: Optional[Dict[str, Any]] = {}
     account_expiration_days: Optional[int] = 7
     approved_domains: Optional[List[str]] = []
     coupons: Optional[List[str]] = []
-    registration_group: Optional[str] = ""    
-    affinity: SelfRegistrationConfig = SelfRegistrationConfig()
+    registration_group: Optional[str] = ""
+    registration_message: Optional[str] = ""
+    affinity: SelfRegistrationAffinityConfig = SelfRegistrationAffinityConfig()
 
 
 class InputSchema(Base):
     self_registration: SelfRegistrationConfig = SelfRegistrationConfig()
 
+
 class SelfRegistrationStage(NebariTerraformStage):
     name = "self-registration"
     priority = 103
-    wait = True # wait for install to complete on nebari deploy
+    wait = True  # wait for install to complete on nebari deploy
     input_schema = InputSchema
 
     def tf_objects(self) -> List[Dict]:
         return [
             NebariTerraformState(self.name, self.config),
             NebariKubernetesProvider(self.config),
         ]
 
-
-
     @property
     def template_directory(self):
         return Path(inspect.getfile(self.__class__)).parent / "terraform"
-    
+
     def _attempt_keycloak_connection(
         self,
         keycloak_url,
         username,
         password,
         master_realm_name,
         client_id,
@@ -80,67 +80,63 @@
                     username=username,
                     password=password,
                     user_realm_name=master_realm_name,
                     realm_name=client_realm_name,
                     client_id=client_id,
                     verify=verify,
                 )
-                c = realm_admin.get_client_id(CLIENT_NAME) # lookup client guid
-                existing_client = realm_admin.get_client(c) # query client info
+                c = realm_admin.get_client_id(CLIENT_NAME)  # lookup client guid
+                existing_client = realm_admin.get_client(c)  # query client info
                 if existing_client != None and existing_client["name"] == CLIENT_NAME:
-                    print(
-                        f"Attempt {i+1} succeeded connecting to keycloak and nebari client={CLIENT_NAME} exists"
-                    )
+                    print(f"Attempt {i+1} succeeded connecting to keycloak and nebari client={CLIENT_NAME} exists")
                     return True
                 else:
                     print(
                         f"Attempt {i+1} succeeded connecting to keycloak but nebari client={CLIENT_NAME} did not exist"
                     )
             except KeycloakError as e:
                 print(f"Attempt {i+1} failed connecting to keycloak {client_realm_name} realm -- {e}")
             time.sleep(timeout)
         return False
-    
+
     def check(self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt=False) -> bool:
-                
+
         try:
             _ = self.config.escaped_project_name
             _ = self.config.provider
-            
+
         except KeyError:
-            print(
-                "\nBase config values not found: escaped_project_name, provider"
-            )
+            print("\nBase config values not found: escaped_project_name, provider")
             return False
 
         keycloak_config = self.get_keycloak_config(stage_outputs)
 
         if not self._attempt_keycloak_connection(
-            keycloak_url = keycloak_config["keycloak_url"],
-            username = keycloak_config["username"],
-            password = keycloak_config["password"],
-            master_realm_name = keycloak_config["master_realm_id"],
-            client_id = keycloak_config["master_client_id"],
-            client_realm_name = keycloak_config["realm_id"],
+            keycloak_url=keycloak_config["keycloak_url"],
+            username=keycloak_config["username"],
+            password=keycloak_config["password"],
+            master_realm_name=keycloak_config["master_realm_id"],
+            client_id=keycloak_config["master_client_id"],
+            client_realm_name=keycloak_config["realm_id"],
             verify=False,
         ):
             print(
                 f"ERROR: unable to connect to keycloak master realm and ensure that nebari client={CLIENT_NAME} exists"
             )
             sys.exit(1)
 
         print(f"Keycloak successfully configured with {CLIENT_NAME} client")
         return True
 
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         keycloak_config = self.get_keycloak_config(stage_outputs)
-    
+
         try:
             domain = stage_outputs["stages/04-kubernetes-ingress"]["domain"]
-            
+
         except KeyError:
             raise Exception("Prerequisite stage output(s) not found: stages/04-kubernetes-ingress")
 
         chart_ns = self.config.self_registration.namespace
         create_ns = True
         if chart_ns == None or chart_ns == "" or chart_ns == self.config.namespace:
             chart_ns = self.config.namespace
@@ -148,41 +144,47 @@
 
         return {
             "chart_name": self.config.self_registration.name,
             "account_expiration_days": self.config.self_registration.account_expiration_days,
             "approved_domains": self.config.self_registration.approved_domains,
             "coupons": self.config.self_registration.coupons,
             "registration_group": self.config.self_registration.registration_group,
+            "registration_message": self.config.self_registration.registration_message,
             "project_name": self.config.escaped_project_name,
             "realm_id": keycloak_config["realm_id"],
             "client_id": CLIENT_NAME,
             "base_url": f"https://{keycloak_config['domain']}/self-registration",
             "external_url": keycloak_config["keycloak_url"],
             "create_namespace": create_ns,
             "namespace": chart_ns,
             "ingress_host": domain,
             "overrides": self.config.self_registration.values,
             "affinity": {
                 "enabled": self.config.self_registration.affinity.enabled,
-                "selector": self.config.self_registration.affinity.selector.__dict__
-                if isinstance(self.config.self_registration.affinity.selector, SelfRegistrationAffinitySelectorConfig)
-                else self.config.self_registration.affinity.selector,
+                "selector": (
+                    self.config.self_registration.affinity.selector.__dict__
+                    if isinstance(
+                        self.config.self_registration.affinity.selector, SelfRegistrationAffinitySelectorConfig
+                    )
+                    else self.config.self_registration.affinity.selector
+                ),
             },
-
+            "theme": self.config.theme.jupyterhub.dict(),
         }
 
     def get_keycloak_config(self, stage_outputs: Dict[str, Dict[str, Any]]):
         directory = "stages/05-kubernetes-keycloak"
 
         return {
             "domain": stage_outputs["stages/04-kubernetes-ingress"]["domain"],
             "keycloak_url": f"{stage_outputs[directory]['keycloak_credentials']['value']['url']}/auth/",
             "username": stage_outputs[directory]["keycloak_credentials"]["value"]["username"],
             "password": stage_outputs[directory]["keycloak_credentials"]["value"]["password"],
             "master_realm_id": stage_outputs[directory]["keycloak_credentials"]["value"]["realm"],
             "master_client_id": stage_outputs[directory]["keycloak_credentials"]["value"]["client_id"],
             "realm_id": stage_outputs["stages/06-kubernetes-keycloak-configuration"]["realm_id"]["value"],
         }
-    
+
+
 @hookimpl
 def nebari_stage() -> List[NebariStage]:
-    return [ SelfRegistrationStage ]
+    return [SelfRegistrationStage]
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/main.tf` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/main.tf`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
   account_expiration_days   = var.account_expiration_days
   chart_name                = var.chart_name
   coupons                   = var.coupons
   create_namespace          = var.create_namespace
   ingress_host              = var.ingress_host
   self_registration_sa_name = local.self_registration_sa_name
   registration_group        = var.registration_group
+  registration_message      = var.registration_message
   namespace                 = var.namespace
   keycloak_base_url         = var.external_url
   keycloak_config           = module.keycloak.config
   overrides                 = var.overrides
   realm_id                  = var.realm_id
   affinity                  = var.affinity
+  theme                     = var.theme
 }
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/variables.tf` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/variables.tf`

 * *Files 7% similar despite different names*

```diff
@@ -70,14 +70,20 @@
 
 variable "registration_group" {
   description = "Name of Keycloak group to add registering users"
   type        = string
   default     = ""
 }
 
+variable "registration_message" {
+  description = "Custom message to display to registering users"
+  type        = string
+  default     = ""
+}
+
 variable "affinity" {
   type = object({
     enabled  = optional(bool, true)
     selector = optional(any, "general")
   })
 
   default = {
@@ -85,8 +91,14 @@
     selector = "general"
   }
 
   validation {
     condition     = can(tostring(var.affinity.selector)) || (can(var.affinity.selector.default) && length(try(var.affinity.selector.default, "")) > 0)
     error_message = "\"affinity.selector\" argument must be a string or object { default, app, job }"
   }
-}
+}
+
+variable "theme" {
+  description = "Theme configured in theme.jupyterhub"
+  type        = map(any)
+  default     = {}
+}
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf`

 * *Files 7% similar despite different names*

```diff
@@ -75,20 +75,22 @@
         name = var.self_registration_sa_name
       }
       app_configuration = {
         coupons                 = var.coupons
         approved_domains        = var.approved_domains
         account_expiration_days = var.account_expiration_days
         registration_group      = var.registration_group
+        registration_message    = var.registration_message
         keycloak = {
           server_url    = var.keycloak_base_url
           realm_name    = var.realm_id
           client_id     = var.keycloak_config["client_id"]
           client_secret = var.keycloak_config["client_secret"]
         }
+        theme                   = var.theme
       }
       env = [
       ]
     }),
     yamlencode(var.overrides),
   ]
 }
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 }
 
 variable "registration_group" {
   description = "Name of Keycloak group to add registering users"
   type        = string
 }
 
+variable "registration_message" {
+  description = "Custom message to display to registering users"
+  type        = string
+  default     = ""
+}
+
 variable "self_registration_sa_name" {
   description = "Name of K8S service account for Self Registration app workloads"
   type        = string
 }
 
 variable "overrides" {
   type    = map(any)
@@ -73,7 +79,13 @@
   }
 
   validation {
     condition     = can(tostring(var.affinity.selector)) || (can(var.affinity.selector.default) && length(try(var.affinity.selector.default, "")) > 0)
     error_message = "\"affinity.selector\" argument must be a string or object { default, app, job }"
   }
 }
+
+variable "theme" {
+  description = "Theme configured in theme.jupyterhub"
+  type        = map(any)
+  default     = {}
+}
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # a dependency of application charts to inject those utilities and functions into the rendering
 # pipeline. Library charts do not define any templates and therefore cannot be deployed.
 type: application
 
 # This is the chart version. This version number should be incremented each time you make changes
 # to the chart and its templates, including the app version.
 # Versions are expected to follow Semantic Versioning (https://semver.org/)
-version: 0.0.15
+version: 0.0.16
 
 # This is the version number of the application being deployed. This version number should be
 # incremented each time you make changes to the application. Versions are not expected to
 # follow Semantic Versioning. They should reflect the version the application is using.
 # It is recommended to use it with quotes.
-appVersion: "0.0.6"
+appVersion: "0.0.8"
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Declare variables to be passed into your templates.
 
 replicaCount: 1
 image:
   repository: ghcr.io/metrostar/nebari-self-registration
   pullPolicy: IfNotPresent
   # Overrides the image tag whose default is the chart appVersion.
-  tag: "20240213-1718"
+  tag: "20240515-1204"
 
 imagePullSecrets: []
 nameOverride: ""
 fullnameOverride: ""
 
 serviceAccount:
   # Specifies whether a service account should be created
```

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/src/nebari_plugin_self_registration/tests/unit/test_plugin.py` & `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/.gitignore` & `nebari_plugin_self_registration-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/LICENSE` & `nebari_plugin_self_registration-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/README.md` & `nebari_plugin_self_registration-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # Nebari Plugin Self Registration
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-self-registration.svg)](https://pypi.org/project/nebari-plugin-self-registration)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-self-registration.svg)](https://pypi.org/project/nebari-plugin-self-registration)
 
------
+---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install nebari-plugin-self-registration
 ```
 
+## Running locally with Docker
+
+_Note_: running locally requires a `config.yaml` file to be present within the `self-registration` directory. Please create a copy of the `sample.config.yaml`, rename, and update as needed before proceeding:
+
+1. Navigate to the `self-registration` directory
+2. To build the docker image, run the following:
+
+```
+docker build . --file Dockerfile.local -t self-registration
+```
+
+3. To run the app, run the following:
+
+```
+docker run -p 8000:8000 --name self-registration self-registration
+```
+
+4. Navigate to http://0.0.0.0:8000/registration
+
 ## User Registration via this extension
+
 Steps for self registration:
 
 - Navigate to your Nebari domain.
 <p align="center">
   <img src="images/welcome-nebari.png" />
 </p>
 
@@ -30,15 +50,15 @@
   <img src="images/account-register.png" width="400"/>
 </p>
 
 - Enter your email address and coupon code.
 
 - After clicking "Submit" follow the instructions to login with your temporary password. By clicking the "Login" button, it will take you to a Welcome page where you can sign in with Keycloak.
 
-- After you have entered a new password, you will receive a verification email.  
+- After you have entered a new password, you will receive a verification email.
 
 <p align="center">
   <img src="images/account-confirm.png" />
 </p>
 
 - Once your email is verified and you login you will see the Nebari landing page.
```

### Comparing `nebari_plugin_self_registration-0.0.7/pyproject.toml` & `nebari_plugin_self_registration-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.7/PKG-INFO` & `nebari_plugin_self_registration-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nebari-plugin-self-registration
-Version: 0.0.7
+Version: 0.0.8
 Summary: MetroStar - Self-Registration Plugin for Nebari Platform
 Project-URL: Documentation, https://github.com/MetroStar/nebari-self-registration#readme
 Project-URL: Issues, https://github.com/MetroStar/nebari-self-registration/issues
 Project-URL: Source, https://github.com/MetroStar/nebari-self-registration
 Author-email: Ken Foster <kfoster@metrostar.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -20,28 +20,48 @@
 Description-Content-Type: text/markdown
 
 # Nebari Plugin Self Registration
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-self-registration.svg)](https://pypi.org/project/nebari-plugin-self-registration)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-self-registration.svg)](https://pypi.org/project/nebari-plugin-self-registration)
 
------
+---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install nebari-plugin-self-registration
 ```
 
+## Running locally with Docker
+
+_Note_: running locally requires a `config.yaml` file to be present within the `self-registration` directory. Please create a copy of the `sample.config.yaml`, rename, and update as needed before proceeding:
+
+1. Navigate to the `self-registration` directory
+2. To build the docker image, run the following:
+
+```
+docker build . --file Dockerfile.local -t self-registration
+```
+
+3. To run the app, run the following:
+
+```
+docker run -p 8000:8000 --name self-registration self-registration
+```
+
+4. Navigate to http://0.0.0.0:8000/registration
+
 ## User Registration via this extension
+
 Steps for self registration:
 
 - Navigate to your Nebari domain.
 <p align="center">
   <img src="images/welcome-nebari.png" />
 </p>
 
@@ -51,15 +71,15 @@
   <img src="images/account-register.png" width="400"/>
 </p>
 
 - Enter your email address and coupon code.
 
 - After clicking "Submit" follow the instructions to login with your temporary password. By clicking the "Login" button, it will take you to a Welcome page where you can sign in with Keycloak.
 
-- After you have entered a new password, you will receive a verification email.  
+- After you have entered a new password, you will receive a verification email.
 
 <p align="center">
   <img src="images/account-confirm.png" />
 </p>
 
 - Once your email is verified and you login you will see the Nebari landing page.
```

