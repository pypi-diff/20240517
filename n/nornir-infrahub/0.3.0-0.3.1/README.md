# Comparing `tmp/nornir_infrahub-0.3.0.tar.gz` & `tmp/nornir_infrahub-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_infrahub-0.3.0.tar", max compression
+gzip compressed data, was "nornir_infrahub-0.3.1.tar", max compression
```

## Comparing `nornir_infrahub-0.3.0.tar` & `nornir_infrahub-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      738 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/__init__.py
--rw-r--r--   0        0        0     8816 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/inventory/infrahub.py
--rw-r--r--   0        0        0      174 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/__init__.py
--rw-r--r--   0        0        0     2046 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/artifact.py
--rw-r--r--   0        0        0     2231 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 nornir_infrahub-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2024-05-17 09:25:53.097774 nornir_infrahub-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1596 2024-05-17 10:05:14.746168 nornir_infrahub-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 14:00:57.439261 nornir_infrahub-0.3.1/nornir_infrahub/__init__.py
+-rw-r--r--   0        0        0     8816 2024-05-10 14:00:57.439579 nornir_infrahub-0.3.1/nornir_infrahub/plugins/inventory/infrahub.py
+-rw-r--r--   0        0        0      174 2024-05-10 14:00:57.439708 nornir_infrahub-0.3.1/nornir_infrahub/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-10 14:00:57.439794 nornir_infrahub-0.3.1/nornir_infrahub/plugins/tasks/artifact.py
+-rw-r--r--   0        0        0     2272 2024-05-17 10:08:39.527268 nornir_infrahub-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 nornir_infrahub-0.3.1/PKG-INFO
```

### Comparing `nornir_infrahub-0.3.0/nornir_infrahub/plugins/inventory/infrahub.py` & `nornir_infrahub-0.3.1/nornir_infrahub/plugins/inventory/infrahub.py`

 * *Files identical despite different names*

### Comparing `nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/artifact.py` & `nornir_infrahub-0.3.1/nornir_infrahub/plugins/tasks/artifact.py`

 * *Files identical despite different names*

### Comparing `nornir_infrahub-0.3.0/pyproject.toml` & `nornir_infrahub-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "nornir-infrahub"
-version = "0.3.0"
+version = "0.3.1"
 description = "Nornir plugin for Infrahub"
 authors = ["OpsMill <info@opsmill.com>"]
 readme = "README.md"
-packages = [{include = "nornir_infrahub"}]
 license = "Apache-2.0"
-homepage = "https://opsmill.io"
-repository = "https://opsmill.io"
-documentation = "https://opsmill.io"
-
+homepage = "https://opsmill.com"
+repository = "https://github.com/opsmill/nornir-infrahub"
+documentation = "https://docs.infrahub.app/"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
+packages = [
+    { include = "nornir_infrahub" }
+]
+
 [tool.poetry.plugins."nornir.plugins.inventory"]
 "InfrahubInventory" = "nornir_infrahub.plugins.inventory.infrahub:InfrahubInventory"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.13"
 infrahub-sdk = {version = "^0,>=0.9.1", extras=["tests"]}
 ruamel-yaml = "^0.18.5"
```

### Comparing `nornir_infrahub-0.3.0/PKG-INFO` & `nornir_infrahub-0.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-Metadata-Version: 2.1
-Name: nornir-infrahub
-Version: 0.3.0
-Summary: Nornir plugin for Infrahub
-Home-page: https://opsmill.io
-License: Apache-2.0
-Author: OpsMill
-Author-email: info@opsmill.com
-Requires-Python: >=3.9,<3.13
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: infrahub-sdk[tests] (>=0.9.1,<1)
-Requires-Dist: nornir (>=3.4.1,<4.0.0)
-Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
-Requires-Dist: pydantic (>=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0)
-Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
-Requires-Dist: ruamel-yaml (>=0.18.5,<0.19.0)
-Project-URL: Documentation, https://opsmill.io
-Project-URL: Repository, https://opsmill.io
-Description-Content-Type: text/markdown
+<!-- markdownlint-disable -->
+![Infrahub Logo](https://assets-global.website-files.com/657aff4a26dd8afbab24944b/657b0e0678f7fd35ce130776_Logo%20INFRAHUB.svg)
+<!-- markdownlint-restore -->
 
-# [Nornir](https://github.com/nornir-automation/nornir) plugin for [Infrahub](https://github.com/opsmill/infrahub)
+# Nornir plugin for Infrahub
+
+[Infrahub](https://github.com/opsmill/infrahub) by [OpsMill](https://opsmill.com) acts as a central hub to manage the data, templates and playbooks that powers your infrastructure. At its heart, Infrahub is built on 3 fundamental pillars:
+
+- **A Flexible Schema**: A model of the infrastructure and the relation between the objects in the model, that's easily extensible.
+- **Version Control**: Natively integrated into the graph database which opens up some new capabilities like branching, diffing, and merging data directly in the database.
+- **Unified Storage**: By combining a graph database and git, Infrahub stores data and code needed to manage the infrastructure.
+
+## Introduction
+
+A [Nornir](https://github.com/nornir-automation/nornir) plugin for Infrahub. Infrahub can be used as an inventory source for Nornir.
 
 ## Installation
 
-	pip install nornir_infrahub
+```bash
+pip install nornir_infrahub
+```
 
-## Infrahub as the Nornir inventory
+## Usage
 
-Infrahub can be used as an inventory source for Nonir.
 An example of this can be found in [./examples/nornir_inventory.py](./examples/nornir_inventory.py)
 
-## Infrahub Artifact Tasks
+## Infrahub artifact tasks
+
+A set of tasks are provided to operate on Infrahub Artifacts:
 
-A set of tasks are provided to operate on Infrahub Artifacts.
 - `generate_artifacts`: generates the Artifacts for a Artifact Definition
 - `regenerate_artifact`: re-generates an Artifact for a Nornir Host
 - `get_artifact`: retrieve an Artifact for a Nornir Host
 
 An example of this can be found in [./examples/nornir_tasks.py](./examples/nornir_tasks.py)
-
```

