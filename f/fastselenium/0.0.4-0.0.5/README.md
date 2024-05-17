# Comparing `tmp/fastselenium-0.0.4.tar.gz` & `tmp/fastselenium-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastselenium-0.0.4.tar", last modified: Fri Mar 15 03:37:49 2024, max compression
+gzip compressed data, was "fastselenium-0.0.5.tar", last modified: Fri May 17 08:57:48 2024, max compression
```

## Comparing `fastselenium-0.0.4.tar` & `fastselenium-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-15 03:37:49.027928 fastselenium-0.0.4/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2024-03-15 03:36:01.000000 fastselenium-0.0.4/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2024-03-15 03:37:49.027759 fastselenium-0.0.4/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      554 2024-03-15 03:36:01.000000 fastselenium-0.0.4/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-15 03:37:49.026839 fastselenium-0.0.4/fastselenium/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5290 2024-03-15 03:36:01.000000 fastselenium-0.0.4/fastselenium/__init__.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-15 03:37:49.027559 fastselenium-0.0.4/fastselenium.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2024-03-15 03:37:49.000000 fastselenium-0.0.4/fastselenium.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      230 2024-03-15 03:37:49.000000 fastselenium-0.0.4/fastselenium.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-03-15 03:37:49.000000 fastselenium-0.0.4/fastselenium.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       48 2024-03-15 03:37:49.000000 fastselenium-0.0.4/fastselenium.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       13 2024-03-15 03:37:49.000000 fastselenium-0.0.4/fastselenium.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-03-15 03:37:49.027969 fastselenium-0.0.4/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      932 2024-03-15 03:37:27.000000 fastselenium-0.0.4/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-17 08:57:48.048588 fastselenium-0.0.5/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2024-03-15 03:36:01.000000 fastselenium-0.0.5/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2024-05-17 08:57:48.048403 fastselenium-0.0.5/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      554 2024-03-15 03:36:01.000000 fastselenium-0.0.5/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-17 08:57:48.047263 fastselenium-0.0.5/fastselenium/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5769 2024-05-17 08:57:25.000000 fastselenium-0.0.5/fastselenium/__init__.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-17 08:57:48.048157 fastselenium-0.0.5/fastselenium.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2024-05-17 08:57:48.000000 fastselenium-0.0.5/fastselenium.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      230 2024-05-17 08:57:48.000000 fastselenium-0.0.5/fastselenium.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-05-17 08:57:48.000000 fastselenium-0.0.5/fastselenium.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       48 2024-05-17 08:57:48.000000 fastselenium-0.0.5/fastselenium.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       13 2024-05-17 08:57:48.000000 fastselenium-0.0.5/fastselenium.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-05-17 08:57:48.048647 fastselenium-0.0.5/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      932 2024-05-17 08:57:25.000000 fastselenium-0.0.5/setup.py
```

### Comparing `fastselenium-0.0.4/LICENSE` & `fastselenium-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastselenium-0.0.4/PKG-INFO` & `fastselenium-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastselenium
-Version: 0.0.4
+Version: 0.0.5
 Summary: make it easy to use selenium
 Home-page: https://gitee.com/ZeroSeeker/fastselenium
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastselenium-0.0.4/README.md` & `fastselenium-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastselenium-0.0.4/fastselenium/__init__.py` & `fastselenium-0.0.5/fastselenium/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,18 +60,20 @@
         xpath: str = None,  # 第2优先
         try_times: int = try_times_default
 ):
     local_try_times = 0
     while local_try_times < try_times:
         try:
             if css_selector is not None:
-                driver.find_element_by_css_selector(css_selector).click()
+                # driver.find_element_by_css_selector(css_selector).click()
+                driver.find_element(By.CSS_SELECTOR, css_selector).click()
                 return driver
             elif xpath is not None:
-                driver.find_element_by_xpath(xpath).click()
+                # driver.find_element_by_xpath(xpath).click()
+                driver.find_element(By.XPATH, xpath).click()
                 return driver
             else:
                 return
         except:
             local_try_times += 1
             showlog.error('%s/%s retry in 1s ...' % (local_try_times, try_times))
             time.sleep(1)
@@ -85,18 +87,20 @@
         xpath: str = None,  # 第2优先
         try_times: int = try_times_default
 ):
     local_try_times = 0
     while local_try_times < try_times:
         try:
             if css_selector is not None:
-                driver.find_element_by_css_selector(css_selector).send_keys(keys)
+                # driver.find_element_by_css_selector(css_selector).send_keys(keys)
+                driver.find_element(By.CSS_SELECTOR, css_selector).send_keys(keys)
                 return driver
             elif xpath is not None:
-                driver.find_element_by_xpath(xpath).send_keys(keys)
+                # driver.find_element_by_xpath(xpath).send_keys(keys)
+                driver.find_element(By.XPATH, xpath).send_keys(keys)
                 return driver
             else:
                 return
         except:
             local_try_times += 1
             showlog.error('%s/%s retry in 1s ...' % (local_try_times, try_times))
             time.sleep(1)
@@ -108,15 +112,16 @@
         xpath: str = '',
         keys: str = ''
 ):
     # 尝试清除内容后粘贴，不适用于linux
     import pyautogui  # 在无GUI界面的Linux系统中会出现KeyError: 'DISPLAY'的问题，未解决
     while True:
         try:
-            driver.find_element_by_xpath(xpath).click()
+            # driver.find_element_by_xpath(xpath).click()
+            driver.find_element(By.XPATH, xpath).click()
             if platform.system() == 'Darwin':
                 pyautogui.hotkey('command', 'a')
                 pyautogui.press('delete')
                 pyperclip.copy(keys)
                 pyautogui.hotkey('command', 'v')
             elif platform.system() == 'Windows':
                 pyautogui.hotkey('ctrl', 'a')
@@ -168,17 +173,19 @@
         find_by: str = None,
         find_value: str = None
 ):
     """
     按照提供的track滑动
     """
     if class_name is not None:
-        slider = driver.find_element_by_class_name(class_name)
+        # slider = driver.find_element_by_class_name(class_name)
+        slider = driver.find_element(By.CLASS_NAME, class_name)
     elif id_str is not None:
-        slider = driver.find_element_by_id(class_name)
+        # slider = driver.find_element_by_id(class_name)
+        slider = driver.find_element(By.ID, class_name)
     elif find_by is not None and find_value is not None:
         slider = driver.find_element(by=find_by, value=find_value)
     else:
         return False
     action = ActionChains(driver)
     action.click_and_hold(slider).perform()
     for x in track:
```

### Comparing `fastselenium-0.0.4/fastselenium.egg-info/PKG-INFO` & `fastselenium-0.0.5/fastselenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastselenium
-Version: 0.0.4
+Version: 0.0.5
 Summary: make it easy to use selenium
 Home-page: https://gitee.com/ZeroSeeker/fastselenium
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastselenium-0.0.4/setup.py` & `fastselenium-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastselenium",
-    version="0.0.4",
+    version="0.0.5",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastselenium",
     packages=setuptools.find_packages(),
```

