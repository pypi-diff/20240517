# Comparing `tmp/horizon-hwm-store-0.1.4.tar.gz` & `tmp/horizon-hwm-store-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizon-hwm-store-0.1.4.tar", last modified: Wed Feb 14 08:33:19 2024, max compression
+gzip compressed data, was "horizon-hwm-store-0.1.5.tar", last modified: Wed Mar 27 15:05:07 2024, max compression
```

## Comparing `horizon-hwm-store-0.1.4.tar` & `horizon-hwm-store-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 08:33:19.036239 horizon-hwm-store-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-14 08:33:19.036239 horizon-hwm-store-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 08:33:19.036239 horizon-hwm-store-0.1.4/horizon_hwm_store/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/horizon_hwm_store/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/horizon_hwm_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/horizon_hwm_store/horizon_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/horizon_hwm_store/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/horizon_hwm_store/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 08:33:19.036239 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-14 08:33:19.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 08:33:18.000000 horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-14 08:33:19.040239 horizon-hwm-store-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-02-14 08:33:01.000000 horizon-hwm-store-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:07.419757 horizon-hwm-store-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-27 15:05:07.419757 horizon-hwm-store-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:07.419757 horizon-hwm-store-0.1.5/horizon_hwm_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/horizon_hwm_store/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/horizon_hwm_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/horizon_hwm_store/horizon_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/horizon_hwm_store/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/horizon_hwm_store/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:07.419757 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-27 15:05:07.000000 horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-27 15:05:07.423757 horizon-hwm-store-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-27 15:04:42.000000 horizon-hwm-store-0.1.5/setup.py
```

### Comparing `horizon-hwm-store-0.1.4/LICENSE.txt` & `horizon-hwm-store-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `horizon-hwm-store-0.1.4/horizon_hwm_store/horizon_hwm_store.py` & `horizon-hwm-store-0.1.5/horizon_hwm_store/horizon_hwm_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,24 @@
 from horizon.client.sync import HorizonClientSync, RetryConfig, TimeoutConfig
 from horizon.commons.schemas.v1 import (
     HWMCreateRequestV1,
     HWMPaginateQueryV1,
     HWMUpdateRequestV1,
     NamespacePaginateQueryV1,
 )
-from pydantic import Field, PrivateAttr
+
+try:
+    from pydantic.v1 import AnyHttpUrl, Field, PrivateAttr, validator
+except ImportError:
+    from pydantic import (  # type: ignore[no-redef, assignment]
+        AnyHttpUrl,
+        Field,
+        PrivateAttr,
+        validator,
+    )
 
 
 @register_hwm_store_class("horizon")
 class HorizonHWMStore(BaseHWMStore):
     """
     Fetch/store High Water Mark (HWM) values from the Horizon REST API.
 
@@ -132,59 +141,60 @@
                 df = reader.run()
                 writer.run(df)
 
             # will create/update HWM value in Horizon
 
     """
 
-    api_url: str
+    api_url: AnyHttpUrl
     auth: LoginPassword
     namespace: str
     retry: RetryConfig = Field(default_factory=RetryConfig)
     timeout: TimeoutConfig = Field(default_factory=TimeoutConfig)
-    _client: HorizonClientSync = PrivateAttr()
-    _namespace_id: Optional[int] = PrivateAttr()
+    _client: Optional[HorizonClientSync] = PrivateAttr(default=None)
+    _namespace_id: Optional[int] = PrivateAttr(default=None)
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self._client = HorizonClientSync(  # noqa: WPS601
-            base_url=self.api_url,
-            auth=self.auth,
-            retry=self.retry,
-            timeout=self.timeout,
-        )
-        self._namespace_id = None  # noqa: WPS601
+    @property
+    def client(self) -> HorizonClientSync:
+        if not self._client:
+            self._client = HorizonClientSync(  # noqa: WPS601
+                base_url=self.api_url,
+                auth=self.auth,
+                retry=self.retry,
+                timeout=self.timeout,
+            )
+        return self._client
 
     def get_hwm(self, name: str) -> Optional[HWM]:
         namespace_id = self._get_namespace_id()
         hwm_id = self._get_hwm_id(namespace_id, name)
         if hwm_id is None:
             return None
 
-        hwm = self._client.get_hwm(hwm_id)
+        hwm = self.client.get_hwm(hwm_id)
         hwm_data = hwm.dict(exclude={"id", "namespace_id", "changed_by", "changed_at"})
         hwm_data["modified_time"] = hwm.changed_at
         return HWMTypeRegistry.parse(hwm_data)
 
     def set_hwm(self, hwm: HWM) -> str:
         namespace_id = self._get_namespace_id()
 
         hwm_dict = hwm.serialize()
         hwm_dict["namespace_id"] = namespace_id
 
         hwm_id = self._get_hwm_id(namespace_id, hwm.name)  # type: ignore
         if hwm_id is None:
             create_request = HWMCreateRequestV1.parse_obj(hwm_dict)
-            response = self._client.create_hwm(create_request)
+            response = self.client.create_hwm(create_request)
         else:
             update_request = HWMUpdateRequestV1.parse_obj(hwm_dict)
-            response = self._client.update_hwm(hwm_id, update_request)
+            response = self.client.update_hwm(hwm_id, update_request)
 
         # TODO: update response string after implementing UI
-        return f"{self._client.base_url}/v1/hwm/{response.id}"
+        return f"{self.client.base_url}/v1/hwm/{response.id}"
 
     def check(self) -> HorizonHWMStore:
         """
         Perform a health check by making a request to the Horizon server.
 
         This method calls the 'whoami' endpoint of the Horizon client. It's used to verify
         if the backend is accessible and if the provided credentials are correct. The method
@@ -195,18 +205,38 @@
 
         Returns
         -------
         HorizonHWMStore
             Self
 
         """
-        self._client.whoami()
+        self.client.whoami()
         self._get_namespace_id()
         return self
 
+    # LoginPassword, RetryConfig and TimeoutConfig can be inherited from Pydantic v2 BaseModel
+    # which is detected by Pydantic v1 as arbitrary type. So we need to parse them manually.
+    @validator("auth", pre=True)
+    def _check_auth(cls, value: LoginPassword):
+        if not isinstance(value, LoginPassword):
+            return LoginPassword.parse_obj(value)
+        return value
+
+    @validator("retry", pre=True)
+    def _check_retry(cls, value: RetryConfig):
+        if not isinstance(value, RetryConfig):
+            return RetryConfig.parse_obj(value)
+        return value
+
+    @validator("timeout", pre=True)
+    def _check_timeout(cls, value: TimeoutConfig):
+        if not isinstance(value, TimeoutConfig):
+            return TimeoutConfig.parse_obj(value)
+        return value
+
     def _get_namespace_id(self) -> int:
         """
         Fetch the ID of the namespace. Raises an exception if the namespace doesn't exist.
 
         Returns
         -------
         int
@@ -216,15 +246,15 @@
         ------
         RuntimeError
             If the namespace does not exist.
         """
         if self._namespace_id is not None:
             return self._namespace_id
 
-        namespaces = self._client.paginate_namespaces(NamespacePaginateQueryV1(name=self.namespace)).items
+        namespaces = self.client.paginate_namespaces(NamespacePaginateQueryV1(name=self.namespace)).items
         if not namespaces:
             raise RuntimeError(f"Namespace {self.namespace!r} not found. Please create it before using.")
 
         self._namespace_id = namespaces[0].id  # noqa: WPS601
         return self._namespace_id
 
     def _get_hwm_id(self, namespace_id: int, hwm_name: str) -> Optional[int]:
@@ -240,9 +270,9 @@
 
         Returns
         -------
         Optional[int]
             The ID of the HWM, or None if it does not exist.
         """
         hwm_query = HWMPaginateQueryV1(namespace_id=namespace_id, name=hwm_name)
-        hwms = self._client.paginate_hwm(hwm_query).items
+        hwms = self.client.paginate_hwm(hwm_query).items
         return hwms[-1].id if hwms else None
```

