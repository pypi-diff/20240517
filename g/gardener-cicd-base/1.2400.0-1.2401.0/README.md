# Comparing `tmp/gardener_cicd_base-1.2400.0.tar.gz` & `tmp/gardener_cicd_base-1.2401.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_base-1.2400.0.tar", last modified: Fri May 17 13:19:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

