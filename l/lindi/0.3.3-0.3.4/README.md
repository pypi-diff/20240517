# Comparing `tmp/lindi-0.3.3.tar.gz` & `tmp/lindi-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.3.tar", max compression
+gzip compressed data, was "lindi-0.3.4.tar", max compression
```

## Comparing `lindi-0.3.3.tar` & `lindi-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.3/LICENSE
--rw-r--r--   0        0        0     5609 2024-05-09 12:18:43.907992 lindi-0.3.3/README.md
--rw-r--r--   0        0        0     1314 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/File/File.py
--rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/File/__init__.py
--rw-r--r--   0        0        0    30075 2024-05-09 10:57:01.315955 lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      529 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
--rw-r--r--   0        0        0      169 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.3/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11982 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    25313 2024-05-09 12:18:43.907992 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    11404 2024-05-09 12:18:43.907992 lindi-0.3.3/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.3/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    16420 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiRemfile/LindiRemfile.py
--rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiRemfile/__init__.py
--rw-r--r--   0        0        0     8848 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     3506 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0     2299 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LocalCache/LocalCache.py
--rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LocalCache/__init__.py
--rw-r--r--   0        0        0      388 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.3/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.3/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.3/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.3/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      729 2024-05-09 12:18:58.995992 lindi-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 lindi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5609 2024-05-09 21:23:47.131899 lindi-0.3.4/README.md
+-rw-r--r--   0        0        0     1314 2024-05-09 21:23:47.131899 lindi-0.3.4/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.131899 lindi-0.3.4/lindi/File/__init__.py
+-rw-r--r--   0        0        0    30164 2024-05-09 21:23:47.131899 lindi-0.3.4/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      542 2024-05-09 21:23:47.131899 lindi-0.3.4/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.4/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11982 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    25818 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11404 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.4/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.4/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16420 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8772 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.4/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2299 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      388 2024-05-09 21:23:47.135899 lindi-0.3.4/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.4/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.4/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.4/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.4/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.4/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.4/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.4/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.4/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.4/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      729 2024-05-09 21:24:28.923899 lindi-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 lindi-0.3.4/PKG-INFO
```

### Comparing `lindi-0.3.3/LICENSE` & `lindi-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/README.md` & `lindi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/File/File.py` & `lindi-0.3.4/lindi/File/File.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.4/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,38 +65,40 @@
 
         self._external_array_links: Dict[str, Union[dict, None]] = {}
 
     @staticmethod
     def from_file(
         hdf5_file_name_or_url: str,
         *,
-        opts: LindiH5ZarrStoreOpts = LindiH5ZarrStoreOpts(),
+        opts: Union[LindiH5ZarrStoreOpts, None] = None,
         url: Union[str, None] = None,
         local_cache: Union[LocalCache, None] = None
     ):
         """
         Create a LindiH5ZarrStore from a file or url pointing to an HDF5 file.
 
         Parameters
         ----------
         hdf5_file_name_or_url : str
             The name of the HDF5 file or a URL to the HDF5 file.
-        opts : LindiH5ZarrStoreOpts
+        opts : LindiH5ZarrStoreOpts or None
             Options for the store.
         url : str or None
             If hdf5_file_name_or_url is a local file name, then this can
             optionally be set to the URL of the remote file to be used when
             creating references. If None, and the hdf5_file_name_or_url is a
             local file name, then you will need to set
             opts.num_dataset_chunks_threshold to None, and you will not be able
             to use the to_reference_file_system method.
         local_cache : LocalCache or None
             A local cache to use when reading chunks from a remote file. If None,
             then no local cache is used.
         """
+        if opts is None:
+            opts = LindiH5ZarrStoreOpts()  # default options
         if hdf5_file_name_or_url.startswith(
             "http://"
         ) or hdf5_file_name_or_url.startswith("https://"):
             # note that the remfile.File object does not need to be closed
             remf = LindiRemfile(hdf5_file_name_or_url, verbose=False, local_cache=local_cache)
             return LindiH5ZarrStore(_file=remf, _url=hdf5_file_name_or_url, _opts=opts, _entities_to_close=[], _local_cache=local_cache)
         else:
```

### Comparing `lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py` & `lindi-0.3.4/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 from dataclasses import dataclass
 
 
-@dataclass
+@dataclass(frozen=True)
 class LindiH5ZarrStoreOpts:
     """
     Options for the LindiH5ZarrStore class.
 
     Attributes:
         num_dataset_chunks_threshold (Union[int, None]): For each dataset in the
         HDF5 file, if the number of chunks is greater than this threshold, then
```

### Comparing `lindi-0.3.3/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.4/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,27 +54,29 @@
         """
         if local_file_path is None:
             if not url_or_path.startswith("http://") and not url_or_path.startswith("https://"):
                 local_file_path = url_or_path
         return LindiH5pyFile.from_reference_file_system(url_or_path, mode=mode, staging_area=staging_area, local_cache=local_cache, local_file_path=local_file_path)
 
     @staticmethod
