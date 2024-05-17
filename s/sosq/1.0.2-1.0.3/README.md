# Comparing `tmp/sosq-1.0.2.tar.gz` & `tmp/sosq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosq-1.0.2.tar", last modified: Thu Feb 29 06:14:55 2024, max compression
+gzip compressed data, was "sosq-1.0.3.tar", last modified: Sat Mar 23 14:28:31 2024, max compression
```

## Comparing `sosq-1.0.2.tar` & `sosq-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-02-29 06:14:55.443908 sosq-1.0.2/
--rw-r--r--   0 bakircius   (501) staff       (20)    35149 2024-02-29 06:12:58.000000 sosq-1.0.2/LICENSE
--rw-r--r--   0 bakircius   (501) staff       (20)     1015 2024-02-29 06:14:55.443346 sosq-1.0.2/PKG-INFO
--rw-r--r--   0 bakircius   (501) staff       (20)      367 2024-02-29 06:12:58.000000 sosq-1.0.2/README.md
--rw-r--r--   0 bakircius   (501) staff       (20)      658 2024-02-29 06:14:01.000000 sosq-1.0.2/pyproject.toml
--rw-r--r--   0 bakircius   (501) staff       (20)       38 2024-02-29 06:14:55.444015 sosq-1.0.2/setup.cfg
-drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-02-29 06:14:55.437469 sosq-1.0.2/src/
-drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-02-29 06:14:55.439416 sosq-1.0.2/src/sosq/
--rw-r--r--   0 bakircius   (501) staff       (20)     2558 2024-02-29 06:12:58.000000 sosq-1.0.2/src/sosq/__init__.py
-drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-02-29 06:14:55.442672 sosq-1.0.2/src/sosq.egg-info/
--rw-r--r--   0 bakircius   (501) staff       (20)     1015 2024-02-29 06:14:55.000000 sosq-1.0.2/src/sosq.egg-info/PKG-INFO
--rw-r--r--   0 bakircius   (501) staff       (20)      237 2024-02-29 06:14:55.000000 sosq-1.0.2/src/sosq.egg-info/SOURCES.txt
--rw-r--r--   0 bakircius   (501) staff       (20)        1 2024-02-29 06:14:55.000000 sosq-1.0.2/src/sosq.egg-info/dependency_links.txt
--rw-r--r--   0 bakircius   (501) staff       (20)       22 2024-02-29 06:14:55.000000 sosq-1.0.2/src/sosq.egg-info/requires.txt
--rw-r--r--   0 bakircius   (501) staff       (20)        5 2024-02-29 06:14:55.000000 sosq-1.0.2/src/sosq.egg-info/top_level.txt
-drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-02-29 06:14:55.442081 sosq-1.0.2/tests/
--rw-r--r--   0 bakircius   (501) staff       (20)       33 2024-02-29 06:12:58.000000 sosq-1.0.2/tests/test_getResults.py
+drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-03-23 14:28:31.104895 sosq-1.0.3/
+-rw-r--r--   0 bakircius   (501) staff       (20)    35149 2024-02-29 06:12:58.000000 sosq-1.0.3/LICENSE
+-rw-r--r--   0 bakircius   (501) staff       (20)     1323 2024-03-23 14:28:31.103989 sosq-1.0.3/PKG-INFO
+-rw-r--r--   0 bakircius   (501) staff       (20)      367 2024-02-29 06:12:58.000000 sosq-1.0.3/README.md
+-rw-r--r--   0 bakircius   (501) staff       (20)      927 2024-03-23 14:27:27.000000 sosq-1.0.3/pyproject.toml
+-rw-r--r--   0 bakircius   (501) staff       (20)       38 2024-03-23 14:28:31.105105 sosq-1.0.3/setup.cfg
+drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-03-23 14:28:31.096757 sosq-1.0.3/src/
+drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-03-23 14:28:31.099336 sosq-1.0.3/src/sosq/
+-rw-r--r--   0 bakircius   (501) staff       (20)     2436 2024-03-23 14:16:23.000000 sosq-1.0.3/src/sosq/__init__.py
+drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-03-23 14:28:31.103158 sosq-1.0.3/src/sosq.egg-info/
+-rw-r--r--   0 bakircius   (501) staff       (20)     1323 2024-03-23 14:28:31.000000 sosq-1.0.3/src/sosq.egg-info/PKG-INFO
+-rw-r--r--   0 bakircius   (501) staff       (20)      237 2024-03-23 14:28:31.000000 sosq-1.0.3/src/sosq.egg-info/SOURCES.txt
+-rw-r--r--   0 bakircius   (501) staff       (20)        1 2024-03-23 14:28:31.000000 sosq-1.0.3/src/sosq.egg-info/dependency_links.txt
+-rw-r--r--   0 bakircius   (501) staff       (20)       29 2024-03-23 14:28:31.000000 sosq-1.0.3/src/sosq.egg-info/requires.txt
+-rw-r--r--   0 bakircius   (501) staff       (20)        5 2024-03-23 14:28:31.000000 sosq-1.0.3/src/sosq.egg-info/top_level.txt
+drwxr-xr-x   0 bakircius   (501) staff       (20)        0 2024-03-23 14:28:31.102376 sosq-1.0.3/tests/
+-rw-r--r--   0 bakircius   (501) staff       (20)       33 2024-02-29 06:12:58.000000 sosq-1.0.3/tests/test_getResults.py
```

### Comparing `sosq-1.0.2/LICENSE` & `sosq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sosq-1.0.2/pyproject.toml` & `sosq-1.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 [project]
 name = "sosq"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="bakircius", email="burakbakirci@gmail.com" },
 ]
 description = "Building Dataframe from Stack Overflow API with a search query"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "requests",
     "pandas",
-    "numpy"
+    "numpy",
+    "typing"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Development Status :: 5 - Production/Stable",
+    "Framework :: IDLE",
+    "Intended Audience :: Developers",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: Information Analysis"
 ]
 [project.urls]
 Source = "https://github.com/bakircius/sosq"
 Issues = "https://github.com/bakircius/sosq/issues"
 Repository = "https://github.com/bakircius/sosq.git"
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `sosq-1.0.2/src/sosq/__init__.py` & `sosq-1.0.3/src/sosq/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     """Process the API response, returning a DataFrame, has_more, and quota_remaining indicators."""
     df = pd.DataFrame(data=response["items"])
     has_more = response["has_more"]
     quota_remaining = response["quota_remaining"] > 500
     return df, has_more, quota_remaining
 
 def append_dataframes(df1: pd.DataFrame, df2: pd.DataFrame) -> pd.DataFrame:
-    """Append one DataFrame to another, handling the first iteration case."""
+    """Append one DataFrame to another, handling the first iteration case.
+    append deprecated, concat usesd instead.
+    
+    """
     if df1 is None:
         return df2
     else:
         df1 = pd.concat([df1, df2])
         return df1
 
 def update_params(params: Dict[str, str], page: int) -> Dict[str, str]:
@@ -76,14 +79,8 @@
         df_combined = append_dataframes(df_combined, df)
         page += 1
         params = update_params(params, page)
         print("Page", page, "ok")
 
     save_to_csv(df_combined, query + ".csv")
     return df_combined
-    print("Query for", query, "successfully saved as csv")
-
-# Uncomment to run the getResults function
-df = get_result('ibm-cloud-api', '03Geb7p3Isfshr2VDAdkrA((', 'WH2dFoAm0Ol4Q61TIi*0Pg))')
-
-
-# results will be in your project folder.
+    print("Query for", query, "successfully saved as csv")
```

