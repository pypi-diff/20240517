# Comparing `tmp/deker_server_adapters-1.0.5.tar.gz` & `tmp/deker_server_adapters-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker_server_adapters-1.0.5.tar", max compression
+gzip compressed data, was "deker_server_adapters-1.0.6.tar", max compression
```

## Comparing `deker_server_adapters-1.0.5.tar` & `deker_server_adapters-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/LICENSE
--rw-r--r--   0        0        0      356 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/README.md
--rw-r--r--   0        0        0       45 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/__init__.py
--rw-r--r--   0        0        0     2716 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/array_adapter.py
--rw-r--r--   0        0        0    16842 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/base.py
--rw-r--r--   0        0        0     4475 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/collection_adapter.py
--rw-r--r--   0        0        0      582 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/consts.py
--rw-r--r--   0        0        0     2743 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/errors.py
--rw-r--r--   0        0        0     7087 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/factory.py
--rw-r--r--   0        0        0     4673 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/hash_ring.py
--rw-r--r--   0        0        0     2690 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/httpx_client.py
--rw-r--r--   0        0        0     3802 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/utils.py
--rw-r--r--   0        0        0      895 2024-04-16 13:47:25.277088 deker_server_adapters-1.0.5/deker_server_adapters/varray_adapter.py
--rw-r--r--   0        0        0     7094 2024-04-16 13:47:33.585137 deker_server_adapters-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 deker_server_adapters-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/LICENSE
+-rw-r--r--   0        0        0      356 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/README.md
+-rw-r--r--   0        0        0       45 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/__init__.py
+-rw-r--r--   0        0        0     2716 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/array_adapter.py
+-rw-r--r--   0        0        0    17145 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/base.py
+-rw-r--r--   0        0        0     4475 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/collection_adapter.py
+-rw-r--r--   0        0        0      582 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/consts.py
+-rw-r--r--   0        0        0     2743 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/errors.py
+-rw-r--r--   0        0        0     7087 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/factory.py
+-rw-r--r--   0        0        0     4673 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/hash_ring.py
+-rw-r--r--   0        0        0     2690 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/httpx_client.py
+-rw-r--r--   0        0        0     3802 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/utils.py
+-rw-r--r--   0        0        0      895 2024-05-17 14:04:16.890564 deker_server_adapters-1.0.6/deker_server_adapters/varray_adapter.py
+-rw-r--r--   0        0        0     7094 2024-05-17 14:04:25.774602 deker_server_adapters-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 deker_server_adapters-1.0.6/PKG-INFO
```

### Comparing `deker_server_adapters-1.0.5/LICENSE` & `deker_server_adapters-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/array_adapter.py` & `deker_server_adapters-1.0.6/deker_server_adapters/array_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/base.py` & `deker_server_adapters-1.0.6/deker_server_adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,30 +126,32 @@
         :param node: Node to merge with
         """
         return f"{node.rstrip('/')}{self.collection_path.path}"
 
     def create(self, array: Union[dict, "BaseArray"]) -> BaseArray:
         """Create array on server.
 
-        :param array: Array instance
-        :return:
+        :param array: Array instance or dict
         """
+        if isinstance(array, dict):
+            primary_attributes = array["primary_attributes"]
+            custom_attributes = array["custom_attributes"]
+            id_ = array.get("id_") or (self.client.cluster_mode and get_id() or None)
+            array["id_"] = id_
+        else:
+            primary_attributes = array.primary_attributes
+            custom_attributes = array.custom_attributes
+            id_ = array.id
+
         kwargs = {
-            "primary_attributes": convert_datetime_attrs_to_iso(
-                array["primary_attributes"],
-            ),
-            "custom_attributes": convert_datetime_attrs_to_iso(
-                array["custom_attributes"],
-            ),
+            "primary_attributes": convert_datetime_attrs_to_iso(primary_attributes),
+            "custom_attributes": convert_datetime_attrs_to_iso(custom_attributes),
+            "id_": id_,
         }
 
-        if isinstance(array, dict):
-            kwargs["id_"] = array.get("id_") or (self.client.cluster_mode and get_id() or None)
-            array["id_"] = kwargs["id_"]
-
         path = self.collection_path.raw_url.rstrip("/")
 
         if self.type == ArrayType.array and self.client.cluster_mode:
             node_id = self.hash_ring.get_node(get_hash_key(array))
             node = self.get_host_url(node_id)
             path = self.__merge_node_and_collection_path(node)
 
@@ -158,30 +160,32 @@
             raise DekerServerError(response, "Couldn't create an array")
 
         try:
             data = response.json()
         except JSONDecodeError:
             raise DekerServerError(response, "Couldn't parse json")
 
-        instance_id = data.get("id")
-        if not instance_id:
-            raise DekerServerError(response, "Server response doesn't contain ID field")
-
-        kwargs = {
-            "collection": array["collection"],
-            "adapter": array["adapter"],
-            "id_": instance_id,
-            "primary_attributes": array["primary_attributes"],
-            "custom_attributes": array["custom_attributes"],
-        }
-
-        model = self.type.value
-        if model == VArray:
-            kwargs["array_adapter"] = array["array_adapter"]
-        return model(**kwargs)
+        if isinstance(array, dict):
+            instance_id = data.get("id")
+            if not instance_id:
+                raise DekerServerError(response, "Server response doesn't contain ID field")
+
+            kwargs = {
+                "collection": array["collection"],
+                "adapter": array["adapter"],
+                "id_": instance_id,
+                "primary_attributes": array["primary_attributes"],
+                "custom_attributes": array["custom_attributes"],
+            }
+
+            model = self.type.value
+            if model == VArray:
+                kwargs["array_adapter"] = array["array_adapter"]
+            return model(**kwargs)
+        return array
 
     def read_meta(self, array: "BaseArray") -> ArrayMeta:
         """Read metadata of (v)array.
 
         :param array: Instance of (v)array
         :return:
         """
```

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/collection_adapter.py` & `deker_server_adapters-1.0.6/deker_server_adapters/collection_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/consts.py` & `deker_server_adapters-1.0.6/deker_server_adapters/consts.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/errors.py` & `deker_server_adapters-1.0.6/deker_server_adapters/errors.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/factory.py` & `deker_server_adapters-1.0.6/deker_server_adapters/factory.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/hash_ring.py` & `deker_server_adapters-1.0.6/deker_server_adapters/hash_ring.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/httpx_client.py` & `deker_server_adapters-1.0.6/deker_server_adapters/httpx_client.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/utils.py` & `deker_server_adapters-1.0.6/deker_server_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/deker_server_adapters/varray_adapter.py` & `deker_server_adapters-1.0.6/deker_server_adapters/varray_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_server_adapters-1.0.5/pyproject.toml` & `deker_server_adapters-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.poetry]
 name = "deker_server_adapters"
-version = "1.0.5"
+version = "1.0.6"
 description = "Plugin with server adapters for Deker"
 authors = ["OpenWeather <info@openweathermap.org>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "deker_server_adapters"}]
 documentation = 'https://docs.deker.io/'
 homepage = 'https://deker.io/'
```

### Comparing `deker_server_adapters-1.0.5/PKG-INFO` & `deker_server_adapters-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker_server_adapters
-Version: 1.0.5
+Version: 1.0.6
 Summary: Plugin with server adapters for Deker
 Home-page: https://deker.io/
 License: GPL-3.0-only
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

