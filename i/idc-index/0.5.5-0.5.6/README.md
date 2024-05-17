# Comparing `tmp/idc_index-0.5.5.tar.gz` & `tmp/idc_index-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May  9 19:55:58 2024, max compression
+gzip compressed data, last modified: Fri May 17 21:32:59 2024, max compression
```

## Comparing `idc_index-0.5.5.tar` & `idc_index-0.5.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      125 2024-05-09 19:55:58.000000 idc_index-0.5.5/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-09 19:55:58.000000 idc_index-0.5.5/.gitattributes
--rw-r--r--   0        0        0     2357 2024-05-09 19:55:58.000000 idc_index-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-09 19:55:58.000000 idc_index-0.5.5/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-05-09 19:55:58.000000 idc_index-0.5.5/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1585 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-05-09 19:55:58.000000 idc_index-0.5.5/docs/conf.py
--rw-r--r--   0        0        0      196 2024-05-09 19:55:58.000000 idc_index-0.5.5/docs/index.md
--rw-r--r--   0        0        0      263 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/_version.pyi
--rw-r--r--   0        0        0    61680 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0    13853 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      279 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_bogus.s5cmd
--rw-r--r--   0        0        0      419 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-05-09 19:55:58.000000 idc_index-0.5.5/.gitignore
--rw-r--r--   0        0        0     1077 2024-05-09 19:55:58.000000 idc_index-0.5.5/LICENSE
--rw-r--r--   0        0        0     4290 2024-05-09 19:55:58.000000 idc_index-0.5.5/README.md
--rw-r--r--   0        0        0     6130 2024-05-09 19:55:58.000000 idc_index-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     7551 2024-05-09 19:55:58.000000 idc_index-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-17 21:32:59.000000 idc_index-0.5.6/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-17 21:32:59.000000 idc_index-0.5.6/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-17 21:32:59.000000 idc_index-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-17 21:32:59.000000 idc_index-0.5.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-17 21:32:59.000000 idc_index-0.5.6/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1585 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      920 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/conf.py
+-rw-r--r--   0        0        0      662 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/index.md
+-rw-r--r--   0        0        0      278 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/api/idc_index.rst
+-rw-r--r--   0        0        0      262 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/_version.pyi
+-rw-r--r--   0        0        0    64739 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0    14639 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      279 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_bogus.s5cmd
+-rw-r--r--   0        0        0      419 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-17 21:32:59.000000 idc_index-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-17 21:32:59.000000 idc_index-0.5.6/LICENSE
+-rw-r--r--   0        0        0     4303 2024-05-17 21:32:59.000000 idc_index-0.5.6/README.md
+-rw-r--r--   0        0        0     6269 2024-05-17 21:32:59.000000 idc_index-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     7588 2024-05-17 21:32:59.000000 idc_index-0.5.6/PKG-INFO
```

### Comparing `idc_index-0.5.5/.pre-commit-config.yaml` & `idc_index-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/noxfile.py` & `idc_index-0.5.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/.github/CONTRIBUTING.md` & `idc_index-0.5.6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/.github/matchers/pylint.json` & `idc_index-0.5.6/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/.github/workflows/cd.yml` & `idc_index-0.5.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/.github/workflows/ci.yml` & `idc_index-0.5.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/docs/conf.py` & `idc_index-0.5.6/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 myst_enable_extensions = [
     "colon_fence",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
+    "pandas": ("http://pandas.pydata.org/pandas-docs/stable", None),
 }
 
 nitpick_ignore = [
     ("py:class", "_io.StringIO"),
     ("py:class", "_io.BytesIO"),
 ]
```

### Comparing `idc_index-0.5.5/idc_index/index.py` & `idc_index-0.5.6/idc_index/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,38 @@
 from importlib.metadata import distribution
 from pathlib import Path
 
 import duckdb
 import idc_index_data
 import pandas as pd
 import psutil
+import requests
 from packaging.version import Version
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.DEBUG)
+logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.INFO)
 
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
 
 
 class IDCClient:
