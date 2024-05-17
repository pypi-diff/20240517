# Comparing `tmp/web-ui-helper-0.1.1.tar.gz` & `tmp/web-ui-helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.1.1.tar", last modified: Fri May 17 08:32:00 2024, max compression
+gzip compressed data, was "web-ui-helper-0.1.2.tar", last modified: Fri May 17 08:33:20 2024, max compression
```

## Comparing `web-ui-helper-0.1.1.tar` & `web-ui-helper-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.203671 web-ui-helper-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-17 08:32:00.201628 web-ui-helper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 08:32:00.203671 web-ui-helper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-17 08:31:54.000000 web-ui-helper-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.152759 web-ui-helper-0.1.1/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.1.1/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.174723 web-ui-helper-0.1.1/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.1.1/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.180684 web-ui-helper-0.1.1/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-07 17:56:47.000000 web-ui-helper-0.1.1/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.182678 web-ui-helper-0.1.1/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.186693 web-ui-helper-0.1.1/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    31243 2024-05-17 08:31:45.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.191681 web-ui-helper-0.1.1/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 07:19:52.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.194666 web-ui-helper-0.1.1/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-07 17:57:06.000000 web-ui-helper-0.1.1/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.198660 web-ui-helper-0.1.1/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.1.1/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:00.200654 web-ui-helper-0.1.1/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-17 08:32:00.000000 web-ui-helper-0.1.1/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-17 08:32:00.000000 web-ui-helper-0.1.1/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:32:00.000000 web-ui-helper-0.1.1/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-17 08:32:00.000000 web-ui-helper-0.1.1/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 08:32:00.000000 web-ui-helper-0.1.1/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.529798 web-ui-helper-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-17 08:33:20.527804 web-ui-helper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:33:20.530794 web-ui-helper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-17 08:32:37.000000 web-ui-helper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.478933 web-ui-helper-0.1.2/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.1.2/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.500874 web-ui-helper-0.1.2/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.1.2/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.506858 web-ui-helper-0.1.2/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-07 17:56:47.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.508854 web-ui-helper-0.1.2/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.512841 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    31244 2024-05-17 08:32:46.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.516833 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 07:19:52.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.519851 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-07 17:57:06.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.522842 web-ui-helper-0.1.2/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.525836 web-ui-helper-0.1.2/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.1.1/LICENSE` & `web-ui-helper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/PKG-INFO` & `web-ui-helper-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.1.1/setup.py` & `web-ui-helper-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.1.1',
+    version='0.1.2',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.1.2/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/dir.py` & `web-ui-helper-0.1.2/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/log.py` & `web-ui-helper-0.1.2/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.1.2/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/platforms.py` & `web-ui-helper-0.1.2/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.1.2/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.1.2/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.1.2/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.1.2/web_ui_helper/selenium/frame/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
         select_date_regx = './/a[text()="{}"]'.format(int(date))
         # 定位到日历中的日期元素
         self.submit_click(locator="xpath", regx=select_date_regx)
         time.sleep(0.5)
 
     def exception_html_save_to_txt(self):
         su = get_current_datetime_int_str()
-        file_name = os.path.join(self.browser_proxy.LOG_PATH, "exception_{}.txt".format(su))
+        file_name = os.path.join(self.browser_proxy.LOG_PATH, "exception_{}.html".format(su))
         with open(file_name, "w", encoding="utf-8") as file:
             file.write(self.get_page_source())
 
 
 @element_find_exception
 def scroll_to_bottom(driver: webdriver) -> None:
     """模拟页面滚动到底部"""
```

### Comparing `web-ui-helper-0.1.1/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.1.2/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.1.2/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper/terminal/device.py` & `web-ui-helper-0.1.2/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.1/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.1.2/web_ui_helper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.1.1/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.1.2/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

