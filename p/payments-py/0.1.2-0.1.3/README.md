# Comparing `tmp/payments_py-0.1.2.tar.gz` & `tmp/payments_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payments_py-0.1.2.tar", max compression
+gzip compressed data, was "payments_py-0.1.3.tar", max compression
```

## Comparing `payments_py-0.1.2.tar` & `payments_py-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-08 09:33:07.825491 payments_py-0.1.2/LICENSE
--rw-r--r--   0        0        0      584 2024-04-08 09:33:07.825491 payments_py-0.1.2/README.md
--rw-r--r--   0        0        0      159 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/environments.py
--rw-r--r--   0        0        0    14796 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/payments.py
--rw-r--r--   0        0        0      229 2024-04-08 09:33:07.829491 payments_py-0.1.2/payments_py/utils.py
--rw-r--r--   0        0        0      496 2024-04-08 09:33:07.829491 payments_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 payments_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 14:22:54.811456 payments_py-0.1.3/LICENSE
+-rw-r--r--   0        0        0      584 2024-05-06 14:22:54.811456 payments_py-0.1.3/README.md
+-rw-r--r--   0        0        0      159 2024-05-06 14:22:54.815456 payments_py-0.1.3/payments_py/__init__.py
+-rw-r--r--   0        0        0     1081 2024-05-06 14:22:54.815456 payments_py-0.1.3/payments_py/environments.py
+-rw-r--r--   0        0        0    15673 2024-05-06 14:22:54.815456 payments_py-0.1.3/payments_py/payments.py
+-rw-r--r--   0        0        0      229 2024-05-06 14:22:54.815456 payments_py-0.1.3/payments_py/utils.py
+-rw-r--r--   0        0        0      496 2024-05-06 14:22:54.815456 payments_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 payments_py-0.1.3/PKG-INFO
```

### Comparing `payments_py-0.1.2/LICENSE` & `payments_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.2/README.md` & `payments_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.2/payments_py/environments.py` & `payments_py-0.1.3/payments_py/environments.py`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.2/payments_py/payments.py` & `payments_py-0.1.3/payments_py/payments.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,38 @@
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
         url = f"{self.environment.value['backend']}/api/v1/payments/file"
         response = requests.post(url, headers=headers, json=body)
         return response
 
+    def order_subscription(self, subscription_did: str, agreementId: Optional[str] = None):
+        """
+        Orders the subscription.
+
+        Args:
+            subscription_did (str): The DID of the subscription.
+            agreementId (str, optional): The agreement ID.
+
+        Returns:
+            Response: The response from the API call.
+        """
+        body = {
+            "sessionKey": self.session_key,
+            "subscriptionDid": subscription_did,
+            **{snake_to_camel(k): v for k, v in locals().items() if v is not None and k != 'self'}
+        }
+        headers = {
+            'Accept': 'application/json',
+            'Content-Type': 'application/json'
+        }
+        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/order"
+        response = requests.post(url, headers=headers, json=body)
+        return response
+
     def get_asset_ddo(self, did: str):
         """
         Gets the asset DDO.
 
         Args:
             did (str): The DID of the asset.
```

### Comparing `payments_py-0.1.2/PKG-INFO` & `payments_py-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payments-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: enrique
 Author-email: enrique@nevermined.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

