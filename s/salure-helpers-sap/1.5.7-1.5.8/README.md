# Comparing `tmp/salure_helpers_sap-1.5.7.tar.gz` & `tmp/salure_helpers_sap-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_sap-1.5.7.tar", last modified: Tue Apr  2 18:52:01 2024, max compression
+gzip compressed data, was "dist/salure_helpers_sap-1.5.8.tar", last modified: Wed Apr  3 08:43:24 2024, max compression
```

## Comparing `salure_helpers_sap-1.5.7.tar` & `salure_helpers_sap-1.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10687 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/base_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     7670 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/delimit_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/get_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    22850 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/post_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/salure_helpers/sap/sap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/salure_helpers_sap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 18:52:01.000000 salure_helpers_sap-1.5.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-04-02 18:51:45.000000 salure_helpers_sap-1.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/base_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7670 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/delimit_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/get_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    22850 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/post_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/salure_helpers/sap/sap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/salure_helpers_sap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:43:24.000000 salure_helpers_sap-1.5.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-04-03 08:43:06.000000 salure_helpers_sap-1.5.8/setup.py
```

### Comparing `salure_helpers_sap-1.5.7/salure_helpers/sap/base_functions.py` & `salure_helpers_sap-1.5.8/salure_helpers/sap/base_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
                     doc = etree.XML(response.content)
                     error_code = doc.getchildren()[0].text
                     error_message = doc.getchildren()[1].text
                     error_details = doc.getchildren()[2].getchildren()[4].getchildren()[0].getchildren()[1].text
                     error_details_status = doc.getchildren()[2].getchildren()[4].getchildren()[0].getchildren()[3].text
                     error_details_status = "" if error_details_status is None else f"\r\nReal Status: {error_details_status}\r\n"
                 except Exception:
+                    error_code = ""
+                    error_message = "Error in the response from SAP parsing the XML"
                     error_details = ""
                     error_details_status = ""
                 raise HTTPError(
                     f'Error from SAP while calling endpoint {uri}. \r\nThe message is \"{error_message}\" with code {error_code}, \r\nDetails: {error_details}{error_details_status}', response=response)
             else:
                 raise HTTPError(f'Error from SAP while calling endpoint {uri}. There is no message with code {response.status_code}', response=response)
```

### Comparing `salure_helpers_sap-1.5.7/salure_helpers/sap/delimit_endpoints.py` & `salure_helpers_sap-1.5.8/salure_helpers/sap/delimit_endpoints.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.7/salure_helpers/sap/get_endpoints.py` & `salure_helpers_sap-1.5.8/salure_helpers/sap/get_endpoints.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.7/salure_helpers/sap/post_endpoints.py` & `salure_helpers_sap-1.5.8/salure_helpers/sap/post_endpoints.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.7/salure_helpers/sap/sap.py` & `salure_helpers_sap-1.5.8/salure_helpers/sap/sap.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.7/setup.py` & `salure_helpers_sap-1.5.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='salure_helpers_sap',
-    version='1.5.7',
+    version='1.5.8',
     description='SAP wrapper from Salure',
     long_description='SAP wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.sap"],
     license='Salure License',
     install_requires=[
```

