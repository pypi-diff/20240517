# Comparing `tmp/web-ui-helper-0.0.9.tar.gz` & `tmp/web-ui-helper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.0.9.tar", last modified: Mon May  6 01:55:07 2024, max compression
+gzip compressed data, was "web-ui-helper-0.1.0.tar", last modified: Fri May 17 08:21:18 2024, max compression
```

## Comparing `web-ui-helper-0.0.9.tar` & `web-ui-helper-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.893594 web-ui-helper-0.0.9/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-06 01:55:07.890601 web-ui-helper-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 01:55:07.893594 web-ui-helper-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-06 01:54:57.000000 web-ui-helper-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.840735 web-ui-helper-0.0.9/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.9/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.862700 web-ui-helper-0.0.9/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.9/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.870701 web-ui-helper-0.0.9/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.9/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.872649 web-ui-helper-0.0.9/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.875652 web-ui-helper-0.0.9/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    28128 2024-05-06 01:54:46.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.878661 web-ui-helper-0.0.9/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     5206 2024-05-05 18:18:39.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.882650 web-ui-helper-0.0.9/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.9/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.885615 web-ui-helper-0.0.9/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.9/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:55:07.888609 web-ui-helper-0.0.9/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-06 01:55:07.000000 web-ui-helper-0.0.9/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-06 01:55:07.000000 web-ui-helper-0.0.9/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 01:55:07.000000 web-ui-helper-0.0.9/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-06 01:55:07.000000 web-ui-helper-0.0.9/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-06 01:55:07.000000 web-ui-helper-0.0.9/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.468006 web-ui-helper-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-17 08:21:18.465025 web-ui-helper-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:21:18.468006 web-ui-helper-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-17 08:21:14.000000 web-ui-helper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.417139 web-ui-helper-0.1.0/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.1.0/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.439080 web-ui-helper-0.1.0/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.1.0/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.445064 web-ui-helper-0.1.0/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-07 17:56:47.000000 web-ui-helper-0.1.0/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.447059 web-ui-helper-0.1.0/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.452046 web-ui-helper-0.1.0/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    31206 2024-05-17 08:21:06.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.455037 web-ui-helper-0.1.0/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 07:19:52.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.458029 web-ui-helper-0.1.0/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-07 17:57:06.000000 web-ui-helper-0.1.0/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.461049 web-ui-helper-0.1.0/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.1.0/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:18.463016 web-ui-helper-0.1.0/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-17 08:21:18.000000 web-ui-helper-0.1.0/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-17 08:21:18.000000 web-ui-helper-0.1.0/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:21:18.000000 web-ui-helper-0.1.0/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-17 08:21:18.000000 web-ui-helper-0.1.0/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 08:21:18.000000 web-ui-helper-0.1.0/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.0.9/LICENSE` & `web-ui-helper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/PKG-INFO` & `web-ui-helper-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.9
+Version: 0.1.0
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.9/setup.py` & `web-ui-helper-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.0.9',
+    version='0.1.0',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.1.0/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/dir.py` & `web-ui-helper-0.1.0/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/log.py` & `web-ui-helper-0.1.0/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.1.0/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/platforms.py` & `web-ui-helper-0.1.0/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.1.0/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.1.0/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.1.0/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.1.0/web_ui_helper/selenium/frame/browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import selenium
 from PIL import Image
 from io import BytesIO
 from selenium import webdriver
 from abc import abstractmethod
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.ui import Select
 from seleniumwire import webdriver as driver_wire
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.common.exceptions import NoSuchElementException
 # expected_conditions 类负责条件
@@ -103,25 +104,31 @@
         chrome_options = driver_wire.ChromeOptions()
         # 谷歌文档提到需要加上这个属性来规避bug
         chrome_options.add_argument('--disable-gpu')
         # 隐身模式（无痕模式）
         # chrome_options.add_argument('--incognito')
         # 隐藏"Chrome正在受到自动软件的控制"
         chrome_options.add_argument('disable-infobars')
+        # 禁用 WebRTC
+        chrome_options.add_argument("--disable-webrtc")
         chrome_options.add_argument('--user-data-dir={}'.format(self.USERDATA_PATH))
         # chrome_options.add_argument("--disable-autofill-passwords")  # 禁用自动填充密码
         # chrome_options.add_argument("--disable-save-password-bubble")  # 禁用保存密码提示框
