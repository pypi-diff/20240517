# Comparing `tmp/sqlman-0.3.2.tar.gz` & `tmp/sqlman-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlman-0.3.2.tar", last modified: Thu May 16 11:47:57 2024, max compression
+gzip compressed data, was "sqlman-0.3.3.tar", last modified: Fri May 17 16:37:32 2024, max compression
```

## Comparing `sqlman-0.3.2.tar` & `sqlman-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.022647 sqlman-0.3.2/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-16 11:47:57.022430 sqlman-0.3.2/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     3702 2024-05-10 06:15:07.000000 sqlman-0.3.2/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-16 11:47:57.022686 sqlman-0.3.2/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-16 11:47:03.000000 sqlman-0.3.2/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.021258 sqlman-0.3.2/sqlman/
--rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.2/sqlman/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     6497 2024-05-10 05:04:46.000000 sqlman-0.3.2/sqlman/handler.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     9514 2024-05-16 11:47:03.000000 sqlman-0.3.2/sqlman/table_controller.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3.2/sqlman/tools.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.021993 sqlman-0.3.2/sqlman.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/top_level.txt
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.022160 sqlman-0.3.2/tests/
--rw-r--r--   0 wangtuo    (501) staff       (20)      279 2024-05-10 05:38:51.000000 sqlman-0.3.2/tests/test-0.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740825 sqlman-0.3.3/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-17 16:37:32.740593 sqlman-0.3.3/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3694 2024-05-17 16:37:22.000000 sqlman-0.3.3/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-17 16:37:32.740862 sqlman-0.3.3/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-17 16:37:22.000000 sqlman-0.3.3/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.738690 sqlman-0.3.3/sqlman/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.3/sqlman/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     6732 2024-05-17 16:36:11.000000 sqlman-0.3.3/sqlman/handler.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     9514 2024-05-16 11:47:03.000000 sqlman-0.3.3/sqlman/table_controller.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3.3/sqlman/tools.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740113 sqlman-0.3.3/sqlman.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740254 sqlman-0.3.3/tests/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      371 2024-05-17 16:30:01.000000 sqlman-0.3.3/tests/test-0.py
```

### Comparing `sqlman-0.3.2/PKG-INFO` & `sqlman-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.2
+Version: 0.3.3
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
 
 # 如何安装？
 
 - `pip install sqlman`
 
-
-
 # 拿什么吸引你这个靓仔？
 
 - 使用方式简单暴力
 
 - 不用写SQL就能进行增删改查
 
-
-
 ### 连接方式是如此简易
 
 - 一个字典参数即可
 
-
-
 ### 插入数据是如此贴心
 
 - 自动推导
     - 传入dict是插入一条数据，传入list是插入多条数据
 
 - 多种插入模式
     - 模式1，插入时，数据冲突则报错
     - 模式2，插入时，数据冲突则忽略
     - 模式3，插入时，数据发生冲突，把数据进行更新操作
     - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-
-
 # 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
```

### Comparing `sqlman-0.3.2/README.md` & `sqlman-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # 如何安装？
 
 - `pip install sqlman`
 
-
-
 # 拿什么吸引你这个靓仔？
 
 - 使用方式简单暴力
 
 - 不用写SQL就能进行增删改查
 
-
-
 ### 连接方式是如此简易
 
 - 一个字典参数即可
 
-
-
 ### 插入数据是如此贴心
 
 - 自动推导
     - 传入dict是插入一条数据，传入list是插入多条数据
 
 - 多种插入模式
     - 模式1，插入时，数据冲突则报错
     - 模式2，插入时，数据冲突则忽略
     - 模式3，插入时，数据发生冲突，把数据进行更新操作
     - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-
-
 # 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
```

### Comparing `sqlman-0.3.2/setup.py` & `sqlman-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='sqlman',
-    version='0.3.2',
+    version='0.3.3',
     description='告别SQL语句，python操作mysql的贴心助手',
     url='https://github.com/markadc/sqlman',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `sqlman-0.3.2/sqlman/handler.py` & `sqlman-0.3.3/sqlman/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,28 +84,39 @@
             if con:
                 con.rollback()
             return 0
 
         finally:
             self.close_connect(cur, con)
 
+    @staticmethod
+    def _getfv(data: dict | list) -> tuple:
+        item = data if isinstance(data, dict) else data[0]
+        fs = []
+        vs = []
+        for k in item.keys():
+            fs.append('`{}`'.format(k))
+            vs.append('%s')
+        fileds = ', '.join(fs)
+        values = ', '.join(vs)
+        return fileds, values
+
     def _insert_one(self, table: str, item: dict, update: str = None, unique_index: str = None) -> int:
         """
         插入数据
         Args:
             table: 表
             item: 数据
             update: 数据重复，则更新数据
             unique_index: 唯一索引
 
         Returns:
             受影响的行数
         """
-        fields = ', '.join(item.keys())
-        values = ', '.join(['%s'] * len(item.keys()))
+        fields, values = self._getfv(item)
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
         affect = self.exe_sql(sql, args=tuple(item.values()))['affect']
         return affect
 
@@ -117,16 +128,15 @@
             items: 数据
             update: 数据重复，则更新数据
             unique_index: 唯一索引
 
         Returns:
             受影响的行数
         """
-        fields = ', '.join(items[0].keys())
-        values = ', '.join(['%s'] * len(items[0].keys()))
+        fields, values = self._getfv(items)
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
         affect = self.exem_sql(sql, args=[tuple(item.values()) for item in items])
         return affect
```

### Comparing `sqlman-0.3.2/sqlman/table_controller.py` & `sqlman-0.3.3/sqlman/table_controller.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.2/sqlman/tools.py` & `sqlman-0.3.3/sqlman/tools.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.2/sqlman.egg-info/PKG-INFO` & `sqlman-0.3.3/sqlman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.2
+Version: 0.3.3
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
 
 # 如何安装？
 
 - `pip install sqlman`
 
-
-
 # 拿什么吸引你这个靓仔？
 
 - 使用方式简单暴力
 
 - 不用写SQL就能进行增删改查
 
-
-
 ### 连接方式是如此简易
 
 - 一个字典参数即可
 
-
-
 ### 插入数据是如此贴心
 
 - 自动推导
     - 传入dict是插入一条数据，传入list是插入多条数据
 
 - 多种插入模式
     - 模式1，插入时，数据冲突则报错
     - 模式2，插入时，数据冲突则忽略
     - 模式3，插入时，数据发生冲突，把数据进行更新操作
     - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-
-
 # 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
```

