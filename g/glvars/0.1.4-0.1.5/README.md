# Comparing `tmp/glvars-0.1.4.tar.gz` & `tmp/glvars-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glvars-0.1.4.tar", max compression
+gzip compressed data, was "glvars-0.1.5.tar", max compression
```

## Comparing `glvars-0.1.4.tar` & `glvars-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2022-09-08 11:17:22.572666 glvars-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2022-09-08 11:30:01.517734 glvars-0.1.4/glvars/__init__.py
--rw-r--r--   0        0        0      901 2022-09-11 22:18:35.818862 glvars-0.1.4/glvars/config.py
--rw-r--r--   0        0        0      793 2022-09-14 21:38:54.626740 glvars-0.1.4/glvars/main.py
--rw-r--r--   0        0        0     1042 2022-09-11 22:18:53.270341 glvars-0.1.4/glvars/schemas.py
--rw-r--r--   0        0        0     3380 2022-09-19 17:58:12.684763 glvars-0.1.4/glvars/synchronizer.py
--rw-r--r--   0        0        0      613 2023-01-16 21:46:33.728247 glvars-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 glvars-0.1.4/setup.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 glvars-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-08 11:17:22.572666 glvars-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2022-09-08 11:30:01.517734 glvars-0.1.5/glvars/__init__.py
+-rw-r--r--   0        0        0      901 2022-09-11 22:18:35.818862 glvars-0.1.5/glvars/config.py
+-rw-r--r--   0        0        0      793 2022-09-14 21:38:54.626740 glvars-0.1.5/glvars/main.py
+-rw-r--r--   0        0        0     1035 2024-05-17 10:40:47.966179 glvars-0.1.5/glvars/schemas.py
+-rw-r--r--   0        0        0     3380 2022-09-19 17:58:12.684763 glvars-0.1.5/glvars/synchronizer.py
+-rw-r--r--   0        0        0      615 2024-05-17 10:55:08.720486 glvars-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 glvars-0.1.5/PKG-INFO
```

### Comparing `glvars-0.1.4/LICENSE` & `glvars-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glvars-0.1.4/glvars/config.py` & `glvars-0.1.5/glvars/config.py`

 * *Files identical despite different names*

### Comparing `glvars-0.1.4/glvars/main.py` & `glvars-0.1.5/glvars/main.py`

 * *Files identical despite different names*

### Comparing `glvars-0.1.4/glvars/schemas.py` & `glvars-0.1.5/glvars/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     value: str
     variable_type: Optional[VariableType] = None
     protected: Optional[bool] = None
     masked: Optional[bool] = None
     environment_scope: Optional[str] = None
 
     class Config:
-        orm_mode = True
+        from_attributes = True
 
 
 class GlVarsConfig(BaseModel):
     gitlab_url: str = Field(default="", alias="gitlab-url")
     gitlab_private_token: str = Field(alias="gitlab-private-token")
     gitlab_project_id: str = Field(alias="gitlab-project-id")
     variables: Union[list[Variable], dict[str, str]]
 
     class Config:
-        allow_population_by_field_name = True
+        populate_by_name = True
 
     def get_variables(self) -> list[Variable]:
         if isinstance(self.variables, list):
             return self.variables
         return [Variable(key=key, value=value) for key, value in self.variables.items()]
```

### Comparing `glvars-0.1.4/glvars/synchronizer.py` & `glvars-0.1.5/glvars/synchronizer.py`

 * *Files identical despite different names*

### Comparing `glvars-0.1.4/pyproject.toml` & `glvars-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "glvars"
-version = "0.1.4"
+version = "0.1.5"
 description = "CLI utility for managing variables in Gitlab"
 authors = ["Alexey Tylindus <a.tylindus@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-gitlab = "^3.9"
-pydantic = "^1"
+pydantic = "^2"
 PyYAML = "^6.0"
 typer = {version = ">=0.6.1", extras = ["all"]}
+python-gitlab = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 icecream = "^2.1.3"
 isort = "^5.10.1"
 termcolor = "^1.1.0"
 wemake-python-styleguide = "^0.16.1"
```

### Comparing `glvars-0.1.4/PKG-INFO` & `glvars-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: glvars
-Version: 0.1.4
+Version: 0.1.5
 Summary: CLI utility for managing variables in Gitlab
 License: MIT
 Author: Alexey Tylindus
 Author-email: a.tylindus@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: pydantic (>=1,<2)
-Requires-Dist: python-gitlab (>=3.9,<4.0)
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: python-gitlab (>=4.5.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.6.1)
```