+    # Default download hierarchy template
     DOWNLOAD_HIERARCHY_DEFAULT = (
         "%collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID"
     )
 
+    # Defined citation formats that can be passed to the citations request methods
+    # see acceptable values at https://citation.crosscite.org/docs.html#sec-4
+    CITATION_FORMAT_APA = "text/x-bibliography; style=apa; locale=en-US"
+    CITATION_FORMAT_TURTLE = "text/turtle"
+    CITATION_FORMAT_JSON = "application/vnd.citationstyles.csl+json"
+    CITATION_FORMAT_BIBTEX = "application/x-bibtex"
+
     def __init__(self):
         file_path = idc_index_data.IDC_INDEX_PARQUET_FILEPATH
 
         # Read index file
         logger.debug(f"Reading index file v{idc_index_data.__version__}")
         self.index = pd.read_parquet(file_path)
         # self.index = self.index.astype(str).replace("nan", "")
@@ -74,14 +83,57 @@
         filtered_df = dataframe[dataframe[key].isin(values)].copy()
         if filtered_df.empty:
             error_message = f"No data found for the {key} with the values {values}."
             raise ValueError(error_message)
         return filtered_df
 
     @staticmethod
+    def _safe_filter_by_selection(
+        df_index, collection_id, patientId, studyInstanceUID, seriesInstanceUID
+    ):
+        if collection_id is not None:
+            if not isinstance(collection_id, str) and not isinstance(
+                collection_id, list
+            ):
+                raise TypeError("collection_id must be a string or list of strings")
+        if patientId is not None:
+            if not isinstance(patientId, str) and not isinstance(patientId, list):
+                raise TypeError("patientId must be a string or list of strings")
+        if studyInstanceUID is not None:
+            if not isinstance(studyInstanceUID, str) and not isinstance(
+                studyInstanceUID, list
+            ):
+                raise TypeError("studyInstanceUID must be a string or list of strings")
+        if seriesInstanceUID is not None:
+            if not isinstance(seriesInstanceUID, str) and not isinstance(
+                seriesInstanceUID, list
+            ):
+                raise TypeError("seriesInstanceUID must be a string or list of strings")
+
+        if collection_id is not None:
+            result_df = IDCClient._filter_by_collection_id(df_index, collection_id)
+        else:
+            result_df = df_index
+
+        if patientId is not None:
+            result_df = IDCClient._filter_by_patient_id(result_df, patientId)
+
+        if studyInstanceUID is not None:
+            result_df = IDCClient._filter_by_dicom_study_uid(
+                result_df, studyInstanceUID
+            )
+
+        if seriesInstanceUID is not None:
+            result_df = IDCClient._filter_by_dicom_series_uid(
+                result_df, seriesInstanceUID
+            )
+
+        return result_df
+
+    @staticmethod
     def _filter_by_collection_id(df_index, collection_id):
         return IDCClient._filter_dataframe_by_id(
             "collection_id", df_index, collection_id
         )
 
     @staticmethod
     def _filter_by_patient_id(df_index, patient_id):
@@ -113,37 +165,44 @@
         """
         unique_collections = self.index["collection_id"].unique()
         return unique_collections.tolist()
 
     def get_series_size(self, seriesInstanceUID):
         """
         Gets cumulative size (MB) of the DICOM instances in a given SeriesInstanceUID.
+
         Args:
             seriesInstanceUID (str): The DICOM SeriesInstanceUID.
+
         Returns:
             float: The cumulative size of the DICOM instances in the given SeriesInstanceUID rounded to two digits, in MB.
+
         Raises:
             ValueError: If the `seriesInstanceUID` does not exist.
         """
 
         resp = self.index[["SeriesInstanceUID"] == seriesInstanceUID][
             "series_size_MB"
         ].iloc[0]
         return resp
 
     def get_patients(self, collection_id, outputFormat="dict"):
         """
         Gets the patients in a collection.
+
         Args:
