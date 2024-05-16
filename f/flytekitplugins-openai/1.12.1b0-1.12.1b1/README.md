# Comparing `tmp/flytekitplugins_openai-1.12.1b0.tar.gz` & `tmp/flytekitplugins_openai-1.12.1b1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_openai-1.12.1b0.tar", last modified: Thu May  9 17:17:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

