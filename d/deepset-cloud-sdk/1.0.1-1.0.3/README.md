# Comparing `tmp/deepset_cloud_sdk-1.0.1.tar.gz` & `tmp/deepset_cloud_sdk-1.0.3.tar.gz`

## Comparing `deepset_cloud_sdk-1.0.1.tar` & `deepset_cloud_sdk-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/assets/cli.gif
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/assets/logo.png
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/config.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/deepset_cloud_api.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/files.py
--rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/upload_sessions.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/__init__.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/upload.py
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_utils/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_utils/datetime.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/utils.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/index.md
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/upload_files.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_images/favicon.svg
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_images/white-logo.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/renderers.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/requirements.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/async_client.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/cli.yml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_pydoc/config/sync_client.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/_stylesheets/extra.css
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/sdk/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/docs/examples/sdk/upload.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example.txt.meta.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example2.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/test-upload/example2.txt.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/.gitignore
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/LICENSE
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/README.md
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/mkdocs.yml
+-rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/assets/cli.gif
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/assets/logo.png
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0    13248 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/config.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/deepset_cloud_api.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/files.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/upload_sessions.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_s3/__init__.py
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_s3/upload.py
+-rw-r--r--   0        0        0    31445 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_utils/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_utils/constants.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_utils/datetime.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/sync_client/utils.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/index.md
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/upload_files.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_images/favicon.svg
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_images/white-logo.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/renderers.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/requirements.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/config/async_client.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/config/cli.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_pydoc/config/sync_client.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/_stylesheets/extra.css
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/sdk/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/docs/examples/sdk/upload.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/test-upload/example.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/test-upload/example.txt.meta.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/test-upload/example2.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/test-upload/example2.txt.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/.gitignore
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.3/PKG-INFO
```

### Comparing `deepset_cloud_sdk-1.0.1/.pre-commit-config.yaml` & `deepset_cloud_sdk-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/CONTRIBUTING.md` & `deepset_cloud_sdk-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/mkdocs.yml` & `deepset_cloud_sdk-1.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/assets/cli.gif` & `deepset_cloud_sdk-1.0.3/assets/cli.gif`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/assets/logo.png` & `deepset_cloud_sdk-1.0.3/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/cli.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,15 +312,27 @@
 
 @cli_app.callback()
 def main(
     _: Optional[bool] = typer.Option(
         None, "--version", callback=version_callback, is_eager=True, help="Show the SDK version and exit."
     )
 ) -> None:  # noqa
-    """The CLI for the deepset Cloud SDK."""
+    """The CLI for the deepset Cloud SDK.
+
+    This documentation uses Python type hints to provide information about the arguments and return values.
+    Typer turns these type hints into a CLI interface. To see how these arguments are used in the CLI, check the
+    Typer documentation: https://typer.tiangolo.com/tutorial/arguments/optional or run
+    `deepset-cloud <command> --help` to see the arguments for a specific command.
+
+    Boolean values are converted to `-no-<variable>` or `-<variable>` flags in the CLI. For example, to disable
+    the progress bar, use `--no-show-progress`.
+
+    Lists can be passed by using the same flag multiple times. For example, to scan only `.txt` and `.pdf` files,
+    when uploading use `--use-type .txt --use-type .pdf`.
+    """
 
 
 def run_packaged() -> None:
     """Run the packaged CLI.
 
     This is the entrypoint for the package to enable running the CLI using typer.
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/config.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/config.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/deepset_cloud_api.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/deepset_cloud_api.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/files.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from uuid import UUID
 
 import structlog
 from httpx import codes
 
 from deepset_cloud_sdk._api.deepset_cloud_api import DeepsetCloudAPI
 from deepset_cloud_sdk._api.upload_sessions import WriteMode
+from deepset_cloud_sdk._utils.constants import SUPPORTED_TYPE_SUFFIXES
 from deepset_cloud_sdk._utils.datetime import from_isoformat
 
 logger = structlog.get_logger(__name__)
 
 
 class NotMatchingFileTypeException(Exception):
     """Exception raised when a file is not matching the file type."""
@@ -200,46 +201,49 @@
         if response.status_code != codes.CREATED or response.json().get("file_id") is None:
             raise FailedToUploadFileException(
                 f"Failed to upload file with status code {response.status_code}. response was: {response.text}"
             )
         file_id: UUID = UUID(response.json()["file_id"])
         return file_id
 
-    async def direct_upload_text(
+    async def direct_upload_in_memory(
         self,
         workspace_name: str,
-        text: str,
+        content: Union[bytes, str],
         file_name: str,
         meta: Optional[Dict[str, Any]] = None,
         write_mode: WriteMode = WriteMode.KEEP,
     ) -> UUID:
-        """Directly upload text to deepset Cloud.
+        """Directly upload files to deepset Cloud.
 
         :param workspace_name: Name of the workspace to use.
         :param text: File text to upload.
         :param file_name: Name of the file to upload.
         :param meta: Meta information to attach to the file.
         :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
         Possible options are:
         KEEP - uploads the file with the same name and keeps both files in the workspace.
         OVERWRITE - overwrites the file that is in the workspace.
         FAIL - fails to upload the file with the same name.
         :return: ID of the uploaded file.
         """
-        if not file_name.endswith(".txt"):
+        file_name_suffix = f".{file_name.split('.')[1]}"
+        if file_name_suffix not in SUPPORTED_TYPE_SUFFIXES:
             raise NotMatchingFileTypeException(
-                f"File name {file_name} is not a textfile. Please use '.txt' for text uploads."
+                f"File name {file_name} is not a supported file type. Please use one of {'` '.join(SUPPORTED_TYPE_SUFFIXES)} for text uploads."
             )
 
         response = await self._deepset_cloud_api.post(
             workspace_name,
             "files",
-            data={"text": text, "meta": json.dumps(meta)},
-            params={"write_mode": write_mode.value, "file_name": file_name},
+            files={"file": (file_name, content)},
+            data={"meta": json.dumps(meta)},
+            params={"write_mode": write_mode.value},
         )
