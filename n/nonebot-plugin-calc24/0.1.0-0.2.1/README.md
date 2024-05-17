# Comparing `tmp/nonebot_plugin_calc24-0.1.0.tar.gz` & `tmp/nonebot_plugin_calc24-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_calc24-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_calc24-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_calc24-0.1.0.tar` & `nonebot_plugin_calc24-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2024-05-16 02:49:10.788138 nonebot_plugin_calc24-0.1.0/LICENSE
--rw-r--r--   0        0        0     2124 2024-05-16 00:05:22.185004 nonebot_plugin_calc24-0.1.0/nonebot_plugin_calc24/__init__.py
--rw-r--r--   0        0        0     5303 2024-05-12 14:19:02.891052 nonebot_plugin_calc24-0.1.0/nonebot_plugin_calc24/calc24_invalid_data.json
--rw-r--r--   0        0        0     1541 2024-05-16 02:21:29.568208 nonebot_plugin_calc24-0.1.0/nonebot_plugin_calc24/xj_calc24.py
--rw-r--r--   0        0        0      701 2024-05-16 03:44:35.820767 nonebot_plugin_calc24-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 11:22:47.408837 nonebot_plugin_calc24-0.1.0/README.md
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4237 2024-05-17 00:18:49.701488 nonebot_plugin_calc24-0.2.1/nonebot_plugin_calc24/__init__.py
+-rw-r--r--   0        0        0     5303 2024-05-17 01:11:38.483619 nonebot_plugin_calc24-0.2.1/nonebot_plugin_calc24/calc24_invalid_data.json
+-rw-r--r--   0        0        0     1844 2024-05-17 00:00:38.454487 nonebot_plugin_calc24-0.2.1/nonebot_plugin_calc24/xj_calc24.py
+-rw-r--r--   0        0        0      701 2024-05-17 02:00:39.161132 nonebot_plugin_calc24-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.1/README.md
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_calc24-0.1.0/LICENSE` & `nonebot_plugin_calc24-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.1.0/nonebot_plugin_calc24/calc24_invalid_data.json` & `nonebot_plugin_calc24-0.2.1/nonebot_plugin_calc24/calc24_invalid_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.1.0/nonebot_plugin_calc24/xj_calc24.py` & `nonebot_plugin_calc24-0.2.1/nonebot_plugin_calc24/xj_calc24.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,25 +26,34 @@
     if check_if_in_dict(a_data):
         return random.sample(intdata, 4) 
     return a_data
 
 def paixu(sort_array):
         return sorted(sort_array, reverse=True)
 
+def regular_expression(regular , string):
+    matching_result = re.findall(regular, string)
+    if matching_result:
+        return True
+    return False
+
+
 class xj_calc24:
-    def a_main(self):
+    def calc_a_main(self):
         return random_number_generator()
-    
-    
 
+    def calc_b_main(self, equation, array):
+
+        regular_a = r'(?:[+\-*/]{2})'
+        if regular_expression(regular_a, equation):
+            return 'CONTINUOUS_OPERATOR'
 
-    def b_main(self, equation, array):
-        numbers_str = re.findall(r'\d+', equation)
-        # 将匹配到的数字字符串转换为整数数组
+        plain_english_text = equation.replace('（', '(').replace('）', ')')
+        numbers_str = re.findall(r'\d+', plain_english_text)
         numbers_int = [int(num) for num in numbers_str]
         # print("csaa",numbers_int)
         if paixu(numbers_int) != paixu(array):
-            return 'no'
+            return 'NO'
     
-        if eval(equation) == 24:
-            return '傻逼你居然答对了'
-        return '傻逼我'
+        if eval(plain_english_text) == 24:
+            return
+        return 'ERROR'
```

### Comparing `nonebot_plugin_calc24-0.1.0/pyproject.toml` & `nonebot_plugin_calc24-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-calc24"
-version = "0.1.0"
+version = "0.2.1"
 description = "A 24-point game plugin implemented using NoneBot."
 authors = ["AwAjie <139576615+ajdgg@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/ajdgg/nonebot-plugin-calc24"
 repository = "https://github.com/ajdgg/nonebot-plugin-calc24"
 documentation = "https://github.com/ajdgg/nonebot-plugin-calc24"
```

### Comparing `nonebot_plugin_calc24-0.1.0/PKG-INFO` & `nonebot_plugin_calc24-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-calc24
-Version: 0.1.0
+Version: 0.2.1
 Summary: A 24-point game plugin implemented using NoneBot.
 Home-page: https://github.com/ajdgg/nonebot-plugin-calc24
 License: LICENSE
 Keywords: nonebot,nonebot2
 Author: AwAjie
 Author-email: 139576615+ajdgg@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -17,8 +17,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Project-URL: Documentation, https://github.com/ajdgg/nonebot-plugin-calc24
 Project-URL: Repository, https://github.com/ajdgg/nonebot-plugin-calc24
 Description-Content-Type: text/markdown
 
+<div align="center">
 
+
+# nonebot-plugin-calc24
+
+_✨ NoneBot 插件简单描述 ✨_
+
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

