# Comparing `tmp/llama_index_readers_microsoft_sharepoint-0.2.2.tar.gz` & `tmp/llama_index_readers_microsoft_sharepoint-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.2.2.tar", max compression
+gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.2.3.tar", max compression
```

## Comparing `llama_index_readers_microsoft_sharepoint-0.2.2.tar` & `llama_index_readers_microsoft_sharepoint-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1782 2024-04-30 21:14:32.067069 llama_index_readers_microsoft_sharepoint-0.2.2/README.md
--rw-r--r--   0        0        0      107 2024-04-30 21:14:32.067069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/__init__.py
--rw-r--r--   0        0        0    19700 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/base.py
--rw-r--r--   0        0        0    41139 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/file_path_info.png
--rw-r--r--   0        0        0     1594 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1782 2024-05-17 17:17:17.120633 llama_index_readers_microsoft_sharepoint-0.2.3/README.md
+-rw-r--r--   0        0        0      107 2024-03-13 22:17:44.729353 llama_index_readers_microsoft_sharepoint-0.2.3/llama_index/readers/microsoft_sharepoint/__init__.py
+-rw-r--r--   0        0        0    28314 2024-05-17 17:33:12.046604 llama_index_readers_microsoft_sharepoint-0.2.3/llama_index/readers/microsoft_sharepoint/base.py
+-rw-r--r--   0        0        0    41139 2024-03-13 22:17:44.729668 llama_index_readers_microsoft_sharepoint-0.2.3/llama_index/readers/microsoft_sharepoint/file_path_info.png
+-rw-r--r--   0        0        0     1601 2024-05-17 17:33:12.046926 llama_index_readers_microsoft_sharepoint-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.2.3/PKG-INFO
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.2/README.md` & `llama_index_readers_microsoft_sharepoint-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 If the files are present in the `Test` folder in SharePoint Site under `root` directory, then the input for the loader for `file_path` is `Test`
 
 ![FilePath](file_path_info.png)
 
 ```python
 from llama_index.readers.microsoft_sharepoint import SharePointReader
 
-loader = SharePointLoader(
+loader = SharePointReader(
     client_id="<Client ID of the app>",
     client_secret="<Client Secret of the app>",
     tenant_id="<Tenant ID of the Microsoft Azure Directory>",
 )
 
 documents = loader.load_data(
     sharepoint_site_name="<Sharepoint Site Name>",
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/base.py` & `llama_index_readers_microsoft_sharepoint-0.2.3/llama_index/readers/microsoft_sharepoint/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """SharePoint files reader."""
 
 import logging
 import os
+from pathlib import Path
 import tempfile
 from typing import Any, Dict, List, Union, Optional
 from typing import Any, Dict, List, Optional
 
 import requests
-from llama_index.core.readers import SimpleDirectoryReader
-from llama_index.core.readers.base import BaseReader, BasePydanticReader
+from llama_index.core.readers import SimpleDirectoryReader, FileSystemReaderMixin
+from llama_index.core.readers.base import (
+    BaseReader,
+    BasePydanticReader,
+    ResourcesReaderMixin,
+)
 from llama_index.core.schema import Document
 from llama_index.core.bridge.pydantic import PrivateAttr, Field
 
 logger = logging.getLogger(__name__)
 
 
-class SharePointReader(BasePydanticReader):
-    """SharePoint reader.
+class SharePointReader(BasePydanticReader, ResourcesReaderMixin, FileSystemReaderMixin):
+    """
+    SharePoint reader.
 
 
     Reads folders from the SharePoint site from a folder under documents.
 
     Args:
         client_id (str): The Application ID for the app registered in Microsoft Azure Portal.
             The application must also be configured with MS Graph permissions "Files.ReadAll", "Sites.ReadAll" and BrowserSiteLists.Read.All.
@@ -117,14 +123,17 @@
 
         Returns:
             str: The ID of the SharePoint site.
 
         Raises:
             Exception: If the specified SharePoint site is not found.
         """
+        if hasattr(self, "_site_id_with_host_name"):
+            return self._site_id_with_host_name
+
         site_information_endpoint = (
             f"https://graph.microsoft.com/v1.0/sites?search={sharepoint_site_name}"
         )
         self._authorization_headers = {"Authorization": f"Bearer {access_token}"}
 
         response = requests.get(
             url=site_information_endpoint,
@@ -153,14 +162,17 @@
 
         Returns:
             str: The ID of the SharePoint site drive.
 
         Raises:
             ValueError: If there is an error in obtaining the drive ID.
         """
+        if hasattr(self, "_drive_id"):
+            return self._drive_id
+
         self._drive_id_endpoint = f"https://graph.microsoft.com/v1.0/sites/{self._site_id_with_host_name}/drives"
 
         response = requests.get(
             url=self._drive_id_endpoint,
             headers=self._authorization_headers,
         )
 
@@ -255,37 +267,54 @@
                     )
                     metadata.update(file_metadata)
             return metadata
         else:
             logger.error(response.json()["error"])
             raise ValueError(response.json()["error"])
 
+    def _get_file_content_by_url(self, item: Dict[str, Any]) -> bytes:
+        """
+        Retrieves the content of the file from the provided URL.
+
+        Args:
+            item (Dict[str, Any]): Dictionary containing file metadata.
+
+        Returns:
+            bytes: The content of the file.
+        """
+        file_download_url = item["@microsoft.graph.downloadUrl"]
+        response = requests.get(file_download_url)
+        if response.status_code != 200:
+            logger.error(response.json()["error"])
+            raise ValueError(response.json()["error_description"])
+
+        return response.content
+
     def _download_file_by_url(self, item: Dict[str, Any], download_dir: str) -> str:
         """
         Downloads the file from the provided URL.
 
         Args:
             item (Dict[str, Any]): Dictionary containing file metadata.
             download_dir (str): The directory where the files should be downloaded.
 
         Returns:
             str: The path of the downloaded file in the temporary directory.
         """
         # Get the download URL for the file.
-        file_download_url = item["@microsoft.graph.downloadUrl"]
         file_name = item["name"]
 
-        response = requests.get(file_download_url)
+        content = self._get_file_content_by_url(item)
 
         # Create the directory if it does not exist and save the file.
         if not os.path.exists(download_dir):
             os.makedirs(download_dir)
         file_path = os.path.join(download_dir, file_name)
         with open(file_path, "wb") as f:
-            f.write(response.content)
+            f.write(content)
 
         return file_path
 
     def _get_permissions_info(self, item: Dict[str, Any]) -> Dict[str, str]:
         """
         Extracts the permissions information for the file. For more information, see:
         https://learn.microsoft.com/en-us/graph/api/resources/permission?view=graph-rest-1.0.
@@ -333,14 +362,21 @@
                     permissions_dict[ids_key] = []
                 if display_names_key not in permissions_dict:
                     permissions_dict[display_names_key] = []
 
                 permissions_dict[ids_key].append(id)
                 permissions_dict[display_names_key].append(display_name)
 
+        # sort to get consistent results, if possible
+        for key in permissions_dict:
+            try:
+                permissions_dict[key] = sorted(permissions_dict[key])
+            except TypeError:
+                pass
+
         return permissions_dict
 
     def _extract_metadata_for_file(self, item: Dict[str, Any]) -> Dict[str, str]:
         """
         Extracts metadata related to the file.
 
         Parameters:
@@ -527,7 +563,216 @@
                 # return self.files_metadata
                 return self._load_documents_with_metadata(
                     files_metadata, temp_dir, recursive
                 )
 
         except Exception as exp:
             logger.error("An error occurred while accessing SharePoint: %s", exp)
+
+    def _list_folder_contents(
+        self, folder_id: str, recursive: bool, current_path: str
+    ) -> List[Path]:
+        """
+        Helper method to fetch the contents of a folder.
+
+        Args:
+            folder_id (str): ID of the folder whose contents are to be listed.
+            recursive (bool): Whether to include subfolders recursively.
+
+        Returns:
+            List[Path]: List of file paths.
+        """
+        folder_contents_endpoint = (
+            f"{self._drive_id_endpoint}/{self._drive_id}/items/{folder_id}/children"
+        )
+        response = requests.get(
+            url=folder_contents_endpoint,
+            headers=self._authorization_headers,
+        )
+        items = response.json().get("value", [])
+
+        file_paths = []
+        for item in items:
+            if "folder" in item and recursive:
+                # Recursive call for subfolder
+                subfolder_id = item["id"]
+                subfolder_paths = self._list_folder_contents(
+                    subfolder_id, recursive, os.path.join(current_path, item["name"])
+                )
+                file_paths.extend(subfolder_paths)
+            elif "file" in item:
+                # Append file path
+                file_path = Path(os.path.join(current_path, item["name"]))
+                file_paths.append(file_path)
+
+        return file_paths
+
+    def list_resources(
+        self,
+        sharepoint_site_name: Optional[str] = None,
+        sharepoint_folder_path: Optional[str] = None,
+        sharepoint_folder_id: Optional[str] = None,
+        recursive: bool = True,
+    ) -> List[Path]:
+        """
+        Lists the files in the specified folder in the SharePoint site.
+
+        Args:
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            List[Path]: A list of paths of the files in the specified folder.
+
+        Raises:
+            Exception: If an error occurs while accessing SharePoint site.
+        """
+        # If no arguments are provided to load_data, default to the object attributes
+        if not sharepoint_site_name:
+            sharepoint_site_name = self.sharepoint_site_name
+
+        if not sharepoint_folder_path:
+            sharepoint_folder_path = self.sharepoint_folder_path
+
+        if not sharepoint_folder_id:
+            sharepoint_folder_id = self.sharepoint_folder_id
+
+        # TODO: make both of these values optional — and just default to the client ID defaults
+        if not sharepoint_site_name:
+            raise ValueError("sharepoint_site_name must be provided.")
+
+        if not sharepoint_folder_path and not sharepoint_folder_id:
+            raise ValueError(
+                "sharepoint_folder_path or sharepoint_folder_id must be provided."
+            )
+
+        file_paths = []
+        try:
+            access_token = self._get_access_token()
+            self._site_id_with_host_name = self._get_site_id_with_host_name(
+                access_token, sharepoint_site_name
+            )
+            self._drive_id = self._get_drive_id()
+            if not sharepoint_folder_id:
+                sharepoint_folder_id = self._get_sharepoint_folder_id(
+                    sharepoint_folder_path
+                )
+
+            # Fetch folder contents
+            folder_contents = self._list_folder_contents(
+                sharepoint_folder_id,
+                recursive,
+                os.path.join(sharepoint_site_name, sharepoint_folder_path),
+            )
+            file_paths.extend(folder_contents)
+            return file_paths
+
+        except Exception as exp:
+            logger.error("An error occurred while listing files in SharePoint: %s", exp)
+            raise
+
+        return file_paths
+
+    def _get_item_from_path(self, input_file: Path) -> Dict[str, Any]:
+        """
+        Retrieves the item details for a specified file in SharePoint.
+
+        Args:
+            input_file (Path): The path of the file in SharePoint.
+                Should include the SharePoint site name and the folder path. e.g. "site_name/folder_path/file_name".
+
+        Returns:
+            Dict[str, Any]: Dictionary containing the item details.
+        """
+        # Get the file ID
+        # remove the site_name prefix
+        file_path = (
+            str(input_file).lstrip("/").replace(f"{self.sharepoint_site_name}/", "", 1)
+        )
+        endpoint = f"{self._drive_id_endpoint}/{self._drive_id}/root:/{file_path}"
+
+        response = requests.get(
+            url=endpoint,
+            headers=self._authorization_headers,
+        )
+
+        return response.json()
+
+    def get_resource_info(self, resource_id: str, **kwargs) -> Dict:
+        """
+        Retrieves metadata for a specified file in SharePoint without downloading it.
+
+        Args:
+            input_file (Path): The path of the file in SharePoint. The path should include
+                                the SharePoint site name and the folder path. e.g. "site_name/folder_path/file_name".
+        """
+        try:
+            item = self._get_item_from_path(Path(resource_id))
+
+            info_dict = {
+                "file_path": resource_id,
+                "size": item.get("size"),
+                "created_at": item.get("createdDateTime"),
+                "modified_at": item.get("lastModifiedDateTime"),
+                "etag": item.get("eTag"),
+            }
+
+            if (
+                self.attach_permission_metadata
+            ):  # changes in access control should trigger a reingestion of the file
+                permissions = self._get_permissions_info(item)
+                info_dict.update(permissions)
+
+            return {
+                meta_key: meta_value
+                for meta_key, meta_value in info_dict.items()
+                if meta_value is not None
+            }
+
+        except Exception as exp:
+            logger.error(
+                "An error occurred while fetching file information from SharePoint: %s",
+                exp,
+            )
+            raise
+
+    def load_resource(self, resource_id: str, **kwargs) -> List[Document]:
+        try:
+            access_token = self._get_access_token()
+            self._site_id_with_host_name = self._get_site_id_with_host_name(
+                access_token, self.sharepoint_site_name
+            )
+            self._drive_id = self._get_drive_id()
+
+            path = Path(resource_id)
+
+            item = self._get_item_from_path(path)
+
+            input_file_dir = path.parent
+
+            with tempfile.TemporaryDirectory() as temp_dir:
+                metadata = self._download_file(item, temp_dir, input_file_dir)
+                return self._load_documents_with_metadata(
+                    metadata, temp_dir, recursive=False
+                )
+
+        except Exception as exp:
+            logger.error(
+                "An error occurred while reading file from SharePoint: %s", exp
+            )
+            raise
+
+    def read_file_content(self, input_file: Path, **kwargs) -> bytes:
+        try:
+            access_token = self._get_access_token()
+            self._site_id_with_host_name = self._get_site_id_with_host_name(
+                access_token, self.sharepoint_site_name
+            )
+            self._drive_id = self._get_drive_id()
+
+            item = self._get_item_from_path(input_file)
+            return self._get_file_content_by_url(item)
+
+        except Exception as exp:
+            logger.error(
+                "An error occurred while reading file content from SharePoint: %s", exp
+            )
+            raise
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/file_path_info.png` & `llama_index_readers_microsoft_sharepoint-0.2.3/llama_index/readers/microsoft_sharepoint/file_path_info.png`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.2/pyproject.toml` & `llama_index_readers_microsoft_sharepoint-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 description = "llama-index readers microsoft_sharepoint integration"
 exclude = ["**/BUILD"]
 keywords = ["microsoft 365", "microsoft365", "sharepoint"]
 license = "MIT"
 maintainers = ["arun-soliton"]
 name = "llama-index-readers-microsoft-sharepoint"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.37.post1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.2/PKG-INFO` & `llama_index_readers_microsoft_sharepoint-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-microsoft-sharepoint
-Version: 0.2.2
+Version: 0.2.3
 Summary: llama-index readers microsoft_sharepoint integration
 License: MIT
 Keywords: microsoft 365,microsoft365,sharepoint
 Author: Your Name
 Author-email: you@example.com
 Maintainer: arun-soliton
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: llama-index-core (>=0.10.37.post1,<0.11.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Microsoft SharePoint Reader
 
 ```bash
 pip install llama-index-readers-microsoft-sharepoint
@@ -48,15 +49,15 @@
 If the files are present in the `Test` folder in SharePoint Site under `root` directory, then the input for the loader for `file_path` is `Test`
 
 ![FilePath](file_path_info.png)
 
 ```python
 from llama_index.readers.microsoft_sharepoint import SharePointReader
 
-loader = SharePointLoader(
+loader = SharePointReader(
     client_id="<Client ID of the app>",
     client_secret="<Client Secret of the app>",
     tenant_id="<Tenant ID of the Microsoft Azure Directory>",
 )
 
 documents = loader.load_data(
     sharepoint_site_name="<Sharepoint Site Name>",
```

