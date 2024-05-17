# Comparing `tmp/JsonsTest-0.0.1.tar.gz` & `tmp/JsonsTest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonsTest-0.0.1.tar", last modified: Fri May 17 12:23:52 2024, max compression
+gzip compressed data, was "JsonsTest-0.0.2.tar", last modified: Fri May 17 12:36:37 2024, max compression
```

## Comparing `JsonsTest-0.0.1.tar` & `JsonsTest-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 12:23:52.672105 JsonsTest-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-17 12:23:52.667552 JsonsTest-0.0.1/JsonsTest.egg-info/
--rw-rw-rw-   0        0        0     1364 2024-05-17 12:23:52.000000 JsonsTest-0.0.1/JsonsTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-17 12:23:52.000000 JsonsTest-0.0.1/JsonsTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 12:23:52.000000 JsonsTest-0.0.1/JsonsTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 12:23:52.000000 JsonsTest-0.0.1/JsonsTest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 12:23:52.000000 JsonsTest-0.0.1/JsonsTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1364 2024-05-17 12:23:52.672105 JsonsTest-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      933 2024-05-17 12:20:51.000000 JsonsTest-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 12:23:52.669016 JsonsTest-0.0.1/praktikaJsons/
--rw-rw-rw-   0        0        0     4132 2024-05-17 12:20:51.000000 JsonsTest-0.0.1/praktikaJsons/Jsons.py
--rw-rw-rw-   0        0        0       20 2024-05-17 12:20:51.000000 JsonsTest-0.0.1/praktikaJsons/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-17 12:23:52.673130 JsonsTest-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-17 12:20:51.000000 JsonsTest-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:36:37.210451 JsonsTest-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-17 12:36:37.205448 JsonsTest-0.0.2/JsonsTest/
+-rw-rw-rw-   0        0        0     4134 2024-05-17 12:36:27.000000 JsonsTest-0.0.2/JsonsTest/Jsons.py
+-rw-rw-rw-   0        0        0       20 2024-05-17 12:20:51.000000 JsonsTest-0.0.2/JsonsTest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:36:37.209451 JsonsTest-0.0.2/JsonsTest.egg-info/
+-rw-rw-rw-   0        0        0     1364 2024-05-17 12:36:37.000000 JsonsTest-0.0.2/JsonsTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-17 12:36:37.000000 JsonsTest-0.0.2/JsonsTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 12:36:37.000000 JsonsTest-0.0.2/JsonsTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 12:36:37.000000 JsonsTest-0.0.2/JsonsTest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 12:36:37.000000 JsonsTest-0.0.2/JsonsTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1364 2024-05-17 12:36:37.210451 JsonsTest-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2024-05-17 12:20:51.000000 JsonsTest-0.0.2/README.md
+-rw-rw-rw-   0        0        0       43 2024-05-17 12:36:37.210451 JsonsTest-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-17 12:32:01.000000 JsonsTest-0.0.2/setup.py
```

### Comparing `JsonsTest-0.0.1/JsonsTest.egg-info/PKG-INFO` & `JsonsTest-0.0.2/JsonsTest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsTest
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsTest-0.0.1/PKG-INFO` & `JsonsTest-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsTest
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsTest-0.0.1/README.md` & `JsonsTest-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `JsonsTest-0.0.1/praktikaJsons/Jsons.py` & `JsonsTest-0.0.2/JsonsTest/Jsons.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
         return results
 
     def find_by_key(self, key, data=None):
         """
         Ищет все вхождения заданного ключа в JSON данных.
 
+
         :param key: Ключ для поиска.
         :param data: JSON данные для поиска. Если не указано, используется загруженный JSON.
         :return: Список значений, связанных с заданным ключом.
         """
         if data is None:
             data = self.json_data
```

### Comparing `JsonsTest-0.0.1/setup.py` & `JsonsTest-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='JsonsTest',
-  version='0.0.1',
+  version='0.0.2',
   author='sonin',
   author_email='fediasonin@gmail.com',
   description='This is the simplest module for quick work with json files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
```

