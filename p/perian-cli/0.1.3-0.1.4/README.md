# Comparing `tmp/perian_cli-0.1.3.tar.gz` & `tmp/perian_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perian_cli-0.1.3.tar", max compression
+gzip compressed data, was "perian_cli-0.1.4.tar", max compression
```

## Comparing `perian_cli-0.1.3.tar` & `perian_cli-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      238 2024-05-16 08:33:28.069526 perian_cli-0.1.3/README.md
--rw-r--r--   0        0        0     1220 2024-05-02 07:42:40.320695 perian_cli-0.1.3/pcli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 07:42:40.320764 perian_cli-0.1.3/pcli/api/__init__.py
--rw-r--r--   0        0        0     3607 2024-05-02 07:42:40.320850 perian_cli-0.1.3/pcli/api/accelerator_type.py
--rw-r--r--   0        0        0     1452 2024-05-02 07:42:40.320918 perian_cli-0.1.3/pcli/api/billing.py
--rw-r--r--   0        0        0     3200 2024-05-02 07:42:40.320995 perian_cli-0.1.3/pcli/api/instance_type.py
--rw-r--r--   0        0        0     3670 2024-05-08 19:41:47.993678 perian_cli-0.1.3/pcli/api/job.py
--rw-r--r--   0        0        0     1020 2024-05-08 19:38:12.714322 perian_cli-0.1.3/pcli/api/organization.py
--rw-r--r--   0        0        0     4950 2024-05-07 11:53:55.387135 perian_cli-0.1.3/pcli/cli.py
--rw-r--r--   0        0        0      133 2024-05-02 07:42:40.321188 perian_cli-0.1.3/pcli/colors.py
--rw-r--r--   0        0        0        0 2024-05-02 07:42:40.321250 perian_cli-0.1.3/pcli/commands/__init__.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:42:40.321328 perian_cli-0.1.3/pcli/commands/accelerator_type.py
--rw-r--r--   0        0        0     1846 2024-05-02 07:42:40.321388 perian_cli-0.1.3/pcli/commands/billing.py
--rw-r--r--   0        0        0      344 2024-05-02 07:42:40.321449 perian_cli-0.1.3/pcli/commands/config.py
--rw-r--r--   0        0        0      898 2024-05-02 07:42:40.321513 perian_cli-0.1.3/pcli/commands/currency.py
--rw-r--r--   0        0        0     3526 2024-05-02 07:42:40.321588 perian_cli-0.1.3/pcli/commands/instance_type.py
--rw-r--r--   0        0        0     9529 2024-05-16 06:57:29.587333 perian_cli-0.1.3/pcli/commands/job.py
--rw-r--r--   0        0        0     4523 2024-05-07 11:53:55.388603 perian_cli-0.1.3/pcli/commands/registry.py
--rw-r--r--   0        0        0     5756 2024-05-08 19:41:47.994564 perian_cli-0.1.3/pcli/responses.py
--rw-r--r--   0        0        0      446 2024-05-07 14:19:49.243150 perian_cli-0.1.3/pcli/settings.py
--rw-r--r--   0        0        0     4452 2024-05-07 11:53:55.389921 perian_cli-0.1.3/pcli/util/__init__.py
--rw-r--r--   0        0        0     3688 2024-05-02 07:42:40.322636 perian_cli-0.1.3/pcli/util/currencies.py
--rw-r--r--   0        0        0     1086 2024-05-02 07:42:40.322715 perian_cli-0.1.3/pcli/util/db.py
--rw-r--r--   0        0        0    18983 2024-05-15 13:00:01.635606 perian_cli-0.1.3/pcli/util/formatter.py
--rw-r--r--   0        0        0      566 2024-05-02 07:42:40.322935 perian_cli-0.1.3/pcli/util/organization.py
--rw-r--r--   0        0        0    24293 2024-05-02 07:42:40.323042 perian_cli-0.1.3/pcli/util/rich_utils.py
--rw-r--r--   0        0        0     1185 2024-05-07 11:53:55.390884 perian_cli-0.1.3/pcli/util/setup.py
--rw-r--r--   0        0        0      653 2024-05-16 09:18:45.579379 perian_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 perian_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1220 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/accelerator_type.py
+-rw-r--r--   0        0        0     1452 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/billing.py
+-rw-r--r--   0        0        0     3200 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/instance_type.py
+-rw-r--r--   0        0        0     3670 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/job.py
+-rw-r--r--   0        0        0     1020 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/api/organization.py
+-rw-r--r--   0        0        0     4950 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/cli.py
+-rw-r--r--   0        0        0      133 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/colors.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/accelerator_type.py
+-rw-r--r--   0        0        0     1846 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/billing.py
+-rw-r--r--   0        0        0      344 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/config.py
+-rw-r--r--   0        0        0      898 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/currency.py
+-rw-r--r--   0        0        0     3526 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/instance_type.py
+-rw-r--r--   0        0        0     9529 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/job.py
+-rw-r--r--   0        0        0     4523 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/commands/registry.py
+-rw-r--r--   0        0        0     5756 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/responses.py
+-rw-r--r--   0        0        0      446 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/settings.py
+-rw-r--r--   0        0        0     4452 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/__init__.py
+-rw-r--r--   0        0        0     3688 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/currencies.py
+-rw-r--r--   0        0        0     1086 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/db.py
+-rw-r--r--   0        0        0    18983 2024-05-17 10:42:58.482600 perian_cli-0.1.4/pcli/util/formatter.py
+-rw-r--r--   0        0        0      566 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/organization.py
+-rw-r--r--   0        0        0    24293 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/rich_utils.py
+-rw-r--r--   0        0        0     1185 2024-05-16 14:06:00.296518 perian_cli-0.1.4/pcli/util/setup.py
+-rw-r--r--   0        0        0      633 2024-05-17 12:49:40.140266 perian_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 perian_cli-0.1.4/PKG-INFO
```

### Comparing `perian_cli-0.1.3/pcli/__init__.py` & `perian_cli-0.1.4/pcli/__init__.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/api/accelerator_type.py` & `perian_cli-0.1.4/pcli/api/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/api/billing.py` & `perian_cli-0.1.4/pcli/api/billing.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/api/instance_type.py` & `perian_cli-0.1.4/pcli/api/instance_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/api/job.py` & `perian_cli-0.1.4/pcli/api/job.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/api/organization.py` & `perian_cli-0.1.4/pcli/api/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/cli.py` & `perian_cli-0.1.4/pcli/cli.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/accelerator_type.py` & `perian_cli-0.1.4/pcli/commands/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/billing.py` & `perian_cli-0.1.4/pcli/commands/billing.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/currency.py` & `perian_cli-0.1.4/pcli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/instance_type.py` & `perian_cli-0.1.4/pcli/commands/instance_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/job.py` & `perian_cli-0.1.4/pcli/commands/job.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/commands/registry.py` & `perian_cli-0.1.4/pcli/commands/registry.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/responses.py` & `perian_cli-0.1.4/pcli/responses.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/__init__.py` & `perian_cli-0.1.4/pcli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/currencies.py` & `perian_cli-0.1.4/pcli/util/currencies.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/db.py` & `perian_cli-0.1.4/pcli/util/db.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/formatter.py` & `perian_cli-0.1.4/pcli/util/formatter.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/organization.py` & `perian_cli-0.1.4/pcli/util/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/rich_utils.py` & `perian_cli-0.1.4/pcli/util/rich_utils.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pcli/util/setup.py` & `perian_cli-0.1.4/pcli/util/setup.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.1.3/pyproject.toml` & `perian_cli-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "perian-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "Perian Sky Platform CLI"
 authors = ["Perian <info@perian.io>"]
 homepage = "https://perian.io"
 documentation = "https://perian.io"
 packages = [{include = "pcli"}]
-readme = "README.md"
 
 [tool.poetry.scripts]
 perian = "pcli.cli:pcli"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 typer = "0.12.3"
 validators = "0.28.1"
 pydantic = "2.7.0"
 click = "8.1.7"
 rich = "13.7.1"
 toml = "0.10.2"
-perian = "0.2.0"
+perian = "0.2.1"
 requests = "2.31.0"
 pydantic-settings = "2.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
```