-    def from_hdf5_file(url_or_path: str, *, mode: LindiFileMode = "r", local_cache: Union[LocalCache, None] = None, zarr_store_opts: LindiH5ZarrStoreOpts = LindiH5ZarrStoreOpts()):
+    def from_hdf5_file(url_or_path: str, *, mode: LindiFileMode = "r", local_cache: Union[LocalCache, None] = None, zarr_store_opts: Union[LindiH5ZarrStoreOpts, None] = None):
         """
         Create a LindiH5pyFile from a URL or path to an HDF5 file.
 
         Parameters
         ----------
         url_or_path : str
             The URL or path to the remote or local HDF5 file.
         mode : Literal["r", "r+", "w", "w-", "x", "a"], optional
             The mode to open the file object in. See api docs for
             h5py.File for more information on the modes, by default "r".
         local_cache : Union[LocalCache, None], optional
             The local cache to use for caching data chunks, by default None.
+        zarr_store_opts : Union[LindiH5ZarrStoreOpts, None], optional
+            The options to use for the zarr store, by default None.
         """
         from ..LindiH5ZarrStore.LindiH5ZarrStore import LindiH5ZarrStore  # avoid circular import
         if mode != "r":
             raise Exception("Opening hdf5 file in write mode is not supported")
         zarr_store = LindiH5ZarrStore.from_file(url_or_path, local_cache=local_cache, opts=zarr_store_opts, url=url_or_path)
         return LindiH5pyFile.from_zarr_store(
             zarr_store=zarr_store,
@@ -259,27 +261,32 @@
         -------
         str
             The URL (or local path) of the uploaded reference file system .json
             file.
         """
         rfs = self.to_reference_file_system()
         blobs_to_upload = set()
+        # Get the set of all local URLs in rfs['refs']
         for k, v in rfs['refs'].items():
             if isinstance(v, list) and len(v) == 3:
                 url = _apply_templates(v[0], rfs.get('templates', {}))
                 if not url.startswith("http://") and not url.startswith("https://"):
                     local_path = url
                     blobs_to_upload.add(local_path)
+        # Upload each of the local blobs using the given upload function and get a mapping from
+        # the original file paths to the URLs of the uploaded files
         blob_mapping = _upload_blobs(blobs_to_upload, on_upload_blob=on_upload_blob)
+        # Replace the local URLs in rfs['refs'] with URLs of the uploaded files
         for k, v in rfs['refs'].items():
             if isinstance(v, list) and len(v) == 3:
                 url1 = _apply_templates(v[0], rfs.get('templates', {}))
                 url2 = blob_mapping.get(url1, None)
                 if url2 is not None:
                     v[0] = url2
+        # Write the updated LINDI file to a temp directory and upload it
         with tempfile.TemporaryDirectory() as tmpdir:
             rfs_fname = f"{tmpdir}/rfs.lindi.json"
             LindiReferenceFileSystemStore.use_templates_in_rfs(rfs)
             _write_rfs_to_file(rfs=rfs, output_file_name=rfs_fname)
             return on_upload_main(rfs_fname)
 
     def write_lindi_file(self, filename: str, *, generation_metadata: Union[dict, None] = None):
```

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.4/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.4/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.4/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiRemfile/LindiRemfile.py` & `lindi-0.3.4/lindi/LindiRemfile/LindiRemfile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.4/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,14 @@
             offset,
             size
         ]
 
     def consolidate_chunks(self):
         """
         Consolidate the chunks in the staging area.
-
-        This method is called by `upload` if `consolidate_chunks` is True.
         """
         rfs = self._base_store.rfs
         refs_keys_by_reference_parent_path = {}
         for k, v in rfs['refs'].items():
             if isinstance(v, list) and len(v) == 3:
                 url = v[0]
                 if not url.startswith(self._staging_area.directory + '/'):
```

### Comparing `lindi-0.3.3/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.4/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/LocalCache/LocalCache.py` & `lindi-0.3.4/lindi/LocalCache/LocalCache.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/attr_conversion.py` & `lindi-0.3.4/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.4/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/decode_references.py` & `lindi-0.3.4/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.4/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.4/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.4/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.3/pyproject.toml` & `lindi-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

### Comparing `lindi-0.3.3/PKG-INFO` & `lindi-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

