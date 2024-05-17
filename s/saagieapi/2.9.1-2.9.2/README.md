# Comparing `tmp/saagieapi-2.9.1.tar.gz` & `tmp/saagieapi-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.9.1.tar", max compression
+gzip compressed data, was "saagieapi-2.9.2.tar", max compression
```

## Comparing `saagieapi-2.9.1.tar` & `saagieapi-2.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-10-31 12:57:59.589901 saagieapi-2.9.1/LICENSE
--rw-r--r--   0        0        0     1990 2023-10-31 12:57:59.589901 saagieapi-2.9.1/README.md
--rw-r--r--   0        0        0     1611 2023-10-31 12:58:26.810024 saagieapi-2.9.1/pyproject.toml
--rw-r--r--   0        0        0      583 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    56623 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/apps/apps.py
--rw-r--r--   0        0        0    10408 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0    11992 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    55011 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     4677 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       49 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/groups/__init__.py
--rw-r--r--   0        0        0    16989 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/groups/groups.py
--rw-r--r--   0        0        0       43 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0    14243 2023-10-31 12:57:59.589901 saagieapi-2.9.1/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    72087 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      222 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0    12990 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     3540 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    73181 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/profiles/__init__.py
--rw-r--r--   0        0        0     5869 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/profiles/profiles.py
--rw-r--r--   0        0        0       55 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     3176 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    29905 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    22585 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    30963 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0    13170 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/storages/storages.py
--rw-r--r--   0        0        0       46 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/users/__init__.py
--rw-r--r--   0        0        0    13001 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/users/users.py
--rw-r--r--   0        0        0        0 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1758 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3666 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0     2364 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/request_client.py
--rw-r--r--   0        0        0       54 2023-10-31 12:57:59.593901 saagieapi-2.9.1/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 saagieapi-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-13 16:49:26.764720 saagieapi-2.9.2/LICENSE
+-rw-r--r--   0        0        0     1990 2023-11-13 16:49:26.764720 saagieapi-2.9.2/README.md
+-rw-r--r--   0        0        0     1640 2023-11-13 16:49:50.048634 saagieapi-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0      583 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    56623 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0    10408 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0    11992 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    55011 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     4690 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       49 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/groups/__init__.py
+-rw-r--r--   0        0        0    16989 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/groups/groups.py
+-rw-r--r--   0        0        0       43 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0    14243 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    72097 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      222 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0    12990 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     3540 2023-11-13 16:49:26.764720 saagieapi-2.9.2/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    73181 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/profiles/__init__.py
+-rw-r--r--   0        0        0     5869 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/profiles/profiles.py
+-rw-r--r--   0        0        0       55 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     3176 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    29905 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    22585 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    30963 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0    13170 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0       46 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/users/__init__.py
+-rw-r--r--   0        0        0    13001 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/users/users.py
+-rw-r--r--   0        0        0        0 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3666 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0     2364 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/request_client.py
+-rw-r--r--   0        0        0       54 2023-11-13 16:49:26.768720 saagieapi-2.9.2/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 saagieapi-2.9.2/PKG-INFO
```

### Comparing `saagieapi-2.9.1/LICENSE` & `saagieapi-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/README.md` & `saagieapi-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/pyproject.toml` & `saagieapi-2.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.9.1"
+version = "2.9.2"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
@@ -21,14 +21,15 @@
 python-semantic-release = "7.28.1"
 pytest = "^7.4.0"
 pylint = "^2.17.5"
 isort = "^5.12.0"
 black = "^23.7.0"
 pre-commit = "^3.3.3"
 sphinx-rtd-theme = "^1.3.0"
+sphinx-book-theme = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `saagieapi-2.9.1/saagieapi/__init__.py` & `saagieapi-2.9.2/saagieapi/__init__.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/apps/apps.py` & `saagieapi-2.9.2/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/apps/gql_queries.py` & `saagieapi-2.9.2/saagieapi/apps/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.9.2/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.9.2/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/env_vars/env_vars.py` & `saagieapi-2.9.2/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.9.2/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/gql_queries.py` & `saagieapi-2.9.2/saagieapi/gql_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # | .__/|_|\__,_|\__|_|  \___/|_|  |_| |_| |_|
 # |_|
 
 GQL_GET_PLATFORM_INFO = """
 {
     platform{
         id
+        name
         counts{
             projects
             jobs
             apps
             pipelines
         }
     }
```

