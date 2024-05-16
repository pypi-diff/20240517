# Comparing `tmp/s3func-0.1.2.tar.gz` & `tmp/s3func-0.1.3.tar.gz`

## Comparing `s3func-0.1.2.tar` & `s3func-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/__init__.py
--rw-r--r--   0        0        0    19646 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/main.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.2/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.2/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.2/README.md
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/__init__.py
+-rw-r--r--   0        0        0    18957 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/main.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/tests/__init__.py
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 s3func-0.1.3/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.3/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.3/README.md
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.3/PKG-INFO
```

### Comparing `s3func-0.1.2/s3func/main.py` & `s3func-0.1.3/s3func/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import boto3
 import botocore
 import copy
 # import requests
 import urllib.parse
 from urllib3.util import Retry, Timeout
 import datetime
+import hashlib
 # from requests import Session
 # from requests.adapters import HTTPAdapter
 import urllib3
 
 from . import utils
 # import utils
 
@@ -160,15 +161,16 @@
     """
     if session is None:
         session = url_session(**url_session_kwargs)
 
     headers = utils.build_url_headers(range_start=range_start, range_end=range_end)
 
     response = session.request('get', url, headers=headers, preload_content=False)
-    response.content_length = int(response.headers['Content-Length'])
+    metadata = utils.add_metadata_from_urllib3(response)
+    response.metadata = metadata
 
     return response
 
 
 def base_url_to_stream(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
     """
 
@@ -213,23 +215,20 @@
         s3 = s3_client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id, range_start=range_start, range_end=range_end)
 
     try:
         response = s3.get_object(**params)
         stream = response['Body']
-        stream.status = 200
-        stream.etag = response['ETag'].strip('"')
-        stream.content_length = response['ContentLength']
-        stream.version_id = response['VersionId']
-        stream.last_modified = datetime.datetime.fromtimestamp(int(response['VersionId'].split('_u')[1]) * 0.001, datetime.timezone.utc)
-        stream.metadata = response['Metadata']
+        metadata = utils.add_metadata_from_s3(response)
     except s3.exceptions.NoSuchKey:
         stream = utils.S3ErrorResponse()
-        stream.status = 404
+        metadata = {'status': 404}
+
+    stream.metadata = metadata
 
     return stream
 
 
 def get_object_combo(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, session: urllib3.poolmanager.PoolManager=None, base_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **kwargs):
     """
     Combo function to get an object from an S3 bucket either using the S3 get_object function or the base_url_to_stream function. One of s3, connection_config, or base_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
@@ -277,36 +276,30 @@
 
     """
     if session is None:
         session = url_session(**url_session_kwargs)
 
     response = session.request('head', url)
 