-            collection_id (str or a list of str): The collection id or list of collection ids. This should be in lower case separated by underscores.
-                                For example, 'pdmr_texture_analysis'. or ['pdmr_texture_analysis','nlst']
-            outputFormat (str, optional): The format in which to return the patient IDs. Available options are 'dict',
-                                        'df', and 'list'. Default is 'dict'.
+            collection_id (str or list[str]): The collection id or list of collection ids. This should be in lower case separated by underscores.
+                For example, 'pdmr_texture_analysis'. or ['pdmr_texture_analysis','nlst']
+
+            outputFormat (str): The format in which to return the patient IDs. Available options are 'dict',
+                'df', and 'list'. Default is 'dict'.
+
         Returns:
             dict or pandas.DataFrame or list: Patient IDs in the requested output format. By default, it returns a dictionary.
+
         Raises:
             ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
         """
 
         if not isinstance(collection_id, str) and not isinstance(collection_id, list):
             raise TypeError("collection_id must be a string or list of strings")
 
@@ -177,20 +236,24 @@
         logger.debug("Get patient response: %s", str(response))
 
         return response
 
     def get_dicom_studies(self, patientId, outputFormat="dict"):
         """
         Returns Studies for a given patient or list of patients.
+
         Args:
             patientId (str or list of str): The patient Id or a list of patient Ids.
-            outputFormat (str, optional): The format in which to return the studies. Available options are 'dict',
-                                        'df', and 'list'. Default is 'dict'.
+
+            outputFormat (str): The format in which to return the studies. Available options are 'dict',
+                'df', and 'list'. Default is 'dict'.
+
         Returns:
             dict or pandas.DataFrame or list: Studies in the requested output format. By default, it returns a dictionary.
+
         Raises:
             ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
             ValueError: If any of the `patientId` does not exist.
         """
 
         if not isinstance(patientId, str) and not isinstance(patientId, list):
             raise TypeError("patientId must be a string or list of strings")
@@ -226,20 +289,24 @@
         logger.debug("Get patient study response: %s", str(response))
 
         return response
 
     def get_dicom_series(self, studyInstanceUID, outputFormat="dict"):
         """
         Returns Series for a given study or list of studies.
+
         Args:
             studyInstanceUID (str or list of str): The DICOM StudyInstanceUID or a list of StudyInstanceUIDs.
-            outputFormat (str, optional): The format in which to return the series. Available options are 'dict',
-                                        'df', and 'list'. Default is 'dict'.
+
+            outputFormat (str): The format in which to return the series. Available options are 'dict',
+                'df', and 'list'. Default is 'dict'.
+
         Returns:
             dict or pandas.DataFrame or list: Series in the requested output format. By default, it returns a dictionary.
