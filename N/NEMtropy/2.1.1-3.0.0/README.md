# Comparing `tmp/NEMtropy-2.1.1.tar.gz` & `tmp/NEMtropy-3.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMtropy-2.1.1.tar", last modified: Thu Jun 23 16:36:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

