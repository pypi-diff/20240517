# Comparing `tmp/vbpy-2.0.4.tar.gz` & `tmp/vbpy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.0.4.tar", last modified: Fri May 17 01:51:23 2024, max compression
+gzip compressed data, was "vbpy-2.0.5.tar", last modified: Fri May 17 02:11:58 2024, max compression
```

## Comparing `vbpy-2.0.4.tar` & `vbpy-2.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 01:51:23.600000 vbpy-2.0.4/
--rw-rw-rw-   0        0        0      122 2024-05-17 01:51:24.000000 vbpy-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-17 01:51:24.000000 vbpy-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-17 01:51:10.000000 vbpy-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 01:51:23.650000 vbpy-2.0.4/vbpy/
--rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.4/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.4/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0    18226 2024-05-17 01:50:44.000000 vbpy-2.0.4/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.4/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-17 01:51:23.680000 vbpy-2.0.4/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-17 01:51:24.000000 vbpy-2.0.4/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-17 01:51:24.000000 vbpy-2.0.4/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 01:51:24.000000 vbpy-2.0.4/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-17 01:51:24.000000 vbpy-2.0.4/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 02:11:58.130000 vbpy-2.0.5/
+-rw-rw-rw-   0        0        0      122 2024-05-17 02:12:00.000000 vbpy-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-17 02:12:00.000000 vbpy-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-17 02:04:38.000000 vbpy-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:11:58.160000 vbpy-2.0.5/vbpy/
+-rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.5/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.5/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0    18569 2024-05-17 02:11:34.000000 vbpy-2.0.5/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.5/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:11:58.200000 vbpy-2.0.5/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-17 02:11:58.000000 vbpy-2.0.5/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-17 02:12:00.000000 vbpy-2.0.5/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 02:11:58.000000 vbpy-2.0.5/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-17 02:11:58.000000 vbpy-2.0.5/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.0.4/setup.py` & `vbpy-2.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.0.4',
+    version='2.0.5',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.0.4/vbpy/combine_data_file.py` & `vbpy-2.0.5/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.0.4/vbpy/load_claim_auto_file.py` & `vbpy-2.0.5/vbpy/load_claim_auto_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,25 @@
                         'Hạch toán': 'HACH_TOAN',
                         'Ghi chú': 'GHI_CHU'
                     }
 
                     df.rename(columns={col: df_clm_dict[col] for col in df.columns if col in df_clm_dict}, inplace=True)
 
                     
-                    """ SEPARATE SO MAY and SO KHUNG"""
-                    print("--------------------------------------------------------------------------\nSeparating SO MAY/SO KHUNG:")
-                    df['SO_KHUNG/SO_MAY'].fillna('/')
-                    df[['SO_KHUNG', 'SO_MAY']] = df['SO_KHUNG/SO_MAY'].str.split('/', expand=True)
-                    df.drop('SO_KHUNG/SO_MAY', axis = 1, inplace = True)
+                    # """ SEPARATE SO MAY and SO KHUNG"""
+                    # print("--------------------------------------------------------------------------\nSeparating SO MAY/SO KHUNG:")
+                    # df['SO_KHUNG/SO_MAY'].fillna('/')
+                    # def get_part(x, index):
+                    #     parts = x.split('/')
+                    #     return parts[index] if len(parts) > index else np.nan
+
+                    # # Apply this function to create the new columns
+                    # df['SO_KHUNG'] = df['SO_KHUNG/SO_MAY'].apply(lambda x: get_part(x, 0))
+                    # df['SO_MAY'] = df['SO_KHUNG/SO_MAY'].apply(lambda x: get_part(x, 1))
+                    # df.drop('SO_KHUNG/SO_MAY', axis = 1, inplace = True)
                     
                         
                     """ REMOVE UNNECESSARY COLUMNS"""
                     print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
                     removed_cols = [
                         'Lĩnh vực kinh doanh',
                         'Cán bộ cấp đơn',
```

### Comparing `vbpy-2.0.4/vbpy/load_revenue_auto_file.py` & `vbpy-2.0.5/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

