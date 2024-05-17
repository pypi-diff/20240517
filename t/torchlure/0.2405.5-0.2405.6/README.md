# Comparing `tmp/torchlure-0.2405.5.tar.gz` & `tmp/torchlure-0.2405.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.5.tar", last modified: Fri May 17 11:32:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

