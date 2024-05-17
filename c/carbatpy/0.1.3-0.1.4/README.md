# Comparing `tmp/carbatpy-0.1.3.tar.gz` & `tmp/carbatpy-0.1.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbatpy-0.1.3.tar", last modified: Thu May 16 13:33:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

