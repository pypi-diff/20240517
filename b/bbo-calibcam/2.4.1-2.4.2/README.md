# Comparing `tmp/bbo-calibcam-2.4.1.tar.gz` & `tmp/bbo_calibcam-2.4.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-calibcam-2.4.1.tar", last modified: Fri Apr 26 05:46:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

