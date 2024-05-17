# Comparing `tmp/rov_db_access-0.1.8.tar.gz` & `tmp/rov_db_access-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-0.1.8.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.0.tar", max compression
```

## Comparing `rov_db_access-0.1.8.tar` & `rov_db_access-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,34 @@
--rw-r--r--   0        0        0      453 2024-05-15 19:14:44.176545 rov_db_access-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.8/README.md
--rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.8/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.8/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.8/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.8/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-0.1.8/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0     1115 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.8/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     7617 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/gis/models.py
--rw-r--r--   0        0        0    25385 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.8/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.8/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.8/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0     1522 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.8/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      587 2024-05-17 19:53:02.768503 rov_db_access-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-1.0.0/README.md
+-rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-1.0.0/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-1.0.0/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-1.0.0/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1233 2024-05-17 19:52:58.172569 rov_db_access-1.0.0/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.172569 rov_db_access-1.0.0/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-1.0.0/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0      939 2024-05-17 19:52:58.173574 rov_db_access-1.0.0/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.174567 rov_db_access-1.0.0/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     2032 2024-05-17 19:52:58.176075 rov_db_access-1.0.0/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-1.0.0/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     7617 2024-05-15 19:14:44.177669 rov_db_access-1.0.0/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       81 2024-05-17 19:52:58.176594 rov_db_access-1.0.0/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    35434 2024-05-17 19:52:58.177603 rov_db_access-1.0.0/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.178602 rov_db_access-1.0.0/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-17 19:52:58.178602 rov_db_access-1.0.0/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2368 2024-05-17 19:52:58.179605 rov_db_access-1.0.0/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.179605 rov_db_access-1.0.0/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9336 2024-05-17 19:52:58.180604 rov_db_access-1.0.0/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7363 2024-05-17 19:52:58.181603 rov_db_access-1.0.0/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.181603 rov_db_access-1.0.0/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-17 19:52:58.182603 rov_db_access-1.0.0/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     6062 2024-05-17 19:52:58.183605 rov_db_access-1.0.0/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6703 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-1.0.0/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-1.0.0/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     6053 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1157 2024-05-17 19:52:58.187649 rov_db_access-1.0.0/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.0/PKG-INFO
```

### Comparing `rov_db_access-0.1.8/rov_db_access/authentication/models.py` & `rov_db_access-1.0.0/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.8/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.0/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.8/rov_db_access/config/settings.py` & `rov_db_access-1.0.0/rov_db_access/config/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
 
-    access_token_expire_minutes: int
-    auth_algorithm: str
-    auth_secret_key: str
-
     aws_key: str
     aws_secret: str
 
     db_ine_url: str
 
     db_rov_geodata_database: str
     db_rov_geodata_host: str
@@ -32,21 +28,16 @@
 
     db_rov_sentinel_database: str
     db_rov_sentinel_host: str
     db_rov_sentinel_password: str
     db_rov_sentinel_port: str
     db_rov_sentinel_user: str
 
-    geoapify_api_key: str
-
-    geoserver_api_url: str
-
     gis_inference_bucket: str
     gis_inference_region: str
 
     run_results_bucket: str
 
     s3_region: str
 
-    sentinel_bucket: str
     sentinel_user: str
     sentinel_password: str
```

### Comparing `rov_db_access-0.1.8/rov_db_access/gis/models.py` & `rov_db_access-1.0.0/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.8/rov_db_access/gis/worker.py` & `rov_db_access-1.0.0/rov_db_access/gis/worker.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import hashlib
 from botocore.client import Config
 from botocore.exceptions import ClientError
 
 from rov_db_access.authentication.models import User
 from rov_db_access.utils.s3_utils import S3Client
 from rov_db_access.utils.utils import wkbelement_to_wkt
-from rov_db_access.config.db_utils import BaseWorker
+from rov_db_access.config.db_utils import init_db_engine
 from rov_db_access.config.settings import Settings
 from rov_db_access.sentinel.worker import is_valid_uuid
 from rov_db_access.gis.models import Process, Image, InferenceModel, Input, ResultsRaster, Run, ResultsRaw
 from sqlalchemy import select, and_, func
