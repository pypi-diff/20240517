# Comparing `tmp/nodestream_plugin_gcp_asset_inventory-0.1.3.tar.gz` & `tmp/nodestream_plugin_gcp_asset_inventory-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_gcp_asset_inventory-0.1.3.tar", max compression
+gzip compressed data, was "nodestream_plugin_gcp_asset_inventory-0.1.4.tar", max compression
```

## Comparing `nodestream_plugin_gcp_asset_inventory-0.1.3.tar` & `nodestream_plugin_gcp_asset_inventory-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-01 17:19:18.855690 nodestream_plugin_gcp_asset_inventory-0.1.3/README.md
--rw-r--r--   0        0        0      224 2024-05-08 17:22:49.266110 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/__init__.py
--rw-r--r--   0        0        0      383 2024-05-07 23:38:31.762760 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcpAsset.yaml
--rw-r--r--   0        0        0      488 2024-05-07 23:41:04.640465 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcpPolicy.yaml
--rw-r--r--   0        0        0       84 2024-05-08 17:22:57.264368 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_asset/__init__.py
--rw-r--r--   0        0        0      720 2024-05-14 05:00:16.996097 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_asset/gcp_asset_extractor.py
--rw-r--r--   0        0        0       87 2024-05-08 17:23:01.170915 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_policy/__init__.py
--rw-r--r--   0        0        0     1429 2024-05-14 05:00:30.877616 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_policy/gcp_policy_extractor.py
--rw-r--r--   0        0        0      307 2024-05-07 22:41:39.102862 nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/plugin.py
--rw-r--r--   0        0        0      463 2024-05-14 06:05:15.240129 nodestream_plugin_gcp_asset_inventory-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 nodestream_plugin_gcp_asset_inventory-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 17:19:18.855690 nodestream_plugin_gcp_asset_inventory-0.1.4/README.md
+-rw-r--r--   0        0        0      224 2024-05-08 17:22:49.266110 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-16 23:55:35.664483 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcpAsset.yaml
+-rw-r--r--   0        0        0      606 2024-05-16 23:57:59.339655 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcpPolicy.yaml
+-rw-r--r--   0        0        0       84 2024-05-08 17:22:57.264368 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_asset/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-14 05:00:16.996097 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_asset/gcp_asset_extractor.py
+-rw-r--r--   0        0        0       87 2024-05-08 17:23:01.170915 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_policy/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-14 05:00:30.877616 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_policy/gcp_policy_extractor.py
+-rw-r--r--   0        0        0      307 2024-05-07 22:41:39.102862 nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/plugin.py
+-rw-r--r--   0        0        0      504 2024-05-17 00:17:08.214291 nodestream_plugin_gcp_asset_inventory-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 nodestream_plugin_gcp_asset_inventory-0.1.4/PKG-INFO
```

### Comparing `nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_asset/gcp_asset_extractor.py` & `nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_asset/gcp_asset_extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_gcp_asset_inventory-0.1.3/nodestream_plugin_gcp_asset_inventory/gcp_policy/gcp_policy_extractor.py` & `nodestream_plugin_gcp_asset_inventory-0.1.4/nodestream_plugin_gcp_asset_inventory/gcp_policy/gcp_policy_extractor.py`

 * *Files identical despite different names*