+
         Raises:
             ValueError: If `outputFormat` is not one of 'dict', 'df', 'list'.
             ValueError: If any of the `studyInstanceUID` does not exist.
         """
 
         if not isinstance(studyInstanceUID, str) and not isinstance(
             studyInstanceUID, list
@@ -350,21 +417,21 @@
         will be used (OHIF v2 or v3 for radiology modalities, and Slim for SM).
 
         This function will validate the provided SeriesInstanceUID or StudyInstanceUID against IDC
         index to ensure that the series or study is available in IDC.
 
         Args:
             SeriesInstanceUID: string containing the value of DICOM SeriesInstanceUID for a series
-            available in IDC
+                available in IDC
 
             StudyInstanceUID: string containing the value of DICOM SeriesInstanceUID for a series
-            available in IDC
+                available in IDC
 
             viewer_selector: string containing the name of the viewer to use. Must be one of the following:
-            ohif_v2, ohif_v3, or slim. If not provided, default viewers will be used.
+                ohif_v2, ohif_v3, or slim. If not provided, default viewers will be used.
 
         Returns:
             string containing the IDC viewer URL for the given SeriesInstanceUID
         """
 
         if seriesInstanceUID is None and studyInstanceUID is None:
             raise ValueError(
@@ -416,14 +483,15 @@
                 index
             WHERE
                 StudyInstanceUID='{studyInstanceUID}'
             """
             query_result = self.sql_query(query)
             modality = query_result.Modality[0]
 
+        viewer_url = None
         if viewer_selector is None:
             if "SM" in modality:
                 viewer_selector = "slim"
             else:
                 viewer_selector = "ohif_v2"
 
         if viewer_selector == "ohif_v2":
@@ -434,15 +502,15 @@
         elif viewer_selector == "ohif_v3":
             if seriesInstanceUID is None:
                 viewer_url = f"https://viewer.imaging.datacommons.cancer.gov/v3/viewer/?StudyInstanceUIDs={studyInstanceUID}"
             else:
                 viewer_url = f"https://viewer.imaging.datacommons.cancer.gov/v3/viewer/?StudyInstanceUIDs={studyInstanceUID}&SeriesInstanceUID={seriesInstanceUID}"
         elif viewer_selector == "volview":
             # TODO! Not implemented yet
-            pass
+            viewer_url = None
         elif viewer_selector == "slim":
             if seriesInstanceUID is None:
                 viewer_url = f"https://viewer.imaging.datacommons.cancer.gov/slim/studies/{studyInstanceUID}"
             else:
                 viewer_url = f"https://viewer.imaging.datacommons.cancer.gov/slim/studies/{studyInstanceUID}/series/{seriesInstanceUID}"
 
         return viewer_url
@@ -457,17 +525,17 @@
     ) -> tuple[float, str, Path]:
         """
         Validates the manifest file by checking the URLs in the manifest
 
         Args:
             manifestFile (str): The path to the manifest file.
             downloadDir (str): The path to the download directory.
-            validate_manifest (bool, optional): If True, validates the manifest for any errors. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            validate_manifest (bool): If True, validates the manifest for any errors. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): A template string for the directory path. Must start with %. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT. It can contain attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) wrapped in '%'. Special characters can be used as connectors: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). Can be disabled by None.
 
         Returns:
             total_size (float): The total size of all series in the manifest file.
             endpoint_to_use (str): The endpoint URL to use (either AWS or GCP).
             temp_manifest_file(Path): Path to the temporary manifest file for downstream steps
         Raises:
@@ -531,14 +599,16 @@
                 index_temp
             ON
                 index_temp.index_crdc_series_uuid = manifest_temp.manifest_crdc_series_uuid
         """
         # ruff: noqa: end
         merged_df = duckdb.query(sql).df()
 
+        endpoint_to_use = None
+
         if validate_manifest:
             # Check if crdc_instance_uuid is found in the index
             if not all(merged_df["crdc_series_uuid_match"]):
                 missing_manifest_cp_cmds = merged_df.loc[
                     ~merged_df["crdc_series_uuid_match"], "manifest_cp_cmd"
                 ]
                 missing_manifest_cp_cmds_str = f"The following manifest copy commands do not have any associated series in the index: {missing_manifest_cp_cmds.tolist()}"
@@ -874,17 +944,17 @@
         to the console.
 
         Args:
             endpoint_to_use (str): The endpoint URL to download the files from.
             manifest_file (str): The path to the manifest file listing the files to be downloaded.
             total_size (float): The total size of the files to be downloaded in MB.
             downloadDir (str): The local directory where the files will be downloaded.
-            quiet (bool, optional): If True, suppresses the stdout and stderr of the s5cmd command.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the stdout and stderr of the s5cmd command.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template.
 
         Raises:
             subprocess.CalledProcessError: If the s5cmd command fails.
 
         Returns:
             None
@@ -1063,18 +1133,18 @@
         is first validated to ensure every line contains a valid urls. It then
         gets the total size to be downloaded and runs download process on one
         process and download progress on another process.
 
         Args:
             manifestFile (str): The path to the manifest file.
             downloadDir (str): The directory to download the files to.
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
-            validate_manifest (bool, optional): If True, validates the manifest for any errors. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True.
+            validate_manifest (bool): If True, validates the manifest for any errors. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Raises:
             ValueError: If the download directory does not exist.
         """
 
         downloadDir = os.path.abspath(downloadDir).replace("\\", "/")
