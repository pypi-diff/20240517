# Comparing `tmp/browsercookie-0.7.8.tar.gz` & `tmp/browsercookie-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browsercookie-0.7.8.tar", last modified: Fri Mar 22 02:30:33 2024, max compression
+gzip compressed data, was "browsercookie-0.7.9.tar", last modified: Fri May 17 02:36:24 2024, max compression
```

## Comparing `browsercookie-0.7.8.tar` & `browsercookie-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-22 02:30:33.268977 browsercookie-0.7.8/
--rw-r--r--   0 baron      (501) staff       (20)    26530 2024-03-22 02:29:09.000000 browsercookie-0.7.8/LICENSE.txt
--rw-r--r--   0 baron      (501) staff       (20)       19 2024-03-22 02:29:09.000000 browsercookie-0.7.8/MANIFEST.in
--rw-r--r--   0 baron      (501) staff       (20)     3697 2024-03-22 02:30:33.268864 browsercookie-0.7.8/PKG-INFO
--rw-r--r--   0 baron      (501) staff       (20)     3298 2024-03-22 02:29:09.000000 browsercookie-0.7.8/README.rst
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-22 02:30:33.268037 browsercookie-0.7.8/browsercookie/
--rw-r--r--   0 baron      (501) staff       (20)    24152 2024-03-22 02:29:09.000000 browsercookie-0.7.8/browsercookie/__init__.py
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-22 02:30:33.268680 browsercookie-0.7.8/browsercookie.egg-info/
--rw-r--r--   0 baron      (501) staff       (20)     3697 2024-03-22 02:30:33.000000 browsercookie-0.7.8/browsercookie.egg-info/PKG-INFO
--rw-r--r--   0 baron      (501) staff       (20)      253 2024-03-22 02:30:33.000000 browsercookie-0.7.8/browsercookie.egg-info/SOURCES.txt
--rw-r--r--   0 baron      (501) staff       (20)        1 2024-03-22 02:30:33.000000 browsercookie-0.7.8/browsercookie.egg-info/dependency_links.txt
--rw-r--r--   0 baron      (501) staff       (20)       61 2024-03-22 02:30:33.000000 browsercookie-0.7.8/browsercookie.egg-info/requires.txt
--rw-r--r--   0 baron      (501) staff       (20)       14 2024-03-22 02:30:33.000000 browsercookie-0.7.8/browsercookie.egg-info/top_level.txt
--rw-r--r--   0 baron      (501) staff       (20)       38 2024-03-22 02:30:33.269017 browsercookie-0.7.8/setup.cfg
--rw-r--r--   0 baron      (501) staff       (20)      743 2024-03-22 02:29:53.000000 browsercookie-0.7.8/setup.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-05-17 02:36:24.254326 browsercookie-0.7.9/
+-rw-r--r--   0 baron      (501) staff       (20)    26530 2024-03-22 02:29:09.000000 browsercookie-0.7.9/LICENSE.txt
+-rw-r--r--   0 baron      (501) staff       (20)       19 2024-03-22 02:29:09.000000 browsercookie-0.7.9/MANIFEST.in
+-rw-r--r--   0 baron      (501) staff       (20)     3815 2024-05-17 02:36:24.254143 browsercookie-0.7.9/PKG-INFO
+-rw-r--r--   0 baron      (501) staff       (20)     3298 2024-03-22 02:29:09.000000 browsercookie-0.7.9/README.rst
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-05-17 02:36:24.253038 browsercookie-0.7.9/browsercookie/
+-rw-r--r--   0 baron      (501) staff       (20)    24323 2024-05-17 02:35:03.000000 browsercookie-0.7.9/browsercookie/__init__.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-05-17 02:36:24.253944 browsercookie-0.7.9/browsercookie.egg-info/
+-rw-r--r--   0 baron      (501) staff       (20)     3815 2024-05-17 02:36:24.000000 browsercookie-0.7.9/browsercookie.egg-info/PKG-INFO
+-rw-r--r--   0 baron      (501) staff       (20)      253 2024-05-17 02:36:24.000000 browsercookie-0.7.9/browsercookie.egg-info/SOURCES.txt
+-rw-r--r--   0 baron      (501) staff       (20)        1 2024-05-17 02:36:24.000000 browsercookie-0.7.9/browsercookie.egg-info/dependency_links.txt
+-rw-r--r--   0 baron      (501) staff       (20)       61 2024-05-17 02:36:24.000000 browsercookie-0.7.9/browsercookie.egg-info/requires.txt
+-rw-r--r--   0 baron      (501) staff       (20)       14 2024-05-17 02:36:24.000000 browsercookie-0.7.9/browsercookie.egg-info/top_level.txt
+-rw-r--r--   0 baron      (501) staff       (20)       38 2024-05-17 02:36:24.254362 browsercookie-0.7.9/setup.cfg
+-rw-r--r--   0 baron      (501) staff       (20)      743 2024-05-17 02:35:13.000000 browsercookie-0.7.9/setup.py
```

### Comparing `browsercookie-0.7.8/LICENSE.txt` & `browsercookie-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsercookie-0.7.8/PKG-INFO` & `browsercookie-0.7.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: browsercookie
-Version: 0.7.8
-Summary: Loads cookies from your browser into a cookiejar object so can download with urllib and other libraries the same content you see in the web browser.
-Home-page: https://github.com/richardpenman/browsercookie
-Author: Richard Penman
-Author-email: richard.penman@gmail.com
-License: lgpl
-Requires-Python: >=3.4
-License-File: LICENSE.txt
-
 Browser Cookie
 ==============
 
 The **browsercookie** module loads cookies used by your web browser
 into a cookiejar object. This can be useful if you want to use python to
 download the same content you see in the web browser without needing to
 login.
