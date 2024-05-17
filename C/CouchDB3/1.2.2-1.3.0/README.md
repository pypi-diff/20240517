# Comparing `tmp/couchdb3-1.2.2.tar.gz` & `tmp/couchdb3-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchdb3-1.2.2.tar", last modified: Sun May 12 09:27:34 2024, max compression
+gzip compressed data, was "couchdb3-1.3.0.tar", last modified: Fri May 17 12:52:55 2024, max compression
```

## Comparing `couchdb3-1.2.2.tar` & `couchdb3-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/
--rwxr-xr-x   0 niko      (1000) niko      (1000)     1073 2024-05-12 09:24:20.000000 couchdb3-1.2.2/LICENSE
--rw-r--r--   0 niko      (1000) niko      (1000)     4646 2024-05-12 09:27:34.225151 couchdb3-1.2.2/PKG-INFO
--rwxr-xr-x   0 niko      (1000) niko      (1000)     3955 2024-05-12 09:24:20.000000 couchdb3-1.2.2/README.md
--rwxr-xr-x   0 niko      (1000) niko      (1000)      120 2024-05-12 09:24:20.000000 couchdb3-1.2.2/pyproject.toml
--rw-r--r--   0 niko      (1000) niko      (1000)       38 2024-05-12 09:27:34.225151 couchdb3-1.2.2/setup.cfg
--rwxr-xr-x   0 niko      (1000) niko      (1000)     1015 2024-05-12 09:25:53.000000 couchdb3-1.2.2/setup.py
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.221818 couchdb3-1.2.2/src/
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/src/CouchDB3.egg-info/
--rw-r--r--   0 niko      (1000) niko      (1000)     4646 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/PKG-INFO
--rwxrwxrwx   0 niko      (1000) niko      (1000)      508 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/SOURCES.txt
--rwxrwxrwx   0 niko      (1000) niko      (1000)        1 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/dependency_links.txt
--rwxrwxrwx   0 niko      (1000) niko      (1000)        9 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/requires.txt
--rwxrwxrwx   0 niko      (1000) niko      (1000)        9 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/top_level.txt
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.221818 couchdb3-1.2.2/src/couchdb3/
--rwxr-xr-x   0 niko      (1000) niko      (1000)     4155 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/__init__.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)    17094 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/base.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)    59367 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/database.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     5902 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/document.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     4201 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/exceptions.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)    16342 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/server.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)    11830 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/utils.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     2717 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/view.py
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/tests/
--rwxr-xr-x   0 niko      (1000) niko      (1000)    13649 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_database.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     1854 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_partitioned_database.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     3538 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_server.py
--rwxr-xr-x   0 niko      (1000) niko      (1000)     1239 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_utils.py
+drwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)        0 2024-05-17 12:52:55.571725 couchdb3-1.3.0/
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     1073 2024-05-17 07:24:09.000000 couchdb3-1.3.0/LICENSE
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)     4655 2024-05-17 12:52:55.571573 couchdb3-1.3.0/PKG-INFO
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     3964 2024-05-17 12:52:06.000000 couchdb3-1.3.0/README.md
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)      120 2024-05-17 07:24:09.000000 couchdb3-1.3.0/pyproject.toml
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)       38 2024-05-17 12:52:55.571762 couchdb3-1.3.0/setup.cfg
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     1015 2024-05-17 12:52:06.000000 couchdb3-1.3.0/setup.py
+drwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)        0 2024-05-17 12:52:55.568554 couchdb3-1.3.0/src/
+drwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)        0 2024-05-17 12:52:55.571387 couchdb3-1.3.0/src/CouchDB3.egg-info/
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)     4655 2024-05-17 12:52:55.000000 couchdb3-1.3.0/src/CouchDB3.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)      508 2024-05-17 12:52:55.000000 couchdb3-1.3.0/src/CouchDB3.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)        1 2024-05-17 12:52:55.000000 couchdb3-1.3.0/src/CouchDB3.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)        9 2024-05-17 12:52:55.000000 couchdb3-1.3.0/src/CouchDB3.egg-info/requires.txt
+-rw-r--r--   0 nikolaivlahovic   (501) staff       (20)        9 2024-05-17 12:52:55.000000 couchdb3-1.3.0/src/CouchDB3.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)        0 2024-05-17 12:52:55.570826 couchdb3-1.3.0/src/couchdb3/
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     4164 2024-05-17 12:52:06.000000 couchdb3-1.3.0/src/couchdb3/__init__.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)    17094 2024-05-17 07:24:09.000000 couchdb3-1.3.0/src/couchdb3/base.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)    58811 2024-05-17 12:52:06.000000 couchdb3-1.3.0/src/couchdb3/database.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     5916 2024-05-17 12:52:06.000000 couchdb3-1.3.0/src/couchdb3/document.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     4201 2024-05-17 07:24:09.000000 couchdb3-1.3.0/src/couchdb3/exceptions.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)    16342 2024-05-17 07:24:09.000000 couchdb3-1.3.0/src/couchdb3/server.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     8156 2024-05-17 12:52:06.000000 couchdb3-1.3.0/src/couchdb3/utils.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     2718 2024-05-17 12:52:06.000000 couchdb3-1.3.0/src/couchdb3/view.py
+drwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)        0 2024-05-17 12:52:55.571255 couchdb3-1.3.0/tests/
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)    15115 2024-05-17 12:52:06.000000 couchdb3-1.3.0/tests/test_database.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     1854 2024-05-17 07:24:09.000000 couchdb3-1.3.0/tests/test_partitioned_database.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     3538 2024-05-17 07:24:09.000000 couchdb3-1.3.0/tests/test_server.py
+-rwxr-xr-x   0 nikolaivlahovic   (501) staff       (20)     1239 2024-05-17 07:24:09.000000 couchdb3-1.3.0/tests/test_utils.py
```

### Comparing `couchdb3-1.2.2/LICENSE` & `couchdb3-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/PKG-INFO` & `couchdb3-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CouchDB3
-Version: 1.2.2
+Version: 1.3.0
 Summary: A wrapper around the CouchDB API.
 Home-page: https://github.com/n-vlahovic/couchdb3
 Author: Nikolai Vlahovic
 Author-email: nikolai@nexup.com
 Project-URL: Bug Tracker, https://github.com/n-vlahovic/couchdb3/issues
 Project-URL: Contributing, https://github.com/N-Vlahovic/couchdb3/blob/master/contributing.md
 Project-URL: Documentation, https://n-vlahovic.github.io/couchdb3/
