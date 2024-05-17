# Comparing `tmp/deciphonctl-0.4.1.tar.gz` & `tmp/deciphonctl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphonctl-0.4.1.tar", max compression
+gzip compressed data, was "deciphonctl-0.4.2.tar", max compression
```

## Comparing `deciphonctl-0.4.1.tar` & `deciphonctl-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/LICENSE
--rw-r--r--   0        0        0       15 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/__init__.py
--rw-r--r--   0        0        0       28 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/__main__.py
--rw-r--r--   0        0        0     6028 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/cli.py
--rw-r--r--   0        0        0      755 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/consumer.py
--rw-r--r--   0        0        0      677 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/download.py
--rw-r--r--   0        0        0     1088 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/files.py
--rw-r--r--   0        0        0     2386 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/models.py
--rw-r--r--   0        0        0      107 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/permissions.py
--rw-r--r--   0        0        0     3479 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/presser.py
--rw-r--r--   0        0        0     1242 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress.py
--rw-r--r--   0        0        0      423 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress_informer.py
--rw-r--r--   0        0        0      871 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress_logger.py
--rw-r--r--   0        0        0     3230 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/scanner.py
--rw-r--r--   0        0        0     5858 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/sched.py
--rw-r--r--   0        0        0      435 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/settings.py
--rw-r--r--   0        0        0      387 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/signals.py
--rw-r--r--   0        0        0      305 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/url.py
--rw-r--r--   0        0        0     1055 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/worker.py
--rw-r--r--   0        0        0      792 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 deciphonctl-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/__main__.py
+-rw-r--r--   0        0        0     6028 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/cli.py
+-rw-r--r--   0        0        0      755 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/consumer.py
+-rw-r--r--   0        0        0      677 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/download.py
+-rw-r--r--   0        0        0      157 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/file_path.py
+-rw-r--r--   0        0        0     1088 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/files.py
+-rw-r--r--   0        0        0     2382 2024-05-17 09:44:48.129710 deciphonctl-0.4.2/deciphonctl/models.py
+-rw-r--r--   0        0        0      107 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/permissions.py
+-rw-r--r--   0        0        0     3514 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/presser.py
+-rw-r--r--   0        0        0     1242 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress.py
+-rw-r--r--   0        0        0      423 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress_informer.py
+-rw-r--r--   0        0        0      871 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/progress_logger.py
+-rw-r--r--   0        0        0     3246 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/scanner.py
+-rw-r--r--   0        0        0     5922 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/sched.py
+-rw-r--r--   0        0        0      474 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/settings.py
+-rw-r--r--   0        0        0      387 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/signals.py
+-rw-r--r--   0        0        0      240 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/url.py
+-rw-r--r--   0        0        0     1055 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/deciphonctl/worker.py
+-rw-r--r--   0        0        0      792 2024-05-17 09:44:48.133710 deciphonctl-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 deciphonctl-0.4.2/PKG-INFO
```

### Comparing `deciphonctl-0.4.1/LICENSE` & `deciphonctl-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/cli.py` & `deciphonctl-0.4.2/deciphonctl/cli.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/consumer.py` & `deciphonctl-0.4.2/deciphonctl/consumer.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/download.py` & `deciphonctl-0.4.2/deciphonctl/download.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/files.py` & `deciphonctl-0.4.2/deciphonctl/files.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/models.py` & `deciphonctl-0.4.2/deciphonctl/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     name: str
 
     @property
     def hmm_file_name(self):
         return HMMFileName(name=str(Path(self.name).with_suffix(".hmm")))
 
 
-class HMMFile(HMMName):
-    ...
+class HMMFile(HMMName): ...
 
 
 class DBFile(DBName):
     gencode: Gencode
     epsilon: float
```

### Comparing `deciphonctl-0.4.1/deciphonctl/presser.py` & `deciphonctl-0.4.2/deciphonctl/presser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import shutil
 from multiprocessing import JoinableQueue, Process
 from pathlib import Path
 
 from deciphon_core.press import PressContext
 from deciphon_core.schema import HMMFile
 from loguru import logger
-from pydantic import FilePath, HttpUrl
+from pydantic import HttpUrl
 
 from deciphonctl.consumer import Consumer
 from deciphonctl.download import download
+from deciphonctl.file_path import file_path
 from deciphonctl.files import atomic_file_creation, remove_temporary_files
 from deciphonctl.models import DBFile, JobUpdate, PressRequest
 from deciphonctl.permissions import normalise_file_permissions
 from deciphonctl.progress_informer import ProgressInformer
 from deciphonctl.progress_logger import ProgressLogger
 from deciphonctl.sched import Sched
 from deciphonctl.settings import Settings
@@ -35,15 +36,15 @@
             logger.info(f"pressing {x}")
             dcptmp = self._press(x, request)
             shutil.move(dcptmp, dcpfile)
         return dcpfile
 
     def _press(self, hmmfile: Path, req: PressRequest):
         dcpfile = hmmfile.with_suffix(".dcp")
-        hmm = HMMFile(path=FilePath(hmmfile))
+        hmm = HMMFile(path=file_path(hmmfile))
         db = req.db
         with PressContext(hmm, gencode=db.gencode, epsilon=db.epsilon) as press:
             self._qout.put(JobUpdate.run(req.job_id, 0).model_dump_json())
             with ProgressLogger(str(hmmfile)) as progress:
                 for i, x in enumerate([press] * press.nproteins):
                     x.next()
                     progress.percent = (100 * (i + 1)) // press.nproteins