+
         if response.status_code != codes.CREATED or response.json().get("file_id") is None:
             raise FailedToUploadFileException(
                 f"Failed to upload file with status code {response.status_code}. response was: {response.text}"
             )
         file_id: UUID = UUID(response.json()["file_id"])
         return file_id
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_api/upload_sessions.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_api/upload_sessions.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_s3/upload.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_s3/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Module for upload-related S3 operations."""
 import asyncio
-import json
 import os
 import re
 from dataclasses import dataclass
 from http import HTTPStatus
 from pathlib import Path
-from typing import Any, Coroutine, List, Optional, Union
+from typing import Any, Coroutine, List, Optional, Sequence, Union
 
 import aiofiles
 import aiohttp
 import structlog
 from pyrate_limiter import Duration, Limiter, Rate
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 from tqdm.asyncio import tqdm
 
 from deepset_cloud_sdk._api.upload_sessions import (
     AWSPrefixedRequestConfig,
     UploadSession,
 )
-from deepset_cloud_sdk.models import DeepsetCloudFile
+from deepset_cloud_sdk.models import DeepsetCloudFileBase
 
 logger = structlog.get_logger(__name__)
 
 
 class RetryableHttpError(Exception):
     """An error that indicates a function should be retried."""
 
@@ -177,22 +176,22 @@
                         "Could not upload a file to deepset Cloud",
                         file_name=file_name,
                         session_id=upload_session.session_id,
                         exception=str(exception),
                     )
                     return S3UploadResult(file_name=file_name, success=False, exception=exception)
 
-    async def upload_from_string(
+    async def upload_from_memory(
         self,
         file_name: str,
         upload_session: UploadSession,
-        content: str,
+        content: Union[bytes, str],
         client_session: aiohttp.ClientSession,
     ) -> S3UploadResult:
-        """Upload text to the prefixed S3 namespace.
+        """Upload content to the prefixed S3 namespace.
 
         :param file_name: Name of the file.
         :param upload_session: UploadSession to associate the upload with.
         :param content: Content of the file.
         :param client_session: The aiohttp ClientSession to use for this request.
         :return: S3UploadResult object.
         """
