# Comparing `tmp/d2b-asl-2.0.0.tar.gz` & `tmp/d2b_asl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2b-asl-2.0.0.tar", max compression
+gzip compressed data, was "d2b_asl-2.0.1.tar", max compression
```

## Comparing `d2b-asl-2.0.0.tar` & `d2b_asl-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     2005 2021-09-18 06:48:00.055597 d2b-asl-2.0.0/README.md
--rw-r--r--   0        0        0     1470 2021-09-18 06:48:00.055597 d2b-asl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10259 2021-09-18 06:48:00.059597 d2b-asl-2.0.0/src/d2b_asl.py
--rw-r--r--   0        0        0     2833 2021-09-18 06:48:09.585772 d2b-asl-2.0.0/setup.py
--rw-r--r--   0        0        0     3313 2021-09-18 06:48:09.586071 d2b-asl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    13148 2024-05-17 15:38:53.600790 d2b_asl-2.0.1/README.md
+-rw-r--r--   0        0        0     1476 2024-05-17 15:38:53.600790 d2b_asl-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10287 2024-05-17 15:38:53.600790 d2b_asl-2.0.1/src/d2b_asl.py
+-rw-r--r--   0        0        0    14609 1970-01-01 00:00:00.000000 d2b_asl-2.0.1/PKG-INFO
```

### Comparing `d2b-asl-2.0.0/pyproject.toml` & `d2b_asl-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "d2b-asl"
-version = "2.0.0"
+version = "2.0.1"
 description = "Plugin for the d2b package to handle ASL data"
 authors = ["Andrew Ross <andrew.ross.mail@gmail.com>"]
 
 readme = "README.md"
 
 keywords = ["neuroscience", "neuroimaging", "bids", "d2b", "plugin"]
 
@@ -31,19 +31,19 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 d2b = "^1.1.4"
 nibabel = "^3.2.1"
 
-[tool.poetry.dev-dependencies]
-black = "^21.8b0"
+[tool.poetry.group.dev.dependencies]
+black = "^24.4.2"
 flake8 = "^3.9.2"
 pylint = "^2.10.2"
-reorder-python-imports = "^2.6.0"
+reorder-python-imports = "^2.8.0"
 pre-commit = "^2.14.1"
 bump2version = "^1.0.1"
 
 [tool.poetry.plugins.d2b]
 "asl" = "d2b_asl"
```

### Comparing `d2b-asl-2.0.0/src/d2b_asl.py` & `d2b_asl-2.0.1/src/d2b_asl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from d2b.hookspecs import hookimpl
 from d2b.utils import first_nii
 
 if TYPE_CHECKING:
     from d2b.d2b import D2B, Acquisition
 
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 ASL_CONTEXT_DESCRIPTION_PROPERTY = "aslContext"
 BIDS_LABELS = ["cbf", "control", "deltam", "label", "m0scan"]
 ALLOWED_NON_BIDS_LABELS = ["discard"]
 
 
 @hookimpl
@@ -91,15 +91,15 @@
 
 def find_asl_acquisitions(acquisitions: list[Acquisition]) -> list[Acquisition]:
     return [acq for acq in acquisitions if is_asl(acq)]
 
 
 def is_asl(acquisition: Acquisition) -> bool:
     description = acquisition.description
-    return description.data_type == "perf"
+    return description.modality_label == "_asl"
 
 
 class Aslcontext:
     def __init__(self, labels: list[str], file_root: str | Path | None = None):
         self.labels = labels
         self.file_root = file_root
 
@@ -124,15 +124,15 @@
         if self.file_root is None:
             raise TypeError("Cannot write json file with NoneType file_root attribute.")
         dst_root = Path(self.file_root)
         return dst_root.parent / f"{dst_root.stem}_aslcontext.json"
 
     def validate(self, asl_file: str | Path):
         img: nib.Nifti1Image = nib.load(asl_file)
-        nvols, nlabels = img.shape[-1], len(self.labels)
+        nvols, nlabels = img.header["dim"][4], len(self.labels)  # type: ignore
         if nvols != nlabels:
             raise AslContextConfigurationError(asl_file, nvols, nlabels)
         for label in self.labels:
             if not (label in BIDS_LABELS or label in ALLOWED_NON_BIDS_LABELS):
                 raise InvalidAslcontextLabelError(label)
 
     def tagged_labels(self) -> list[TaggedLabel]:
```

