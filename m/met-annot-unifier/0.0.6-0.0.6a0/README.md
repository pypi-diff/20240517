# Comparing `tmp/met_annot_unifier-0.0.6.tar.gz` & `tmp/met_annot_unifier-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met_annot_unifier-0.0.6.tar", max compression
+gzip compressed data, was "met_annot_unifier-0.0.6a0.tar", max compression
```

## Comparing `met_annot_unifier-0.0.6.tar` & `met_annot_unifier-0.0.6a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-05-15 11:17:06.725050 met_annot_unifier-0.0.6/LICENSE
--rw-r--r--   0        0        0     4691 2024-05-15 11:17:06.725050 met_annot_unifier-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/aligner/__init__.py
--rw-r--r--   0        0        0     7537 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/aligner/aligner.py
--rw-r--r--   0        0        0     9393 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/aligner/parser.py
--rw-r--r--   0        0        0     2644 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/aligner/utils.py
--rw-r--r--   0        0        0     4947 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/cli.py
--rw-r--r--   0        0        0    10938 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/config/column_config.json
--rw-r--r--   0        0        0      694 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/exceptions.py
--rw-r--r--   0        0        0      267 2024-05-15 11:17:06.757050 met_annot_unifier-0.0.6/met_annot_unifier/foo.py
--rw-r--r--   0        0        0     2409 2024-05-15 11:17:29.981114 met_annot_unifier-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-17 09:10:37.736973 met_annot_unifier-0.0.6a0/LICENSE
+-rw-r--r--   0        0        0     4691 2024-05-17 09:10:37.736973 met_annot_unifier-0.0.6a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 09:10:37.764973 met_annot_unifier-0.0.6a0/met_annot_unifier/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:10:37.764973 met_annot_unifier-0.0.6a0/met_annot_unifier/aligner/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-17 09:10:37.764973 met_annot_unifier-0.0.6a0/met_annot_unifier/aligner/aligner.py
+-rw-r--r--   0        0        0     9393 2024-05-17 09:10:37.764973 met_annot_unifier-0.0.6a0/met_annot_unifier/aligner/parser.py
+-rw-r--r--   0        0        0     7740 2024-05-17 09:10:37.768973 met_annot_unifier-0.0.6a0/met_annot_unifier/aligner/utils.py
+-rw-r--r--   0        0        0     5209 2024-05-17 09:10:37.768973 met_annot_unifier-0.0.6a0/met_annot_unifier/cli.py
+-rw-r--r--   0        0        0    10938 2024-05-17 09:10:37.768973 met_annot_unifier-0.0.6a0/met_annot_unifier/config/column_config.json
+-rw-r--r--   0        0        0      694 2024-05-17 09:10:37.768973 met_annot_unifier-0.0.6a0/met_annot_unifier/exceptions.py
+-rw-r--r--   0        0        0      267 2024-05-17 09:10:37.768973 met_annot_unifier-0.0.6a0/met_annot_unifier/foo.py
+-rw-r--r--   0        0        0     2410 2024-05-17 09:10:56.416962 met_annot_unifier-0.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.6a0/PKG-INFO
```

### Comparing `met_annot_unifier-0.0.6/LICENSE` & `met_annot_unifier-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.6/README.md` & `met_annot_unifier-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.6/met_annot_unifier/aligner/parser.py` & `met_annot_unifier-0.0.6a0/met_annot_unifier/aligner/parser.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.6/met_annot_unifier/cli.py` & `met_annot_unifier-0.0.6a0/met_annot_unifier/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,38 +39,45 @@
     else:
         click.echo(aligned_data)
 
 
 @cli.command()
 @click.option("--canopus-file", type=click.Path(), default=None, help="Path to CANOPUS output file.")
 @click.option("--gnps-file", type=click.Path(), default=None, help="Path to GNPS output file.")
+@click.option("--gnps-mn-file", type=click.Path(), default=None, help="Path to GNPS MN output file.")
 @click.option("--isdb-file", type=click.Path(), default=None, help="Path to ISDB output file.")
 @click.option("--sirius-file", type=click.Path(), default=None, help="Path to Sirius output file.")
 @click.option("--output", "-o", type=click.Path(), help="Output file to save the merged data.")
 def align_horizontally(
     canopus_file: Optional[str],
     gnps_file: Optional[str],
+    gnps_mn_file: Optional[str],
     isdb_file: Optional[str],
     sirius_file: Optional[str],
     output: Optional[str] = None,
 ) -> None:
     """CLI tool to align and merge data from CANOPUS, GNPS, Sirius, and ISDB horizontally.
 
     Args:
         canopus_file (Optional[str]): Path to CANOPUS output file.
         gnps_file (Optional[str]): Path to GNPS output file.
+        gnps_mn_file (Optional[str]): Path to GNPS MN output file.
         sirius_file (Optional[str]): Path to Sirius output file.
         isdb_file (Optional[str]): Path to ISDB output file.
         output (Optional[str]): Output file to save the merged data.
 
     Returns:
         A dataframe with the aligned data (if the output option is used, the dataframe is saved to a file)
     """
     aligned_data = align_data_horizontally(
-        canopus_file=canopus_file, gnps_file=gnps_file, isdb_file=isdb_file, sirius_file=sirius_file
+        canopus_file=canopus_file,
+        gnps_file=gnps_file,
+        gnps_mn_file=gnps_mn_file,
+        isdb_file=isdb_file,
+        sirius_file=sirius_file,
     )
 
     if output:
         aligned_data.to_csv(output, index=False, sep="\t")
         click.echo(f"Aligned data saved to {output}")
     else:
         click.echo(aligned_data)
```

### Comparing `met_annot_unifier-0.0.6/met_annot_unifier/config/column_config.json` & `met_annot_unifier-0.0.6a0/met_annot_unifier/config/column_config.json`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.6/met_annot_unifier/exceptions.py` & `met_annot_unifier-0.0.6a0/met_annot_unifier/exceptions.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.6/pyproject.toml` & `met_annot_unifier-0.0.6a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "met-annot-unifier"
-version = "0.0.6"
+version = "0.0.6a"
 description = "A Python project to combine tabular outputs from GNPS, Sirius and ISDB"
 authors = ["Pierre-Marie Allard <pierre-marie.allard@unifr.ch>"]
 repository = "https://github.com/mapp-metabolomics-unit/met-annot-unifier"
 documentation = "https://mapp-metabolomics-unit.github.io/met-annot-unifier/"
 readme = "README.md"
 packages = [
   {include = "met_annot_unifier"}
```

### Comparing `met_annot_unifier-0.0.6/PKG-INFO` & `met_annot_unifier-0.0.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: met-annot-unifier
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: A Python project to combine tabular outputs from GNPS, Sirius and ISDB
 Home-page: https://github.com/mapp-metabolomics-unit/met-annot-unifier
 Author: Pierre-Marie Allard
 Author-email: pierre-marie.allard@unifr.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