@@ -263,34 +262,35 @@
 
             for file_path in file_paths:
                 tasks.append(self.upload_from_file(file_path, upload_session, client_session))
 
             result_summary = await self._process_results(tasks, show_progress=show_progress)
             return result_summary
 
-    async def upload_texts(
-        self, upload_session: UploadSession, files: List[DeepsetCloudFile], show_progress: bool = True
+    async def upload_in_memory(
+        self, upload_session: UploadSession, files: Sequence[DeepsetCloudFileBase], show_progress: bool = True
     ) -> S3UploadSummary:
-        """Upload a set of texts to the prefixed S3 namespace given a list of paths.
+        """Upload a set of files to the prefixed S3 namespace given a list of paths.
 
         :param upload_session: UploadSession to associate the upload with.
-        :param files: A list of DeepsetCloudFiles to upload.
+        :param files: A list of DeepsetCloudFileBase to upload.
         :param show_progress: Whether to show a progress bar on the upload.
         :return: S3UploadSummary object.
         """
         async with aiohttp.ClientSession(connector=self.connector) as client_session:
             tasks = []
 
             for file in files:
                 # raw data
                 file_name = file.name
-                tasks.append(self.upload_from_string(file_name, upload_session, file.text, client_session))
+                tasks.append(self.upload_from_memory(file_name, upload_session, file.content(), client_session))
 
                 # meta
                 if file.meta is not None:
                     meta_name = f"{file_name}.meta.json"
-                    metadata = json.dumps(file.meta)
-                    tasks.append(self.upload_from_string(meta_name, upload_session, metadata, client_session))
+                    tasks.append(
+                        self.upload_from_memory(meta_name, upload_session, file.meta_as_string(), client_session)
+                    )
 
             result_summary = await self._process_results(tasks, show_progress=show_progress)
 
             return result_summary
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/_service/files_service.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/_service/files_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 import asyncio
 import json
 import os
 import time
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from pathlib import Path
-from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+)
 from uuid import UUID
 
 import structlog
 from tqdm import tqdm
 from yaspin import yaspin
 
 from deepset_cloud_sdk._api.config import CommonConfig
@@ -27,19 +37,19 @@
     UploadSession,
     UploadSessionDetail,
     UploadSessionsAPI,
     UploadSessionStatus,
     WriteMode,
 )
 from deepset_cloud_sdk._s3.upload import S3, S3UploadResult, S3UploadSummary
-from deepset_cloud_sdk.models import DeepsetCloudFile
+from deepset_cloud_sdk._utils.constants import SUPPORTED_TYPE_SUFFIXES
+from deepset_cloud_sdk.models import DeepsetCloudFileBase
 
 logger = structlog.get_logger(__name__)
 
-SUPPORTED_TYPE_SUFFIXES = [".csv", ".docx", ".html", ".json", ".md", ".txt", ".pdf", ".pptx", ".xlsx", ".xml"]
 META_SUFFIX = ".meta.json"
 DIRECT_UPLOAD_THRESHOLD = 20
 
 
 class FilesService:
     """Service for all file-related operations."""
 
@@ -144,21 +154,26 @@
             )
             logger.info("Successfully uploaded file.", file_path=file_path)
             return S3UploadResult(file_name=file_path.name, success=True)
         except Exception as error:
             logger.error("Failed uploading file.", file_path=file_path, error=error)
             return S3UploadResult(file_name=file_path.name, success=False, exception=error)
 
-    async def _wrapped_direct_upload_text(
-        self, workspace_name: str, text: str, file_name: str, meta: Dict[str, Any], write_mode: WriteMode
+    async def _wrapped_direct_upload_in_memory(
+        self,
+        workspace_name: str,
+        content: Union[str, bytes],
+        file_name: str,
+        meta: Dict[str, Any],
+        write_mode: WriteMode,
     ) -> S3UploadResult:
         try:
-            await self._files.direct_upload_text(
+            await self._files.direct_upload_in_memory(
                 workspace_name=workspace_name,
-                text=text,
+                content=content,
                 meta=meta,
                 file_name=file_name,
                 write_mode=write_mode,
             )
             logger.info("Successfully uploaded file.", file_name=file_name)
             return S3UploadResult(file_name=file_name, success=True)
         except Exception as error:
@@ -486,15 +501,23 @@
         :param show_progress: Shows the upload progress.
         """
         start = time.time()
         logger.info("Start downloading files.", workspace_name=workspace_name)
 
         pbar: Optional[tqdm] = None
         if show_progress:
-            total = (await self._files.list_paginated(workspace_name, limit=1)).total
+            total = (
+                await self._files.list_paginated(
+                    workspace_name,
+                    name=name,
+                    content=content,
+                    odata_filter=odata_filter,
+                    limit=1,
+                )
+            ).total
             pbar = tqdm(total=total, desc="Download Progress")
 
         after_value = None
         after_file_id = None
         has_more: bool = True
         try:
             while has_more:
@@ -531,18 +554,18 @@
                 )
                 if pbar is not None:
                     pbar.update(batch_size)
         finally:
             if pbar is not None:
                 pbar.close()
 
