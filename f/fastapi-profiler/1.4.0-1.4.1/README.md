# Comparing `tmp/fastapi_profiler-1.4.0-py3-none-any.whl.zip` & `tmp/fastapi_profiler-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4521 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      101 b- defN 24-May-14 07:48 fastapi_profiler/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 24-May-14 07:55 fastapi_profiler/_version.py
--rw-rw-rw-  2.0 fat     6935 b- defN 24-May-14 07:49 fastapi_profiler/profiler.py
--rw-rw-rw-  2.0 fat     1084 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1001 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      683 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/RECORD
-8 files, 9966 bytes uncompressed, 3315 bytes compressed:  66.7%
+Zip file size: 4517 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx      101 b- defN 24-May-14 07:48 fastapi_profiler/__init__.py
+-rwxrwxrwx  2.0 unx       53 b- defN 24-May-17 01:25 fastapi_profiler/_version.py
+-rwxrwxrwx  2.0 unx     7124 b- defN 24-May-17 01:22 fastapi_profiler/profiler.py
+-rwxrwxrwx  2.0 unx     1084 b- defN 24-May-17 01:28 fastapi_profiler-1.4.1.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx      974 b- defN 24-May-17 01:28 fastapi_profiler-1.4.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 24-May-17 01:28 fastapi_profiler-1.4.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       17 b- defN 24-May-17 01:28 fastapi_profiler-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      682 b- defN 24-May-17 01:28 fastapi_profiler-1.4.1.dist-info/RECORD
+8 files, 10127 bytes uncompressed, 3311 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: fastapi_profiler/_version.py
 Comment: 
 
 Filename: fastapi_profiler/profiler.py
 Comment: 
 
-Filename: fastapi_profiler-1.4.0.dist-info/LICENSE
+Filename: fastapi_profiler-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_profiler-1.4.0.dist-info/METADATA
+Filename: fastapi_profiler-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_profiler-1.4.0.dist-info/WHEEL
+Filename: fastapi_profiler-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_profiler-1.4.0.dist-info/top_level.txt
+Filename: fastapi_profiler-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fastapi_profiler-1.4.0.dist-info/RECORD
+Filename: fastapi_profiler-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_profiler/_version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 __author__ = "sunhailin-Leo"
```

## fastapi_profiler/profiler.py

```diff
@@ -124,19 +124,19 @@
             renderer = HTMLRenderer()
             if self._open_in_browser:
                 renderer.open_in_browser(
                     session=self._profiler.last_session,
                     output_filename=os.path.abspath(html_file_name),
                 )
             else:
-                html_code = renderer.render(session=self._profiler.last_session)
-                with codecs.open(html_file_name, "w", "utf-8") as f:
-                    f.write(html_code)
-
-            logger.info("Done writing profile to %r", html_file_name)
+                if self._profiler.last_session:
+                    html_code = renderer.render(session=self._profiler.last_session)
+                    with codecs.open(html_file_name, "w", "utf-8") as f:
+                        f.write(html_code)
+                    logger.info("Done writing profile to %r", html_file_name)
         elif self._output_type == "prof":
             prof_file_name = self.DEFAULT_PROF_FILENAME
             if self._prof_file_name is not None:
                 prof_file_name = self._prof_file_name
 
             logger.info(
                 "Compiling and dumping final profile to %r - this may take some time",
@@ -151,25 +151,27 @@
                 prof_file_name = self._prof_file_name
 
             logger.info(
                 "Compiling and dumping final profile to %r - this may take some time",
                 prof_file_name,
             )
 
-            renderer = JSONRenderer()
-            with codecs.open(prof_file_name, "w", "utf-8") as f:
-                f.write(renderer.render(session=self._profiler.last_session))
-            logger.info("Done writing profile to %r", prof_file_name)
+            if self._profiler.last_session:
+                renderer = JSONRenderer()
+                with codecs.open(prof_file_name, "w", "utf-8") as f:
+                    f.write(renderer.render(session=self._profiler.last_session))
+                logger.info("Done writing profile to %r", prof_file_name)
         elif self._output_type == "speedscope":
             prof_file_name = self.DEFAULT_SPEEDSCOPE_FILENAME
             if self._prof_file_name is not None:
                 prof_file_name = self._prof_file_name
 
             logger.info(
                 "Compiling and dumping final profile to %r - this may take some time",
                 prof_file_name,
             )
 
-            renderer = SpeedscopeRenderer()
-            with codecs.open(prof_file_name, "w", "utf-8") as f:
-                f.write(renderer.render(session=self._profiler.last_session))
-            logger.info("Done writing profile to %r", prof_file_name)
+            if self._profiler.last_session:
+                renderer = SpeedscopeRenderer()
+                with codecs.open(prof_file_name, "w", "utf-8") as f:
+                    f.write(renderer.render(session=self._profiler.last_session))
+                logger.info("Done writing profile to %r", prof_file_name)
```

## Comparing `fastapi_profiler-1.4.0.dist-info/LICENSE` & `fastapi_profiler-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

