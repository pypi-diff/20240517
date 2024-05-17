# Comparing `tmp/capsolver_extension_python-1.0.1.tar.gz` & `tmp/capsolver_extension_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver_extension_python-1.0.1.tar", last modified: Fri Jan 26 11:22:56 2024, max compression
+gzip compressed data, was "capsolver_extension_python-1.0.2.tar", last modified: Fri May 17 05:45:39 2024, max compression
```

## Comparing `capsolver_extension_python-1.0.1.tar` & `capsolver_extension_python-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 11:22:56.075355 capsolver_extension_python-1.0.1/
--rw-rw-rw-   0        0        0     1089 2024-01-25 12:15:31.000000 capsolver_extension_python-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3969 2024-01-26 11:22:56.074345 capsolver_extension_python-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2836 2024-01-25 14:00:51.000000 capsolver_extension_python-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-26 11:22:56.022998 capsolver_extension_python-1.0.1/capsolver_extension_python/
--rw-rw-rw-   0        0        0     1187 2024-01-26 09:01:59.000000 capsolver_extension_python-1.0.1/capsolver_extension_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-26 11:22:56.072320 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/
--rw-rw-rw-   0        0        0     3969 2024-01-26 11:22:55.000000 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-01-26 11:22:55.000000 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 11:22:55.000000 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-01-26 11:22:55.000000 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-01-26 11:22:55.000000 capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-01-26 11:22:56.080346 capsolver_extension_python-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1689 2024-01-26 11:15:16.000000 capsolver_extension_python-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:45:39.814119 capsolver_extension_python-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 capsolver_extension_python-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4776 2024-05-17 05:45:39.812867 capsolver_extension_python-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3643 2024-05-17 05:43:48.000000 capsolver_extension_python-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 05:45:39.788372 capsolver_extension_python-1.0.2/capsolver_extension_python/
+-rw-rw-rw-   0        0        0       32 2024-05-17 05:26:00.000000 capsolver_extension_python-1.0.2/capsolver_extension_python/__init__.py
+-rw-rw-rw-   0        0        0      656 2024-05-17 05:33:51.000000 capsolver_extension_python-1.0.2/capsolver_extension_python/extension.py
+-rw-rw-rw-   0        0        0     1287 2024-05-17 05:44:49.000000 capsolver_extension_python-1.0.2/capsolver_extension_python/perform_capsolver_file_updates.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:45:39.811937 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/
+-rw-rw-rw-   0        0        0     4776 2024-05-17 05:45:39.000000 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-05-17 05:45:39.000000 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:45:39.000000 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 05:45:39.000000 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-17 05:45:39.000000 capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-17 05:45:39.817013 capsolver_extension_python-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2024-05-17 05:45:37.000000 capsolver_extension_python-1.0.2/setup.py
```

### Comparing `capsolver_extension_python-1.0.1/LICENSE` & `capsolver_extension_python-1.0.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Chetan Jain
+Copyright (c) 2023-2024 Chetan Jain
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `capsolver_extension_python-1.0.1/PKG-INFO` & `capsolver_extension_python-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver_extension_python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Capsolver Extension Python allows you to easily integrate Capsolver Extension in web automation frameworks like Botasaurus, Selenium, and Playwright. 
 Home-page: https://github.com/omkarcloud/capsolver-extension-python
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: capsolver-extension-python
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,21 +35,21 @@
 ```bash 
 python -m pip install capsolver_extension_python
 ```
 
 ## Usage with [Botasaurus Web Scraping Framework](https://github.com/omkarcloud/botasaurus)
 
 ```python
-from botasaurus import *
+from botasaurus.browser import browser, Driver
 from capsolver_extension_python import Capsolver
 
 @browser(
     extensions=[Capsolver(api_key="CAP-MY_KEY")], # TODO: Replace with your own CapSolver Key
 )  
-def solve_captcha(driver: AntiDetectDriver, data):
+def solve_captcha(driver: Driver, data):
     driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     driver.prompt()
 
 solve_captcha()
 ```
 
 ## Usage with Selenium 
@@ -98,14 +98,35 @@
         ],
     )
     page = browser.new_page()
     page.goto("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     input("Press Enter to exit...")
     browser.close()
 ```
+## Use App ID
+
+```python
+from botasaurus.browser import browser, Driver
+from capsolver_extension_python import Capsolver
+
+@browser(
+    extensions=[Capsolver(api_key="CAP-MY_KEY", app_id="DC601421-43D5-45E4-9FDB-B3BAF7A2C3FD")], # TODO: Replace with your own CapSolver Key and App ID
+)  
+def solve_captcha(driver: Driver, data):
+    driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
+    driver.prompt()
+
+solve_captcha()
+```
+
+## Note
+
+When you use the Capsolver Extension, we integrate our own app ID into the extension if you haven't provided one. This allows us to earn a small commission from each captcha you solve, at no extra cost to you. 
+
+These funds supports us in our efforts to develop awesome open-source projects to make your life easy.
 
 ## Love It? [Star It ⭐!](https://github.com/omkarcloud/capsolver-extension-python)
 
 Become one of our amazing stargazers by giving us a star ⭐ on GitHub!
 
 It's just one click, but it means the world to me.
