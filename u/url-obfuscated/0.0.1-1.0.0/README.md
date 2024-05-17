# Comparing `tmp/url-obfuscated-0.0.1.tar.gz` & `tmp/url-obfuscated-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url-obfuscated-0.0.1.tar", last modified: Fri Mar 17 05:42:39 2023, max compression
+gzip compressed data, was "url-obfuscated-1.0.0.tar", last modified: Fri May 17 06:51:02 2024, max compression
```

## Comparing `url-obfuscated-0.0.1.tar` & `url-obfuscated-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11357 2023-03-16 10:19:39.000000 url-obfuscated-0.0.1/LICENSE
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       34 2023-03-15 11:16:56.000000 url-obfuscated-0.0.1/MANIFEST.in
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     3399 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/PKG-INFO
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     2055 2023-03-16 10:19:39.000000 url-obfuscated-0.0.1/README.md
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/obfuscated/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-03-15 10:21:35.000000 url-obfuscated-0.0.1/obfuscated/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      397 2023-03-15 10:21:35.000000 url-obfuscated-0.0.1/obfuscated/asgi.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     3264 2023-03-17 04:28:02.000000 url-obfuscated-0.0.1/obfuscated/settings.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1125 2023-03-16 06:26:07.000000 url-obfuscated-0.0.1/obfuscated/urls.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      551 2023-03-16 06:21:09.000000 url-obfuscated-0.0.1/obfuscated/views.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      397 2023-03-15 10:21:35.000000 url-obfuscated-0.0.1/obfuscated/wsgi.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       38 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/setup.cfg
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1479 2023-03-16 09:52:06.000000 url-obfuscated-0.0.1/setup.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/url_obfuscated/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-03-15 10:24:07.000000 url-obfuscated-0.0.1/url_obfuscated/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      159 2023-03-15 10:24:07.000000 url-obfuscated-0.0.1/url_obfuscated/apps.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      443 2023-03-17 05:06:09.000000 url-obfuscated-0.0.1/url_obfuscated/decorators.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     2002 2023-03-15 17:52:39.000000 url-obfuscated-0.0.1/url_obfuscated/helpers.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/url_obfuscated/migrations/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-03-15 10:24:07.000000 url-obfuscated-0.0.1/url_obfuscated/migrations/__init__.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/url_obfuscated/templatetags/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-03-15 10:24:07.000000 url-obfuscated-0.0.1/url_obfuscated/templatetags/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      278 2023-03-17 05:25:48.000000 url-obfuscated-0.0.1/url_obfuscated/templatetags/obfuscate_tags.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-03-17 05:42:39.684761 url-obfuscated-0.0.1/url_obfuscated.egg-info/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     3399 2023-03-17 05:42:39.000000 url-obfuscated-0.0.1/url_obfuscated.egg-info/PKG-INFO
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      579 2023-03-17 05:42:39.000000 url-obfuscated-0.0.1/url_obfuscated.egg-info/SOURCES.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-03-17 05:42:39.000000 url-obfuscated-0.0.1/url_obfuscated.egg-info/dependency_links.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       28 2023-03-17 05:42:39.000000 url-obfuscated-0.0.1/url_obfuscated.egg-info/requires.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       26 2023-03-17 05:42:39.000000 url-obfuscated-0.0.1/url_obfuscated.egg-info/top_level.txt
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)    10763 2024-05-13 15:55:01.000000 url-obfuscated-1.0.0/LICENSE
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)       34 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/MANIFEST.in
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     2943 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/PKG-INFO
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     2056 2024-05-12 17:51:12.000000 url-obfuscated-1.0.0/README.md
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/obfuscated/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)        0 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/__init__.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      397 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/asgi.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     3264 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/settings.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     1125 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/urls.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      551 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/views.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      397 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/obfuscated/wsgi.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)       38 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/setup.cfg
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     1484 2024-05-17 06:49:31.000000 url-obfuscated-1.0.0/setup.py
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/url_obfuscated/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)        0 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/__init__.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      159 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/apps.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      443 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/decorators.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     2078 2024-05-12 17:49:42.000000 url-obfuscated-1.0.0/url_obfuscated/helpers.py
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/url_obfuscated/migrations/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)        0 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/migrations/__init__.py
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/url_obfuscated/templatetags/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)        0 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/templatetags/__init__.py
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      278 2024-05-12 14:40:27.000000 url-obfuscated-1.0.0/url_obfuscated/templatetags/obfuscate_tags.py
+drwxrwxr-x   0 dhyani    (1000) dhyani    (1000)        0 2024-05-17 06:51:02.588398 url-obfuscated-1.0.0/url_obfuscated.egg-info/
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)     2943 2024-05-17 06:51:02.000000 url-obfuscated-1.0.0/url_obfuscated.egg-info/PKG-INFO
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)      579 2024-05-17 06:51:02.000000 url-obfuscated-1.0.0/url_obfuscated.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)        1 2024-05-17 06:51:02.000000 url-obfuscated-1.0.0/url_obfuscated.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)       33 2024-05-17 06:51:02.000000 url-obfuscated-1.0.0/url_obfuscated.egg-info/requires.txt
+-rw-rw-r--   0 dhyani    (1000) dhyani    (1000)       26 2024-05-17 06:51:02.000000 url-obfuscated-1.0.0/url_obfuscated.egg-info/top_level.txt
```

### Comparing `url-obfuscated-0.0.1/LICENSE` & `url-obfuscated-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -171,26 +171,16 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   APPENDIX: How to apply the Apache License to your work.
 
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 Dhyanikumar Palan
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `url-obfuscated-0.0.1/PKG-INFO` & `url-obfuscated-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: url-obfuscated
-Version: 0.0.1
+Version: 1.0.0
 Summary: Easy and Simple method to obfuscate and deobfuscate your Django URLs.
 Home-page: https://github.com/dhyanipalan/url_obfuscated
+Download-URL: https://github.com/dhyanipalan/url_obfuscated
 Author: Dhyanikumar Palan
 Author-email: dhyanipalan@gmail.com
 Maintainer: Dhyanikumar Palan
 Maintainer-email: dhyanipalan@gmail.com
 License: Apache License
-Download-URL: https://github.com/dhyanipalan/url_obfuscated
-Description: # url_obfuscated
-        Easy and Simple method to obfuscate and deobfuscate your Django URLs.
-        Works with both normal urls as well as those with params
-        
-        ## Quick start
-        Install using pip or easy_install
-        
-            $ pip install url-obfuscated
-        
-            $ easy_install url-obfuscated
-        
-        Add "url_obfuscate" to your INSTALLED_APPS setting like this:
-        
-            INSTALLED_APPS = (
-                ...
-                'url-obfuscated',
-            )
-        
-        ## Usage
-        To obfuscate Django's URLs, modify the URL declaration in the urls.py file by replacing the regex definition with the funcion generate_url_pattern, as follows:
-        
-            from url_obfuscated.helpers import generate_url_pattern
-            .....
-        
-            urlpatterns = [
-                url(generate_url_pattern('/'), home, name='home'),
-                url(generate_url_pattern('obfuscated_link', params=['(?P<name>[^/]+)']), obfuscated_link, name='obfuscated_link'),
-                url(generate_url_pattern('optional_param', params=['(?:(?P<param>[^/]+)/)?']), optional_param, name='optional_param'),
-            ]
-        
-        For the home URL, use / path. To include params in the URL, declare them in the desired order inside the params attribute. When obfuscating a URL with parameters, it is necessary to use the deobfuscate decorator to recover the original value of the parameter.
-        
-            from url_obfuscated.decorators import deobfuscate
-            ...
-        
-            @deobfuscate
-            def obfuscated_link(request, name):
-                return render(request, 'obfuscate_result.html', { 'name': name })
-        
-        When declaring URLs with parameters inside templates, use the obfuscate template tag, as follows:
-        
-            {% load obfuscate_tags %}
-            ...
-            <p><a href="{% url 'obfuscated_link' 'Dan Brown'|obfuscate %}">Obfuscated link: {% url 'obfuscated_link' 'Dan'|obfuscate %}</a></p>
-            ...
-        
-        You can also obfuscate any value from inside a view, use the obfuscate function, as follows:
-        
-            from url_obfuscate.helpers import obfuscate
-            ...
-        
-            def home(request):
-                links = list()
-                for i in range(10):
-                    links.append(obfuscate('Name %d' % (i+1)))
-                return render(request, 'index.html', { 'links': links })
-        
 Keywords: django,Python,urlobfuscate,encrypt
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# url_obfuscated
+Easy and Simple method to obfuscate and deobfuscate your Django URLs.
+Works with both normal urls as well as those with params
+
+## Quick start
+Install using pip or easy_install
+
+    $ pip install url-obfuscated
+
+    $ easy_install url-obfuscated
+
+Add "url_obfuscate" to your INSTALLED_APPS setting like this:
+
+    INSTALLED_APPS = (
+        ...
+        'url_obfuscated',
+    )
+
+## Usage
+To obfuscate Django's URLs, modify the URL declaration in the urls.py file by replacing the regex definition with the funcion generate_url_pattern, as follows:
+
+    from url_obfuscated.helpers import generate_url_pattern
+    .....
+
+    urlpatterns = [
+        url(generate_url_pattern('/'), home, name='home'),
+        url(generate_url_pattern('obfuscated_link', params=['(?P<name>[^/]+)']), obfuscated_link, name='obfuscated_link'),
+        url(generate_url_pattern('optional_param', params=['(?:(?P<param>[^/]+)/)?']), optional_param, name='optional_param'),
+    ]
+
+For the home URL, use / path. To include params in the URL, declare them in the desired order inside the params attribute. When obfuscating a URL with parameters, it is necessary to use the deobfuscate decorator to recover the original value of the parameter.
+
+    from url_obfuscated.decorators import deobfuscate
+    ...
+
+    @deobfuscate
+    def obfuscated_link(request, name):
+        return render(request, 'obfuscate_result.html', { 'name': name })
+
+When declaring URLs with parameters inside templates, use the obfuscate template tag, as follows:
+
+    {% load obfuscate_tags %}
+    ...
+    <p><a href="{% url 'obfuscated_link' 'Dan Brown'|obfuscate %}">Obfuscated link: {% url 'obfuscated_link' 'Dan'|obfuscate %}</a></p>
+    ...
+
+You can also obfuscate any value from inside a view, use the obfuscate function, as follows:
+
+    from url_obfuscated.helpers import obfuscate
+    ...
+
+    def home(request):
+        links = list()
+        for i in range(10):
+            links.append(obfuscate('Name %d' % (i+1)))
+        return render(request, 'index.html', { 'links': links })
```