@@ -1106,14 +1176,70 @@
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
             dirTemplate=dirTemplate,
             list_of_directories=list_of_directories,
         )
 
+    def citations_from_selection(
+        self,
+        collection_id=None,
+        patientId=None,
+        studyInstanceUID=None,
+        seriesInstanceUID=None,
+        citation_format=CITATION_FORMAT_APA,
+    ):
+        """Get the list of publications that should be cited/attributed for the specific collection, patient (case) ID, study or series UID.
+
+        Args:
+            collection_id: string or list of strings containing the values of collection_id to filter by
+            patientId: string or list of strings containing the values of PatientID to filter by
+            studyInstanceUID: string or list of strings containing the values of DICOM StudyInstanceUID to filter by
+            seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
+            format: string containing the format of the citation. Must be one of the following: CITATION_FORMAT_APA, CITATION_FORMAT_BIBTEX, CITATION_FORMAT_JSON. Defaults to CITATION_FORMAT_APA. Can be initialized to the alternative formats as allowed by DOI API, see https://citation.crosscite.org/docs.html#sec-4.
+        """
+        result_df = self._safe_filter_by_selection(
+            self.index,
+            collection_id=collection_id,
+            patientId=patientId,
+            studyInstanceUID=studyInstanceUID,
+            seriesInstanceUID=seriesInstanceUID,
+        )
+
+        citations = []
+
+        if not result_df.empty:
+            distinct_dois = result_df["source_DOI"].unique().tolist()
+
+            if len(distinct_dois) == 0:
+                logger.error("No DOIs found for the selection.")
+                return citations
+
+            # include citation for the currently main IDC publication
+            # https://doi.org/10.1148/rg.230180
+            distinct_dois.append("10.1148/rg.230180")
+
+            headers = {"accept": citation_format}
+            timeout = 30
+
+            for doi in distinct_dois:
+                url = "https://dx.doi.org/" + doi
+
+                response = requests.get(url, headers=headers, timeout=timeout)
+
+                if response.status_code == 200:
+                    if citation_format == self.CITATION_FORMAT_JSON:
+                        citations.append(response.json())
+                    else:
+                        citations.append(response.text)
+                else:
+                    logger.error(f"Failed to get citation for DOI: {url}")
+
+        return citations
+
     def download_from_selection(
         self,
         downloadDir,
         dry_run=False,
         collection_id=None,
         patientId=None,
         studyInstanceUID=None,
@@ -1129,74 +1255,46 @@
         Args:
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             collection_id: string or list of strings containing the values of collection_id to filter by
             patientId: string or list of strings containing the values of PatientID to filter by
             studyInstanceUID: string or list of strings containing the values of DICOM StudyInstanceUID to filter by
             seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         """
 
         downloadDir = os.path.abspath(downloadDir).replace("\\", "/")
         if not os.path.exists(downloadDir):
             raise ValueError("Download directory does not exist.")
 
-        if collection_id is not None:
-            if not isinstance(collection_id, str) and not isinstance(
-                collection_id, list
-            ):
-                raise TypeError("collection_id must be a string or list of strings")
-        if patientId is not None:
-            if not isinstance(patientId, str) and not isinstance(patientId, list):
-                raise TypeError("patientId must be a string or list of strings")
-        if studyInstanceUID is not None:
-            if not isinstance(studyInstanceUID, str) and not isinstance(
-                studyInstanceUID, list
-            ):
-                raise TypeError("studyInstanceUID must be a string or list of strings")
-        if seriesInstanceUID is not None:
-            if not isinstance(seriesInstanceUID, str) and not isinstance(
-                seriesInstanceUID, list
-            ):
-                raise TypeError("seriesInstanceUID must be a string or list of strings")
-
-        if collection_id is not None:
-            result_df = self._filter_by_collection_id(self.index, collection_id)
-        else:
-            result_df = self.index
-
-        if patientId is not None:
-            result_df = self._filter_by_patient_id(result_df, patientId)
-
-        if studyInstanceUID is not None:
-            result_df = self._filter_by_dicom_study_uid(result_df, studyInstanceUID)
-
-        if seriesInstanceUID is not None:
-            result_df = self._filter_by_dicom_series_uid(result_df, seriesInstanceUID)
+        result_df = self._safe_filter_by_selection(
+            self.index,
+            collection_id=collection_id,
+            patientId=patientId,
+            studyInstanceUID=studyInstanceUID,
+            seriesInstanceUID=seriesInstanceUID,
+        )
 
         total_size = round(result_df["series_size_MB"].sum(), 2)
-        logger.info(
-            "Total size of files to download: " + str(float(total_size) / 1000) + "GB"
-        )
+        logger.info("Total size of files to download: " + self._format_size(total_size))
         logger.info(
             "Total free space on disk: "
             + str(psutil.disk_usage(downloadDir).free / (1000 * 1000 * 1000))
             + "GB"
         )
 
         if dry_run:
             logger.info(
                 "Dry run. Not downloading files. Rerun with dry_run=False to download the files."
             )
-        else:
-            logger.info("Total size: " + self._format_size(total_size))
+            return
 
         if dirTemplate is not None:
             hierarchy = self._generate_sql_concat_for_building_directory(
                 downloadDir=downloadDir,
                 dirTemplate=dirTemplate,
             )
             sql = f"""
@@ -1271,17 +1369,17 @@
         """
         Download the files corresponding to the seriesInstanceUID to the specified directory.
 
         Args:
             seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If seriesInstanceUID(s) passed is(are) not a string or list
 
@@ -1309,17 +1407,17 @@
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             studyInstanceUID: string or list of strings containing the values of DICOM studyInstanceUID to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If seriesInstanceUID(s) passed is(are) not a string or list
 
@@ -1347,17 +1445,17 @@
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             patientId: string or list of strings containing the values of DICOM patientId to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If patientId(s) passed is(are) not a string or list
 
@@ -1385,17 +1483,17 @@
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             collection_id: string or list of strings containing the values of DICOM patientId to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
-            show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            quiet (bool): If True, suppresses the output of the subprocess. Defaults to True.
+            show_progress_bar (bool): If True, tracks the progress of download
+            use_s5cmd_sync (bool): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
             dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If collection_id(s) passed is(are) not a string or list
 
@@ -1416,12 +1514,12 @@
         Args:
             sql_query: string containing the SQL query to execute. The table name to use in the FROM clause is 'index' (without quotes).
 
         Returns:
             pandas dataframe containing the results of the query
 
         Raises:
-            any exception that duckdb.query() raises
+            duckdb.Error: any exception that duckdb.query() raises
         """
 
         index = self.index
         return duckdb.query(sql_query).to_df()
```

### Comparing `idc_index-0.5.5/tests/idcindex.py` & `idc_index-0.5.6/tests/idcindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,10 +347,29 @@
                     validate_manifest=validate_manifest,
                     show_progress_bar=show_progress_bar,
                     use_s5cmd_sync=use_s5cmd_sync,
                 )
 
                 self.assertEqual(len(os.listdir(temp_dir)), 0)
 
