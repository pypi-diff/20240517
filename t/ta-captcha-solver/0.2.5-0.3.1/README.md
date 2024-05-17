# Comparing `tmp/ta_captcha_solver-0.2.5.tar.gz` & `tmp/ta_captcha_solver-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-idjb_l90/ta_captcha_solver-0.2.5.tar", last modified: Wed Feb 14 18:23:45 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-i36_rapy/ta_captcha_solver-0.3.1.tar", last modified: Fri May 17 08:52:03 2024, max compression
```

## Comparing `ta_captcha_solver-0.2.5.tar` & `ta_captcha_solver-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8545 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7887 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-02-14 18:23:45.670475 ta_captcha_solver-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.662475 ta_captcha_solver-0.2.5/ta_captcha_solver/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/ta_captcha_solver/browser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3319 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/browser/browser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1775 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/cloudflare.py
--rw-rw-rw-   0 root         (0) root         (0)     3756 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/fun_captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/image_captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     3339 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/re_captcha_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      968 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/logger.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4064 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/captcha_guru_2_captcha.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/service_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4577 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/ta_captcha_solver/ta_captcha_solver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8545 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-02-14 18:23:45.000000 ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 18:23:45.666475 ta_captcha_solver-0.2.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7076 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/tests/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)     8891 2024-02-14 18:22:31.000000 ta_captcha_solver-0.2.5/tests/test_solve.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8717 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8059 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-17 08:52:03.050478 ta_captcha_solver-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/ta_captcha_solver/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/ta_captcha_solver/browser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3319 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/browser/browser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/cloudflare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3756 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/fun_captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/hcaptcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/image_captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     3339 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/re_captcha_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      968 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/logger.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4064 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/captcha_guru_2_captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/service_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4705 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/ta_captcha_solver/ta_captcha_solver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8717 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 08:52:02.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-17 08:52:03.000000 ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 08:52:03.046478 ta_captcha_solver-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7076 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/tests/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     9581 2024-05-17 08:51:11.000000 ta_captcha_solver-0.3.1/tests/test_solve.py
```

### Comparing `ta_captcha_solver-0.2.5/PKG-INFO` & `ta_captcha_solver-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta_captcha_solver
-Version: 0.2.5
+Version: 0.3.1
 Summary: Thoughtful Captcha Solver Package
 Home-page: https://www.thoughtful.ai/
 Author: Bohdan Sukhov
 Author-email: bohdan.sukhov@thoughtful.ai
 Keywords: ta_captcha_solver
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -74,14 +74,27 @@
 1. http://learn.captcha.guru/#/
 2. https://2captcha.com/2captcha-api
 
 You should have valid API key that could be obtained from web version of service after you put some money to the account balance
 
 |
 
+Supported Captcha Types
+---------------------------
+
+Currently we support these:
+
+1. CloudFlare
+2. Arkose Labs Fun Captcha
+3. HCaptcha
+4. ReCaptcha v2
+5. Image Captcha
+
+|
+
 Available Settings
 ------------------
 
 If param is not required and not set then this action would not be performed and you a responsible for it. E.g. if you dont provide *check_xpath* then you should check that captcha has been solved by you own.
 
 +----------------------+-------------------+-------+-------------------------------------------------------------------------+
 | Param                | Required          | Type  | Description                                                             |
```

### Comparing `ta_captcha_solver-0.2.5/README.rst` & `ta_captcha_solver-0.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,27 @@
 1. http://learn.captcha.guru/#/
 2. https://2captcha.com/2captcha-api
 
 You should have valid API key that could be obtained from web version of service after you put some money to the account balance
 
 |
 
+Supported Captcha Types
+---------------------------
+
+Currently we support these:
+
+1. CloudFlare
+2. Arkose Labs Fun Captcha
+3. HCaptcha
+4. ReCaptcha v2
+5. Image Captcha
+
+|
+
 Available Settings
 ------------------
 
 If param is not required and not set then this action would not be performed and you a responsible for it. E.g. if you dont provide *check_xpath* then you should check that captcha has been solved by you own.
 
 +----------------------+-------------------+-------+-------------------------------------------------------------------------+
 | Param                | Required          | Type  | Description                                                             |
