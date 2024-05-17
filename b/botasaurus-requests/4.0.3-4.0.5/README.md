# Comparing `tmp/botasaurus_requests-4.0.3.tar.gz` & `tmp/botasaurus_requests-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_requests-4.0.3.tar", last modified: Thu May 16 15:05:38 2024, max compression
+gzip compressed data, was "botasaurus_requests-4.0.5.tar", last modified: Thu May 16 16:08:58 2024, max compression
```

## Comparing `botasaurus_requests-4.0.3.tar` & `botasaurus_requests-4.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.684731 botasaurus_requests-4.0.3/
--rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.3/LICENSE
--rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14535 2024-05-16 15:05:38.683715 botasaurus_requests-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-05-16 07:09:14.000000 botasaurus_requests-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.627621 botasaurus_requests-4.0.3/botasaurus_requests/
--rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.3/botasaurus_requests/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/__main__.py
--rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.678490 botasaurus_requests-4.0.3/botasaurus_requests/bin/
--rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.3/botasaurus_requests/bin/__init__.py
--rw-rw-rw-   0        0        0     7338 2024-05-16 13:27:52.000000 botasaurus_requests-4.0.3/botasaurus_requests/cffi.py
--rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.3/botasaurus_requests/client.py
--rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.3/botasaurus_requests/cookies.py
--rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.3/botasaurus_requests/exceptions.py
--rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/headers.py
--rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/parser.py
--rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.3/botasaurus_requests/reqs.py
--rw-rw-rw-   0        0        0     8486 2024-05-16 11:43:30.000000 botasaurus_requests-4.0.3/botasaurus_requests/request_class.py
--rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.3/botasaurus_requests/request_functions.py
--rw-rw-rw-   0        0        0     9871 2024-05-16 15:04:13.000000 botasaurus_requests-4.0.3/botasaurus_requests/response.py
--rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/session.py
--rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.3/botasaurus_requests/toolbelt.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.681515 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/
--rw-rw-rw-   0        0        0    14535 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2024-05-16 15:05:36.000000 botasaurus_requests-4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-16 15:05:38.688470 botasaurus_requests-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.065683 botasaurus_requests-4.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.5/LICENSE
+-rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    14770 2024-05-16 16:08:58.064833 botasaurus_requests-4.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-05-16 16:06:45.000000 botasaurus_requests-4.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.008049 botasaurus_requests-4.0.5/botasaurus_requests/
+-rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.5/botasaurus_requests/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/__main__.py
+-rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.059888 botasaurus_requests-4.0.5/botasaurus_requests/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.5/botasaurus_requests/bin/__init__.py
+-rw-rw-rw-   0        0        0     7338 2024-05-16 13:27:52.000000 botasaurus_requests-4.0.5/botasaurus_requests/cffi.py
+-rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.5/botasaurus_requests/client.py
+-rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.5/botasaurus_requests/cookies.py
+-rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.5/botasaurus_requests/exceptions.py
+-rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/headers.py
+-rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/parser.py
+-rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.5/botasaurus_requests/reqs.py
+-rw-rw-rw-   0        0        0     8395 2024-05-16 16:07:08.000000 botasaurus_requests-4.0.5/botasaurus_requests/request_class.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.5/botasaurus_requests/request_functions.py
+-rw-rw-rw-   0        0        0     9871 2024-05-16 15:04:13.000000 botasaurus_requests-4.0.5/botasaurus_requests/response.py
+-rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/session.py
+-rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.5/botasaurus_requests/toolbelt.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.062134 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/
+-rw-rw-rw-   0        0        0    14770 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1008 2024-05-16 16:08:55.000000 botasaurus_requests-4.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-16 16:08:58.068862 botasaurus_requests-4.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.5/setup.py
```

### Comparing `botasaurus_requests-4.0.3/LICENSE` & `botasaurus_requests-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/PKG-INFO` & `botasaurus_requests-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.3
+Version: 4.0.5
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,15 +218,19 @@
 Requires-Dist: urllib3
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: gevent
 
 # Botasaurus Requests
 
-botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library with the playwright dependencies removed.
+botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library, featuring the following updates:
+
+- Removal of the playwright dependencies, to make it more lightweight.
+- Bug fixes to ensure smooth execution on Windows, eliminating runtime errors.
+- Addition of the Google Referer header in the get method to make requests more humane.
 
 ## Installation
 
 ```bash
 pip install botasaurus-requests
 ```
