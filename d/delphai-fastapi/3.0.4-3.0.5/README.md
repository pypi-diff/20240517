# Comparing `tmp/delphai_fastapi-3.0.4.tar.gz` & `tmp/delphai_fastapi-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-3.0.4.tar", max compression
+gzip compressed data, was "delphai_fastapi-3.0.5.tar", max compression
```

## Comparing `delphai_fastapi-3.0.4.tar` & `delphai_fastapi-3.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       86 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/app.py
--rw-r--r--   0        0        0     5713 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     5582 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0        0 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/funding_rounds/__init__.py
--rw-r--r--   0        0        0     1623 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/funding_rounds/models.py
--rw-r--r--   0        0        0     1314 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/instrumentation.py
--rw-r--r--   0        0        0        0 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/job_posts/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/job_posts/models.py
--rw-r--r--   0        0        0     1386 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/models.py
--rw-r--r--   0        0        0        0 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/news_articles/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/news_articles/models.py
--rw-r--r--   0        0        0        0 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/projects/__init__.py
--rw-r--r--   0        0        0     1523 2024-05-15 09:39:40.360150 delphai_fastapi-3.0.4/delphai_fastapi/projects/models.py
--rw-r--r--   0        0        0      405 2024-05-15 09:39:40.364150 delphai_fastapi-3.0.4/delphai_fastapi/server.py
--rw-r--r--   0        0        0     2909 2024-05-15 09:39:40.364150 delphai_fastapi-3.0.4/delphai_fastapi/types.py
--rw-r--r--   0        0        0      590 2024-05-15 09:39:40.364150 delphai_fastapi-3.0.4/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     5713 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     5582 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/funding_rounds/__init__.py
+-rw-r--r--   0        0        0     1623 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/funding_rounds/models.py
+-rw-r--r--   0        0        0     1314 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0     3124 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1386 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/projects/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/projects/models.py
+-rw-r--r--   0        0        0      405 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/server.py
+-rw-r--r--   0        0        0     2909 2024-05-17 09:44:04.016368 delphai_fastapi-3.0.5/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      590 2024-05-17 09:44:04.020368 delphai_fastapi-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.5/PKG-INFO
```

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/app.py` & `delphai_fastapi-3.0.5/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/auth.py` & `delphai_fastapi-3.0.5/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/companies/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/funding_rounds/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/funding_rounds/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/instrumentation.py` & `delphai_fastapi-3.0.5/delphai_fastapi/instrumentation.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/job_posts/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/job_posts/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     classifications: Optional[List[JobClassification]] = None
 
 
 class AddJobPost(BaseJobPost):
     company_name: str = Field(
         ..., description="Name of the company posting the job post"
     )
+    added_by: str = Field(
+        ..., description="ID of the process or person this job post was added by"
+    )
     company_id: ObjectId = Field(None, description="Internal company ID")
     original_description: Optional[str] = Field(
         None, description="Description in original language"
     )
     translated_description: Optional[str] = Field(
         None,
         description="Translated description in english. Only necessary if original language is not english",
```

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/news_articles/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/news_articles/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/projects/models.py` & `delphai_fastapi-3.0.5/delphai_fastapi/projects/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/delphai_fastapi/types.py` & `delphai_fastapi-3.0.5/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.4/pyproject.toml` & `delphai_fastapi-3.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-fastapi"
-version = "3.0.4"
+version = "3.0.5"
 description = "Package for fastAPI models"
 authors = ["Berinike Tech <berinike@delphai.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0"
 pymongo = ">3"
```

### Comparing `delphai_fastapi-3.0.4/PKG-INFO` & `delphai_fastapi-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 3.0.4
+Version: 3.0.5
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