```

### Comparing `ta_captcha_solver-0.2.5/setup.py` & `ta_captcha_solver-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     long_description=readme,
     include_package_data=True,
     keywords="ta_captcha_solver",
     name="ta_captcha_solver",
     packages=find_packages(include=["ta_captcha_solver", "ta_captcha_solver.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.2.5",
+    version="0.3.1",
     zip_safe=False,
 )
```

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/browser/browser.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/browser/browser.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/captcha.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/captcha.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/cloudflare.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/cloudflare.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/fun_captcha.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/image_captcha.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/image_captcha.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/captcha/re_captcha_v2.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/captcha/re_captcha_v2.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/exceptions.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/exceptions.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/logger.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/logger.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/captcha_guru_2_captcha.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/captcha_guru_2_captcha.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/service_provider/service_provider.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/service_provider/service_provider.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver/ta_captcha_solver.py` & `ta_captcha_solver-0.3.1/ta_captcha_solver/ta_captcha_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 
+from .captcha.hcaptcha import HCaptcha
 from .captcha.cloudflare import CloudflareTurnstile
 from .captcha.image_captcha import ImageCaptcha
 from .captcha.re_captcha_v2 import ReCaptchaV2
 from .captcha.fun_captcha import FunCaptcha
 
 from .exceptions import ParamsException
 
@@ -51,14 +52,16 @@
             return ImageCaptcha(**params)
         elif "v2" in params["captcha_type"]:
             return ReCaptchaV2(**params)
         elif "fun_captcha" in params["captcha_type"]:
             return FunCaptcha(**params)
         elif "cloudflare_turnstile" in params["captcha_type"]:
             return CloudflareTurnstile(**params)
+        elif "hcaptcha" in params["captcha_type"]:
+            return HCaptcha(**params)
         else:
             raise ParamsException(
                 "Incorrect captcha_type '{}' provided. Dont know what captcha need to solve!".format(
                     params["captcha_type"]
                 )
             )
```

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/PKG-INFO` & `ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta_captcha_solver
-Version: 0.2.5
+Version: 0.3.1
 Summary: Thoughtful Captcha Solver Package
 Home-page: https://www.thoughtful.ai/
 Author: Bohdan Sukhov
 Author-email: bohdan.sukhov@thoughtful.ai
 Keywords: ta_captcha_solver
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -74,14 +74,27 @@
 1. http://learn.captcha.guru/#/
 2. https://2captcha.com/2captcha-api
 
 You should have valid API key that could be obtained from web version of service after you put some money to the account balance
 
 |
 
+Supported Captcha Types
+---------------------------
+
+Currently we support these:
+
+1. CloudFlare
+2. Arkose Labs Fun Captcha
+3. HCaptcha
+4. ReCaptcha v2
+5. Image Captcha
+
+|
+
 Available Settings
 ------------------
 
 If param is not required and not set then this action would not be performed and you a responsible for it. E.g. if you dont provide *check_xpath* then you should check that captcha has been solved by you own.
 
 +----------------------+-------------------+-------+-------------------------------------------------------------------------+
 | Param                | Required          | Type  | Description                                                             |
```

### Comparing `ta_captcha_solver-0.2.5/ta_captcha_solver.egg-info/SOURCES.txt` & `ta_captcha_solver-0.3.1/ta_captcha_solver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ta_captcha_solver.egg-info/top_level.txt
 ta_captcha_solver/browser/__init__.py
 ta_captcha_solver/browser/browser.py
 ta_captcha_solver/captcha/__init__.py
 ta_captcha_solver/captcha/captcha.py
 ta_captcha_solver/captcha/cloudflare.py
 ta_captcha_solver/captcha/fun_captcha.py
+ta_captcha_solver/captcha/hcaptcha.py
 ta_captcha_solver/captcha/image_captcha.py
 ta_captcha_solver/captcha/re_captcha_v2.py
 ta_captcha_solver/service_provider/__init__.py
 ta_captcha_solver/service_provider/captcha_guru_2_captcha.py
 ta_captcha_solver/service_provider/service_provider.py
 tests/test_get.py
 tests/test_solve.py
```

### Comparing `ta_captcha_solver-0.2.5/tests/test_get.py` & `ta_captcha_solver-0.3.1/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `ta_captcha_solver-0.2.5/tests/test_solve.py` & `ta_captcha_solver-0.3.1/tests/test_solve.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.captcha_guru_api_key = os.getenv("CAPTCHA_GURU_API_KEY")
         self.two_captcha_api_key = os.getenv("TWO_CAPTCHA_API_KEY")
         self.remote_url = os.getenv("SELENIUM_GRID_URL")
         self.v2_url = "https://google.com/recaptcha/api2/demo"
         self.fun_captcha_url = "https://www.linkedin.com/checkpoint/rp/request-password-reset"
         self.fun_captcha_url2 = "https://client-demo.arkoselabs.com/solo-animals"
         self.image_url = "https://captcha.com/demos/features/captcha-demo.aspx"
+        self.hcaptcha_url = "https://accounts.hcaptcha.com/demo"
         self.image_source = os.path.join(os.getcwd(), "tests/captcha_screenshot.png")
         self.incorrect_image_source = os.path.join(os.getcwd(), "tests/incorrect_captcha_screenshot.png")
 
         # We need this var for bitbucket pipelines sucessfull run
         self.executable_path = os.path.join(os.getcwd(), "chromedriver")
         if not os.path.exists(self.executable_path):
             self.executable_path = None
@@ -221,7 +222,25 @@
         captcha = TACaptchaSolver.get(
             captcha_type="image",
             captcha_guru_api_key=self.captcha_guru_api_key,
             image_source=self.incorrect_image_source,
         )
         with pytest.raises(APICaptchaUnsolvable):
             captcha.solve()
+
+    def test_hcaptcha_req_params(self):
+        self.browser.open_browser(
+            browser="chrome",
+            url=self.hcaptcha_url,
+            remote_url=self.remote_url,
+            executable_path=self.executable_path,
+        )
+        sleep(5)
+        captcha = TACaptchaSolver.get(
+            captcha_type="hcaptcha",
+            browser=self.browser,
+            service_provider_name="2captcha",
+            service_provider_key=self.two_captcha_api_key,
+            check_xpath="//pre[@class='hcaptcha-success']",
+            click_xpath="//input[@type='submit']",
+        )
+        assert captcha.solve()
```

