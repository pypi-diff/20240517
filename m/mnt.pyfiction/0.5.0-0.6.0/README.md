# Comparing `tmp/mnt.pyfiction-0.5.0.tar.gz` & `tmp/mnt.pyfiction-0.6.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnt.pyfiction-0.5.0.tar", last modified: Wed Nov 22 16:55:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