@@ -137,15 +137,15 @@
 ```python
 docid = "mydoc-id"
 print(db.delete(docid=docid, rev=db.rev(docid)))  # Fetch the revision on the go
 # True
 ```
 
 ### Working with partitions
-For a partitioned database, the `couchdb3.Partition` class offers a wrapper around partitions (acting similarly 
+For a partitioned database, the `couchdb3.database.Partition` class offers a wrapper around partitions (acting similarly 
 to collections in Mongo). 
 
 ```python
 from couchdb3 import Server, Database, Partition
 
 
 client: Server = Server(...)
```

### Comparing `couchdb3-1.2.2/README.md` & `couchdb3-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 ```python
 docid = "mydoc-id"
 print(db.delete(docid=docid, rev=db.rev(docid)))  # Fetch the revision on the go
 # True
 ```
 
 ### Working with partitions
-For a partitioned database, the `couchdb3.Partition` class offers a wrapper around partitions (acting similarly 
+For a partitioned database, the `couchdb3.database.Partition` class offers a wrapper around partitions (acting similarly 
 to collections in Mongo). 
 
 ```python
 from couchdb3 import Server, Database, Partition
 
 
 client: Server = Server(...)
```

### Comparing `couchdb3-1.2.2/setup.py` & `couchdb3-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CouchDB3",
-    version="1.2.2",
+    version="1.3.0",
     author="Nikolai Vlahovic",
     author_email="nikolai@nexup.com",
     description="A wrapper around the CouchDB API.",
     install_requires=[
         "requests"
     ],
     long_description=long_description,
```

### Comparing `couchdb3-1.2.2/src/CouchDB3.egg-info/PKG-INFO` & `couchdb3-1.3.0/src/CouchDB3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CouchDB3
-Version: 1.2.2
+Version: 1.3.0
 Summary: A wrapper around the CouchDB API.
 Home-page: https://github.com/n-vlahovic/couchdb3
 Author: Nikolai Vlahovic
 Author-email: nikolai@nexup.com
 Project-URL: Bug Tracker, https://github.com/n-vlahovic/couchdb3/issues
 Project-URL: Contributing, https://github.com/N-Vlahovic/couchdb3/blob/master/contributing.md
 Project-URL: Documentation, https://n-vlahovic.github.io/couchdb3/
@@ -137,15 +137,15 @@
 ```python
 docid = "mydoc-id"
 print(db.delete(docid=docid, rev=db.rev(docid)))  # Fetch the revision on the go
 # True
 ```
 
 ### Working with partitions
-For a partitioned database, the `couchdb3.Partition` class offers a wrapper around partitions (acting similarly 
+For a partitioned database, the `couchdb3.database.Partition` class offers a wrapper around partitions (acting similarly 
 to collections in Mongo). 
 
 ```python
 from couchdb3 import Server, Database, Partition
 
 
 client: Server = Server(...)
```

### Comparing `couchdb3-1.2.2/src/couchdb3/__init__.py` & `couchdb3-1.3.0/src/couchdb3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 ```python
 docid = "mydoc-id"
 print(db.delete(docid=docid, rev=db.rev(docid)))  # Fetch the revision on the go
 # True
 ```
 
 ### Working with partitions
-For a partitioned database, the `couchdb3.Partition` class offers a wrapper around partitions (acting similarly 
+For a partitioned database, the `couchdb3.database.Partition` class offers a wrapper around partitions (acting similarly 
 to collections in Mongo). 
 
 ```python
 from couchdb3 import Server, Database, Partition
 
 
 client: Server = Server(...)
```

### Comparing `couchdb3-1.2.2/src/couchdb3/base.py` & `couchdb3-1.3.0/src/couchdb3/base.py`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/src/couchdb3/database.py` & `couchdb3-1.3.0/src/couchdb3/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
+import mimetypes
 import requests
 
 from .base import Base
 from .document import Document, AttachmentDocument, extract_document_id_and_rev, SecurityDocument, \
     SecurityDocumentElement
 from .exceptions import CouchDBError, NameComplianceError
-from .utils import validate_db_name, content_type_getter, DEFAULT_TIMEOUT, partitioned_db_resource_parser
+from .utils import validate_db_name, DEFAULT_TIMEOUT, partitioned_db_resource_parser
 from .view import ViewResult
 
 
 __all__ = [
     "Database",
     "Partition",
 ]
@@ -726,84 +727,65 @@
 
     def put_attachment(
             self,
             docid: str,
             attname: str,
             path: str = None,
             *,
-            content: Any = None,
+            content: bytes = None,
+            content_type: str = None,
             rev: str = None,
     ) -> Tuple[str, bool, str]:
         """
         Uploads the supplied content as an attachment to the specified document.
-        The appropriate content-type is generated using `couchdb3.utils.content_type_getter`.
 
         Parameters
         ----------
         docid : str
             The document's id.
         attname : str
             The attachment's name.
         path : str
             The path ot the local file to be uploaded.
             Precisely one of the arguments `path` or `content` must be supplied.
-        content : str
+        content : bytes
             The content to be uploaded.
             Precisely one of the arguments `path` or `content` must be supplied.
+        content_type : str
+            The attachment's content-type (mime-type).
+            Must be provided when passing the `content` argument.
         rev : str
             The document's current revision. Must be supplied for existing documents.
 
         Returns
         -------
         Tuple[str, bool, str] : A tuple consisting of the following elements.
 
           - the document's id ( `str`)
           - the operation status (`bool`)
           - the revision ( `str`)
         """
         if (not content and not path) or (content and path):
             raise ValueError("Precisely one of the arguments \"attdata\" and  \"attloc\" must be provided.")
-        content_type = content_type_getter(data=content, file_name=path if path else attname)
+        if content and not content_type:
+            raise ValueError("Argument \"content_type\" cannot be empty when \"content\" is provided.")
         resource = f"{docid}/{attname}"
         query_kwargs = {"rev": rev}
-        req_kwargs = {
-            "headers": {
-                "content-type": content_type_getter(data=content, file_name=path if path else attname)
-            }
-        }
+        content_type = content_type if content_type else mimetypes.guess_type(path)[0]
         if path:
             with open(path, "rb") as file:
-                response = self._put(
-                    resource=resource,
-                    query_kwargs=query_kwargs,
-                    data=file,
-                    headers={
-                        "content-type": content_type
-                    }
-                )
-        elif content_type in ('application/xml'):
-            req_kwargs.update({"body": content})
-            response = self._put(
-                resource=resource,
-                query_kwargs=query_kwargs,
-                data=content,
-                headers={
-                    "content-type": content_type
-                },
-            )      
-        else:
-            req_kwargs.update({"body": content})
-            response = self._put(
-                resource=resource,
-                query_kwargs=query_kwargs,
-                body=content,
-                headers={
-                    "content-type": content_type
-                },
-            )
+                content = file.read()
+        response = self._put(
+            resource=resource,
+            query_kwargs=query_kwargs,
+            data=content,
+            headers={
+                "content-type": content_type
+            },
+        )
         data = response.json()
         return data["id"], data["ok"], data["rev"]
 
     def put_design(
             self,
             ddoc: str,
             *,
@@ -1593,26 +1575,28 @@
 
     def put_attachment(
             self,
             docid: str,
             attname: str,
             path: str = None,
             *,
-            content: Any = None,
+            content: bytes = None,
+            content_type: str = None,
             rev: str = None,
     ) -> Tuple[str, bool, str]:
         """
         See `Database.put_attachment`.
 
         Note:
         Appends the partition's ID to the document's ID.
         """
         return super(Partition, self).put_attachment(
             docid=self.add_partition_to_str(docid),
             attname=attname,
+            content_type=content_type,
             path=path,
             content=content,
             rev=rev,
         )
 
     def rev(
             self,
```

### Comparing `couchdb3-1.2.2/src/couchdb3/document.py` & `couchdb3-1.3.0/src/couchdb3/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,30 +224,30 @@
     @property
     def admins(self) -> SecurityDocumentElement:
         """
         Returns
         -------
         SecurityDocument : The document's admins.
         """
-        return self.get("admins", SecurityDocument())
+        return self.get("admins", SecurityDocumentElement())
     
     @admins.setter
     def admins(self, value: SecurityDocumentElement) -> None:
         self.update({
             "admins": value
         })
 
     @property
     def members(self) -> SecurityDocumentElement:
         """
         Returns
         -------
         SecurityDocument : The document's members.
         """
-        return self.get("members", SecurityDocument())
+        return self.get("members", SecurityDocumentElement())
 
     @members.setter
     def members(self, value: SecurityDocumentElement) -> None:
         self.update({
             "members": value
         })
```

### Comparing `couchdb3-1.2.2/src/couchdb3/exceptions.py` & `couchdb3-1.3.0/src/couchdb3/exceptions.py`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/src/couchdb3/server.py` & `couchdb3-1.3.0/src/couchdb3/server.py`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/src/couchdb3/view.py` & `couchdb3-1.3.0/src/couchdb3/view.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
         -------
         int : The view's total number of rows.
         """
         return self._total_rows
 
     @total_rows.setter
     def total_rows(self, value: int) -> None:
-        self._total_rows = value
+        self._total_rows = value
```

### Comparing `couchdb3-1.2.2/tests/test_database.py` & `couchdb3-1.3.0/tests/test_database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import atexit
 import datetime
+import mimetypes
 import random
 import string
 
 import unittest
 
 from couchdb3.database import Database, Partition
 from couchdb3.document import Document, AttachmentDocument
 from couchdb3.server import Server
 from couchdb3.view import ViewResult, ViewRow
-from couchdb3.utils import user_name_to_id
+from couchdb3.utils import user_name_to_id, MimeTypeEnum
 
 from tests.credentials import ATTACHMENT_PATH_HTML, ATTACHMENT_PATH_JSON, ATTACHMENT_PATH_PNG, ATTACHMENT_PATH_TXT, \
-    ATTACHMENT_PATH_ZIP, COUCHDB_USER, COUCHDB_PASSWORD, COUCHDB0_URL, DOCUMENT_VIEW
+    ATTACHMENT_PATH_ZIP, COUCHDB_USER, COUCHDB_PASSWORD, COUCHDB0_URL, DOCUMENT_VIEW, ATTACHMENT_PATH_PDF
 
 
 def get_or_create_db(db_name: str, client: Server, partitioned: bool = False) -> Database:
     return client.get(db_name) if db_name in client else client.create(db_name, partitioned=partitioned)
 
 
 CLIENT: Server = Server(COUCHDB0_URL, user=COUCHDB_USER, password=COUCHDB_PASSWORD)
@@ -57,15 +58,15 @@
     def test___contains__(self):
         _id = "test-doc-__contains__"
         doc = {
             "type": "test-doc-__contains__",
             "_id": _id
         }
         DB.create(doc)
-        self.assertIn(_id, DB)
+        self.assertIn(_id, DB)  # noqa
 
     def test_bulk_docs(self):
         docs = [{
             "_id": f"doc-{_}",
             "name": f"Document {_}",
         } for _ in range(10)]
         results = DB.bulk_docs(docs=docs)
@@ -225,53 +226,86 @@
         self.assertIsInstance(dbdoc, Document)
         for key in doc:
             self.assertEqual(doc[key], dbdoc[key])
 
     def test_delete_attachment(self):
         docid = "test-doc-delete-attachment"
         DB.save({"_id": docid})
+        content_type = MimeTypeEnum.mime_type_json.value  # noqa
         for attname, content in [
             ("test-dict", {"hello": "world", 1: 2, 3: None}),
             ("test-str", "Hello World! 123"),
             ("test-list", ["Hello", "World", 1, 2, 3])
         ]:
             result = DB.put_attachment(
                 docid=docid,
                 attname=attname,
-                content=content,
+                content=str(content).encode('utf-8'),
+                content_type=content_type,
                 rev=DB.rev(docid)
             )
             self.assertTrue(DB.delete_attachment(
                 docid=docid,
                 attname=attname,
                 rev=result[2]
             ))
 
-    def test_get_attachment(self):
-        docid = "test-doc-get-attachment"
+    def test_attachment_via_path(self):
+        docid = self.test_attachment_via_path.__name__.replace('_', '-')
         DB.save({"_id": docid})
         for attname, path in [
             ("test.html", ATTACHMENT_PATH_HTML),
             ("test.json", ATTACHMENT_PATH_JSON),
             ("test.png", ATTACHMENT_PATH_PNG),
             ("test.txt", ATTACHMENT_PATH_TXT),
             ("test.zip", ATTACHMENT_PATH_ZIP),
+            ("test.pdf", ATTACHMENT_PATH_PDF),
         ]:
             DB.put_attachment(
                 docid=docid,
                 attname=attname,
                 path=path,
                 rev=DB.rev(docid)
             )
             response = DB.get_attachment(
                 docid=docid,
                 attname=attname
             )
             self.assertIsInstance(response, AttachmentDocument)
             self.assertIsInstance(response.content, bytes)
+            self.assertIsInstance(response.content_length, int)
+            self.assertIsInstance(response.digest, str)
+
+    def test_attachment_via_content(self):
+        docid = self.test_attachment_via_content.__name__.replace('_', '-')
+        DB.save({"_id": docid})
+        for attname, path in [
+            ("test.html", ATTACHMENT_PATH_HTML),
+            ("test.json", ATTACHMENT_PATH_JSON),
+            ("test.png", ATTACHMENT_PATH_PNG),
+            ("test.txt", ATTACHMENT_PATH_TXT),
+            ("test.zip", ATTACHMENT_PATH_ZIP),
+            ("test.pdf", ATTACHMENT_PATH_PDF),
+        ]:
+            with open(path, 'rb') as f:
+                content = f.read()
+                content_type = mimetypes.guess_type(path)[0]
+            DB.put_attachment(
+                docid=docid,
+                attname=attname,
+                content=content,
+                content_type=content_type,
+                rev=DB.rev(docid),
+            )
+            response = DB.get_attachment(
+                docid=docid,
+                attname=attname
+            )
+            self.assertIsInstance(response, AttachmentDocument)
+            self.assertIsInstance(response.content, bytes)
             self.assertIsInstance(response.content_length, int)
             self.assertIsInstance(response.digest, str)
 
     def test_put_design(self):
         for partitioned, db in [
             (False, DB),
             (True, DB_PARTITIONED),
```

### Comparing `couchdb3-1.2.2/tests/test_partitioned_database.py` & `couchdb3-1.3.0/tests/test_partitioned_database.py`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/tests/test_server.py` & `couchdb3-1.3.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `couchdb3-1.2.2/tests/test_utils.py` & `couchdb3-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

