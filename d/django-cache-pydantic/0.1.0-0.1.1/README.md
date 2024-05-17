# Comparing `tmp/django_cache_pydantic-0.1.0.tar.gz` & `tmp/django_cache_pydantic-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cache_pydantic-0.1.0.tar", last modified: Fri May 10 09:27:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

