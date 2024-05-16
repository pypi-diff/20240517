# Comparing `tmp/boostrsa-0.0.1.dev0.tar.gz` & `tmp/boostrsa-0.0.1.dev1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boostrsa-0.0.1.dev0.tar", last modified: Thu May  9 11:41:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

