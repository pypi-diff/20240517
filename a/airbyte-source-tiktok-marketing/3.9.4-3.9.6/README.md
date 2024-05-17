# Comparing `tmp/airbyte_source_tiktok_marketing-3.9.4.tar.gz` & `tmp/airbyte_source_tiktok_marketing-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_tiktok_marketing-3.9.4.tar", max compression
+gzip compressed data, was "airbyte_source_tiktok_marketing-3.9.6.tar", max compression
```

## Comparing `airbyte_source_tiktok_marketing-3.9.4.tar` & `airbyte_source_tiktok_marketing-3.9.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4676 2024-03-25 20:20:22.320083 airbyte_source_tiktok_marketing-3.9.4/README.md
--rw-r--r--   0        0        0      830 2024-03-25 20:23:37.269764 airbyte_source_tiktok_marketing-3.9.4/pyproject.toml
--rw-r--r--   0        0        0     1183 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/__init__.py
--rw-r--r--   0        0        0      258 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/run.py
--rw-r--r--   0        0        0     9740 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/ad_groups.json
--rw-r--r--   0        0        0     6374 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/ads.json
--rw-r--r--   0        0        0      154 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/advertiser_ids.json
--rw-r--r--   0        0        0     1781 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/advertisers.json
--rw-r--r--   0        0        0     4618 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/audience_reports.json
--rw-r--r--   0        0        0      767 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/audiences.json
--rw-r--r--   0        0        0     7572 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/basic_reports.json
--rw-r--r--   0        0        0     1587 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0      876 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/creative_assets_images.json
--rw-r--r--   0        0        0     1029 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/creative_assets_music.json
--rw-r--r--   0        0        0      269 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/creative_assets_portfolios.json
--rw-r--r--   0        0        0     1337 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/creative_assets_videos.json
--rw-r--r--   0        0        0     8989 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/source.py
--rw-r--r--   0        0        0     5711 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/spec.json
--rw-r--r--   0        0        0    33489 2024-03-25 20:20:22.324083 airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/streams.py
--rw-r--r--   0        0        0     5408 1970-01-01 00:00:00.000000 airbyte_source_tiktok_marketing-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     4676 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/README.md
+-rw-r--r--   0        0        0      834 2024-05-07 13:35:52.243032 airbyte_source_tiktok_marketing-3.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1183 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/run.py
+-rw-r--r--   0        0        0    16860 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/ad_groups.json
+-rw-r--r--   0        0        0    12120 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/ads.json
+-rw-r--r--   0        0        0      350 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/advertiser_ids.json
+-rw-r--r--   0        0        0     3977 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/advertisers.json
+-rw-r--r--   0        0        0     8244 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/audience_reports.json
+-rw-r--r--   0        0        0     1523 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/audiences.json
+-rw-r--r--   0        0        0    13794 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/basic_reports.json
+-rw-r--r--   0        0        0     3350 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     1742 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/creative_assets_images.json
+-rw-r--r--   0        0        0     2119 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/creative_assets_music.json
+-rw-r--r--   0        0        0      534 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/creative_assets_portfolios.json
+-rw-r--r--   0        0        0     2465 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/creative_assets_videos.json
+-rw-r--r--   0        0        0     8989 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/source.py
+-rw-r--r--   0        0        0     5711 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/spec.json
+-rw-r--r--   0        0        0    33489 2024-05-07 11:15:22.000000 airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/streams.py
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 airbyte_source_tiktok_marketing-3.9.6/PKG-INFO
```

### Comparing `airbyte_source_tiktok_marketing-3.9.4/README.md` & `airbyte_source_tiktok_marketing-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_tiktok_marketing-3.9.4/pyproject.toml` & `airbyte_source_tiktok_marketing-3.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.9.4"
+version = "3.9.6"
 name = "airbyte-source-tiktok-marketing"
 description = "Source implementation for Tiktok Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_tiktok_marketing" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-tiktok-marketing = "source_tiktok_marketing.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "==1.9.3"
 timeout-decorator = "==0.5.0"
```

### Comparing `airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/__init__.py` & `airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/schemas/creative_assets_videos.json` & `airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/schemas/audiences.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7574404761904762%*

 * *Differences: {"'properties'": "{'create_time': {'description': 'Timestamp indicating when the audience was "*

 * *                 "created'}, 'shared': OrderedDict([('description', 'Flag indicating if the "*

 * *                 "audience is shared with others'), ('type', ['null', 'boolean'])]), 'is_creator': "*

 * *                 "OrderedDict([('description', 'Flag indicating if the audience creator is the "*

 * *                 "user'), ('type', ['null', 'boolean'])]), 'audience_id': "*

 * *                 "OrderedDict([('description', ' […]*

```diff
@@ -1,123 +1,84 @@
 {
     "properties": {
-        "allow_download": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "allowed_placements": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "bit_rate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "create_time": {
-            "format": "date-time",
+        "audience_id": {
+            "description": "Unique identifier for the audience",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "displayable": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "duration": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "file_name": {
+        "audience_type": {
+            "description": "Type of audience (e.g., demographic, interest-based)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "format": {
+        "calculate_type": {
+            "description": "Method used to calculate audience data",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "height": {
+        "cover_num": {
+            "description": "Number of audience members covered",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "material_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "modify_time": {
+        "create_time": {
+            "description": "Timestamp indicating when the audience was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "preview_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "preview_url_expire_time": {
-            "airbyte_type": "timestamp_without_timezone",
+        "expired_time": {
+            "description": "Timestamp indicating when the audience data expires",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "signature": {
+        "is_creator": {
+            "description": "Flag indicating if the audience creator is the user",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "size": {
+        "is_expiring": {
+            "description": "Flag indicating if the audience data is expiring soon",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "video_cover_url": {
+        "is_valid": {
+            "description": "Flag indicating if the audience data is valid",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "video_id": {
+        "name": {
+            "description": "Name of the audience",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "width": {
+        "shared": {
+            "description": "Flag indicating if the audience is shared with others",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/source.py` & `airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/spec.json` & `airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_tiktok_marketing-3.9.4/source_tiktok_marketing/streams.py` & `airbyte_source_tiktok_marketing-3.9.6/source_tiktok_marketing/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_tiktok_marketing-3.9.4/PKG-INFO` & `airbyte_source_tiktok_marketing-3.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-tiktok-marketing
-Version: 3.9.4
+Version: 3.9.6
 Summary: Source implementation for Tiktok Marketing.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/tiktok-marketing
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Tiktok-Marketing source connector
```

