# Comparing `tmp/kokojson-0.1.0.tar.gz` & `tmp/kokojson-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kokojson-0.1.0.tar", last modified: Thu May 16 22:22:31 2024, max compression
+gzip compressed data, was "kokojson-0.1.1.tar", last modified: Thu May 16 22:28:13 2024, max compression
```

## Comparing `kokojson-0.1.0.tar` & `kokojson-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-16 22:22:31.798623 kokojson-0.1.0/
--rw-r--r--   0 ct         (502) staff       (20)     1778 2024-05-16 22:22:31.798516 kokojson-0.1.0/PKG-INFO
-drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-16 22:22:31.798358 kokojson-0.1.0/kokojson.egg-info/
--rw-r--r--   0 ct         (502) staff       (20)     1778 2024-05-16 22:22:31.000000 kokojson-0.1.0/kokojson.egg-info/PKG-INFO
--rw-r--r--   0 ct         (502) staff       (20)      136 2024-05-16 22:22:31.000000 kokojson-0.1.0/kokojson.egg-info/SOURCES.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-16 22:22:31.000000 kokojson-0.1.0/kokojson.egg-info/dependency_links.txt
--rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-16 22:22:31.000000 kokojson-0.1.0/kokojson.egg-info/top_level.txt
--rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-16 22:22:31.798659 kokojson-0.1.0/setup.cfg
--rw-r--r--   0 ct         (502) staff       (20)     1897 2024-05-16 22:20:10.000000 kokojson-0.1.0/setup.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-16 22:28:13.120911 kokojson-0.1.1/
+-rw-r--r--   0 ct         (502) staff       (20)     1766 2024-05-16 22:28:13.120713 kokojson-0.1.1/PKG-INFO
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-16 22:28:13.119717 kokojson-0.1.1/kokojson/
+-rw-r--r--   0 ct         (502) staff       (20)       23 2024-05-16 22:26:12.000000 kokojson-0.1.1/kokojson/__init__.py
+-rw-r--r--   0 ct         (502) staff       (20)     1194 2024-05-16 22:26:00.000000 kokojson-0.1.1/kokojson/main.py
+drwxr-xr-x   0 ct         (502) staff       (20)        0 2024-05-16 22:28:13.120491 kokojson-0.1.1/kokojson.egg-info/
+-rw-r--r--   0 ct         (502) staff       (20)     1766 2024-05-16 22:28:13.000000 kokojson-0.1.1/kokojson.egg-info/PKG-INFO
+-rw-r--r--   0 ct         (502) staff       (20)      174 2024-05-16 22:28:13.000000 kokojson-0.1.1/kokojson.egg-info/SOURCES.txt
+-rw-r--r--   0 ct         (502) staff       (20)        1 2024-05-16 22:28:13.000000 kokojson-0.1.1/kokojson.egg-info/dependency_links.txt
+-rw-r--r--   0 ct         (502) staff       (20)        9 2024-05-16 22:28:13.000000 kokojson-0.1.1/kokojson.egg-info/top_level.txt
+-rw-r--r--   0 ct         (502) staff       (20)       38 2024-05-16 22:28:13.120958 kokojson-0.1.1/setup.cfg
+-rw-r--r--   0 ct         (502) staff       (20)     1922 2024-05-16 22:28:09.000000 kokojson-0.1.1/setup.py
```

### Comparing `kokojson-0.1.0/PKG-INFO` & `kokojson-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: kokojson
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for safe JSON handling in Python
 Home-page: https://github.com/your_username/kokojson
-Author: Your Name
-Author-email: your.email@example.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author: kokofixcomputers
+Author-email: kokocanfixit@kokofixcomputers.serv00.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -56,9 +54,7 @@
 print(json_data.get("person").get("email"))  # Output: None
 print(json_data.get("company").get("website"))  # Output: None
 
 # Provide a default value for non-existing keys
 print(json_data.get("person").get("email", "No email found"))  # Output: No email found
 print(json_data.get("company").get("website", "https://example.com"))  # Output: https://example.com
 ```
-
-
```

### Comparing `kokojson-0.1.0/kokojson.egg-info/PKG-INFO` & `kokojson-0.1.1/kokojson.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: kokojson
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for safe JSON handling in Python
 Home-page: https://github.com/your_username/kokojson
-Author: Your Name
-Author-email: your.email@example.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author: kokofixcomputers
+Author-email: kokocanfixit@kokofixcomputers.serv00.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -56,9 +54,7 @@
 print(json_data.get("person").get("email"))  # Output: None
 print(json_data.get("company").get("website"))  # Output: None
 
 # Provide a default value for non-existing keys
 print(json_data.get("person").get("email", "No email found"))  # Output: No email found
 print(json_data.get("company").get("website", "https://example.com"))  # Output: https://example.com
 ```
-
-
```

### Comparing `kokojson-0.1.0/setup.py` & `kokojson-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kokojson",
-    version="0.1.0",
-    author="Your Name",
-    author_email="your.email@example.com",
+    version="0.1.1",
+    author="kokofixcomputers",
+    author_email="kokocanfixit@kokofixcomputers.serv00.net",
     description="A module for safe JSON handling in Python",
     long_description='''## A module for safe JSON handling in Python
 
 ### Example Usage:
 data.json:
 ```json
 {
```