+    def test_citations(self):
+        citations = self.client.citations_from_selection(
+            collection_id="tcga_gbm",
+            citation_format=index.IDCClient.CITATION_FORMAT_APA,
+        )
+        self.assertIsNotNone(citations)
+
+        citations = self.client.citations_from_selection(
+            seriesInstanceUID="1.3.6.1.4.1.14519.5.2.1.7695.4164.588007658875211151397302775781",
+            citation_format=index.IDCClient.CITATION_FORMAT_BIBTEX,
+        )
+        self.assertIsNotNone(citations)
+
+        citations = self.client.citations_from_selection(
+            studyInstanceUID="1.2.840.113654.2.55.174144834924218414213677353968537663991",
+            citation_format=index.IDCClient.CITATION_FORMAT_BIBTEX,
+        )
+        self.assertIsNotNone(citations)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `idc_index-0.5.5/.gitignore` & `idc_index-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/LICENSE` & `idc_index-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.5/README.md` & `idc_index-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 [![Documentation Status][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 [![Discourse Forum][discourse-forum-badge]][discourse-forum-link]
 
+> [!WARNING]
+>
+> This package is in its early development stages. Its functionality and API
+> will change.
+>
+> Stay tuned for the updates and documentation, and please share your feedback
+> about it by opening issues in this repository, or by starting a discussion in
+> [IDC User forum](https://discourse.canceridc.dev/).
+
 <!-- SPHINX-START -->
 
 ## About
 
 `idc-index` is a Python package that enables query of the basic metadata and
 download of DICOM files hosted by the
 [NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
 
-👷 🚧 This package is in its early development stages. Its functionality and API
-will change. Stay tuned for the updates and documentation, and please share your
-feedback about it by opening issues in this repository, or by starting a
-discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
-
 ## Usage
 
 There are no prerequisites - just install the package ...
 
 ```bash
 $ pip install idc-index
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `idc_index-0.5.5/pyproject.toml` & `idc_index-0.5.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 dependencies = [
   'duckdb>=0.10.0',
   "idc-index-data==18.0.1",
   "packaging",
   "pandas<2.2",
   "psutil",
   "pyarrow",
+  "requests",
   "s5cmd",
   "tqdm"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
@@ -123,14 +124,15 @@
 
 [tool.ruff.lint]
 extend-select = [
   "B",        # flake8-bugbear
   "I",        # isort
   "ARG",      # flake8-unused-arguments
   "C4",       # flake8-comprehensions
+  "D",        # pydocstyle
   "EM",       # flake8-errmsg
   "ICN",      # flake8-import-conventions
   "G",        # flake8-logging-format
   "PGH",      # pygrep-hooks
   "PIE",      # flake8-pie
   "PL",       # pylint
   "PT",       # flake8-pytest-style
@@ -176,16 +178,26 @@
   "T201",     # print found
 ]
 isort.required-imports = ["from __future__ import annotations"]
 # Uncomment if using a _compat.typing backport
 # typing-modules = ["idc_index._compat.typing"]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/**" = ["T20"]
-"noxfile.py" = ["T20"]
+"docs/conf.py" = ["D"]
+"tests/**" = [
+  "D",
+  "T20",
+]
+"noxfile.py" = [
+  "D",
+  "T20",
+]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
 
 
 [tool.pylint]
 py-version = "3.8"
 ignore-paths = [".*/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
```