```

### Comparing `deciphonctl-0.4.1/deciphonctl/progress.py` & `deciphonctl-0.4.2/deciphonctl/progress.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/progress_logger.py` & `deciphonctl-0.4.2/deciphonctl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/deciphonctl/scanner.py` & `deciphonctl-0.4.2/deciphonctl/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from subprocess import DEVNULL
 
 from deciphon.h3daemon import H3Daemon
 from deciphon_core.scan import Params, Scan
 from deciphon_core.schema import DBFile, HMMFile, NewSnapFile
 from deciphon_core.sequence import Sequence
 from loguru import logger
-from pydantic import FilePath
 
 from deciphonctl.consumer import Consumer
 from deciphonctl.download import download
+from deciphonctl.file_path import file_path
 from deciphonctl.files import (
     atomic_file_creation,
     remove_temporary_files,
     unique_temporary_file,
 )
 from deciphonctl.models import ScanRequest
 from deciphonctl.progress import Progress
@@ -47,18 +47,18 @@
         if not dbfile.exists():
             with atomic_file_creation(dbfile) as t:
                 download(self._sched.presigned.download_db_url(dbfile.name), t)
 
         with unique_temporary_file(".dcs") as t:
             snap = NewSnapFile(path=t)
 
-            db = DBFile(path=FilePath(dbfile))
+            db = DBFile(path=file_path(dbfile))
 
             logger.info("starting h3daemon")
-            with H3Daemon(HMMFile(path=FilePath(hmmfile)), stdout=DEVNULL) as daemon:
+            with H3Daemon(HMMFile(path=file_path(hmmfile)), stdout=DEVNULL) as daemon:
                 params = Params(
                     num_threads=self._num_threads,
                     multi_hits=x.multi_hits,
                     hmmer3_compat=x.hmmer3_compat,
                 )
                 logger.info(f"scan parameters: {params}")
                 scan = Scan(params, db)
```

### Comparing `deciphonctl-0.4.1/deciphonctl/sched.py` & `deciphonctl-0.4.2/deciphonctl/sched.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
-from requests_toolbelt import MultipartEncoder
 import urllib.parse
 from pathlib import Path
 from typing import Any, Optional
 
 import requests
 from deciphon_core.schema import Gencode
 from loguru import logger
 from pydantic import BaseModel, FilePath, HttpUrl
 from requests.models import HTTPError
+from requests_toolbelt import MultipartEncoder
 
 from deciphonctl.models import DBFile, HMMFile, JobUpdate, Scan
+from deciphonctl.url import http_url
 
 
 class SchedHTTPError(HTTPError):
     def __init__(self, response):
         try:
             response.raise_for_status()
             assert False
@@ -117,15 +118,17 @@
         json = {"state": x.state.value, "progress": x.progress, "error": x.error}
         self.patch(self.url(f"jobs/{x.id}"), json=json)
 
     def seq_list(self):
         return self.get(self.url("seqs")).json()
 
     def snap_post(self, scan_id: int, snap: FilePath):
-        post = UploadPost(url=HttpUrl(self.url(f"scans/{scan_id}/snap.dcs")), fields={})
+        post = UploadPost(
+            url=http_url(self.url(f"scans/{scan_id}/snap.dcs")), fields={}
+        )
         self.upload(snap, post)
 
     def snap_get(self, scan_id: int):
         return self.get(self.url(f"scans/{scan_id}/snap.dcs")).content
 
     def snap_delete(self, scan_id: int):
         self.delete(self.url(f"scans/{scan_id}/snap.dcs"))
@@ -143,28 +146,28 @@
         self._sched = sched
 
     def _request(self, path: str):
         return self._sched.get(self._sched.url(path)).json()
 
     def download_hmm_url(self, filename: str):
         x = self._request(f"hmms/presigned-download/{filename}")
-        return HttpUrl(x["url"])
+        return http_url(x["url"])
 
     def download_db_url(self, filename: str):
         x = self._request(f"dbs/presigned-download/{filename}")
-        return HttpUrl(x["url"])
+        return http_url(x["url"])
 
     def upload_hmm_post(self, filename: str):
         x = self._request(f"hmms/presigned-upload/{filename}")
-        url = self._sched.s3_url if self._sched.s3_url else HttpUrl(x["url"])
+        url = self._sched.s3_url if self._sched.s3_url else http_url(x["url"])
         return UploadPost(url=url, fields=x["fields"])
 
     def upload_db_post(self, filename: str):
         x = self._request(f"dbs/presigned-upload/{filename}")
-        url = self._sched.s3_url if self._sched.s3_url else HttpUrl(x["url"])
+        url = self._sched.s3_url if self._sched.s3_url else http_url(x["url"])
         return UploadPost(url=url, fields=x["fields"])
 
 
 class UploadPost(BaseModel):
     url: HttpUrl
     fields: dict[str, Any]
```

### Comparing `deciphonctl-0.4.1/deciphonctl/worker.py` & `deciphonctl-0.4.2/deciphonctl/worker.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.1/pyproject.toml` & `deciphonctl-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphonctl"
-version = "0.4.1"
+version = "0.4.2"
 description = "Control Deciphon server."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphonctl" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphonctl-0.4.1/PKG-INFO` & `deciphonctl-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphonctl
-Version: 0.4.1
+Version: 0.4.2
 Summary: Control Deciphon server.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