```

#### html2text {}

```diff
@@ -1,16 +1,11 @@
-Metadata-Version: 2.1 Name: browsercookie Version: 0.7.8 Summary: Loads cookies
-from your browser into a cookiejar object so can download with urllib and other
-libraries the same content you see in the web browser. Home-page: https://
-github.com/richardpenman/browsercookie Author: Richard Penman Author-email:
-richard.penman@gmail.com License: lgpl Requires-Python: >=3.4 License-File:
-LICENSE.txt Browser Cookie ============== The **browsercookie** module loads
-cookies used by your web browser into a cookiejar object. This can be useful if
-you want to use python to download the same content you see in the web browser
-without needing to login. Install ------- .. sourcecode:: bash pip install
+Browser Cookie ============== The **browsercookie** module loads cookies used
+by your web browser into a cookiejar object. This can be useful if you want to
+use python to download the same content you see in the web browser without
+needing to login. Install ------- .. sourcecode:: bash pip install
 browsercookie On Windows the builtin sqlite module will raise an error when
 loading the FireFox database. An updated version of sqlite can be installed
 with: .. sourcecode:: bash pip install pysqlite Usage ----- Here is a hack to
 extract the title from a webpage: .. sourcecode:: python >>> import re >>>
 get_title = lambda html: re.findall('
 ', html, flags=re.DOTALL)[0].strip() And here is the webpage title when
 downloaded normally: .. sourcecode:: python >>> import urllib2 >>> url =
```

### Comparing `browsercookie-0.7.8/README.rst` & `browsercookie-0.7.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: browsercookie
+Version: 0.7.9
+Summary: Loads cookies from your browser into a cookiejar object so can download with urllib and other libraries the same content you see in the web browser.
+Home-page: https://github.com/richardpenman/browsercookie
+Author: Richard Penman
+Author-email: richard.penman@gmail.com
+License: lgpl
+Requires-Python: >=3.4
+License-File: LICENSE.txt
+Requires-Dist: pycryptodome
+Requires-Dist: keyring
+Requires-Dist: lz4
+Requires-Dist: pywin32; sys_platform == "win32"
+
 Browser Cookie
 ==============
 
 The **browsercookie** module loads cookies used by your web browser
 into a cookiejar object. This can be useful if you want to use python to
 download the same content you see in the web browser without needing to
 login.
```

#### html2text {}

```diff
@@ -1,16 +1,23 @@
-Browser Cookie ============== The **browsercookie** module loads cookies used
-by your web browser into a cookiejar object. This can be useful if you want to
-use python to download the same content you see in the web browser without
-needing to login. Install ------- .. sourcecode:: bash pip install
-browsercookie On Windows the builtin sqlite module will raise an error when
-loading the FireFox database. An updated version of sqlite can be installed
-with: .. sourcecode:: bash pip install pysqlite Usage ----- Here is a hack to
-extract the title from a webpage: .. sourcecode:: python >>> import re >>>
-get_title = lambda html: re.findall('
+Metadata-Version: 2.1 Name: browsercookie Version: 0.7.9 Summary: Loads cookies
+from your browser into a cookiejar object so can download with urllib and other
+libraries the same content you see in the web browser. Home-page: https://
+github.com/richardpenman/browsercookie Author: Richard Penman Author-email:
+richard.penman@gmail.com License: lgpl Requires-Python: >=3.4 License-File:
+LICENSE.txt Requires-Dist: pycryptodome Requires-Dist: keyring Requires-Dist:
+lz4 Requires-Dist: pywin32; sys_platform == "win32" Browser Cookie
+============== The **browsercookie** module loads cookies used by your web
+browser into a cookiejar object. This can be useful if you want to use python
+to download the same content you see in the web browser without needing to
+login. Install ------- .. sourcecode:: bash pip install browsercookie On
+Windows the builtin sqlite module will raise an error when loading the FireFox
+database. An updated version of sqlite can be installed with: .. sourcecode::
+bash pip install pysqlite Usage ----- Here is a hack to extract the title from
+a webpage: .. sourcecode:: python >>> import re >>> get_title = lambda html:
+re.findall('
 ', html, flags=re.DOTALL)[0].strip() And here is the webpage title when
 downloaded normally: .. sourcecode:: python >>> import urllib2 >>> url =
 'https://bitbucket.org/' >>> public_html = urllib2.urlopen(url).read() >>>
 get_title(public_html) 'Git and Mercurial code management for teams' Now let's
 try with **browsercookie** - make sure you are logged into Bitbucket in Firefox
 before trying this example: .. sourcecode:: python >>> import browsercookie >>>
 cj = browsercookie.firefox() >>> opener = urllib2.build_opener
```

### Comparing `browsercookie-0.7.8/browsercookie/__init__.py` & `browsercookie-0.7.9/browsercookie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,17 @@
             return str(path.expanduser().absolute())
         raise BrowserCookieError('No default Firefox profile found')
 
     def find_default_profile(self):
         if sys.platform == 'darwin':
             return glob.glob(os.path.expanduser('~/Library/Application Support/Firefox/profiles.ini'))
         elif sys.platform.startswith('linux'):
-            return glob.glob(os.path.expanduser('~/.mozilla/firefox/profiles.ini'))
+            trad_filename = glob.glob(os.path.expanduser('~/.mozilla/firefox/profiles.ini'))
+            snap_filename = glob.glob(os.path.expanduser('~/snap/firefox/common/.mozilla/firefox/profiles.ini'))
+            return trad_filename + snap_filename
         elif sys.platform == 'win32':
             return glob.glob(os.path.join(os.getenv('APPDATA', ''), 'Mozilla/Firefox/profiles.ini'))
         else:
             raise BrowserCookieError('Unsupported operating system: ' + sys.platform)
 
     def find_cookie_files(self):
         profile = self.find_default_profile()
```

### Comparing `browsercookie-0.7.8/browsercookie.egg-info/PKG-INFO` & `browsercookie-0.7.9/browsercookie.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: browsercookie
-Version: 0.7.8
+Version: 0.7.9
 Summary: Loads cookies from your browser into a cookiejar object so can download with urllib and other libraries the same content you see in the web browser.
 Home-page: https://github.com/richardpenman/browsercookie
 Author: Richard Penman
 Author-email: richard.penman@gmail.com
 License: lgpl
 Requires-Python: >=3.4
 License-File: LICENSE.txt
+Requires-Dist: pycryptodome
+Requires-Dist: keyring
+Requires-Dist: lz4
+Requires-Dist: pywin32; sys_platform == "win32"
 
 Browser Cookie
 ==============
 
 The **browsercookie** module loads cookies used by your web browser
 into a cookiejar object. This can be useful if you want to use python to
 download the same content you see in the web browser without needing to
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.1 Name: browsercookie Version: 0.7.8 Summary: Loads cookies
+Metadata-Version: 2.1 Name: browsercookie Version: 0.7.9 Summary: Loads cookies
 from your browser into a cookiejar object so can download with urllib and other
 libraries the same content you see in the web browser. Home-page: https://
 github.com/richardpenman/browsercookie Author: Richard Penman Author-email:
 richard.penman@gmail.com License: lgpl Requires-Python: >=3.4 License-File:
-LICENSE.txt Browser Cookie ============== The **browsercookie** module loads
-cookies used by your web browser into a cookiejar object. This can be useful if
-you want to use python to download the same content you see in the web browser
-without needing to login. Install ------- .. sourcecode:: bash pip install
-browsercookie On Windows the builtin sqlite module will raise an error when
-loading the FireFox database. An updated version of sqlite can be installed
-with: .. sourcecode:: bash pip install pysqlite Usage ----- Here is a hack to
-extract the title from a webpage: .. sourcecode:: python >>> import re >>>
-get_title = lambda html: re.findall('
+LICENSE.txt Requires-Dist: pycryptodome Requires-Dist: keyring Requires-Dist:
+lz4 Requires-Dist: pywin32; sys_platform == "win32" Browser Cookie
+============== The **browsercookie** module loads cookies used by your web
+browser into a cookiejar object. This can be useful if you want to use python
+to download the same content you see in the web browser without needing to
+login. Install ------- .. sourcecode:: bash pip install browsercookie On
+Windows the builtin sqlite module will raise an error when loading the FireFox
+database. An updated version of sqlite can be installed with: .. sourcecode::
+bash pip install pysqlite Usage ----- Here is a hack to extract the title from
+a webpage: .. sourcecode:: python >>> import re >>> get_title = lambda html:
+re.findall('
 ', html, flags=re.DOTALL)[0].strip() And here is the webpage title when
 downloaded normally: .. sourcecode:: python >>> import urllib2 >>> url =
 'https://bitbucket.org/' >>> public_html = urllib2.urlopen(url).read() >>>
 get_title(public_html) 'Git and Mercurial code management for teams' Now let's
 try with **browsercookie** - make sure you are logged into Bitbucket in Firefox
 before trying this example: .. sourcecode:: python >>> import browsercookie >>>
 cj = browsercookie.firefox() >>> opener = urllib2.build_opener
```

### Comparing `browsercookie-0.7.8/setup.py` & `browsercookie-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name='browsercookie', 
-    version='0.7.8',
+    version='0.7.9',
     python_requires='>=3.4',
     packages=['browsercookie'],
     author='Richard Penman',
     author_email='richard.penman@gmail.com',
     description='Loads cookies from your browser into a cookiejar object so can download with urllib and other libraries the same content you see in the web browser.',
     long_description=read('README.rst'),
     url='https://github.com/richardpenman/browsercookie',
```