```

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/__init__.py` & `botasaurus_requests-4.0.5/botasaurus_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/__main__.py` & `botasaurus_requests-4.0.5/botasaurus_requests/__main__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/cffi.py` & `botasaurus_requests-4.0.5/botasaurus_requests/cffi.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/client.py` & `botasaurus_requests-4.0.5/botasaurus_requests/client.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/cookies.py` & `botasaurus_requests-4.0.5/botasaurus_requests/cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/exceptions.py` & `botasaurus_requests-4.0.5/botasaurus_requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/headers.py` & `botasaurus_requests-4.0.5/botasaurus_requests/headers.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/parser.py` & `botasaurus_requests-4.0.5/botasaurus_requests/parser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/reqs.py` & `botasaurus_requests-4.0.5/botasaurus_requests/reqs.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/request_class.py` & `botasaurus_requests-4.0.5/botasaurus_requests/request_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Request(Session):
 
     def __init__(self, proxy=None):
         self._proxy = proxy
 
     def get(
         self,
-        url: str | bytes,
+        url,
         referer="https://www.google.com/",
         params=None,
         data=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
@@ -53,15 +53,15 @@
 
         kwargs = {k: v for k, v in named_args.items() if v is not None}
 
         return reqs.get(url, **kwargs)
 
     def options(
         self,
-        url: str | bytes,
+        url,
         params=None,
         data=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
         auth=None,
@@ -93,15 +93,15 @@
                 "browser": browser,
             }
         )
         return reqs.options(url, **self._merge_kwargs(kwargs))
 
     def head(
         self,
-        url: str | bytes,
+        url,
         params=None,
         data=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
         auth=None,
@@ -133,15 +133,15 @@
                 "browser": browser,
             }
         )
         return reqs.head(url, **self._merge_kwargs(kwargs))
 
     def post(
         self,
-        url: str | bytes,
+        url,
         data=None,
         json=None,
         params=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
@@ -173,15 +173,15 @@
                 "browser": browser,
             }
         )
         return reqs.post(url, **self._merge_kwargs(kwargs))
 
     def put(
         self,
-        url: str | bytes,
+        url,
         data=None,
         json=None,
         params=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
@@ -213,15 +213,15 @@
                 "browser": browser,
             }
         )
         return reqs.put(url, **kwargs)
 
     def patch(
         self,
-        url: str | bytes,
+        url,
         data=None,
         json=None,
         params=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
@@ -253,15 +253,15 @@
                 "browser": browser,
             }
         )
         return reqs.patch(url, **self._merge_kwargs(kwargs))
 
     def delete(
         self,
-        url: str | bytes,
+        url,
         params=None,
         data=None,
         headers=None,
         browser: Optional[Literal["firefox", "chrome"]] = "firefox",
         cookies=None,
         files=None,
         auth=None,
```

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/response.py` & `botasaurus_requests-4.0.5/botasaurus_requests/response.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/session.py` & `botasaurus_requests-4.0.5/botasaurus_requests/session.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests/toolbelt.py` & `botasaurus_requests-4.0.5/botasaurus_requests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests.egg-info/PKG-INFO` & `botasaurus_requests-4.0.5/botasaurus_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.3
+Version: 4.0.5
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,15 +218,19 @@
 Requires-Dist: urllib3
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: gevent
 
 # Botasaurus Requests
 
-botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library with the playwright dependencies removed.
+botasaurus-requests is a fork of the [hrequests](https://github.com/daijro/hrequests) library, featuring the following updates:
+
+- Removal of the playwright dependencies, to make it more lightweight.
+- Bug fixes to ensure smooth execution on Windows, eliminating runtime errors.
+- Addition of the Google Referer header in the get method to make requests more humane.
 
 ## Installation
 
 ```bash
 pip install botasaurus-requests
 ```
```

### Comparing `botasaurus_requests-4.0.3/botasaurus_requests.egg-info/SOURCES.txt` & `botasaurus_requests-4.0.5/botasaurus_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.3/pyproject.toml` & `botasaurus_requests-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_requests"
-version="4.0.3"
+version="4.0.5"
 description = "botasaurus_requests is a fork of the requests library with the playwright dependencies removed."
 authors = [
   {name = "Chetan", email = "chetan@omkar.cloud" } # Optional
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
```