+        # 在 ChromeOptions 中禁用缓存
+        # chrome_options.add_argument("--disable-cache")
+        # chrome_options.add_argument("--disk-cache-size=0")
         # 设置中文
         # chrome_options.add_argument('lang=zh_CN.UTF-8')
         # chrome_options.add_argument('--no-sandbox')  # linux下
         if self.is_headless is True:
             # 谷歌浏览器后台运行模式
             chrome_options.add_argument('--headless')
             # 指定浏览器分辨率
-            chrome_options.add_argument('--window-size=1920,1080')
+            # chrome_options.add_argument('--window-size=1920,1080')
+            chrome_options.add_argument('--window-size=2560,1440')
         else:
             # 浏览器最大化
             chrome_options.add_argument('--start-maximized')
         chrome_options.add_argument('--disable-dev-shm-usage')
         # 或者使用下面的设置, 提升速度
         # chrome_options.add_argument('blink-settings=imagesEnabled=false')
         # 隐藏滚动条, 应对一些特殊页面
@@ -232,35 +239,39 @@
         process_name = get_browser_process_name(self.BROWSER_NAME)
         return is_process_running(process_name=process_name)
 
 
 class SeleniumProxy(object):
 
     def __init__(self, browser_name: str, proxy_address: str, browser_path: str = None,
-                 is_headless: bool = False) -> None:
+                 is_headless: bool = False, is_single_instance: bool = True) -> None:
         if browser_path:
             if not is_file(browser_path):
                 raise ValueError("browser path is not exist")
         else:
             browser_path = get_var_path(var=browser_name)
             if not browser_path:
                 raise ValueError("system not installed {} browser.".format(browser_name))
         exe_name = get_browser_bin_exe(browser_name=browser_name)
         exe_file = os.path.join(browser_path, exe_name)
         if browser_name == "Chrome":
             self.browser_proxy = ChromeBrowser(browser_path=exe_file, is_headless=is_headless,
                                                proxy_address=proxy_address)
