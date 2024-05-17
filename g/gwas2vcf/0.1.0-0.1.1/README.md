# Comparing `tmp/gwas2vcf-0.1.0.tar.gz` & `tmp/gwas2vcf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas2vcf-0.1.0.tar", last modified: Fri May 17 19:28:19 2024, max compression
+gzip compressed data, was "gwas2vcf-0.1.1.tar", last modified: Fri May 17 19:44:51 2024, max compression
```

## Comparing `gwas2vcf-0.1.0.tar` & `gwas2vcf-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:28:19.775171 gwas2vcf-0.1.0/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       19 2024-05-17 19:26:12.000000 gwas2vcf-0.1.0/MANIFEST.in
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1344 2024-05-17 19:28:19.775171 gwas2vcf-0.1.0/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      815 2024-05-17 19:13:31.000000 gwas2vcf-0.1.0/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:28:19.775171 gwas2vcf-0.1.0/gwas2vcf.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1344 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      234 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       58 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       12 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 19:28:19.000000 gwas2vcf-0.1.0/gwas2vcf.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       79 2024-05-17 19:28:19.775171 gwas2vcf-0.1.0/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      913 2024-05-17 19:25:09.000000 gwas2vcf-0.1.0/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:44:51.329778 gwas2vcf-0.1.1/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       19 2024-05-17 19:26:12.000000 gwas2vcf-0.1.1/MANIFEST.in
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      932 2024-05-17 19:44:51.329778 gwas2vcf-0.1.1/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      403 2024-05-17 19:39:53.000000 gwas2vcf-0.1.1/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:44:51.329778 gwas2vcf-0.1.1/gwas2vcf.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      932 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      234 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       58 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       12 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 19:44:51.000000 gwas2vcf-0.1.1/gwas2vcf.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       79 2024-05-17 19:44:51.329778 gwas2vcf-0.1.1/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      913 2024-05-17 19:44:21.000000 gwas2vcf-0.1.1/setup.py
```

### Comparing `gwas2vcf-0.1.0/setup.py` & `gwas2vcf-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gwas2vcf",
-    version="0.1.0",
+    version="0.1.1",
     author="Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN",
     author_email="vijay-kumar.ulaganathan@uni-tuebingen.de",
     description="A tool to convert GWAS TSV files to VCF format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VJ-Ulaganathan/gwas2vcf/",
     packages=find_packages(),
```