```

### Comparing `capsolver_extension_python-1.0.1/README.md` & `capsolver_extension_python-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 ```bash 
 python -m pip install capsolver_extension_python
 ```
 
 ## Usage with [Botasaurus Web Scraping Framework](https://github.com/omkarcloud/botasaurus)
 
 ```python
-from botasaurus import *
+from botasaurus.browser import browser, Driver
 from capsolver_extension_python import Capsolver
 
 @browser(
     extensions=[Capsolver(api_key="CAP-MY_KEY")], # TODO: Replace with your own CapSolver Key
 )  
-def solve_captcha(driver: AntiDetectDriver, data):
+def solve_captcha(driver: Driver, data):
     driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     driver.prompt()
 
 solve_captcha()
 ```
 
 ## Usage with Selenium 
@@ -73,14 +73,35 @@
         ],
     )
     page = browser.new_page()
     page.goto("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     input("Press Enter to exit...")
     browser.close()
 ```
+## Use App ID
+
+```python
+from botasaurus.browser import browser, Driver
+from capsolver_extension_python import Capsolver
+
+@browser(
+    extensions=[Capsolver(api_key="CAP-MY_KEY", app_id="DC601421-43D5-45E4-9FDB-B3BAF7A2C3FD")], # TODO: Replace with your own CapSolver Key and App ID
+)  
+def solve_captcha(driver: Driver, data):
+    driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
+    driver.prompt()
+
+solve_captcha()
+```
+
+## Note
+
+When you use the Capsolver Extension, we integrate our own app ID into the extension if you haven't provided one. This allows us to earn a small commission from each captcha you solve, at no extra cost to you. 
+
+These funds supports us in our efforts to develop awesome open-source projects to make your life easy.
 
 ## Love It? [Star It ⭐!](https://github.com/omkarcloud/capsolver-extension-python)
 
 Become one of our amazing stargazers by giving us a star ⭐ on GitHub!
 
 It's just one click, but it means the world to me.
```

### Comparing `capsolver_extension_python-1.0.1/capsolver_extension_python.egg-info/PKG-INFO` & `capsolver_extension_python-1.0.2/capsolver_extension_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver_extension_python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Capsolver Extension Python allows you to easily integrate Capsolver Extension in web automation frameworks like Botasaurus, Selenium, and Playwright. 
 Home-page: https://github.com/omkarcloud/capsolver-extension-python
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: capsolver-extension-python
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,21 +35,21 @@
 ```bash 
 python -m pip install capsolver_extension_python
 ```
 
 ## Usage with [Botasaurus Web Scraping Framework](https://github.com/omkarcloud/botasaurus)
 
 ```python
-from botasaurus import *
+from botasaurus.browser import browser, Driver
 from capsolver_extension_python import Capsolver
 
 @browser(
     extensions=[Capsolver(api_key="CAP-MY_KEY")], # TODO: Replace with your own CapSolver Key
 )  
-def solve_captcha(driver: AntiDetectDriver, data):
+def solve_captcha(driver: Driver, data):
     driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     driver.prompt()
 
 solve_captcha()
 ```
 
 ## Usage with Selenium 
@@ -98,14 +98,35 @@
         ],
     )
     page = browser.new_page()
     page.goto("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
     input("Press Enter to exit...")
     browser.close()
 ```
+## Use App ID
+
+```python
+from botasaurus.browser import browser, Driver
+from capsolver_extension_python import Capsolver
+
+@browser(
+    extensions=[Capsolver(api_key="CAP-MY_KEY", app_id="DC601421-43D5-45E4-9FDB-B3BAF7A2C3FD")], # TODO: Replace with your own CapSolver Key and App ID
+)  
+def solve_captcha(driver: Driver, data):
+    driver.get("https://recaptcha-demo.appspot.com/recaptcha-v2-checkbox.php")
+    driver.prompt()
+
+solve_captcha()
+```
+
+## Note
+
+When you use the Capsolver Extension, we integrate our own app ID into the extension if you haven't provided one. This allows us to earn a small commission from each captcha you solve, at no extra cost to you. 
+
+These funds supports us in our efforts to develop awesome open-source projects to make your life easy.
 
 ## Love It? [Star It ⭐!](https://github.com/omkarcloud/capsolver-extension-python)
 
 Become one of our amazing stargazers by giving us a star ⭐ on GitHub!
 
 It's just one click, but it means the world to me.
```

### Comparing `capsolver_extension_python-1.0.1/setup.py` & `capsolver_extension_python-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return long_description
     except:
         return None
 
 
 setup(
     name="capsolver_extension_python",
-    version="1.0.1",
+    version="1.0.2",
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="Capsolver Extension Python allows you to easily integrate Capsolver Extension in web automation frameworks like Botasaurus, Selenium, and Playwright. ",
     license="MIT",
     keywords=["capsolver-extension-python"],
     url="https://github.com/omkarcloud/capsolver-extension-python",
     packages=["capsolver_extension_python"],
```

