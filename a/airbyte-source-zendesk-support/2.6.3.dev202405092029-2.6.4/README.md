# Comparing `tmp/airbyte_source_zendesk_support-2.6.3.dev202405092029.tar.gz` & `tmp/airbyte_source_zendesk_support-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_support-2.6.3.dev202405092029.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_support-2.6.4.tar", max compression
```

## Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029.tar` & `airbyte_source_zendesk_support-2.6.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     4673 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/README.md
--rw-r--r--   0        0        0      852 2024-05-09 20:29:45.877950 airbyte_source_zendesk_support-2.6.3.dev202405092029/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/__init__.py
--rw-r--r--   0        0        0     3294 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/components.py
--rw-r--r--   0        0        0    19960 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/manifest.yaml
--rw-r--r--   0        0        0      255 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/run.py
--rw-r--r--   0        0        0      798 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/account_attributes.json
--rw-r--r--   0        0        0     2103 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/article_comments.json
--rw-r--r--   0        0        0     3577 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/articles.json
--rw-r--r--   0        0        0     3046 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/attribute_definitions.json
--rw-r--r--   0        0        0     1741 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/audit_logs.json
--rw-r--r--   0        0        0     2061 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/brands.json
--rw-r--r--   0        0        0     9569 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/custom_roles.json
--rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/deleted_tickets.json
--rw-r--r--   0        0        0     1098 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/group_memberships.json
--rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/groups.json
--rw-r--r--   0        0        0     2642 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/macros.json
--rw-r--r--   0        0        0     2659 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organization_fields.json
--rw-r--r--   0        0        0     1453 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organization_memberships.json
--rw-r--r--   0        0        0     2262 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organizations.json
--rw-r--r--   0        0        0     1978 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/post_comments.json
--rw-r--r--   0        0        0     3315 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/posts.json
--rw-r--r--   0        0        0     1843 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0     1239 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/schedules.json
--rw-r--r--   0        0        0     1958 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/attachments.json
--rw-r--r--   0        0        0     1835 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/metadata.json
--rw-r--r--   0        0        0     4521 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/tickets.json
--rw-r--r--   0        0        0     1617 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/via.json
--rw-r--r--   0        0        0     2707 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/via_channel.json
--rw-r--r--   0        0        0     3655 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/sla_policies.json
--rw-r--r--   0        0        0      320 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/tags.json
--rw-r--r--   0        0        0     2114 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_activities.json
--rw-r--r--   0        0        0    29608 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_audits.json
--rw-r--r--   0        0        0     2495 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_comments.json
--rw-r--r--   0        0        0     4685 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_fields.json
--rw-r--r--   0        0        0     2644 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_forms.json
--rw-r--r--   0        0        0      855 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_metric_events.json
--rw-r--r--   0        0        0     7095 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_metrics.json
--rw-r--r--   0        0        0     1013 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_skips.json
--rw-r--r--   0        0        0       27 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/tickets.json
--rw-r--r--   0        0        0     1735 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/topics.json
--rw-r--r--   0        0        0     2182 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/user_fields.json
--rw-r--r--   0        0        0     8484 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/users.json
--rw-r--r--   0        0        0     1170 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/votes.json
--rw-r--r--   0        0        0     7876 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/source.py
--rw-r--r--   0        0        0     5975 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/spec.json
--rw-r--r--   0        0        0    39231 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/streams.py
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.3.dev202405092029/PKG-INFO
+-rw-r--r--   0        0        0     4673 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/README.md
+-rw-r--r--   0        0        0      836 2024-05-17 12:50:04.319633 airbyte_source_zendesk_support-2.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/__init__.py
+-rw-r--r--   0        0        0     3294 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/components.py
+-rw-r--r--   0        0        0    19960 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/manifest.yaml
+-rw-r--r--   0        0        0      255 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/run.py
+-rw-r--r--   0        0        0      798 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/account_attributes.json
+-rw-r--r--   0        0        0     2103 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/article_comments.json
+-rw-r--r--   0        0        0     3577 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/articles.json
+-rw-r--r--   0        0        0     3046 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/attribute_definitions.json
+-rw-r--r--   0        0        0     1741 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/audit_logs.json
+-rw-r--r--   0        0        0     2061 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/brands.json
+-rw-r--r--   0        0        0     9569 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/custom_roles.json
+-rw-r--r--   0        0        0     1211 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/deleted_tickets.json
+-rw-r--r--   0        0        0     1098 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/group_memberships.json
+-rw-r--r--   0        0        0     1211 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/groups.json
+-rw-r--r--   0        0        0     2642 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/macros.json
+-rw-r--r--   0        0        0     2659 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organization_fields.json
+-rw-r--r--   0        0        0     1453 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organization_memberships.json
+-rw-r--r--   0        0        0     2262 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organizations.json
+-rw-r--r--   0        0        0     1978 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/post_comments.json
+-rw-r--r--   0        0        0     3315 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/posts.json
+-rw-r--r--   0        0        0     1843 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0     1239 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/schedules.json
+-rw-r--r--   0        0        0     1958 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/attachments.json
+-rw-r--r--   0        0        0     1835 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/metadata.json
+-rw-r--r--   0        0        0     4521 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/tickets.json
+-rw-r--r--   0        0        0     1617 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/via.json
+-rw-r--r--   0        0        0     2707 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/via_channel.json
+-rw-r--r--   0        0        0     3655 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/sla_policies.json
+-rw-r--r--   0        0        0      320 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/tags.json
+-rw-r--r--   0        0        0     2114 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_activities.json
+-rw-r--r--   0        0        0    29608 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_audits.json
+-rw-r--r--   0        0        0     2495 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_comments.json
+-rw-r--r--   0        0        0     4685 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     2644 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_forms.json
+-rw-r--r--   0        0        0      855 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_metric_events.json
+-rw-r--r--   0        0        0     7095 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_metrics.json
+-rw-r--r--   0        0        0     1013 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_skips.json
+-rw-r--r--   0        0        0       27 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/tickets.json
+-rw-r--r--   0        0        0     1735 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/topics.json
+-rw-r--r--   0        0        0     2182 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/user_fields.json
+-rw-r--r--   0        0        0     8484 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/users.json
+-rw-r--r--   0        0        0     1170 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/votes.json
+-rw-r--r--   0        0        0     7876 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/source.py
+-rw-r--r--   0        0        0     5975 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/spec.json
+-rw-r--r--   0        0        0    39319 2024-05-17 11:02:35.000000 airbyte_source_zendesk_support-2.6.4/source_zendesk_support/streams.py
+-rw-r--r--   0        0        0     5434 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.4/PKG-INFO
```

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/README.md` & `airbyte_source_zendesk_support-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/pyproject.toml` & `airbyte_source_zendesk_support-2.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.6.3.dev202405092029"
+version = "2.6.4"
 name = "airbyte-source-zendesk-support"
 description = "Source implementation for Zendesk Support."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/__init__.py` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/components.py` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/manifest.yaml` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/account_attributes.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/account_attributes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/article_comments.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/article_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/articles.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/attribute_definitions.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/attribute_definitions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/audit_logs.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/audit_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/brands.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/brands.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/custom_roles.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/custom_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/deleted_tickets.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/deleted_tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/group_memberships.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/groups.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/macros.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organization_fields.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organization_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organization_memberships.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organization_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/organizations.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/post_comments.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/post_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/posts.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/posts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/satisfaction_ratings.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/schedules.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/schedules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/attachments.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/metadata.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/tickets.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/via.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/shared/via_channel.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/shared/via_channel.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/sla_policies.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_activities.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_audits.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_comments.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_fields.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_forms.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_metric_events.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_metric_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_metrics.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/ticket_skips.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/ticket_skips.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/topics.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/topics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/user_fields.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/user_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/users.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/schemas/votes.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/schemas/votes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/source.py` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/spec.json` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/source_zendesk_support/streams.py` & `airbyte_source_zendesk_support-2.6.4/source_zendesk_support/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,17 +376,17 @@
 
 
 class SourceZendeskSupportTicketEventsExportStream(SourceZendeskIncrementalExportStream):
     """Incremental Export from TicketEvents stream:
     https://developer.zendesk.com/api-reference/ticketing/ticket-management/incremental_exports/#incremental-ticket-event-export
 
     @ param response_list_name: the main nested entity to look at inside of response, default = "ticket_events"
-    @ param response_target_entity: nested property inside of `response_list_name`, default = "child_events"
+    @ param response_target_entity: nested property inside `response_list_name`, default = "child_events"
     @ param list_entities_from_event : the list of nested child_events entities to include from parent record
-    @ param event_type : specific event_type to check ["Audit", "Change", "Comment", etc]
+    @ param event_type : specific event_type to check ["Audit", "Change", "Comment", etc.]
     @ param sideload_param : parameter variable to include various information to response
     """
 
     cursor_field = "created_at"
     event_type: str = None
     list_entities_from_event: List[str] = None
     response_list_name: str = "ticket_events"
@@ -503,35 +503,37 @@
         return {}
 
     def stream_slices(
         self, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, stream_state: Optional[Mapping[str, Any]] = None
     ) -> Iterable[Optional[Mapping[str, Any]]]:
         parent_stream_state = None
         if stream_state:
-            cursor_value = pendulum.parse(stream_state.get(self.cursor_field)).int_timestamp
-            parent_stream_state = {self.parent.cursor_field: cursor_value}
+            cursor_value = stream_state.get(self.cursor_field)
+            parent_stream_state = {self.parent.cursor_field: pendulum.parse(cursor_value).int_timestamp}
+        else:
+            cursor_value = self._start_date
 
         parent_records = self.parent.read_records(
             sync_mode=SyncMode.incremental, cursor_field=cursor_field, stream_slice=None, stream_state=parent_stream_state
         )
 
         for record in parent_records:
-            yield {"ticket_id": record["id"]}
+            yield {"ticket_id": record["id"], self.cursor_field: cursor_value}
 
     def should_retry(self, response: requests.Response) -> bool:
         if response.status_code == 404:
             #  not found in case of deleted ticket
             setattr(self, "raise_on_http_errors", False)
             return False
         return super().should_retry(response)
 
 
 class TicketComments(SourceZendeskSupportTicketEventsExportStream):
     """
-    Fetch the TicketComments incrementaly from TicketEvents Export stream
+    Fetch the TicketComments incrementally from TicketEvents Export stream
     """
 
     list_entities_from_event = ["via_reference_id", "ticket_id", "timestamp"]
     sideload_param = "comment_events"
     event_type = "Comment"
 
     def parse_response(self, response: requests.Response, **kwargs) -> Iterable[Mapping]:
@@ -599,31 +601,34 @@
         *,
         stream_state: Optional[Mapping[str, Any]] = None,
         stream_slice: Optional[Mapping[str, Any]] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> str:
         return f"tickets/{stream_slice['ticket_id']}/metrics"
 
-    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
+    def parse_response(
+        self,
+        response: requests.Response,
+        stream_state: Mapping[str, Any],
+        stream_slice: Optional[Mapping[str, Any]] = None,
+        **kwargs,
+    ) -> Iterable[Mapping]:
         """try to select relevant data only"""
 
         try:
             data = response.json().get(self.response_list_name or self.name) or {}
         except requests.exceptions.JSONDecodeError:
             data = {}
 
         # no data in case of http errors
         if data:
-            if not self.cursor_field:
+            cursor_date = (stream_slice or {}).get(self.cursor_field)
+            updated = data[self.cursor_field]
+            if not cursor_date or updated >= cursor_date:
                 yield data
-            else:
-                cursor_date = (stream_state or {}).get(self.cursor_field)
-                updated = data[self.cursor_field]
-                if not cursor_date or updated >= cursor_date:
-                    yield data
 
 
 class TicketSkips(CursorPaginationZendeskSupportStream):
     """TicketSkips stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_skips/"""
 
     response_list_name = "skips"
```

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405092029/PKG-INFO` & `airbyte_source_zendesk_support-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-support
-Version: 2.6.3.dev202405092029
+Version: 2.6.4
 Summary: Source implementation for Zendesk Support.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