### Comparing `url-obfuscated-0.0.1/README.md` & `url-obfuscated-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     $ easy_install url-obfuscated
 
 Add "url_obfuscate" to your INSTALLED_APPS setting like this:
 
     INSTALLED_APPS = (
         ...
-        'url-obfuscated',
+        'url_obfuscated',
     )
 
 ## Usage
 To obfuscate Django's URLs, modify the URL declaration in the urls.py file by replacing the regex definition with the funcion generate_url_pattern, as follows:
 
     from url_obfuscated.helpers import generate_url_pattern
     .....
@@ -42,15 +42,15 @@
     {% load obfuscate_tags %}
     ...
     <p><a href="{% url 'obfuscated_link' 'Dan Brown'|obfuscate %}">Obfuscated link: {% url 'obfuscated_link' 'Dan'|obfuscate %}</a></p>
     ...
 
 You can also obfuscate any value from inside a view, use the obfuscate function, as follows:
 
-    from url_obfuscate.helpers import obfuscate
+    from url_obfuscated.helpers import obfuscate
     ...
 
     def home(request):
         links = list()
         for i in range(10):
             links.append(obfuscate('Name %d' % (i+1)))
         return render(request, 'index.html', { 'links': links })
```

### Comparing `url-obfuscated-0.0.1/obfuscated/settings.py` & `url-obfuscated-1.0.0/obfuscated/settings.py`

 * *Files identical despite different names*

### Comparing `url-obfuscated-0.0.1/obfuscated/urls.py` & `url-obfuscated-1.0.0/obfuscated/urls.py`

 * *Files identical despite different names*

### Comparing `url-obfuscated-0.0.1/obfuscated/views.py` & `url-obfuscated-1.0.0/obfuscated/views.py`

 * *Files identical despite different names*

### Comparing `url-obfuscated-0.0.1/setup.py` & `url-obfuscated-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-VERSION = '0.0.1'
+VERSION = '1.0.0'
 NAME = 'Dhyanikumar Palan'
 EMAIL = 'dhyanipalan@gmail.com'
 setup(
     name='url-obfuscated',
     version=VERSION,
     packages=find_packages(),
 
     # Dependencies
-    install_requires=['Django>=2.2', 'pycrypto==2.6.1'],
+    install_requires=['Django>=2.2', 'pycryptodome==3.20.0'],
 
     # Metadata for PyPI
     author=NAME,
     author_email=EMAIL,
     maintainer=NAME,
     maintainer_email=EMAIL,
     description='Easy and Simple method to obfuscate and deobfuscate your Django URLs.',
```

### Comparing `url-obfuscated-0.0.1/url_obfuscated/helpers.py` & `url-obfuscated-1.0.0/url_obfuscated/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,28 +33,28 @@
     """Adds Padding if Secret Key is not of Legal AES Block Size ie. 16, 24, 32"""
     if not len(secret) in (16, 24, 32):
         return secret + (blocksize - len(secret)) * padding
     return secret
 
 def obfuscate(value):
     secret = _pad(settings.SECRET_KEY[0:16])
-    encrypt_obj = AES.new(secret)
+    encrypt_obj = AES.new(secret.encode('utf-8'), AES.MODE_ECB)
 
     value = str.encode(value)
     value = str(value, 'utf-8')
     value = value + (' ' * (16 - (len(value) % 16)))
-    encrypted = encrypt_obj.encrypt(value)
+    encrypted = encrypt_obj.encrypt(value.encode('utf-8'))
     hex_value = binascii.hexlify(encrypted)
     response = str(binascii.b2a_base64(hex_value)[:-1]).replace('+', '-').replace('/', '_').replace('=', '')
     response = response[2:-1]
     return response
 
 def deobfuscate(value):
     secret = _pad(settings.SECRET_KEY[0:16])
-    encrypt_obj = AES.new(secret)
+    encrypt_obj = AES.new(secret.encode('utf-8'), AES.MODE_ECB)
 
     value = str.encode(value)
     value = str(value, 'utf-8')
     value = value.replace('-', '+').replace('_', '/')
     value = value + ('=' * (16 - (len(value) % 16)))
     decoded = binascii.a2b_base64(value).decode("utf-8")
     unhex = binascii.unhexlify(decoded)
```

### Comparing `url-obfuscated-0.0.1/url_obfuscated.egg-info/PKG-INFO` & `url-obfuscated-1.0.0/url_obfuscated.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: url-obfuscated
-Version: 0.0.1
+Version: 1.0.0
 Summary: Easy and Simple method to obfuscate and deobfuscate your Django URLs.
 Home-page: https://github.com/dhyanipalan/url_obfuscated
+Download-URL: https://github.com/dhyanipalan/url_obfuscated
 Author: Dhyanikumar Palan
 Author-email: dhyanipalan@gmail.com
 Maintainer: Dhyanikumar Palan
 Maintainer-email: dhyanipalan@gmail.com
 License: Apache License
-Download-URL: https://github.com/dhyanipalan/url_obfuscated
-Description: # url_obfuscated
-        Easy and Simple method to obfuscate and deobfuscate your Django URLs.
-        Works with both normal urls as well as those with params
-        
-        ## Quick start
-        Install using pip or easy_install
-        
-            $ pip install url-obfuscated
-        
-            $ easy_install url-obfuscated
-        
-        Add "url_obfuscate" to your INSTALLED_APPS setting like this:
-        
-            INSTALLED_APPS = (
-                ...
-                'url-obfuscated',
-            )
-        
-        ## Usage
-        To obfuscate Django's URLs, modify the URL declaration in the urls.py file by replacing the regex definition with the funcion generate_url_pattern, as follows:
-        
-            from url_obfuscated.helpers import generate_url_pattern
-            .....
-        
-            urlpatterns = [
-                url(generate_url_pattern('/'), home, name='home'),
-                url(generate_url_pattern('obfuscated_link', params=['(?P<name>[^/]+)']), obfuscated_link, name='obfuscated_link'),
-                url(generate_url_pattern('optional_param', params=['(?:(?P<param>[^/]+)/)?']), optional_param, name='optional_param'),
-            ]
-        
-        For the home URL, use / path. To include params in the URL, declare them in the desired order inside the params attribute. When obfuscating a URL with parameters, it is necessary to use the deobfuscate decorator to recover the original value of the parameter.
-        
-            from url_obfuscated.decorators import deobfuscate
-            ...
-        
-            @deobfuscate
-            def obfuscated_link(request, name):
-                return render(request, 'obfuscate_result.html', { 'name': name })
-        
-        When declaring URLs with parameters inside templates, use the obfuscate template tag, as follows:
-        
-            {% load obfuscate_tags %}
-            ...
-            <p><a href="{% url 'obfuscated_link' 'Dan Brown'|obfuscate %}">Obfuscated link: {% url 'obfuscated_link' 'Dan'|obfuscate %}</a></p>
-            ...
-        
-        You can also obfuscate any value from inside a view, use the obfuscate function, as follows:
-        
-            from url_obfuscate.helpers import obfuscate
-            ...
-        
-            def home(request):
-                links = list()
-                for i in range(10):
-                    links.append(obfuscate('Name %d' % (i+1)))
-                return render(request, 'index.html', { 'links': links })
-        
 Keywords: django,Python,urlobfuscate,encrypt
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# url_obfuscated
+Easy and Simple method to obfuscate and deobfuscate your Django URLs.
+Works with both normal urls as well as those with params
+
+## Quick start
+Install using pip or easy_install
+
+    $ pip install url-obfuscated
+
+    $ easy_install url-obfuscated
+
+Add "url_obfuscate" to your INSTALLED_APPS setting like this:
+
+    INSTALLED_APPS = (
+        ...
+        'url_obfuscated',
+    )
+
+## Usage
+To obfuscate Django's URLs, modify the URL declaration in the urls.py file by replacing the regex definition with the funcion generate_url_pattern, as follows:
+
+    from url_obfuscated.helpers import generate_url_pattern
+    .....
+
+    urlpatterns = [
+        url(generate_url_pattern('/'), home, name='home'),
+        url(generate_url_pattern('obfuscated_link', params=['(?P<name>[^/]+)']), obfuscated_link, name='obfuscated_link'),
+        url(generate_url_pattern('optional_param', params=['(?:(?P<param>[^/]+)/)?']), optional_param, name='optional_param'),
+    ]
+
+For the home URL, use / path. To include params in the URL, declare them in the desired order inside the params attribute. When obfuscating a URL with parameters, it is necessary to use the deobfuscate decorator to recover the original value of the parameter.
+
+    from url_obfuscated.decorators import deobfuscate
+    ...
+
+    @deobfuscate
+    def obfuscated_link(request, name):
+        return render(request, 'obfuscate_result.html', { 'name': name })
+
+When declaring URLs with parameters inside templates, use the obfuscate template tag, as follows:
+
+    {% load obfuscate_tags %}
+    ...
+    <p><a href="{% url 'obfuscated_link' 'Dan Brown'|obfuscate %}">Obfuscated link: {% url 'obfuscated_link' 'Dan'|obfuscate %}</a></p>
+    ...
+
+You can also obfuscate any value from inside a view, use the obfuscate function, as follows:
+
+    from url_obfuscated.helpers import obfuscate
+    ...
+
+    def home(request):
+        links = list()
+        for i in range(10):
+            links.append(obfuscate('Name %d' % (i+1)))
+        return render(request, 'index.html', { 'links': links })
```

### Comparing `url-obfuscated-0.0.1/url_obfuscated.egg-info/SOURCES.txt` & `url-obfuscated-1.0.0/url_obfuscated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