### Comparing `idc_index-0.5.5/PKG-INFO` & `idc_index-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.5
+Version: 0.5.6
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -47,14 +47,15 @@
 Requires-Python: >=3.8
 Requires-Dist: duckdb>=0.10.0
 Requires-Dist: idc-index-data==18.0.1
 Requires-Dist: packaging
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
 Requires-Dist: pyarrow
+Requires-Dist: requests
 Requires-Dist: s5cmd
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
@@ -73,27 +74,31 @@
 [![Documentation Status][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 [![Discourse Forum][discourse-forum-badge]][discourse-forum-link]
 
+> [!WARNING]
+>
+> This package is in its early development stages. Its functionality and API
+> will change.
+>
+> Stay tuned for the updates and documentation, and please share your feedback
+> about it by opening issues in this repository, or by starting a discussion in
+> [IDC User forum](https://discourse.canceridc.dev/).
+
 <!-- SPHINX-START -->
 
 ## About
 
 `idc-index` is a Python package that enables query of the basic metadata and
 download of DICOM files hosted by the
 [NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
 
-👷 🚧 This package is in its early development stages. Its functionality and API
-will change. Stay tuned for the updates and documentation, and please share your
-feedback about it by opening issues in this repository, or by starting a
-discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
-
 ## Usage
 
 There are no prerequisites - just install the package ...
 
 ```bash
 $ pip install idc-index
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

