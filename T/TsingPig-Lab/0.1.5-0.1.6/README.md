# Comparing `tmp/TsingPig_Lab-0.1.5.tar.gz` & `tmp/TsingPig_Lab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.5.tar", last modified: Thu May 16 08:08:34 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.6.tar", last modified: Fri May 17 15:09:42 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.5.tar` & `TsingPig_Lab-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:08:34.842591 TsingPig_Lab-0.1.5/
--rw-rw-rw-   0        0        0     3068 2024-05-16 08:08:34.842591 TsingPig_Lab-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2023 2024-05-16 08:07:53.000000 TsingPig_Lab-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:08:34.835449 TsingPig_Lab-0.1.5/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0     3068 2024-05-16 08:08:34.000000 TsingPig_Lab-0.1.5/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-16 08:08:34.000000 TsingPig_Lab-0.1.5/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:08:34.000000 TsingPig_Lab-0.1.5/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 08:08:34.000000 TsingPig_Lab-0.1.5/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:08:34.843594 TsingPig_Lab-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:08:34.840472 TsingPig_Lab-0.1.5/tsingpig_lab/
--rw-rw-rw-   0        0        0     3124 2024-05-16 07:19:47.000000 TsingPig_Lab-0.1.5/tsingpig_lab/Algorithms.py
--rw-rw-rw-   0        0        0     1322 2024-05-16 07:56:09.000000 TsingPig_Lab-0.1.5/tsingpig_lab/DataStructures.py
--rw-rw-rw-   0        0        0      449 2024-05-16 08:08:25.000000 TsingPig_Lab-0.1.5/tsingpig_lab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.760136 TsingPig_Lab-0.1.6/
+-rw-rw-rw-   0        0        0     6924 2024-05-17 15:09:42.758658 TsingPig_Lab-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-05-17 15:09:32.000000 TsingPig_Lab-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.752412 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0     6924 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:09:42.760136 TsingPig_Lab-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.758155 TsingPig_Lab-0.1.6/tsingpig_lab/
+-rw-rw-rw-   0        0        0     3264 2024-05-17 15:07:22.000000 TsingPig_Lab-0.1.6/tsingpig_lab/Algorithms.py
+-rw-rw-rw-   0        0        0     1322 2024-05-16 07:56:09.000000 TsingPig_Lab-0.1.6/tsingpig_lab/DataStructures.py
+-rw-rw-rw-   0        0        0      260 2024-05-17 15:09:18.000000 TsingPig_Lab-0.1.6/tsingpig_lab/__init__.py
```

### Comparing `TsingPig_Lab-0.1.5/setup.py` & `TsingPig_Lab-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.5/tsingpig_lab/Algorithms.py` & `TsingPig_Lab-0.1.6/tsingpig_lab/Algorithms.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         # 检查输入是否在有效范围内
         if not 2 <= a <= 16 or not 2 <= b <= 16:
             raise ValueError("进制必须在[2, 16]范围内！")
 
         if not isinstance(a, int) or not isinstance(b, int):
             raise ValueError("进制必须是整数！")
 
-    def convert(self, num: str):
+    def convert(self, num: str) -> str:
         """
         将 a 进制的数字 number 转换为 b 进制
         :param num: a进制的数字对应的字符串
         :return: b进制的数字对应的字符串
         """
         # 检查输入是否是有效的数字
 
@@ -34,50 +34,52 @@
         if num[0] == '-':
             flag = 1
             num = num[1:]
 
         # 将输入数字从 a 进制转换为十进制
         num_dec = 0
         for c in num:
-            num_dec = num_dec * self.a + self._char_to_int(c)
+            num_dec = num_dec * self.a + self.char_to_int(c)
 
         # 将十进制数字转换为 b 进制
         res = ""
         while num_dec > 0:
             r = num_dec % self.b
-            res = self._int_to_char(r) + res
+            res = self.int_to_char(r) + res
             num_dec //= self.b
 
         return '-' + res if flag else res
 
-    def _char_to_int(self, c):
+    def char_to_int(self, c: str) -> int:
         """
-        将字符转换为数字
-        :param c:
-        :return:
+        将字符串形式的数字字符串，转换为整数
+        :param c: 字符串表示的数字
+        :return: 对应的整数
         """
         if c.isdigit():
             return int(c)
         else:
             c = c.upper()
             return ord(c) - ord('A') + 10
 
-    def _int_to_char(self, n):
+    def int_to_char(self, n: int) -> str:
         """
-        将数字转换为字符
-        :param n:
-        :return:
+        将整数数字n转换为对应的字符串形式
+        :param n: 整数
+        :return: 对应的字符串
         """
         if n < 10:
             return str(n)
         else:
             return chr(ord('A') + n - 10)
 
 
-# 二进制码转换器
+
+
+# 二进制类
 class Bin():
     def __init__(self, num: str, b: int = 2):
         """
         :param num: 数字字符串
         :param base: num的进制，默认为10
         """
         if b != 2:
@@ -93,21 +95,19 @@
         if num[0] == '-': num = num[1:]
         res = num[0]
         n = len(num)
         for i in range(1, n):
             res += str(int(res[-1]) ^ int(num[i]))
         return res
 
-
     def bin_to_grey(self) -> str:
         """
         将当前的二进制码视为二进制码，求解其对应的格雷码
         :return: 对应的格雷码
         """
         num = self.num
         if num[0] == '-': num = num[1:]
         n = len(num)
         res = num[0]
         for i in range(1, n):
             res += str(int(num[i - 1]) ^ int(num[i]))
         return res
-
```

### Comparing `TsingPig_Lab-0.1.5/tsingpig_lab/DataStructures.py` & `TsingPig_Lab-0.1.6/tsingpig_lab/DataStructures.py`

 * *Files identical despite different names*

