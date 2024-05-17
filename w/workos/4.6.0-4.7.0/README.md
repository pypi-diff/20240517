# Comparing `tmp/workos-4.6.0.tar.gz` & `tmp/workos-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.6.0.tar", last modified: Fri May  3 20:17:54 2024, max compression
+gzip compressed data, was "workos-4.7.0.tar", last modified: Fri May 17 14:02:34 2024, max compression
```

## Comparing `workos-4.6.0.tar` & `workos-4.7.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:17:46.000000 workos-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 20:17:54.251297 workos-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 20:17:46.000000 workos-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:17:54.255297 workos-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-03 20:17:46.000000 workos-4.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 20:17:46.000000 workos-4.6.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-03 20:17:46.000000 workos-4.6.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-03 20:17:46.000000 workos-4.6.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-03 20:17:46.000000 workos-4.6.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-03 20:17:46.000000 workos-4.6.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-03 20:17:46.000000 workos-4.6.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 20:17:46.000000 workos-4.6.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-03 20:17:46.000000 workos-4.6.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-03 20:17:46.000000 workos-4.6.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-03 20:17:46.000000 workos-4.6.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 20:17:46.000000 workos-4.6.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-03 20:17:46.000000 workos-4.6.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-03 20:17:46.000000 workos-4.6.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-03 20:17:46.000000 workos-4.6.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:17:52.000000 workos-4.6.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.688580 workos-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 14:02:27.000000 workos-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-17 14:02:34.688580 workos-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-17 14:02:27.000000 workos-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:02:34.688580 workos-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 14:02:27.000000 workos-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 14:02:27.000000 workos-4.7.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 14:02:27.000000 workos-4.7.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-17 14:02:27.000000 workos-4.7.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-17 14:02:27.000000 workos-4.7.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-17 14:02:27.000000 workos-4.7.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 14:02:27.000000 workos-4.7.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-17 14:02:27.000000 workos-4.7.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-17 14:02:27.000000 workos-4.7.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-17 14:02:27.000000 workos-4.7.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 14:02:27.000000 workos-4.7.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 14:02:27.000000 workos-4.7.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-17 14:02:27.000000 workos-4.7.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43591 2024-05-17 14:02:27.000000 workos-4.7.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-17 14:02:27.000000 workos-4.7.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:02:32.000000 workos-4.7.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.6.0/LICENSE` & `workos-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/PKG-INFO` & `workos-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.6.0
+Version: 4.7.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.6.0/README.md` & `workos-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/setup.py` & `workos-4.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/audit_logs.py` & `workos-4.7.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/client.py` & `workos-4.7.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/directory_sync.py` & `workos-4.7.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/events.py` & `workos-4.7.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/exceptions.py` & `workos-4.7.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/mfa.py` & `workos-4.7.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/organizations.py` & `workos-4.7.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/passwordless.py` & `workos-4.7.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/portal.py` & `workos-4.7.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/audit_logs_export.py` & `workos-4.7.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/base.py` & `workos-4.7.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/directory_sync.py` & `workos-4.7.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/event.py` & `workos-4.7.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/list.py` & `workos-4.7.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/mfa.py` & `workos-4.7.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/organizations.py` & `workos-4.7.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/passwordless.py` & `workos-4.7.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/sso.py` & `workos-4.7.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/resources/user_management.py` & `workos-4.7.0/workos/resources/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/sso.py` & `workos-4.7.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/user_management.py` & `workos-4.7.0/workos/user_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 )
 from workos.utils.validation import validate_settings, USER_MANAGEMENT_MODULE
 
 USER_PATH = "user_management/users"
 USER_DETAIL_PATH = "user_management/users/{0}"
 ORGANIZATION_MEMBERSHIP_PATH = "user_management/organization_memberships"
 ORGANIZATION_MEMBERSHIP_DETAIL_PATH = "user_management/organization_memberships/{0}"
+ORGANIZATION_MEMBERSHIP_DEACTIVATE_PATH = (
+    ORGANIZATION_MEMBERSHIP_DETAIL_PATH + "/deactivate"
+)
+ORGANIZATION_MEMBERSHIP_REACTIVATE_PATH = (
+    ORGANIZATION_MEMBERSHIP_DETAIL_PATH + "/reactivate"
+)
 USER_AUTHORIZATION_PATH = "user_management/authorize"
 USER_AUTHENTICATE_PATH = "user_management/authenticate"
 USER_SEND_PASSWORD_RESET_PATH = "user_management/password_reset/send"
 USER_RESET_PASSWORD_PATH = "user_management/password_reset/confirm"
 USER_SEND_VERIFICATION_EMAIL_PATH = "user_management/users/{0}/email_verification/send"
 USER_VERIFY_EMAIL_CODE_PATH = "user_management/users/{0}/email_verification/confirm"
 MAGIC_AUTH_DETAIL_PATH = "user_management/magic_auth/{0}"