### Comparing `horizon-hwm-store-0.1.4/horizon_hwm_store.egg-info/SOURCES.txt` & `horizon-hwm-store-0.1.5/horizon_hwm_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horizon-hwm-store-0.1.4/pyproject.toml` & `horizon-hwm-store-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 line-length = 120
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''(\.eggs|\.git|\.mypy_cache|\.tox|\.venv|_build|buck-out|build|dist)'''
 
 [tool.mypy]
 plugins = 'pydantic.mypy'
-python_version = 3.7
+python_version = 3.8
 follow_imports = "silent"
 ignore_missing_imports = true
 pretty = true
 show_error_codes = true
 strict_optional = true
 
 [tool.towncrier]
```

### Comparing `horizon-hwm-store-0.1.4/setup.cfg` & `horizon-hwm-store-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 	S608,
 	E402,
 	RST399,
 	F821,
 	WPS432,
 	WPS615,
 	RST213,
-	RST307
+	RST307,
+	N805
 per-file-ignores = 
 	__init__.py:
 	F401,
 	WPS410,
 	test*:
 	S101,
 	WPS122,
```

### Comparing `horizon-hwm-store-0.1.4/setup.py` & `horizon-hwm-store-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     name="horizon-hwm-store",
     version=get_version(),
     author="DataOps.ETL Team",
     author_email="onetools@mts.ru",
     description="onETL Plugin for Horizon store",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    license="Apache License 2.0",
+    license="Apache-2.0",
     license_files=("LICENSE.txt",),
     url="https://github.com/MobileTeleSystems/horizon-hwm-store",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

