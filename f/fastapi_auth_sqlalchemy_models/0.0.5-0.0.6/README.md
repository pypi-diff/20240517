# Comparing `tmp/fastapi_auth_sqlalchemy_models-0.0.5.tar.gz` & `tmp/fastapi_auth_sqlalchemy_models-0.0.6.tar.gz`

## Comparing `fastapi_auth_sqlalchemy_models-0.0.5.tar` & `fastapi_auth_sqlalchemy_models-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/fastapi_auth_sqlalchemy_models/__init__.py
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/fastapi_auth_sqlalchemy_models/models.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/fastapi_auth_sqlalchemy_models/repositories.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/LICENSE
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/fastapi_auth_sqlalchemy_models/__init__.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/fastapi_auth_sqlalchemy_models/models.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/fastapi_auth_sqlalchemy_models/repositories.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/LICENSE
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastapi_auth_sqlalchemy_models-0.0.6/PKG-INFO
```

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/.github/workflows/workflow.yml` & `fastapi_auth_sqlalchemy_models-0.0.6/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/fastapi_auth_sqlalchemy_models/models.py` & `fastapi_auth_sqlalchemy_models-0.0.6/fastapi_auth_sqlalchemy_models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     async def save(self, created: bool = False, **kwargs) -> None:
         session: AsyncSession = kwargs.pop('session', None)
         if not session:
             raise ValueError("Session cannot be None")
         await main_signal.emit_before_save(instance=self, session=session)
         session.add(self)
         await session.flush()
+        await session.refresh(self)
         await session.commit()
         return await main_signal.emit_after_save(instance=self, created=created, session=session)
 
     @classmethod
     async def create(cls, **kwargs) -> object:
         session: AsyncSession = kwargs.pop('session', None)
         if session is None:
@@ -54,14 +55,15 @@
         if not session:
             raise ValueError("Session cannot be None")
         if not self.key:
             self.key = self.generate_key()
         await main_signal.emit_before_save(instance=self, session=session)
         session.add(self)
         await session.flush()
+        await session.refresh(self)
         await session.commit()
         return await main_signal.emit_after_save(instance=self, created=created, session=session)
 
     @classmethod
     async def create(cls, **kwargs: Any) -> object:
         session: AsyncSession = kwargs.pop('session', None)
         if session is None:
```

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/fastapi_auth_sqlalchemy_models/repositories.py` & `fastapi_auth_sqlalchemy_models-0.0.6/fastapi_auth_sqlalchemy_models/repositories.py`

 * *Files identical despite different names*

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/LICENSE` & `fastapi_auth_sqlalchemy_models-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/pyproject.toml` & `fastapi_auth_sqlalchemy_models-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_auth_sqlalchemy_models-0.0.5/PKG-INFO` & `fastapi_auth_sqlalchemy_models-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastapi_auth_sqlalchemy_models
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sqlalchemy repositories and models for fastapi-auth library
 Author: zayycev22
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

