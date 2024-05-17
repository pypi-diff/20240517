# Comparing `tmp/pbixray-0.1.4-py3-none-any.whl.zip` & `tmp/pbixray-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 79115 bytes, number of entries: 27
+Zip file size: 16953 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Oct-23 09:05 pbixray/__init__.py
 -rw-rw-rw-  2.0 fat     1514 b- defN 23-Oct-24 17:34 pbixray/core.py
--rw-rw-rw-  2.0 fat     4060 b- defN 23-Oct-24 17:45 pbixray/pbix_unpacker.py
+-rw-rw-rw-  2.0 fat     4042 b- defN 23-Oct-30 14:34 pbixray/pbix_unpacker.py
 -rw-rw-rw-  2.0 fat      955 b- defN 23-Oct-24 17:20 pbixray/utils.py
 -rw-rw-rw-  2.0 fat     7889 b- defN 23-Oct-24 17:46 pbixray/vertipaq_decoder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-06 13:44 pbixray/abf/__init__.py
 -rw-rw-rw-  2.0 fat     2528 b- defN 23-Oct-20 15:40 pbixray/abf/backup_log.py
 -rw-rw-rw-  2.0 fat     1311 b- defN 23-Oct-06 16:35 pbixray/abf/backup_log_header.py
 -rw-rw-rw-  2.0 fat      147 b- defN 23-Oct-24 17:14 pbixray/abf/data_model.py
 -rw-rw-rw-  2.0 fat     2940 b- defN 23-Oct-24 17:41 pbixray/abf/parser.py
@@ -15,15 +15,12 @@
 -rw-rw-rw-  2.0 fat     3914 b- defN 23-Sep-26 13:03 pbixray/column_data/hidx.py
 -rw-rw-rw-  2.0 fat     1928 b- defN 23-Sep-20 13:58 pbixray/column_data/idf.py
 -rw-rw-rw-  2.0 fat     9004 b- defN 23-Oct-07 22:06 pbixray/column_data/idfmeta.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-06 15:24 pbixray/meta/__init__.py
 -rw-rw-rw-  2.0 fat     2186 b- defN 23-Oct-24 17:46 pbixray/meta/metadata_handler.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 23-Oct-23 14:29 pbixray/meta/metadata_query.py
 -rw-rw-rw-  2.0 fat     1188 b- defN 23-Oct-23 16:34 pbixray/meta/sqlite_handler.py
--rw-rw-rw-  2.0 fat    49664 b- defN 23-Oct-16 14:51 pbixray-0.1.4.data/data/lib/libxpress9.dll
--rw-rw-rw-  2.0 fat    84344 b- defN 23-Oct-16 14:51 pbixray-0.1.4.data/data/lib/libxpress9.dylib
--rw-rw-rw-  2.0 fat    72376 b- defN 23-Oct-16 14:50 pbixray-0.1.4.data/data/lib/libxpress9.so
--rw-rw-rw-  2.0 fat      106 b- defN 23-Oct-30 13:59 pbixray-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-30 13:59 pbixray-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Oct-30 13:59 pbixray-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2245 b- defN 23-Oct-30 13:59 pbixray-0.1.4.dist-info/RECORD
-27 files, 259753 bytes uncompressed, 75487 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat      106 b- defN 23-Oct-30 14:35 pbixray-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-30 14:35 pbixray-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Oct-30 14:35 pbixray-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1944 b- defN 23-Oct-30 14:35 pbixray-0.1.5.dist-info/RECORD
+24 files, 53050 bytes uncompressed, 13807 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -54,29 +54,20 @@
 
 Filename: pbixray/meta/metadata_query.py
 Comment: 
 
 Filename: pbixray/meta/sqlite_handler.py
 Comment: 
 
-Filename: pbixray-0.1.4.data/data/lib/libxpress9.dll
+Filename: pbixray-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pbixray-0.1.4.data/data/lib/libxpress9.dylib
+Filename: pbixray-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pbixray-0.1.4.data/data/lib/libxpress9.so
+Filename: pbixray-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pbixray-0.1.4.dist-info/METADATA
-Comment: 
-
-Filename: pbixray-0.1.4.dist-info/WHEEL
-Comment: 
-
-Filename: pbixray-0.1.4.dist-info/top_level.txt
-Comment: 
-
-Filename: pbixray-0.1.4.dist-info/RECORD
+Filename: pbixray-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pbixray/pbix_unpacker.py