-            if self.browser_proxy.is_running() is True:
-                raise ValueError("Chrome browser is already running.")
+            # 单实例模式下，系统只能有一个chrome浏览器进程在运行中
+            if is_single_instance is True:
+                if self.browser_proxy.is_running() is True:
+                    raise ValueError("Chrome browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         elif browser_name == "Firefox":
             self.browser_proxy = FirefoxBrowser(browser_path=exe_file, is_headless=is_headless,
                                                 proxy_address=proxy_address)
-            if self.browser_proxy.is_running() is True:
-                raise ValueError("Firefox browser is already running.")
+            # 单实例模式下，系统只能有一个firefox浏览器进程在运行中
+            if is_single_instance is True:
+                if self.browser_proxy.is_running() is True:
+                    raise ValueError("Firefox browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         else:
             raise ValueError("Browser name must be Chrome or Firefox.")
 
     def input_text(self, locator: str, regx: str, value: str) -> bool:
         """
         locator 选择器
@@ -280,15 +291,18 @@
             # 清除存在的值
             # input_1.clear()
             # 使用 JavaScript 清除输入框的内容
             # self.browser.execute_script("arguments[0].setAttribute('value', '')", input_1)
             input_1.send_keys('{}'.format(value))
             flag = True
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，捕获输入框设置文本<{}>失败，error：{}".format(locator, regx, value, e)
+            err_str = "通过选择器：{}，表达式: {}，捕获输入框设置文本<{}>失败".format(locator, regx, value)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return flag
 
     def submit_click(self, locator: str, regx: str) -> bool:
         """
         locator 选择器
         regx 选择器所要匹配的表达式
@@ -298,15 +312,18 @@
         try:
             submit = self.wait.until(
                 ec.element_to_be_clickable((Locator.get(locator), regx))
             )
             submit.click()
             flag = True
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，捕获点击对象并点击失败，error：{}".format(locator, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，捕获点击对象并点击失败".format(locator, regx)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return flag
 
     def get_code(self, locator: str, regx: str) -> str:
         logger.warning("开始获取验证码...")
         ocr_result = None
         try:
@@ -339,41 +356,50 @@
             # 根据实际情况定位按钮元素
             element = self.browser.find_element(Locator.get(locator), regx)
             # 获取按钮元素的文本信息
             element_text = element.text.strip() if isinstance(element.text, str) else ""
             logger.warning("获取元素的文字信息为: {}".format(element_text))
             return element_text
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素文本信息失败，error：{}".format(locator, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素文本信息失败".format(locator, regx)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return element_text
 
     def get_element(self, locator: str, regx: str) -> WebElement:
         element = None
         try:
             # 根据实际情况定位按钮元素
             element = self.browser.find_element(Locator.get(locator), regx)
         except (NoSuchElementException,):
             err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(locator, regx)
             logger.warning(err_str)
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(locator, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素失败".format(locator, regx)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return element
 
     def get_elements(self, locator: str, regx: str) -> [WebElement]:
         elements = list()
         try:
             # 根据实际情况定位按钮元素
             elements = self.browser.find_elements(Locator.get(locator), regx)
         except (NoSuchElementException,):
             err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(locator, regx)
             logger.warning(err_str)
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(locator, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素失败".format(locator, regx)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return elements
 
     def get_background_color(self, locator: str, regx: str) -> str:
         background_color = None
         try:
             # 根据实际情况定位按钮元素
@@ -430,15 +456,18 @@
             # 根据实际情况定位按钮元素
             element = self.browser.find_element(Locator.get(locator), regx)
             if element:
                 is_exist = True
         except (NoSuchElementException,):
             pass
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(locator, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，判断元素是否存在失败".format(locator, regx)
+            e_slice = str(e).split("Message:")
+            if e_slice[0]:
+                err_str = err_str + "，error: {}".format(e_slice[0])
             logger.error(err_str)
         return is_exist
 
     def get_button(self, locator: str, regx: str) -> WebElement:
         """
         获取按钮
         :return: 按钮对象
@@ -564,29 +593,60 @@
         return cookies or ''
 
     def get_cookies(self) -> list:
         return self.browser.get_cookies() or list()
 
     def get_cookie(self, name: str) -> dict:
         """
-        {'domain': '.ctrip.com',
+        {
+        'domain': '.ctrip.com',
          'expiry': 1717525670,
          'httpOnly': True,
          'name': 'cticket',
          'path': '/',
          'sameSite': 'None',
          'secure': True,
-         'value': '275F2106E6E6CAAA34E1A32FE2452F42450E99443E2B22A31360D38C0BB2DEB3'}
+         'value': '275F2106E6E6CAAA34E1A32FE2452F42450E99443E2B22A31360D38C0BB2DEB3'
+         }
         """
         return self.browser.get_cookie(name=name) or dict()
 
     def refresh(self) -> None:
         # 刷新当前页面
         self.browser.refresh()
 
+    def enter_date_by_date_component(self, locator: str, regx: str, date_value: str):
+        year = date_value[:4]
+        month = date_value[5:7]
+        date = date_value[8:10]
+        # 点击输入文本框，弹出日历控件
+        self.submit_click(locator=locator, regx=regx)
+        time.sleep(0.5)
+        # 弹出选择年下拉选项
+        select_year_regx = "select-year"
+        # 选择指定年
+        select_year = Select(self.browser.find_element(Locator.get("class_name"), select_year_regx))
+        select_year.select_by_visible_text("{}年".format(year))
+        time.sleep(0.5)
+        # 选择指定月
+        select_month_regx = "select-month"
+        select_year = Select(self.browser.find_element(Locator.get("class_name"), select_month_regx))
+        select_year.select_by_visible_text("{}月".format(int(month)))
+        time.sleep(0.5)
+        # 指定日期
+        select_date_regx = './/a[text()="{}"]'.format(int(date))
+        # 定位到日历中的日期元素
+        self.submit_click(locator="xpath", regx=select_date_regx)
+        time.sleep(0.5)
+
+    def exception_html_save_to_txt(self):
+        su = get_current_datetime_int_str()
+        with open(os.path.join(self.browser.LOG_PATH, "exception_{}.txt".format(su)), "w", encoding="utf-8") as file:
+            file.write(self.get_page_source())
+
 
 @element_find_exception
 def scroll_to_bottom(driver: webdriver) -> None:
     """模拟页面滚动到底部"""
     driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
 
 
@@ -623,7 +683,13 @@
     return driver.execute_script(js_str)
 
 
 @loop_find_element
 def execute_script_with_element(driver: webdriver, js_str: str, element: WebElement, **kwargs):
     kwargs.clear()
     return driver.execute_script(js_str, element)
+
+
+@loop_find_element
+def scroll_element(driver: webdriver, element: WebElement, **kwargs):
+    kwargs.clear()
+    return driver.execute_script("arguments[0].scrollIntoView(true);", element)
```

### Comparing `web-ui-helper-0.0.9/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.1.0/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 class DesktopFlight:
 
     @classmethod
     def parse_data(cls, driver: webdriver, elements_data: dict) -> DataFrame:
         index_regx = './/div[@index="{}"]'
         price_regx = './/span[@class="price"]'
         airline_regx = './/div[@class="flight-airline"]/div[@class="airline-name"]'
-        plane_no_regx_1 = './/div[@class="plane"]/div[@class="plane"]/span'
-        plane_no_regx_2 = './/div[@class="flight-airline"]/div[@class="plane"]'
+        plane_no_regx_1 = './/div[@class="flight-airline"]/div[@class="plane"]'
+        plane_no_regx_2 = './/div[@class="flight-airline"]'
         depart_time_regx = './/div[@class="depart-box"]/div[@class="time"]'
         depart_airport_regx = './/div[@class="depart-box"]/div[@class="airport"]/span'
         arrive_time_regx = './/div[@class="arrive-box"]/div[@class="time"]'
         arrive_airport_regx = './/div[@class="arrive-box"]/div[@class="airport"]/span'
         columns = [
             "index", "plane_no", "airline", "plane_type", "price", "price_uint",
             "depart_time", "depart_airport", "arrive_time", "cross_days", "arrive_airport"
@@ -56,22 +56,29 @@
             # print(element.get_attribute('outerHTML'))
             price_element = get_sub_element(element=element, locator="xpath", regx=price_regx, interval=1, loop=3)
             price = price_element.text.strip() if price_element else ""
             airline_element = get_sub_element(
                 element=element, locator="xpath", regx=airline_regx, interval=1, loop=3
             )
             airline = airline_element.text.strip() if airline_element else ""
-            plane_no = get_sub_element(element=element, locator="xpath", regx=plane_no_regx_1, interval=1, loop=3)
-            if plane_no:
-                plane_no_slice = plane_no.text.strip().split()
+            plane_no_element = get_sub_element(
+                element=element, locator="xpath", regx=plane_no_regx_1, interval=1, loop=3
+            )
+            if plane_no_element and plane_no_element.text:
+                plane_no_slice = plane_no_element.text.strip().split()
                 plane_no = plane_no_slice[0].strip()
                 plane_type = plane_no_slice[1].strip()
             else:
-                plane_no = element.find_element(Locator.get("xpath"), plane_no_regx_2)
-                plane_no = plane_no.get_attribute('id').split("_")[0].split("-")[1].strip()
+                plane_no_element = get_sub_element(
+                    element=element, locator="xpath", regx=plane_no_regx_2, interval=1, loop=3
+                )
+                if plane_no_element.get_attribute('id'):
+                    plane_no = plane_no_element.get_attribute('id').split("_")[0].split("-")[1].strip()
+                else:
+                    plane_no = ""
                 plane_type = ""
             depart_time_element = get_sub_element(
                 element=element, locator="xpath", regx=depart_time_regx, interval=1, loop=3
             )
             depart_time = depart_time_element.text.strip() if depart_time_element else ""
             arrive_time_element = get_sub_element(
                 element=element, locator="xpath", regx=arrive_time_regx, interval=1, loop=3
```

### Comparing `web-ui-helper-0.0.9/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.1.0/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper/terminal/device.py` & `web-ui-helper-0.1.0/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.9/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.1.0/web_ui_helper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.9
+Version: 0.1.0
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.9/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.1.0/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

