# Comparing `tmp/imsciences-0.5.6.9.tar.gz` & `tmp/imsciences-0.5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.9.tar", last modified: Fri May 17 09:31:18 2024, max compression
+gzip compressed data, was "imsciences-0.5.7.0.tar", last modified: Fri May 17 09:33:12 2024, max compression
```

## Comparing `imsciences-0.5.6.9.tar` & `imsciences-0.5.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 09:31:18.851545 imsciences-0.5.6.9/
--rw-rw-rw-   0        0        0     9976 2024-05-17 09:31:18.846536 imsciences-0.5.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.6.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 09:31:18.810535 imsciences-0.5.6.9/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.9/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80452 2024-05-17 09:31:11.000000 imsciences-0.5.6.9/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-17 09:31:18.843537 imsciences-0.5.6.9/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-17 09:31:18.000000 imsciences-0.5.6.9/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-17 09:31:18.000000 imsciences-0.5.6.9/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 09:31:18.000000 imsciences-0.5.6.9/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 09:31:18.000000 imsciences-0.5.6.9/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 09:31:18.000000 imsciences-0.5.6.9/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 09:31:18.851545 imsciences-0.5.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-17 09:31:02.000000 imsciences-0.5.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:33:12.329815 imsciences-0.5.7.0/
+-rw-rw-rw-   0        0        0     9976 2024-05-17 09:33:12.324845 imsciences-0.5.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 09:33:12.286991 imsciences-0.5.7.0/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.0/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80458 2024-05-17 09:33:05.000000 imsciences-0.5.7.0/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:33:12.319278 imsciences-0.5.7.0/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-17 09:33:12.000000 imsciences-0.5.7.0/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-17 09:33:12.000000 imsciences-0.5.7.0/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:33:12.000000 imsciences-0.5.7.0/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 09:33:12.000000 imsciences-0.5.7.0/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 09:33:12.000000 imsciences-0.5.7.0/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:33:12.329815 imsciences-0.5.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-17 09:32:47.000000 imsciences-0.5.7.0/setup.py
```

### Comparing `imsciences-0.5.6.9/PKG-INFO` & `imsciences-0.5.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.9
+Version: 0.5.7.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.9/README.md` & `imsciences-0.5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.6.9/imsciences/datafunctions.py` & `imsciences-0.5.7.0/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                 daily_records.append(daily_row)
 
         # Convert the list of daily records into a DataFrame
         daily_df = pd.DataFrame(daily_records)
         
         return daily_df
     
-    def plot_two(df1, col1, df2, col2, date_column, same_axis=True):
+    def plot_two(self, df1, col1, df2, col2, date_column, same_axis=True):
         """
         Plots specified columns from two different dataframes with both different and the same lengths,
         using a specified date column as the X-axis, and charting on either the same or separate y axes.
 
         :param df1: First DataFrame
         :param col1: Column name from the first DataFrame
         :param df2: Second DataFrame
```

### Comparing `imsciences-0.5.6.9/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.7.0/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.9
+Version: 0.5.7.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.9/setup.py` & `imsciences-0.5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.9'
+VERSION = '0.5.7.0'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