### Comparing `saagieapi-2.9.1/saagieapi/groups/groups.py` & `saagieapi-2.9.2/saagieapi/groups/groups.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/jobs/gql_queries.py` & `saagieapi-2.9.2/saagieapi/jobs/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/jobs/jobs.py` & `saagieapi-2.9.2/saagieapi/jobs/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1873,15 +1873,15 @@
         Returns
         -------
         dict
             Dict of number of job instances before the given date
 
         Examples
         --------
-        >>> saagie_api.jobs.count_instances_by_date(job_id=job_id, date_before="2023-06-01T00:00:00+01:00")
+        >>> saagie_api.jobs.count_deletable_instances_by_date(job_id=job_id, date_before="2023-06-01T00:00:00+01:00")
         {
             'countJobInstancesByDate': 3
         }
         """
         # need to check the date is in this format : 2023-02-01T00:00:00+01:00
         # if not, it will raise an error and stop the call
         try:
@@ -1925,15 +1925,15 @@
             variable_values={
                 "jobId": job_id,
                 "targetPlatformId": target_platform_id,
                 "targetProjectId": target_project_id,
             },
         )
 
-    def generate_description_by_AI(self, job_id: str):
+    def generate_description_by_ai(self, job_id: str):
         """Generate a description for a job using AI.
         Be careful, by calling this function the code contained in the job package will be sent to OpenAI
         and thus will not be secured anymore by Saagie DataOps Platform.
         Otherwise, the function returns an error if the description is already the one generated by AI.
 
         Parameters
         ----------
@@ -1943,15 +1943,15 @@
         Returns
         -------
         dict
             Dict of the generated description
 
         Examples
         --------
-        >>> saagie_api.jobs.generate_description_by_AI(job_id=job_id)
+        >>> saagie_api.jobs.generate_description_by_ai(job_id=job_id)
         {
             'editJobWithAiGeneratedDescription': {
                 'id': 'bfa25e4a-1796-4ebb-8c3d-138f74146973',
                 'description': 'The purpose of this code is to display the message "Hello World" on the screen.',
                 'aiDescriptionVersionNumber': 1
             }
         }
```

### Comparing `saagieapi-2.9.1/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.9.2/saagieapi/pipelines/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.9.2/saagieapi/pipelines/graph_pipeline.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/pipelines/pipelines.py` & `saagieapi-2.9.2/saagieapi/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/profiles/profiles.py` & `saagieapi-2.9.2/saagieapi/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/projects/gql_queries.py` & `saagieapi-2.9.2/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/projects/projects.py` & `saagieapi-2.9.2/saagieapi/projects/projects.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/repositories/gql_queries.py` & `saagieapi-2.9.2/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/repositories/repositories.py` & `saagieapi-2.9.2/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/saagie_api.py` & `saagieapi-2.9.2/saagieapi/saagie_api.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/storages/gql_queries.py` & `saagieapi-2.9.2/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/storages/storages.py` & `saagieapi-2.9.2/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/users/users.py` & `saagieapi-2.9.2/saagieapi/users/users.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/utils/bearer_auth.py` & `saagieapi-2.9.2/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/utils/folder_functions.py` & `saagieapi-2.9.2/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/utils/gql_client.py` & `saagieapi-2.9.2/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/saagieapi/utils/request_client.py` & `saagieapi-2.9.2/saagieapi/utils/request_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.9.1/PKG-INFO` & `saagieapi-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.9.1
+Version: 2.9.2
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=1.0.1,<2.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: gql (>=3.0.0,<4.0.0)
 Requires-Dist: pytz (>=2021.1)
 Requires-Dist: requests (==2.29.0)
 Requires-Dist: requests_toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: rich (>=12.3.0,<13.0.0)
```