-    headers = dict(response.headers)
-    headers['content_length'] = int(headers['Content-Length'])
-    if 'x-bz-file-id' in headers:
-        headers['version_id'] = headers['x-bz-file-id']
-    if 'X-Bz-Upload-Timestamp' in headers:
-        headers['last_modified'] = datetime.datetime.fromtimestamp(int(headers['X-Bz-Upload-Timestamp']) * 0.001, datetime.timezone.utc)
-    elif 'x-bz-file-id' in headers:
-        headers['last_modified'] = datetime.datetime.fromtimestamp(int(headers['x-bz-file-id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
+    metadata = utils.add_metadata_from_urllib3(response)
+    response.metadata = metadata
 
-    return headers
+    return response
 
 
 def base_url_to_headers(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
     """
 
     """
     if not base_url.endswith('/'):
         base_url += '/'
     url = urllib.parse.urljoin(base_url, obj_key)
-    headers = url_to_headers(url, session, **url_session_kwargs)
+    response = url_to_headers(url, session, **url_session_kwargs)
 
-    return headers
+    return response
 
 
 def head_object(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, version_id: str=None, **s3_client_kwargs):
     """
     Function to get an object from an S3 bucket. Either s3 or connection_config must be used. This function will return a file object of the object in the S3 location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
@@ -329,30 +322,28 @@
     ## Get the object
     if s3 is None:
         s3 = s3_client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
 
     try:
-        response = s3.head_object(**params)
-        response['status']= 200
-        response['etag'] = response.pop('ETag').strip('"')
-        response['content_length'] = response.pop('ContentLength')
-        response['version_id'] = response.pop('VersionId')
-        response['last_modified'] = datetime.datetime.fromtimestamp(int(response['version_id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
-        response['metadata'] = response.pop('Metadata')
-        del response['LastModified']
+        response = utils.S3Response()
+        response.headers = s3.head_object(**params)
+        metadata = utils.add_metadata_from_s3(response.headers)
+
     except s3.exceptions.NoSuchKey:
         response = utils.S3ErrorResponse()
-        response['status'] = 404
+        metadata = {'status': 404}
+
+    response.metadata = metadata
 
     return response
 
 
-def put_object(s3: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict=None, content_type: str=None, object_legal_hold: bool=False):
+def put_object(s3: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict={}, content_type: str=None, object_legal_hold: bool=False):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
@@ -369,22 +360,28 @@
     object_legal_hold : bool
         Should the object be uploaded with a legal hold?
 
     Returns
     -------
     None
     """
+    # TODO : In python version 3.11, the file_digest function can input a file object
+    if isinstance(obj, (bytes, bytearray)) and ('content-md5' not in metadata):
+        metadata['content-md5'] = hashlib.md5(obj).hexdigest()
     params = utils.build_s3_params(bucket, obj_key=obj_key, metadata=metadata, content_type=content_type, object_legal_hold=object_legal_hold)
 
-    response = s3.put_object(Body=obj, **params)
+    try:
+        response = utils.S3Response()
+        response.headers = s3.put_object(Body=obj, **params)
+        metadata = utils.add_metadata_from_s3(response.headers)
+    except s3.exceptions.ClientError:
+        response = utils.S3ErrorResponse()
+        metadata = {'status': 404}
 
-    response.update({'key': obj_key, 'bucket': bucket})
-    etag = response['ETag'].strip('"')
-    response['ResponseMetadata']['HTTPHeaders']['etag'] = etag
-    response['ETag'] = etag
+    response.metadata = metadata
 
     return response
 
 
 #####################################
 ### Other S3 operations
```

### Comparing `s3func-0.1.2/s3func/tests/stns_data.blt` & `s3func-0.1.3/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.1.2/s3func/tests/test_s3func.py` & `s3func-0.1.3/s3func/tests/test_s3func.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,33 +92,33 @@
 
 
 def test_put_object():
     """
 
     """
     ### Upload with bytes
-    with open(script_path.joinpath(file_name), 'rb') as f:
+    with io.open(script_path.joinpath(file_name), 'rb') as f:
         obj = f.read()
 
     resp1 = put_object(s3, bucket, obj_key, obj)
 
-    meta = resp1['ResponseMetadata']
-    if meta['HTTPStatusCode'] != 200:
+    meta = resp1.metadata
+    if meta['status'] != 200:
         raise ValueError('Upload failed')
 
-    resp1_etag = resp1['ETag']
+    resp1_etag = meta['etag']
 
     ## Upload with a file-obj
-    resp2 = put_object(s3, bucket, obj_key, open(script_path.joinpath(file_name), 'rb'))
+    resp2 = put_object(s3, bucket, obj_key, io.open(script_path.joinpath(file_name), 'rb'))
 
-    meta = resp2['ResponseMetadata']
-    if meta['HTTPStatusCode'] != 200:
+    meta = resp2.metadata
+    if meta['status'] != 200:
         raise ValueError('Upload failed')
 
-    resp2_etag = resp2['ETag']
+    resp2_etag = meta['etag']
 
     assert resp1_etag == resp2_etag
 
 
 def test_list_objects():
     """
 
@@ -173,26 +173,26 @@
     assert data1 == data2
 
 
 def test_head_object():
     """
 
     """
-    headers = head_object(obj_key, bucket, s3)
+    response = head_object(obj_key, bucket, s3)
 
-    assert 'version_id' in headers
+    assert 'version_id' in response.metadata
 
 
 def test_url_to_headers():
     """
 
     """
-    headers = url_to_headers(url)
+    response = url_to_headers(url)
 
-    assert 'version_id' in headers
+    assert 'version_id' in response.metadata
 
 
 def test_legal_hold():
     """
 
     """
     hold = get_object_legal_hold(s3, bucket, obj_key)
```

### Comparing `s3func-0.1.2/.gitignore` & `s3func-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.1.2/LICENSE` & `s3func-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.1.2/README.md` & `s3func-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.1.2/pyproject.toml` & `s3func-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.1.2/PKG-INFO` & `s3func-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple functions for working with S3
 Project-URL: Documentation, https://mullenkamp.github.io/s3func/
 Project-URL: Source, https://github.com/mullenkamp/s3func
 Author-email: s3func <mullenkamp1@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: s3func Version: 0.1.2 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.1.3 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```

