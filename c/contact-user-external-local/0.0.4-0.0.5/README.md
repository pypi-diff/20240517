# Comparing `tmp/contact_user_external_local-0.0.4.tar.gz` & `tmp/contact_user_external_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_user_external_local-0.0.4.tar", last modified: Mon May 13 11:35:09 2024, max compression
+gzip compressed data, was "contact_user_external_local-0.0.5.tar", last modified: Fri May 17 15:00:40 2024, max compression
```

## Comparing `contact_user_external_local-0.0.4.tar` & `contact_user_external_local-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.534534 contact_user_external_local-0.0.5/contact_user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/contact_user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/setup.py
```

### Comparing `contact_user_external_local-0.0.4/PKG-INFO` & `contact_user_external_local-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local.py` & `contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
                                 default_id_column_name=default_id_column_name,
                                 default_table_name=default_table_name, default_view_table_name=default_view_table_name,
                                 is_test_data=is_test_data)
         self.user_externals = UserExternalsLocal(is_test_data=is_test_data)
         self.system_id = system_id
 
     def insert_contact_and_link_to_existing_or_new_user_external(
+            # TODO change dict -> dict[Contact]
+            # TODO change str -> EmailAddress
             self, contact_dict: dict, contact_email_address: str,
             contact_id: int, system_id: int = None, user_external_dict: dict = None) -> int or None:
         """
         Insert contact and link to existing or new user_external
         :param contact_dict: contact dict
         :param contact_id: contact id
         :param contact_email_address: contact email address
@@ -61,14 +63,15 @@
             # oauth_token = user_external_dict.get("oauth_token")
             # oauth_token_secret = user_external_dict.get("oauth_token_secret")
             # oauth_callback_confirmed = user_external_dict.get("oauth_callback_confirmed")
             # environment_id_old = user_external_dict.get("environment_id_old")
 
         user_external_id = self.user_externals.select_one_value_by_where(
             select_clause_value="user_external_id", where="username=%s AND system_id=%s",
+            # TODO allow to send to order_by also order_by_array with two items "start_timestamp" and DESC enum- This way we can move to other non SQL databases
             params=(contact_email_address, system_id), order_by="start_timestamp DESC")
 
         if not user_external_id:
             if not access_token:
                 logger.warning(exception_message="access_token is None")
                 logger.end(object={"contact_user_external_id": None})
                 return None
@@ -92,14 +95,15 @@
             contact_user_external_id = self.insert_mapping(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                 entity_id1=contact_id, entity_id2=user_external_id,
                 ignore_duplicate=True)
         else:
             # link to existing user_external
             logger.info(log_message="user_external_id is not None, linking to existing user_external")
+            # TODO contact_user_external_mapping_result_tuple
             mapping_tuple = self.select_multi_mapping_tuple_by_id(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                 entity_id1=contact_id, entity_id2=user_external_id)
             if not mapping_tuple:
                 logger.info(log_message="mapping_tuple is None, creating new mapping")
                 contact_user_external_id = self.insert_mapping(
                     entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
```

### Comparing `contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local_constants.py` & `contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact_user_external_local-0.0.4/contact_user_external_local.egg-info/PKG-INFO` & `contact_user_external_local-0.0.5/contact_user_external_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.4/setup.py` & `contact_user_external_local-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.4',  # https://pypi.org/project/contact-user-external-local/
+    version='0.0.5',  # https://pypi.org/project/contact-user-external-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-user-external-local Python",
     long_description="PyPI Package for Circles contact-user-external-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     package_dir={package_dir: f'{package_dir}/src'},
```

