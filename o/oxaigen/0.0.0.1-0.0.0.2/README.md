# Comparing `tmp/oxaigen-0.0.0.1.tar.gz` & `tmp/oxaigen-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.1.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.2.tar", max compression
```

## Comparing `oxaigen-0.0.0.1.tar` & `oxaigen-0.0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1293 2024-04-06 12:49:14.680802 oxaigen-0.0.0.1/README.md
--rw-r--r--   0        0        0      175 2024-05-16 23:12:08.437620 oxaigen-0.0.0.1/oxaigen_client_sdk/__init__.py
--rw-r--r--   0        0        0      818 2024-05-16 23:07:27.647862 oxaigen-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 oxaigen-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      208 2024-05-16 23:14:00.577589 oxaigen-0.0.0.2/README.md
+-rw-r--r--   0        0        0      175 2024-05-16 23:12:08.437620 oxaigen-0.0.0.2/oxaigen_client_sdk/__init__.py
+-rw-r--r--   0        0        0      818 2024-05-16 23:14:22.071687 oxaigen-0.0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 oxaigen-0.0.0.2/PKG-INFO
```

### Comparing `oxaigen-0.0.0.1/pyproject.toml` & `oxaigen-0.0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.1"
+version = "0.0.0.2"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==1.10.8"
```

