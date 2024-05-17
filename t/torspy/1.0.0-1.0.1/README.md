# Comparing `tmp/torspy-1.0.0.tar.gz` & `tmp/torspy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torspy-1.0.0.tar", last modified: Fri May 17 09:50:24 2024, max compression
+gzip compressed data, was "torspy-1.0.1.tar", last modified: Fri May 17 10:16:10 2024, max compression
```

## Comparing `torspy-1.0.0.tar` & `torspy-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 09:50:23.992066 torspy-1.0.0/
--rw-rw-rw-   0        0        0     1065 2024-05-17 09:47:56.000000 torspy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5549 2024-05-17 09:50:23.992066 torspy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4846 2024-05-17 09:47:56.000000 torspy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 09:50:23.992066 torspy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-17 09:48:37.000000 torspy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 09:50:23.945188 torspy-1.0.0/torspy/
--rw-rw-rw-   0        0        0       78 2024-05-17 09:47:56.000000 torspy-1.0.0/torspy/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-17 09:47:56.000000 torspy-1.0.0/torspy/cli.py
--rw-rw-rw-   0        0        0     4887 2024-05-17 09:47:56.000000 torspy-1.0.0/torspy/scraper.py
--rw-rw-rw-   0        0        0      102 2024-05-17 09:47:56.000000 torspy-1.0.0/torspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 09:50:23.992066 torspy-1.0.0/torspy.egg-info/
--rw-rw-rw-   0        0        0     5549 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 09:50:23.000000 torspy-1.0.0/torspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.956159 torspy-1.0.1/
+-rw-rw-rw-   0        0        0     1065 2024-05-17 10:15:32.000000 torspy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5549 2024-05-17 10:16:10.956159 torspy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4846 2024-05-17 10:15:32.000000 torspy-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:16:10.956159 torspy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-05-17 10:15:32.000000 torspy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.909307 torspy-1.0.1/torspy/
+-rw-rw-rw-   0        0        0       78 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/__init__.py
+-rw-rw-rw-   0        0        0     1145 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/cli.py
+-rw-rw-rw-   0        0        0     4887 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/scraper.py
+-rw-rw-rw-   0        0        0      102 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.956159 torspy-1.0.1/torspy.egg-info/
+-rw-rw-rw-   0        0        0     5549 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/top_level.txt
```

### Comparing `torspy-1.0.0/LICENSE` & `torspy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torspy-1.0.0/PKG-INFO` & `torspy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tor onion site scraping tool
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Keywords: mrfidal,tor,DarkWeb,onion,torspy,scraping,dark web,web scraping,hidden services,privacy,security,beautifulsoup4,requests,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torspy-1.0.0/README.md` & `torspy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `torspy-1.0.0/setup.py` & `torspy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='torspy',
-    version='1.0.0',
+    version='1.0.1',
     author='Fidal',
     author_email='mrfidal@proton.me',
     description='Tor onion site scraping tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mr-fidal/torspy',
     packages=find_packages(),
```

### Comparing `torspy-1.0.0/torspy/cli.py` & `torspy-1.0.1/torspy/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/python3
 # copyright ©️ 2024 author Fidal
 
 import argparse
-from .scraper import scrape_onion_site
+from .scraper import scrape_onion_site, find_directories
 
 def main():
     epilog_text = '''
-Copyright (©️) 2024 author: Fidal
-Issue: https://GitHub.com/mr-fidal/torspy
+Copyright (c) 2024 Author: Fidal
+Report an Issue : https://github.com/mr-fidal/torspy/issues
 '''
     parser = argparse.ArgumentParser(description='Scrape a .onion site.', epilog=epilog_text,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('url', type=str, help='The .onion site URL to scrape')
     parser.add_argument('--find', type=str, help='The text to search for within the site')
     parser.add_argument('-s', '--save', type=str, help='The file name to save the content')
     parser.add_argument('-d', '--directory', type=str, help='The directory to save the file')
-    parser.add_argument('--proxy', type=str, help='The proxy server to use')
-    parser.add_argument('--user-agent', type=str, help='The User-Agent string to use')
-    parser.add_argument('--directories', type=str, help='File containing directories to check')
+    parser.add_argument('--dir', type=str, help='File with list of directories to check')
     args = parser.parse_args()
-    scrape_onion_site(args.url, args.find, args.save, args.directory, args.proxy, args.user_agent, args.directories)
+    
+    if args.dir:
+        find_directories(args.url, args.dir, args.save, args.directory)
+    else:
+        scrape_onion_site(args.url, args.find, args.save, args.directory)
 
 if __name__ == "__main__":
     main()
```

### Comparing `torspy-1.0.0/torspy/scraper.py` & `torspy-1.0.1/torspy/scraper.py`

 * *Files identical despite different names*

### Comparing `torspy-1.0.0/torspy.egg-info/PKG-INFO` & `torspy-1.0.1/torspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tor onion site scraping tool
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Keywords: mrfidal,tor,DarkWeb,onion,torspy,scraping,dark web,web scraping,hidden services,privacy,security,beautifulsoup4,requests,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

