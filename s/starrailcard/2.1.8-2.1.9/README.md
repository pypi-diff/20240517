# Comparing `tmp/starrailcard-2.1.8.tar.gz` & `tmp/starrailcard-2.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.8.tar", last modified: Sat May 11 17:12:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