+from sqlalchemy.orm import Session
 
 settings = Settings()
 
 CreateProcessDict = TypedDict("CreateProcessDict", {
     "name": str,
     "inference_model_id": int,
     "area": float,
@@ -79,152 +80,227 @@
         return None
 
 
 def get_date(obj):
     return tuple(map(int, obj["date"].split("/")[::-1]))
 
 
-class GisWorker(BaseWorker):
+class GisWorker:
 
     def __init__(self) -> None:
-        super().__init__(
+        self.engine = init_db_engine(
             settings.db_rov_gis_user,
             settings.db_rov_gis_password,
             settings.db_rov_gis_host,
             settings.db_rov_gis_port,
             settings.db_rov_gis_database
         )
 
+    def copy_process(self, process_id, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(Process.id == process_id)
+                .limit(1)
+            )
+            process_to_copy = session.scalar(query)
+            if process_to_copy is None:
+                print(f'No process with id ${id} found!')
+                return {}
+            elif process_to_copy.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                process_type = process_to_copy.type
+                new_name = "Copy of " + process_to_copy.name
+                model_id: int = process_to_copy.inference_model_id
+                area: float = process_to_copy.area
+                cost_estimated: float = process_to_copy.cost_estimated
+                data: dict = process_to_copy.data
+                geom: str = wkbelement_to_wkt(process_to_copy.geom)
+                mask = wkbelement_to_wkt(process_to_copy.mask)
+                print(f'Process with id: {process_to_copy.id} found! type: {process_type}')
+
+                if process_type == 'on demand':
+                    images = []
+                    img_ids = []
+                    for run in process_to_copy.runs:
+                        if run.input is None:
+                            print(f'Process with corrupted Run {run.id} without Input data')
+                            return False
+                        input_type = run.input.type
+                        if input_type == 'upload':
+                            images.append(run.input.data)
+                        elif input_type == 'change':
+                            t1 = run.input.data.get("t1")
+                            t1["type"] = 'sentinel'
+                            t2 = run.input.data.get("t2")
+                            t2["type"] = 'sentinel'
+                            if t1.get("id") not in img_ids:
+                                images.append(t1)
+                                img_ids.append(t1.get("id"))
+                            if t2.get("id") not in img_ids:
+                                images.append(t2)
+                                img_ids.append(t2.get("id"))
+                        else:
+                            print(f'Process with corrupted Input data type: {input_type}')
+                            return False
+                    print(f'Images to create as input & runs for process on demand id: {process_id}')
+                    data: CreateProcessDict = {
+                        "name": new_name,
+                        "inference_model_id": model_id,
+                        "area": area,
+                        "cost_estimated": cost_estimated,
+                        "images": images,
+                        "geom": geom,
+                        "mask": mask
+                    }
+                    return self.create_process(data, user)
+                elif process_type == 'tasking':
+                    data: CreateTaskingDict = {
+                        "name": new_name,
+                        "inference_model_id": model_id,
+                        "area": area,
+                        "cost_estimated": cost_estimated,
+                        "tasking_config": data,
+                        "geom": geom,
+                        "mask": mask
+                    }
+                    return self.create_tasking(data, user)
+                else:
+                    return False
+
     def create_process(self, data: CreateProcessDict, user: User):
         name = data["name"]
         inference_model_id = data["inference_model_id"]
         area = data["area"]
         cost_estimated = data["cost_estimated"]
         images = data["images"]
         geom = data["geom"]
         mask = data["mask"]
         user_id = user.id
         organization_id = user.organization_id
 
         print(f'Creating process for user_id: {user_id}')
 
-        # Check if inference_model_id exists
-        model_query = (
-            select(InferenceModel.id)
-            .where(InferenceModel.id == inference_model_id)
-            .limit(1)
-        )
-        model = self.session.scalar(model_query)
-        if model is None:
-            return False
-
-        input_images = {
-            "sentinel": [],
-            "upload": []
-        }
-        unsorted_sentinel = []
-        for img in images:
-            img_type = img.get("type")
-            if img_type == "sentinel":
-                data = {
-                    "id": img.get("id"),
-                    "date": img.get("date"),
-                    "title": img.get("title")
-                }
-                unsorted_sentinel.append(data)
-            elif img_type == "upload":
-                input_images["upload"].append(img.get("id"))
-
-        input_images["sentinel"] = sorted(unsorted_sentinel, key=get_date)
-
-        print(f'Create process validation on images: {input_images}')
-        if len(input_images["upload"]) > 0:
-            # Check upload image exists
-            img_query_count = self.session.scalar(
-                select(func.count(Image.id))
-                .where(
-                    (Image.id.in_(input_images["upload"])) &
-                    (Image.organization_id == organization_id)
-                )
+        with Session(self.engine) as session:
+            # Check if inference_model_id exists
+            model_query = (
+                select(InferenceModel.id)
+                .where(InferenceModel.id == inference_model_id)
+                .limit(1)
             )
-            if img_query_count != len(input_images["upload"]):
-                print(f'Create process validation failed! An Upload image is not valid')
+            model = session.scalar(model_query)
+            if model is None:
                 return False
 
-        if len(input_images["sentinel"]) > 0:
-            # Check format of sentinel uuid
-            for data in input_images["sentinel"]:
-                if not is_valid_uuid(data["id"]):
-                    print(f'Create process validation failed! A Sentinel image is not valid')
+            input_images = {
+                "sentinel": [],
+                "upload": []
+            }
+            unsorted_sentinel = []
+            for img in images:
+                img_type = img.get("type")
+                if img_type == "sentinel":
+                    data = {
+                        "id": img.get("id"),
+                        "date": img.get("date"),
+                        "title": img.get("title")
+                    }
+                    unsorted_sentinel.append(data)
+                elif img_type == "upload":
+                    input_images["upload"].append(img.get("id"))
+
+            input_images["sentinel"] = sorted(unsorted_sentinel, key=get_date)
+
+            print(f'Create process validation on images: {input_images}')
+            if len(input_images["upload"]) > 0:
+                # Check upload image exists
+                img_query_count = session.scalar(
+                    select(func.count(Image.id))
+                    .where(
+                        (Image.id.in_(input_images["upload"])) &
+                        (Image.organization_id == organization_id)
+                    )
+                )
+                if img_query_count != len(input_images["upload"]):
+                    print(f'Create process validation failed! An Upload image is not valid')
                     return False
 
-        print(f'Create process validation ready!. Adding to DB...')
-        process = Process(
-            name=name,
-            cost_estimated=cost_estimated,
-            area=area,
-            type='on demand',
-            inference_model_id=inference_model_id,
-            organization_id=organization_id,
-            geom=geom,
-            mask=mask,
-            user_id=user_id
-        )
+            if len(input_images["sentinel"]) > 0:
+                # Check format of sentinel uuid
+                for data in input_images["sentinel"]:
+                    if not is_valid_uuid(data["id"]):
+                        print(f'Create process validation failed! A Sentinel image is not valid')
+                        return False
+
+            print(f'Create process validation ready!. Adding to DB...')
+            process = Process(
+                name=name,
+                cost_estimated=cost_estimated,
+                area=area,
+                type='on demand',
+                inference_model_id=inference_model_id,
+                organization_id=organization_id,
+                geom=geom,
+                mask=mask,
+                user_id=user_id
+            )
 
-        # if model is change detector with sentinel, then different process creation with multiple runs
-        if inference_model_id == 1:
-            if len(input_images["sentinel"]) < 2:
-                print("ERROR Create change detector process. Not enough sentinel images:")
-                return False
-            for i in range(len(input_images["sentinel"]) - 1):
-                new_input = Input(
-                    type='change',
-                    data={
-                        "t1": input_images["sentinel"][i],
-                        "t2": input_images["sentinel"][i+1]
-                    },
-                    user_id=user_id,
-                    organization_id=organization_id
-                )
-                self.session.add(new_input)
-                new_run = Run(
-                    input=new_input,
-                    inference_model_id=inference_model_id,
-                    process=process
-                )
-                self.session.add(new_run)
-            self.session.add(process)
-            try:
-                self.session.commit()
-                return True
-            except Exception as error:
-                print("ERROR Create change detector process. An exception occurred during DB insertion:", error)
-                return False
-        else:
-            for img in images:
-                new_input = Input(
-                    type=img.get("type"),
-                    data=img,
-                    user_id=user_id,
-                    organization_id=organization_id
-                )
-                self.session.add(new_input)
-                new_run = Run(
-                    input=new_input,
-                    inference_model_id=inference_model_id,
-                    process=process
-                )
-                self.session.add(new_run)
-            self.session.add(process)
-            try:
-                self.session.commit()
-                return True
-            except Exception as error:
-                print("ERROR Create process. An exception occurred during DB insertion:", error)
-                return False
+            # if model is change detector with sentinel, then different process creation with multiple runs
+            if inference_model_id == 1:
+                if len(input_images["sentinel"]) < 2:
+                    print("ERROR Create change detector process. Not enough sentinel images:")
+                    return False
+                for i in range(len(input_images["sentinel"]) - 1):
+                    new_input = Input(
+                        type='change',
+                        data={
+                            "t1": input_images["sentinel"][i],
+                            "t2": input_images["sentinel"][i+1]
+                        },
+                        user_id=user_id,
+                        organization_id=organization_id
+                    )
+                    session.add(new_input)
+                    new_run = Run(
+                        input=new_input,
+                        inference_model_id=inference_model_id,
+                        process=process
+                    )
+                    session.add(new_run)
+                session.add(process)
+                try:
+                    session.commit()
+                    return True
+                except Exception as error:
+                    print("ERROR Create change detector process. An exception occurred during DB insertion:", error)
+                    return False
+            else:
+                for img in images:
+                    new_input = Input(
+                        type=img.get("type"),
+                        data=img,
+                        user_id=user_id,
+                        organization_id=organization_id
+                    )
+                    session.add(new_input)
+                    new_run = Run(
+                        input=new_input,
+                        inference_model_id=inference_model_id,
+                        process=process
+                    )
+                    session.add(new_run)
+                session.add(process)
+                try:
+                    session.commit()
+                    return True
+                except Exception as error:
+                    print("ERROR Create process. An exception occurred during DB insertion:", error)
+                    return False
 
     def create_tasking(self, data: CreateTaskingDict, user: User):
         name = data["name"]
         inference_model_id = data["inference_model_id"]
         area = data["area"]
         cost_estimated = data["cost_estimated"]
         tasking_config = data["tasking_config"]
@@ -232,361 +308,489 @@
         geom = data["geom"]
         mask = data["mask"]
         organization_id = user.organization_id
 
         print(f'Creating tasking for user_id: {user_id}')
 
         # Check if inference_model_id exists
-        model_query = (
-            select(InferenceModel.id)
-            .where(InferenceModel.id == inference_model_id)
-            .limit(1)
-        )
-        model = self.session.scalar(model_query)
-        if model is None:
-            return False
-
-        process = Process(
-            name=name,
-            cost_estimated=cost_estimated,
-            area=area,
-            inference_model_id=inference_model_id,
-            data=tasking_config,
-            organization_id=organization_id,
-            type='tasking',
-            geom=geom,
-            mask=mask,
-            user_id=user_id
-        )
+        with Session(self.engine) as session:
+            model_query = (
+                select(InferenceModel.id)
+                .where(InferenceModel.id == inference_model_id)
+                .limit(1)
+            )
+            model = session.scalar(model_query)
+            if model is None:
+                return False
 
-        self.session.add(process)
-        try:
-            self.session.commit()
-            return True
-        except Exception as error:
-            # handle the exception
-            print("Create tasking. An exception occurred during DB insertion:", error)
-            return False
+            process = Process(
+                name=name,
+                cost_estimated=cost_estimated,
+                area=area,
+                inference_model_id=inference_model_id,
+                data=tasking_config,
+                organization_id=organization_id,
+                type='tasking',
+                geom=geom,
+                mask=mask,
+                user_id=user_id
+            )
+
+            session.add(process)
+            try:
+                session.commit()
+                return True
+            except Exception as error:
+                # handle the exception
+                print("Create tasking. An exception occurred during DB insertion:", error)
+                return False
 
     def get_inference_models(self):
-        query = (
-            select(InferenceModel)
-            .order_by(InferenceModel.id)
-        )
-        models = self.session.execute(query).all()
-        if models is None:
-            return {}
-        result = []
-        for model in models:
-            model = model[0]
-            result.append({
+        with Session(self.engine) as session:
+            query = (
+                select(InferenceModel)
+                .order_by(InferenceModel.id)
+            )
+            models = session.execute(query).all()
+            if models is None:
+                return {}
+            result = []
+            for model in models:
+                model = model[0]
+                result.append({
+                    "id": model.id,
+                    "name": model.name,
+                    "title": model.title,
+                    "description": model.description,
+                    "img_url": model.img_url,
+                    "price": model.price,
+                    "min_resolution": model.min_resolution,
+                    "config": model.config
+                })
+            return result
+
+    def get_inference_model_by_id(self, id: str):
+        with Session(self.engine) as session:
+            query = (
+                select(InferenceModel)
+                .where(InferenceModel.id == id)
+                .limit(1)
+            )
+            model = session.scalar(query)
+            if model is None:
+                return {}
+            print(f'Model with id: {id} found! ')
+            return {
                 "id": model.id,
                 "name": model.name,
                 "title": model.title,
                 "description": model.description,
                 "img_url": model.img_url,
                 "price": model.price,
                 "min_resolution": model.min_resolution,
                 "config": model.config
-            })
-        return result
-
-    def get_inference_model_by_id(self, id: str):
-        query = (
-            select(InferenceModel)
-            .where(InferenceModel.id == id)
-            .limit(1)
-        )
-        model = self.session.scalar(query)
-        if model is None:
-            return {}
-        print(f'Model with id: {id} found! ')
-        return {
-            "id": model.id,
-            "name": model.name,
-            "title": model.title,
-            "description": model.description,
-            "img_url": model.img_url,
-            "price": model.price,
-            "min_resolution": model.min_resolution,
-            "config": model.config
-        }
+            }
 
     def load_images_by_org(self, organization_id: str):
-        query = (
-            select(Image)
-            .where(
-                (Image.organization_id == organization_id)
+        with Session(self.engine) as session:
+            query = (
+                select(Image)
+                .where(
+                    (Image.organization_id == organization_id)
+                )
             )
-        )
-        images = self.session.execute(query).all()
-        if images is None:
-            return {}
-        result = []
-        for img in images:
-            img = img[0]
-            bbox = None
-            footprint = None
-            if img.bbox is not None:
-                bbox = wkbelement_to_wkt(img.bbox)
-            if img.footprint is not None:
-                footprint = wkbelement_to_wkt(img.footprint)
-            result.append({
-                "id": img.id,
-                "name": img.name,
-                "created_at": img.created_at,
-                "url": img.url,
-                "data": img.data,
-                "bbox": bbox,
-                "footprint": footprint,
-                "user": img.user.username
-            })
-        return result
+            images = session.execute(query).all()
+            if images is None:
+                return {}
+            result = []
+            for img in images:
+                img = img[0]
+                bbox = None
+                footprint = None
+                if img.bbox is not None:
+                    bbox = wkbelement_to_wkt(img.bbox)
+                if img.footprint is not None:
+                    footprint = wkbelement_to_wkt(img.footprint)
+                result.append({
+                    "id": img.id,
+                    "name": img.name,
+                    "created_at": img.created_at,
+                    "url": img.url,
+                    "data": img.data,
+                    "bbox": bbox,
+                    "footprint": footprint,
+                    "user": img.user.username
+                })
+            return result
 
     def load_process_by_id(self, id: str, user: User):
-        query = (
-            select(Process)
-            .where(Process.id == id)
-            .limit(1)
-        )
-        process = self.session.scalar(query)
-        if process is None:
-            print(f'No process with id ${id} found!')
-            return {}
-        elif process.organization_id != user.organization_id:
-            print(f'This process is not from this org_id: {user.organization_id}')
-            return None
-        else:
-            print(f'Process with id: {id} found! ')
-            runs = []
-            for run in process.runs:
-                finished_run_time = None
-                if run.finished_at is not None:
-                    finished_run_time = run.finished_at.strftime("%d/%m/%Y: %H:%M")
-                runs.append({
-                    "id": run.id,
-                    "status": run.status,
-                    "created_at": run.created_at.strftime("%d/%m/%Y: %H:%M"),
-                    "finished_at": finished_run_time,
-                    "engine": run.engine,
-                    "runtime": run.runtime,
-                    "cost": run.cost,
-                    "data": run.data,
-                    "input": {
-                        "id": run.input.id,
-                        "type": run.input.type,
-                        "data": run.input.data
-                    },
-                    "model": run.inference_model.name
-                })
-            finished_time = None
-            if process.finished_at is not None:
-                finished_time = process.finished_at.strftime("%d/%m/%Y: %H:%M")
-            geom = None
-            if process.geom is not None:
-                geom = wkbelement_to_wkt(process.geom)
-            mask = None
-            if process.mask is not None:
-                mask = wkbelement_to_wkt(process.mask)
-            return {
-                "id": process.id,
-                "name": process.name,
-                "status": process.status,
-                "type": process.type,
-                "created_at": process.created_at.strftime("%d/%m/%Y: %H:%M"),
-                "finished_at": finished_time,
-                "runtime": process.runtime,
-                "area": process.area,
-                "cost_estimated": process.cost_estimated,
-                "data": process.data,
-                "user": process.user.username,
-                "inference_model_id": process.inference_model_id,
-                "geom": geom,
-                "mask": mask,
-                "runs": runs
-            }
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(Process.id == id)
+                .limit(1)
+            )
+            process = session.scalar(query)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return {}
+            elif process.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                print(f'Process with id: {id} found! ')
+                runs = []
+                for run in process.runs:
+                    finished_run_time = None
+                    if run.finished_at is not None:
+                        finished_run_time = run.finished_at.strftime("%d/%m/%Y: %H:%M")
+                    runs.append({
+                        "id": run.id,
+                        "status": run.status,
+                        "created_at": run.created_at.strftime("%d/%m/%Y: %H:%M"),
+                        "finished_at": finished_run_time,
+                        "engine": run.engine,
+                        "runtime": run.runtime,
+                        "cost": run.cost,
+                        "data": run.data,
+                        "input": {
+                            "id": run.input.id,
+                            "type": run.input.type,
+                            "data": run.input.data
+                        },
+                        "model": run.inference_model.name
+                    })
+                geom = None
+                if process.geom is not None:
+                    geom = wkbelement_to_wkt(process.geom)
+                mask = None
+                if process.mask is not None:
+                    mask = wkbelement_to_wkt(process.mask)
+                return {
+                    "id": process.id,
+                    "name": process.name,
+                    "status": process.status,
+                    "type": process.type,
+                    "created_at": process.created_at,
+                    "finished_at": process.finished_at,
+                    "runtime": process.runtime,
+                    "area": process.area,
+                    "cost_estimated": process.cost_estimated,
+                    "data": process.data,
+                    "user": process.user.username,
+                    "inference_model_id": process.inference_model_id,
+                    "geom": geom,
+                    "mask": mask,
+                    "runs": runs
+                }
 
     def load_processes_by_org(self, org_id: int):
-        query = (
-            select(Process)
-            .where(
-                (Process.organization_id == org_id)
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(
+                    (Process.organization_id == org_id)
+                )
             )
-        )
-        processes = self.session.execute(query).all()
-        if processes is None:
-            return []
-        result = []
-        for process in processes:
-            process = process[0]
-            runs = []
-            for run in process.runs:
-                runs.append({
-                    "id": run.id,
-                    "status": run.status
+            processes = session.execute(query).all()
+            if processes is None:
+                return []
+            result = []
+            for process in processes:
+                process = process[0]
+                geom = None
+                if process.geom is not None:
+                    geom = wkbelement_to_wkt(process.geom)
+                mask = None
+                if process.mask is not None:
+                    mask = wkbelement_to_wkt(process.mask)
+                result.append({
+                    "id": process.id,
+                    "name": process.name,
+                    "status": process.status,
+                    "type": process.type,
+                    "created_at": process.created_at,
+                    "finished_at": process.finished_at,
+                    "runtime": process.runtime,
+                    "area": process.area,
+                    "cost_estimated": process.cost_estimated,
+                    "data": process.data,
+                    "user": process.user.username,
+                    "inference_model_id": process.inference_model_id,
+                    "geom": geom,
+                    "mask": mask,
                 })
-            finished_time = None
-            if process.finished_at is not None:
-                finished_time = process.finished_at.strftime("%d/%m/%Y: %H:%M")
-            geom = None
-            if process.geom is not None:
-                geom = wkbelement_to_wkt(process.geom)
-            mask = None
-            if process.mask is not None:
-                mask = wkbelement_to_wkt(process.mask)
-            result.append({
-                "id": process.id,
-                "name": process.name,
-                "status": process.status,
-                "type": process.type,
-                "created_at": process.created_at.strftime("%d/%m/%Y: %H:%M"),
-                "finished_at": finished_time,
-                "runtime": process.runtime,
-                "area": process.area,
-                "cost_estimated": process.cost_estimated,
-                "data": process.data,
-                "user": process.user.username,
-                "inference_model_id": process.inference_model_id,
-                "geom": geom,
-                "mask": mask,
-                "runs": runs
-            })
-        return result
+            return result
 
     def load_results_by_run_id(self, id: str):
-        query = (
-            select(ResultsRaw)
-            .where(ResultsRaw.run_id == id)
-            .order_by(ResultsRaw.id)
-        )
-        raw_results = self.session.execute(query).all()
-        if raw_results is None:
-            print(f'No results for run_id ${id}')
-            return []
-        else:
-            print(f'Results for run_id={id} found!: {len(raw_results)} results')
+        results = {
+            "raw": [],
+            "raster": []
+        }
+        with Session(self.engine) as session:
+            query_raw = (
+                select(ResultsRaw)
+                .where(ResultsRaw.run_id == id)
+                .order_by(ResultsRaw.id)
+            )
+            raw_results = session.execute(query_raw).all()
+            if raw_results is None:
+                print(f'No raw results for run_id ${id}')
+            else:
+                print(f'Raw results for run_id={id} found!: {len(raw_results)} results')
+                for raw_result in raw_results:
+                    raw_result = raw_result[0]
+                    wkt = wkbelement_to_wkt(raw_result.geom)
+                    results["raw"].append({
+                        "id": raw_result.id,
+                        "data": raw_result.data,
+                        "geom": wkt
+                    })
+
+            query_raster = (
+                select(ResultsRaster)
+                .where(ResultsRaster.run_id == id)
+                .order_by(ResultsRaster.id)
+            )
+            raster_results = session.execute(query_raster).all()
+            if raster_results is None:
+                print(f'No raster results for run_id ${id}')
+            else:
+                print(f'Raster results for run_id={id} found!: {len(raster_results)} results')
+                for raster_result in raster_results:
+                    raster_result = raster_result[0]
+                    wkt = wkbelement_to_wkt(raster_result.bbox)
+                    results["raster"].append({
+                        "id": raster_result.id,
+                        "url": raster_result.url,
+                        "data": raster_result.data,
+                        "bbox": wkt
+                    })
+
+            return results
+
+    def load_runs_by_process(self, id: str, user: User):
+        with Session(self.engine) as session:
+            organization_id = session.scalar(select(Process.organization_id).where(Process.id == id))
+
+            if organization_id is None or organization_id != user.organization_id:
+                return None
+
+            query_run = (
+                select(Run)
+                .where(Run.process_id == id)
+            )
+            runs = session.scalars(query_run)
+
             results = []
-            for result in raw_results:
-                result = result[0]
-                wkt = wkbelement_to_wkt(result.geom)
+
+            for run in runs:
                 results.append({
-                    "id": result.id,
-                    "data": result.data,
-                    "geom": wkt
+                    "id": run.id,
+                    "status": run.status,
+                    "created_at": run.created_at,
+                    "finished_at": run.finished_at,
+                    "engine": run.engine,
+                    "runtime": run.runtime,
+                    "cost": run.cost,
+                    "data": run.data,
+                    "inference_model_id": run.inference_model_id,
+                    "bbox": wkbelement_to_wkt(run.bbox) if run.bbox is not None else None,
                 })
+
             return results
 
     def load_run_by_id(self, id: str, user: User):
-        query_run = (
-            select(Run)
-            .where(Run.id == id)
-            .limit(1)
-        )
-        run = self.session.scalar(query_run)
-        if run is None:
-            print(f'No run with id ${id} found!')
-            return {}
-        elif run.process.organization_id != user.organization_id:
-            print(f'This process is not from this org_id: {user.organization_id}')
-            return None
-        else:
-            print(f'Run with id: {id} found! ')
-            raw_results = []
-            for raw_result in run.results_raw:
-                wkt = wkbelement_to_wkt(raw_result.geom)
-                raw_results.append({
-                    "id": raw_result.id,
-                    "data": raw_result.data,
-                    "geom": wkt
-                })
-            raster_results = []
-            for raster_result in run.results_raster:
-                wkt = wkbelement_to_wkt(raster_result.bbox)
-                raster_results.append({
-                    "id": raster_result.id,
-                    "url": raster_result.url,
-                    "data": raster_result.data,
-                    "bbox": wkt
-                })
-            finished_time = None
-            if run.finished_at is not None:
-                finished_time = run.finished_at.strftime("%d/%m/%Y: %H:%M")
-            return {
-                "id": run.id,
-                "status": run.status,
-                "created_at": run.created_at.strftime("%d/%m/%Y: %H:%M"),
-                "finished_at": finished_time,
-                "engine": run.engine,
-                "runtime": run.runtime,
-                "cost": run.cost,
-                "data": run.data,
-                "process_id": run.process_id,
-                "process_name": run.process.name,
-                "mask": wkbelement_to_wkt(run.process.mask),
-                "inference_model_id": run.inference_model_id,
-                "input_id": run.input_id,
-                "input_data": run.input.data,
-                "organization_id": run.process.organization_id,
-                "organization_name": run.process.organization.name,
-                "results_raw": raw_results,
-                "results_raster": raster_results
-            }
-
-    def load_queued_runs_by_model(self, model_id: str):
-        query_runs = (
-            select(Run)
-            .where(Run.inference_model_id == model_id)
-            .where(
-                (Run.inference_model_id == model_id) &
-                (Run.status == 'queued')
+        with Session(self.engine) as session:
+            query_run = (
+                select(Run)
+                .where(Run.id == id)
+                .limit(1)
             )
-            .order_by(Run.id)
-        )
-        runs = self.session.execute(query_runs).all()
-        if runs is None:
-            return []
-        else:
-            print(f'Queued runs found!: {len(runs)} results')
-            results = []
-            for run in runs:
-                run = run[0]
-                results.append({
+            run = session.scalar(query_run)
+            if run is None:
+                print(f'No run with id ${id} found!')
+                return {}
+            elif run.process.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                print(f'Run with id: {id} found! ')
+                raw_results = []
+                for raw_result in run.results_raw:
+                    wkt = wkbelement_to_wkt(raw_result.geom)
+                    raw_results.append({
+                        "id": raw_result.id,
+                        "data": raw_result.data,
+                        "geom": wkt
+                    })
+                raster_results = []
+                for raster_result in run.results_raster:
+                    wkt = wkbelement_to_wkt(raster_result.bbox)
+                    raster_results.append({
+                        "id": raster_result.id,
+                        "url": raster_result.url,
+                        "data": raster_result.data,
+                        "bbox": wkt
+                    })
+                return {
                     "id": run.id,
                     "status": run.status,
-                    "created_at": run.created_at.strftime("%d/%m/%Y: %H:%M"),
+                    "created_at": run.created_at,
+                    "finished_at": run.finished_at,
                     "engine": run.engine,
                     "runtime": run.runtime,
                     "cost": run.cost,
                     "data": run.data,
                     "process_id": run.process_id,
                     "process_name": run.process.name,
                     "mask": wkbelement_to_wkt(run.process.mask),
                     "inference_model_id": run.inference_model_id,
                     "input_id": run.input_id,
                     "input_data": run.input.data,
                     "organization_id": run.process.organization_id,
-                    "organization_name": run.process.organization.name
-                })
-            return results
+                    "organization_name": run.process.organization.name,
+                    "results_raw": raw_results,
+                    "results_raster": raster_results
+                }
 
     def upload_image(self, img: UploadImageDict, user: User):
         name = img["name"]
         url = img["url"]
         bbox = img["bbox"]
         print(f'Adding new uploaded image: {name} from user_id: {user.id}')
-        new_image = Image(
-            name=name,
-            url=url,
-            bbox=bbox,
-            user_id=user.id,
-            organization_id=user.organization_id
-        )
-        self.session.add(new_image)
-        self.session.commit()
-        return new_image
+        with Session(self.engine) as session:
+            new_image = Image(
+                name=name,
+                url=url,
+                bbox=bbox,
+                user_id=user.id,
+                organization_id=user.organization_id
+            )
+            session.add(new_image)
+            session.commit()
+            return new_image
+
+    def add_results_raster(self, run_id, object_key, data=None, bbox=None):
+        with Session(self.engine) as session:
+            new_result = ResultsRaster(
+                url=object_key,
+                data=data,
+                bbox=bbox,
+                run_id=run_id
+            )
+            session.add(new_result)
+            session.commit()
+            return new_result
+
+    def delete_process(self, id: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(
+                    and_(
+                        (Process.id == id),
+                        (Process.organization_id == user.organization_id)
+                    )
+                )
+                .limit(1)
+            )
+            process = session.scalar(query)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return False
+            else:
+                print(f'Deleting process with id: {id}')
+                session.delete(process)
+                session.commit()
+                return True
+
+    def get_raster_img_url(self, id: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(ResultsRaster)
+                .where(ResultsRaster.id == id)
+                .limit(1)
+            )
+            raster = session.scalar(query)
+            if raster is None:
+                print(f'No raster result with id ${id} found!')
+                return None
+            else:
+                print(f'Raster result with id: {id} found!')
+                return raster.url
+
+    def get_run_thumbnail_url(self, id: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Run)
+                .where(Run.id == id)
+                .limit(1)
+            )
+            run = session.scalar(query)
+            if run is None:
+                print(f'No run with id ${id} found!')
+                return None
+            else:
+                print(f'Run with id: {id} found!')
+                url = run.filepath + "thumbnail.png"
+                return url
+
+    def edit_process_name(self, id: str, name: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(
+                    and_(
+                        (Process.id == id),
+                        (Process.organization_id == user.organization_id)
+                    )
+                )
+                .limit(1)
+            )
+            process = session.scalar(query)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return False
+            else:
+                print(f'Editing process name with id: {id}')
+                process.name = name
+                session.commit()
+                return True
+
+#######################################
+######### library methods #############
+#######################################
+
+    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished', 'failed', 'canceled']):
+        """
+        Updates the status of the run
+
+        Args:
+            run_id: The id of the run
+            status: The new status of the run
+        """
+        assert isinstance(run_id, int), 'Invalid run_id!'
+        assert status in ['queued', 'running', 'finished', 'failed', 'canceled'], 'Invalid status!'
+
+        with Session(self.engine) as session:
+            query = (
+                select(Run)
+                .where(Run.id == run_id)
+                .limit(1)
+            )
+            run = session.scalar(query)
+            if run is None:
+                print(f'No run with id ${run_id} found!')
+                return False
+            run.status = status
+            if status == 'running':
+                run.process.status = 'running'
+            session.commit()
+            return True
 
     def upload_run_results(self, run_id: int, runtime: int, bbox: str, files_path: str, raster_name: str=None, file_names: list[str]=[], data: dict=None):
         """
         Uploads the files to the S3 bucket and updates the run status to finished
 
         Args:
             run_id: The id of the run
@@ -604,97 +808,94 @@
         assert isinstance(files_path, str), 'Invalid files_path!'
         assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
         assert isinstance(file_names, list), 'Invalid file_names!'
         assert data is None or isinstance(data, dict), 'Invalid data!'
 
         assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
 
-        self.check_db_connection()
-
-        # actual function
-        query = (
-            select(Run)
-            .where(Run.id == run_id)
-            .limit(1)
-        )
-        run = self.session.scalar(query)
-        if run is None:
-            print(f'No run with id ${run_id} found!')
-            return False
-
-        process_id = run.process_id
-        #process_name only the first 10 characters
-        process_name = run.process.name[:10]
-        org_id = run.process.organization_id
-        org_name = run.process.organization.name
-        run_id = run.id
-
-        # upload files to bucket
-        s3_client = S3Client()
-        bucket_base_directory = f"{org_id}-{org_name}/{process_id}-{process_name}/{run_id}/"
-
-        for file_name in file_names:
-            if not isinstance(file_name, str):
-                print('Invalid file_name!')
+        with Session(self.engine) as session:
+            # actual function
+            query = (
+                select(Run)
+                .where(Run.id == run_id)
+                .limit(1)
+            )
+            run = session.scalar(query)
+            if run is None:
+                print(f'No run with id ${run_id} found!')
                 return False
-            print(f'Uploading file: {file_name}')
-            object_key = bucket_base_directory + file_name
-            file_path = os.path.join(files_path, file_name)
-            s3_client.upload_file(file_path, object_key)
-            print(f'File uploaded to S3 with key: {object_key}')
-
-        if raster_name is not None:
-            print(f'Uploading raster file: {raster_name}')
-            object_key = bucket_base_directory + raster_name
-            file_path = os.path.join(files_path, raster_name)
-            s3_client.upload_file(file_path, object_key)
-            print(f'File uploaded to S3 with key: {object_key}')
-            self.add_results_raster(run_id, object_key, data, bbox)
-
-        # update run status
-        # when all runs of a process are finished, an SQL trigger will update the process status
-        run.status = 'finished'
-        run.finished_at = func.now()
-        run.bbox = bbox
-        # SQL trigger will update the process runtime
-        run.runtime = runtime
-        run.filepath = bucket_base_directory
-        self.session.commit()
 
-        return True
-
-    def add_results_raster(self, run_id, object_key, data=None, bbox=None):
-        new_result = ResultsRaster(
-            url=object_key,
-            data=data,
-            bbox=bbox,
-            run_id=run_id
-        )
-        self.session.add(new_result)
-        self.session.commit()
-        return new_result
-
-    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished', 'failed', 'canceled']):
-        """
-        Updates the status of the run
+            process_id = run.process_id
+            org_id = run.process.organization_id
+            run_id = run.id
+
+            # upload files to bucket
+            s3_client = S3Client(settings.run_results_bucket, settings.s3_region)
+            bucket_base_directory = f"{org_id}/{process_id}/{run_id}/"
+
+            for file_name in file_names:
+                if not isinstance(file_name, str):
+                    print('Invalid file_name!')
+                    return False
+                print(f'Uploading file: {file_name}')
+                object_key = bucket_base_directory + file_name
+                file_path = os.path.join(files_path, file_name)
+                s3_client.upload_file(file_path, object_key)
+                print(f'File uploaded to S3 with key: {object_key}')
+
+            if raster_name is not None:
+                print(f'Uploading raster file: {raster_name}')
+                object_key = bucket_base_directory + raster_name
+                file_path = os.path.join(files_path, raster_name)
+                s3_client.upload_file(file_path, object_key)
+                print(f'File uploaded to S3 with key: {object_key}')
+                self.add_results_raster(run_id, object_key, data, bbox)
+
+            # update run status
+            # when all runs of a process are finished, an SQL trigger will update the process status
+            run.status = 'finished'
+            run.finished_at = func.now()
+            run.bbox = bbox
+            # SQL trigger will update the process runtime
+            run.runtime = runtime
+            run.filepath = bucket_base_directory
+            session.commit()
 
-        Args:
-            run_id: The id of the run
-            status: The new status of the run
-        """
-        assert isinstance(run_id, int), 'Invalid run_id!'
-        assert status in ['queued', 'running', 'finished', 'failed', 'canceled'], 'Invalid status!'
+            return True
 
-        query = (
-            select(Run)
-            .where(Run.id == run_id)
-            .limit(1)
-        )
-        run = self.session.scalar(query)
-        if run is None:
-            print(f'No run with id ${run_id} found!')
-            return False
-        run.status = status
-        if status == 'running':
-            run.process.status = 'running'
-        self.session.commit()
-        return True
+    def load_queued_runs_by_model(self, model_id: str):
+        with Session(self.engine) as session:
+            query_runs = (
+                select(Run)
+                .where(Run.inference_model_id == model_id)
+                .where(
+                    (Run.inference_model_id == model_id) &
+                    (Run.status == 'queued')
+                )
+                .order_by(Run.id)
+            )
+            runs = session.execute(query_runs).all()
+            if runs is None:
+                return []
+            else:
+                print(f'Queued runs found!: {len(runs)} results')
+                results = []
+                for run in runs:
+                    run = run[0]
+                    results.append({
+                        "id": run.id,
+                        "status": run.status,
+                        "created_at": run.created_at.strftime("%d/%m/%Y: %H:%M"),
+                        "engine": run.engine,
+                        "runtime": run.runtime,
+                        "cost": run.cost,
+                        "data": run.data,
+                        "process_id": run.process_id,
+                        "process_name": run.process.name,
+                        "mask": wkbelement_to_wkt(run.process.mask),
+                        "inference_model_id": run.inference_model_id,
+                        "input_id": run.input_id,
+                        "input_data": run.input.data,
+                        "organization_id": run.process.organization_id,
+                        "organization_name": run.process.organization.name
+                    })
+                return results
```

### Comparing `rov_db_access-0.1.8/rov_db_access/utils/s3_utils.py` & `rov_db_access-1.0.0/rov_db_access/utils/s3_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from typing import Literal
 import boto3
 from botocore.client import Config
 from rov_db_access.config.settings import Settings
 
 settings = Settings()
 
 
 class S3Client:
-    def __init__(self):
-        self.region = settings.s3_region
-        self.bucket_name = settings.run_results_bucket
+    def __init__(self, bucket_name, bucket_region):
+        self.bucket_name = bucket_name
+        self.region = bucket_region
         self.access_key_id = settings.aws_key
         self.secret_access_key = settings.aws_secret
 
         self.s3 = boto3.client(
             "s3",
             aws_access_key_id=self.access_key_id,
             aws_secret_access_key=self.secret_access_key,
@@ -37,7 +38,23 @@
         return response['Body'].read()
 
     def put_file(self, key, data):
         self.s3.put_object(Bucket=self.bucket_name, Key=key, Body=data)
 
     def copy_file(self, src_key, dest_key):
         self.s3.copy_object(Bucket=self.bucket_name, CopySource=self.bucket_name + '/' + src_key, Key=dest_key)
+
+    def get_presigned_url(self, key, action: Literal['get_object', 'put_object']):
+        url = self.s3.generate_presigned_url(
+            action,
+            Params={'Bucket': self.bucket_name, 'Key': key},
+            ExpiresIn=60
+        )
+        return url
+
+    def check_file_exists(self, key):
+        try:
+            self.s3.head_object(Bucket=self.bucket_name, Key=key)
+            return True
+        except:
+            return False
+
```

### Comparing `rov_db_access-0.1.8/rov_db_access/utils/utils.py` & `rov_db_access-1.0.0/rov_db_access/utils/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     ewkt = ';'.join([srid_str, wkt_str])
     return ewkt
 
 
 def wkbelement_to_wkt(ewkt: Optional[WKBElement]) -> Optional[str]:
     if ewkt is None:
         return None
-    return to_shape(ewkt).wkt
+    return to_shape(ewkt).wkt
```

### Comparing `rov_db_access-0.1.8/PKG-INFO` & `rov_db_access-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 0.1.8
+Version: 1.0.0
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: boto3 (>=1.34.99,<2.0.0)
 Requires-Dist: geoalchemy2 (>=0.14.2,<0.15.0)
+Requires-Dist: geojson (>=3.1.0,<4.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
-Requires-Dist: pytest (>=8.0.0,<9.0.0)
+Requires-Dist: pyproj (>=3.6.1,<4.0.0)
+Requires-Dist: rasterio[s3] (>=1.3.10,<2.0.0)
+Requires-Dist: rov-sent-api (>=0.1.23,<0.2.0)
 Requires-Dist: shapely (>=2.0.4,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.23,<3.0.0)
 Description-Content-Type: text/markdown
```