@@ -286,24 +292,26 @@
 
         return WorkOSOrganizationMembership.construct_from_response(response).to_dict()
 
     def list_organization_memberships(
         self,
         user_id=None,
         organization_id=None,
+        statuses=None,
         limit=None,
         before=None,
         after=None,
         order=None,
     ):
         """Get a list of all of your existing organization memberships matching the criteria specified.
 
         Kwargs:
             user_id (str): Filter Organization Memberships by user. (Optional)
             organization_id (str): Filter Organization Memberships by organization. (Optional)
+            statuses (list): Filter Organization Memberships by status. (Optional)
             limit (int): Maximum number of records to return. (Optional)
             before (str): Pagination cursor to receive records before a provided Organization Membership ID. (Optional)
             after (str): Pagination cursor to receive records after a provided Organization Membership ID. (Optional)
             order (Order): Sort records in either ascending or descending order by created_at timestamp: "asc" or "desc" (Optional)
 
         Returns:
             dict: Organization Memberships response from WorkOS.
@@ -311,17 +319,21 @@
 
         default_limit = None
 
         if limit is None:
             limit = RESPONSE_LIMIT
             default_limit = True
 
+        if statuses is not None:
+            statuses = ",".join(statuses)
+
         params = {
             "user_id": user_id,
             "organization_id": organization_id,
+            "statuses": statuses,
             "limit": limit,
             "before": before,
             "after": after,
             "order": order or "desc",
         }
 
         if order is not None:
@@ -360,14 +372,46 @@
         """
         self.request_helper.request(
             ORGANIZATION_MEMBERSHIP_DETAIL_PATH.format(organization_membership_id),
             method=REQUEST_METHOD_DELETE,
             token=workos.api_key,
         )
 
+    def deactivate_organization_membership(self, organization_membership_id):
+        """Deactivate an organization membership.
+
+        Args:
+            organization_membership_id (str) -  The unique ID of the Organization Membership.
+        Returns:
+            dict: OrganizationMembership response from WorkOS.
+        """
+        response = self.request_helper.request(
+            ORGANIZATION_MEMBERSHIP_DEACTIVATE_PATH.format(organization_membership_id),
+            method=REQUEST_METHOD_PUT,
+            token=workos.api_key,
+        )
+
+        return WorkOSOrganizationMembership.construct_from_response(response).to_dict()
+
+    def reactivate_organization_membership(self, organization_membership_id):
+        """Reactivates an organization membership.
+
+        Args:
+            organization_membership_id (str) -  The unique ID of the Organization Membership.
+        Returns:
+            dict: OrganizationMembership response from WorkOS.
+        """
+        response = self.request_helper.request(
+            ORGANIZATION_MEMBERSHIP_REACTIVATE_PATH.format(organization_membership_id),
+            method=REQUEST_METHOD_PUT,
+            token=workos.api_key,
+        )
+
+        return WorkOSOrganizationMembership.construct_from_response(response).to_dict()
+
     def get_authorization_url(
         self,
         redirect_uri,
         connection_id=None,
         organization_id=None,
         provider=None,
         domain_hint=None,
@@ -757,14 +801,38 @@
             params=payload,
         )
 
         return WorkOSRefreshTokenAuthenticationResponse.construct_from_response(
             response
         ).to_dict()
 
+    def get_jwks_url(self):
+        """Get the public key that is used for verifying access tokens.
+
+        Returns:
+            (str): The public JWKS URL.
+        """
+
+        return "%s/sso/jwks/%s" % (workos.base_api_url, workos.client_id)
+
+    def get_logout_url(self, session_id):
+        """Get the URL for ending the session and redirecting the user
+
+        Kwargs:
+            session_id (str): The ID of the user's session
+
+        Returns:
+            (str): URL to redirect the user to to end the session.
+        """
+
+        return "%s/user_management/sessions/logout?session_id=%s" % (
+            workos.base_api_url,
+            session_id,
+        )
+
     def send_password_reset_email(
         self,
         email,
         password_reset_url,
     ):
         """Sends a password reset email to a user.
 
@@ -997,14 +1065,15 @@
 
         factor_and_challenge = {}
         factor_and_challenge[
             "authentication_factor"
         ] = WorkOSAuthenticationFactorTotp.construct_from_response(
             response["authentication_factor"]
         ).to_dict()
+
         factor_and_challenge[
             "authentication_challenge"
         ] = WorkOSChallenge.construct_from_response(
             response["authentication_challenge"]
         ).to_dict()
 
         return factor_and_challenge
```

### Comparing `workos-4.6.0/workos/utils/connection_types.py` & `workos-4.7.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/utils/request.py` & `workos-4.7.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/utils/validation.py` & `workos-4.7.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos/webhooks.py` & `workos-4.7.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.6.0/workos.egg-info/PKG-INFO` & `workos-4.7.0/workos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.6.0
+Version: 4.7.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.6.0/workos.egg-info/SOURCES.txt` & `workos-4.7.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