```diff
@@ -21,19 +21,19 @@
 
     def __setup_library(self):
         # Get the directory of the current file
         current_dir = os.path.dirname(os.path.abspath(__file__))
 
         # Determine the path to the shared library based on the platform
         if platform.system() == "Windows":
-            self.lib_path = os.path.join(current_dir, '..', 'lib', 'libxpress9.dll')
+            self.lib_path = os.path.join(current_dir, 'lib', 'libxpress9.dll')
         elif platform.system() == "Linux":
-            self.lib_path = os.path.join(current_dir, '..', 'lib', 'libxpress9.so')
+            self.lib_path = os.path.join(current_dir, 'lib', 'libxpress9.so')
         elif platform.system() == "Darwin":
-            self.lib_path = os.path.join(current_dir, '..', 'lib', 'libxpress9.dylib')
+            self.lib_path = os.path.join(current_dir, 'lib', 'libxpress9.dylib')
         else:
             raise RuntimeError("Unsupported platform")
 
         # Load the shared library
         self.lib = ctypes.CDLL(self.lib_path)
 
         # Define the function signatures
```

## Comparing `pbixray-0.1.4.dist-info/RECORD` & `pbixray-0.1.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pbixray/__init__.py,sha256=YPfKqP0RXCYJriKyjWhRWWrRlWkxkDMcfIQwOjjEz8o,27
 pbixray/core.py,sha256=zQ0vEYHoGmoYCyUvvwvXSBiFSMH7xbTfrbP86wciucM,1514
-pbixray/pbix_unpacker.py,sha256=e0ZMuRFiJBtcZjW0FqLUtA14OvdnFPdx83MFw642yC0,4060
+pbixray/pbix_unpacker.py,sha256=mMI313PMH4IrexA1biItacRxdNqa3eQPt74OVtx9lac,4042
 pbixray/utils.py,sha256=6hHmBRzJeDusBs9d8Yxf6Q8eCqew185RE2zIU90IEy0,955
 pbixray/vertipaq_decoder.py,sha256=KEklf43khvD8VdMuWILMcHjF1koGT7rggrqxfwW3P50,7889
 pbixray/abf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pbixray/abf/backup_log.py,sha256=_7OlxJtcGtTYJK7XUJPdwoaW2wDY0gpqiIXe9ufh0sA,2528
 pbixray/abf/backup_log_header.py,sha256=91z8QATeNBz57QEAcrZIvKgSsuxB3jfngnzAez52S6Q,1311
 pbixray/abf/data_model.py,sha256=u-KBEe1TYKgWIIPw-vWflVsdx6R1ztHE-rNlhLBDlRo,147
 pbixray/abf/parser.py,sha256=NisY4diYlmLj2OeZ-YxhnYhQO8hJtWBvn_9ci4iG1ZY,2940
@@ -14,14 +14,11 @@
 pbixray/column_data/hidx.py,sha256=c_PPLSpHSghYAPTNvjjdBAvB7s2UEtoJzugY1aYOTAE,3914
 pbixray/column_data/idf.py,sha256=BnOKKqzBVl8sjXHXOTS-uOqi0w0Kxy6sSdhalq3xc4g,1928
 pbixray/column_data/idfmeta.py,sha256=Vjq6Q58j207MrXAjreSfhvUUeG3msZZNM5YMwYB1YUY,9004
 pbixray/meta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pbixray/meta/metadata_handler.py,sha256=pWCf38xWLGnvDcPJmMrAVmd4abo1deQh8mz9Tjfmz8U,2186
 pbixray/meta/metadata_query.py,sha256=CLsuCNHRzeWj7lk3QsZz6C_9cHWl97qjPtLHFw1iGG0,2841
 pbixray/meta/sqlite_handler.py,sha256=xavfWgaZRKuD3LuisQwVhw5NvPziqgclsqiZmAp9v5Y,1188
-pbixray-0.1.4.data/data/lib/libxpress9.dll,sha256=qy2k1kDXtA_leoLuaxGyJL6AkRxSvYK-mocAHZhtn3Y,49664
-pbixray-0.1.4.data/data/lib/libxpress9.dylib,sha256=RKR-aoymEqJ8soplvR9If4oq6Gp9uWzptV0tQ8R_lnI,84344
-pbixray-0.1.4.data/data/lib/libxpress9.so,sha256=4uDzeYakHdCIwDdm9aWyS2ooK5jwSVCgdbLg6GOjDLI,72376
-pbixray-0.1.4.dist-info/METADATA,sha256=-jVZaDDYsBmAP2gUGgcC_qLcSW1T8K8ow0nXuZp4ymo,106
-pbixray-0.1.4.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-pbixray-0.1.4.dist-info/top_level.txt,sha256=IYkCH1cptMvQbg1iB9cYQOR-On9DT3vmXUtbOHgpNZo,8
-pbixray-0.1.4.dist-info/RECORD,,
+pbixray-0.1.5.dist-info/METADATA,sha256=dEjedRqc-S6ztpUrHNI12i5hyCqgNvzi1-9UAcDOS3I,106
+pbixray-0.1.5.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+pbixray-0.1.5.dist-info/top_level.txt,sha256=IYkCH1cptMvQbg1iB9cYQOR-On9DT3vmXUtbOHgpNZo,8
+pbixray-0.1.5.dist-info/RECORD,,
```