-    async def upload_texts(
+    async def upload_in_memory(
         self,
         workspace_name: str,
-        files: List[DeepsetCloudFile],
+        files: Sequence[DeepsetCloudFileBase],
         write_mode: WriteMode = WriteMode.KEEP,
         blocking: bool = True,
         timeout_s: Optional[int] = None,
         show_progress: bool = True,
     ) -> S3UploadSummary:  # noqa
         """
         Upload a list of raw texts to a workspace using upload sessions. This method accepts a list of DeepsetCloudFiles
@@ -566,19 +589,19 @@
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         if len(files) <= DIRECT_UPLOAD_THRESHOLD:
             logger.info("Uploading files to deepset Cloud.", total_text_files=len(files))
             _coroutines = []
             for file in files:
                 _coroutines.append(
-                    self._wrapped_direct_upload_text(
+                    self._wrapped_direct_upload_in_memory(
                         workspace_name=workspace_name,
                         file_name=file.name,
                         meta=file.meta or {},
-                        text=file.text,
+                        content=file.content(),
                         write_mode=write_mode,
                     )
                 )
             result = await asyncio.gather(*_coroutines)
             logger.info(
                 "Finished uploading files.",
                 number_of_successful_files=len(files),
@@ -589,15 +612,15 @@
                 successful_upload_count=len([r for r in result if r.success]),
                 failed_upload_count=len([r for r in result if r.success is False]),
                 failed=[r for r in result if r.success is False],
             )
 
         # create session to upload files to
         async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
-            upload_summary = await self._s3.upload_texts(
+            upload_summary = await self._s3.upload_in_memory(
                 upload_session=upload_session, files=files, show_progress=show_progress
             )
 
             logger.info(
                 "Summary of S3 Uploads",
                 successful_uploads=upload_summary.successful_upload_count,
                 failed_uploads=upload_summary.failed_upload_count,
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from deepset_cloud_sdk._api.files import File
 from deepset_cloud_sdk._api.upload_sessions import (
     UploadSessionDetail,
     UploadSessionStatus,
     WriteMode,
 )
 from deepset_cloud_sdk._s3.upload import S3UploadSummary
-from deepset_cloud_sdk._service.files_service import DeepsetCloudFile, FilesService
+from deepset_cloud_sdk._service.files_service import FilesService
+from deepset_cloud_sdk.models import DeepsetCloudFile, DeepsetCloudFileBytes
 
 
 def _get_config(api_key: Optional[str] = None, api_url: Optional[str] = None) -> CommonConfig:
     return CommonConfig(api_key=api_key or API_KEY, api_url=api_url or API_URL)
 
 
 async def list_files(
@@ -228,15 +229,52 @@
     FAIL - fails to upload the file with the same name.
     :param blocking: Whether to wait for the files to be listed and displayed in deepset Cloud.
     This may take a couple of minutes.
     :param timeout_s: Timeout in seconds for the `blocking` parameter.
     :param show_progress: Shows the upload progress.
     """
     async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
-        return await file_service.upload_texts(
+        return await file_service.upload_in_memory(
+            workspace_name=workspace_name,
+            files=files,
+            write_mode=write_mode,
+            blocking=blocking,
+            timeout_s=timeout_s,
+            show_progress=show_progress,
+        )
+
+
+async def upload_bytes(
+    files: List[DeepsetCloudFileBytes],
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    write_mode: WriteMode = WriteMode.KEEP,
+    blocking: bool = True,
+    timeout_s: Optional[int] = None,
+    show_progress: bool = True,
+) -> S3UploadSummary:
+    """Upload raw texts to deepset Cloud.
+
+    :param files: List of DeepsetCloudFiles to upload.
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+    Possible options are:
+    KEEP - uploads the file with the same name and keeps both files in the workspace.
+    OVERWRITE - overwrites the file that is in the workspace.
+    FAIL - fails to upload the file with the same name.
+    :param blocking: Whether to wait for the files to be listed and displayed in deepset Cloud.
+    This may take a couple of minutes.
+    :param timeout_s: Timeout in seconds for the `blocking` parameter.
+    :param show_progress: Shows the upload progress.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        return await file_service.upload_in_memory(
             workspace_name=workspace_name,
             files=files,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
             show_progress=show_progress,
         )
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/files.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/sync_client/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 from deepset_cloud_sdk._api.files import File
 from deepset_cloud_sdk._api.upload_sessions import (
     UploadSessionDetail,
     UploadSessionStatus,
     WriteMode,
 )
 from deepset_cloud_sdk._s3.upload import S3UploadSummary
-from deepset_cloud_sdk._service.files_service import DeepsetCloudFile
+from deepset_cloud_sdk.models import DeepsetCloudFile, DeepsetCloudFileBytes
 from deepset_cloud_sdk.workflows.async_client.files import download as async_download
 from deepset_cloud_sdk.workflows.async_client.files import (
     get_upload_session as async_get_upload_session,
 )
 from deepset_cloud_sdk.workflows.async_client.files import (
     list_files as async_list_files,
 )
 from deepset_cloud_sdk.workflows.async_client.files import (
     list_upload_sessions as async_list_upload_sessions,
 )
 from deepset_cloud_sdk.workflows.async_client.files import upload as async_upload
 from deepset_cloud_sdk.workflows.async_client.files import (
+    upload_bytes as async_upload_bytes,
+)
+from deepset_cloud_sdk.workflows.async_client.files import (
     upload_texts as async_upload_texts,
 )
 from deepset_cloud_sdk.workflows.sync_client.utils import iter_over_async
 
 logger = structlog.get_logger(__name__)
 
 
@@ -158,14 +161,53 @@
             files=files,
             api_key=api_key,
             api_url=api_url,
             workspace_name=workspace_name,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
+            show_progress=show_progress,
+        )
+    )
+
+
+def upload_bytes(
+    files: List[DeepsetCloudFileBytes],
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    write_mode: WriteMode = WriteMode.KEEP,
+    blocking: bool = True,
+    timeout_s: Optional[int] = None,
+    show_progress: bool = True,
+) -> S3UploadSummary:
+    """Upload any supported file types to deepset Cloud. These include .csv, .docx, .html, .json, .md, .txt, .pdf, .pptx, .xlsx and .xml.
+
+    :param files: List of DeepsetCloudFilesBytes to upload.
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+    Possible options are:
+    KEEP - uploads the file with the same name and keeps both files in the workspace.
+    OVERWRITE - overwrites the file that is in the workspace.
+    FAIL - fails to upload the file with the same name.
+    :param blocking: Whether to wait for the files to be uploaded and listed in deepset Cloud.
+    :param timeout_s: Timeout in seconds for the `blocking` parameter.
+    :param show_progress: Shows the upload progress.
+    """
+    return asyncio.run(
+        async_upload_bytes(
+            files=files,
+            api_key=api_key,
+            api_url=api_url,
+            workspace_name=workspace_name,
+            write_mode=write_mode,
+            blocking=blocking,
+            timeout_s=timeout_s,
             show_progress=show_progress,
         )
     )
 
 
 def get_upload_session(
     session_id: UUID,
```

### Comparing `deepset_cloud_sdk-1.0.1/deepset_cloud_sdk/workflows/sync_client/utils.py` & `deepset_cloud_sdk-1.0.3/deepset_cloud_sdk/workflows/sync_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/index.md` & `deepset_cloud_sdk-1.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/upload_files.md` & `deepset_cloud_sdk-1.0.3/docs/upload_files.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_images/favicon.svg` & `deepset_cloud_sdk-1.0.3/docs/_images/favicon.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_images/white-logo.svg` & `deepset_cloud_sdk-1.0.3/docs/_images/white-logo.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_pydoc/renderers.py` & `deepset_cloud_sdk-1.0.3/docs/_pydoc/renderers.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/async_client.yml` & `deepset_cloud_sdk-1.0.3/docs/_pydoc/config/async_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/cli.yml` & `deepset_cloud_sdk-1.0.3/docs/_pydoc/config/cli.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/_pydoc/config/sync_client.yml` & `deepset_cloud_sdk-1.0.3/docs/_pydoc/config/sync_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/examples/cli/README.md` & `deepset_cloud_sdk-1.0.3/docs/examples/cli/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/examples/data/example.pdf` & `deepset_cloud_sdk-1.0.3/docs/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/examples/sdk/README.md` & `deepset_cloud_sdk-1.0.3/docs/examples/sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/docs/examples/sdk/upload.py` & `deepset_cloud_sdk-1.0.3/docs/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/.gitignore` & `deepset_cloud_sdk-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/LICENSE` & `deepset_cloud_sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/README.md` & `deepset_cloud_sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-1.0.1/pyproject.toml` & `deepset_cloud_sdk-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "httpx==0.27.0",
   "python-dotenv==1.0.1",
   "typer==0.12.3",
   "tenacity==8.2.3",
   "aiohttp==3.9.5",
   "aiofiles==23.2.1",
   "tabulate==0.9.0",
-  "tqdm==4.66.2",
+  "tqdm==4.66.4",
   "yaspin==2.3.0",
   "pyrate-limiter==3.6.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/deepset-cloud-sdk#readme"
 Issues = "https://github.com/deepset-ai/deepset-cloud-sdk/issues"
```

### Comparing `deepset_cloud_sdk-1.0.1/PKG-INFO` & `deepset_cloud_sdk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deepset-cloud-sdk
-Version: 1.0.1
+Version: 1.0.3
 Summary: deepset Cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -21,15 +21,15 @@
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: httpx==0.27.0
 Requires-Dist: pyrate-limiter==3.6.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tenacity==8.2.3
-Requires-Dist: tqdm==4.66.2
+Requires-Dist: tqdm==4.66.4
 Requires-Dist: typer==0.12.3
 Requires-Dist: yaspin==2.3.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.3 Name: deepset-cloud-sdk Version: 1.0.1 Summary: deepset
+Metadata-Version: 2.3 Name: deepset-cloud-sdk Version: 1.0.3 Summary: deepset
 Cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8 Requires-
 Dist: aiofiles==23.2.1 Requires-Dist: aiohttp==3.9.5 Requires-Dist:
 httpx==0.27.0 Requires-Dist: pyrate-limiter==3.6.0 Requires-Dist: python-
 dotenv==1.0.1 Requires-Dist: structlog==24.1.0 Requires-Dist: tabulate==0.9.0
-Requires-Dist: tenacity==8.2.3 Requires-Dist: tqdm==4.66.2 Requires-Dist:
+Requires-Dist: tenacity==8.2.3 Requires-Dist: tqdm==4.66.4 Requires-Dist:
 typer==0.12.3 Requires-Dist: yaspin==2.3.0 Description-Content-Type: text/
 markdown
                               _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _S_D_K_]
 [![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-
 coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-
 cloud-sdk/tree/python-coverage-comment-action-data) [![Tests](https://
 github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-
```

