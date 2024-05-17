# Comparing `tmp/wolta-0.2.2.tar.gz` & `tmp/wolta-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.2.2.tar", last modified: Sun May  5 15:48:51 2024, max compression
+gzip compressed data, was "wolta-0.2.3.tar", last modified: Fri May 17 14:07:28 2024, max compression
```

## Comparing `wolta-0.2.2.tar` & `wolta-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.363189 wolta-0.2.2/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0    20873 2024-05-05 15:48:51.362152 wolta-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    19416 2024-05-05 15:48:10.000000 wolta-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 15:48:51.363189 wolta-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1221 2024-05-05 15:19:08.000000 wolta-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.317525 wolta-0.2.2/wolta/
--rw-rw-rw-   0        0        0      115 2024-04-27 21:13:06.000000 wolta-0.2.2/wolta/__init__.py
--rw-rw-rw-   0        0        0    14525 2024-05-05 14:20:24.000000 wolta-0.2.2/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.2.2/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    33410 2024-04-28 15:10:47.000000 wolta-0.2.2/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.2.2/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.361114 wolta-0.2.2/wolta.egg-info/
--rw-rw-rw-   0        0        0    20873 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:07:28.501594 wolta-0.2.3/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    22795 2024-05-17 14:07:28.500504 wolta-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21298 2024-05-17 14:05:22.000000 wolta-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:07:28.501594 wolta-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2024-05-17 08:21:27.000000 wolta-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:07:28.460561 wolta-0.2.3/wolta/
+-rw-rw-rw-   0        0        0      115 2024-04-27 21:13:06.000000 wolta-0.2.3/wolta/__init__.py
+-rw-rw-rw-   0        0        0    19859 2024-05-16 13:31:49.000000 wolta-0.2.3/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.2.3/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    33410 2024-04-28 15:10:47.000000 wolta-0.2.3/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.2.3/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:07:28.499360 wolta-0.2.3/wolta.egg-info/
+-rw-rw-rw-   0        0        0    22795 2024-05-17 14:07:28.000000 wolta-0.2.3/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-17 14:07:28.000000 wolta-0.2.3/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:07:28.000000 wolta-0.2.3/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-17 14:07:28.000000 wolta-0.2.3/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-05-17 14:07:28.000000 wolta-0.2.3/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.2.2/LICENSE.txt` & `wolta-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.2.2/PKG-INFO` & `wolta-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.2.2
+Version: 0.2.3
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -133,14 +133,54 @@
 **Parameters**:
 
 * df, pandas dataframe
 * print_columns, boolean, False by default
 
 ***
 
+### find_deflection
+
+**Returns**:
+
+1. differences, 1D numpy array, if arr parameter is True
+2. average, average difference between predictions and actual values, if avg is True
+3. amount of succeeded predictions, the amount of predictions which in acceptable range, if gap is not None
+4. indexes of succeeded predictions in y_pred, if success_indexes is True
+
+**Parameters**:
+* y_test
+* y_pred
+* arr, True by default
+* avg, False by default
+* gap, None by default, if it is not None then it must be positive
+* gap_type, the type of usage gap value in the creation of accepted range as 'successful'
+
+| value | meaning                                                                     |
+| --- |-----------------------------------------------------------------------------|
+| exact | prediction and actual value must be same                                    |
+| num | for succession must be 'actual - gap <= prediction <= actual + gap'         |
+| num+ | for succession must be 'actual <= prediction <= actual + gap'               |
+| num- | for succession must be 'actual - gap <= prediction <= actual'               |
+| per | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual * (100 + gap) / 100' |
+| per+ | for succession must be 'actual <= prediction <= actual * (100 + gap) / 100' |
+| per- | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual' |
+
+* dif_type, indicates the way of calculation of difference between prediction and actual value. 'f-i' by default.
+
+| value | meaning |
+| --- | --- |
+| f-i | difference = prediction - actual |
+| i-f | difference = actual - prediction |
+| abs | absolute value |
+
+* avg_w_abs, True by default, indicates the way of calculation of average difference, using difference array with absolute values or not
+* success_indexes, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
```

### Comparing `wolta-0.2.2/README.md` & `wolta-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -109,14 +109,54 @@
 **Parameters**:
 
 * df, pandas dataframe
 * print_columns, boolean, False by default
 
 ***
 
+### find_deflection
+
+**Returns**:
+
+1. differences, 1D numpy array, if arr parameter is True
+2. average, average difference between predictions and actual values, if avg is True
+3. amount of succeeded predictions, the amount of predictions which in acceptable range, if gap is not None
+4. indexes of succeeded predictions in y_pred, if success_indexes is True
+
+**Parameters**:
+* y_test
+* y_pred
+* arr, True by default
+* avg, False by default
+* gap, None by default, if it is not None then it must be positive
+* gap_type, the type of usage gap value in the creation of accepted range as 'successful'
+
+| value | meaning                                                                     |
+| --- |-----------------------------------------------------------------------------|
+| exact | prediction and actual value must be same                                    |
+| num | for succession must be 'actual - gap <= prediction <= actual + gap'         |
+| num+ | for succession must be 'actual <= prediction <= actual + gap'               |
+| num- | for succession must be 'actual - gap <= prediction <= actual'               |
+| per | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual * (100 + gap) / 100' |
+| per+ | for succession must be 'actual <= prediction <= actual * (100 + gap) / 100' |
+| per- | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual' |
+
+* dif_type, indicates the way of calculation of difference between prediction and actual value. 'f-i' by default.
+
+| value | meaning |
+| --- | --- |
+| f-i | difference = prediction - actual |
+| i-f | difference = actual - prediction |
+| abs | absolute value |
+
+* avg_w_abs, True by default, indicates the way of calculation of average difference, using difference array with absolute values or not
+* success_indexes, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
```

### Comparing `wolta-0.2.2/setup.py` & `wolta-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.2.2/wolta/data_tools.py` & `wolta-0.2.3/wolta/data_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -564,7 +564,155 @@
         gen_results[col] = results
 
         if verbose:
             print('***')
 
     if get_dict:
         return gen_results
+
+
+def find_deflection(y_test, y_pred, arr=True, avg=False, gap=None, gap_type='num', dif_type='f-i', avg_w_abs=True, success_indexes=False):
+    if arr == True or avg == True or gap is not None:
+        diffs = []
+
+        first = None
+        second = None
+
+        if dif_type == 'f-i':
+            first = y_pred
+            second = y_test
+        elif dif_type == 'i-f':
+            first = y_test
+            second = y_pred
+        else:
+            first = y_pred
+            second = y_test
+
+        for i in range(y_test.shape[0]):
+            diffs.append(first[i] - second[i])
+
+        diffs = np.array(diffs)
+
+        if dif_type == 'abs':
+            diffs = np.abs(diffs)
+
+        if arr == True and avg == False and gap is None:
+            return diffs
+
+        if avg == True:
+            avg_score = 0
+
+            tot_arr = diffs
+            if dif_type != 'abs' and avg_w_abs == True:
+                tot_arr = np.abs(diffs)
+
+            for i in range(diffs.shape[0]):
+                avg_score += tot_arr[i]
+
+            avg_score /= diffs.shape[0]
+
+            if arr == True and avg == True and gap is None:
+                return diffs, avg_score
+
+            if arr == False and avg == True and gap is None:
+                return avg_score
+
+            indexes = []
+
+            if gap_type == 'exact':
+                for i in range(y_test.shape[0]):
+                    if y_test[i] == y_pred[i]:
+                        indexes.append(i)
+            else:
+                for i in range(y_test.shape[0]):
+                    lowest = None
+                    highest = None
+
+                    if gap_type == 'num':
+                        lowest = y_test[i] - gap
+                        highest = y_test[i] + gap
+                    elif gap_type == 'num+':
+                        lowest = y_test[i]
+                        highest = y_test[i] + gap
+                    elif gap_type == 'num-':
+                        lowest = y_test[i] - gap
+                        highest = y_test[i]
+                    elif gap_type == 'per':
+                        lowest = y_test[i] * (100 - gap) / 100
+                        highest = y_test[i] * (100 + gap) / 100
+                    elif gap_type == 'per+':
+                        lowest = y_test[i]
+                        highest = y_test[i] * (100 + gap) / 100
+                    elif gap_type == 'per-':
+                        lowest = y_test[i] * (100 - gap) / 100
+                        highest = y_test[i]
+
+                    if highest < lowest:
+                        temp = lowest
+                        lowest = highest
+                        highest = temp
+
+                    if lowest <= y_pred[i] <= highest:
+                        indexes.append(i)
+
+            if arr == True and avg == True and gap is not None:
+                if success_indexes == True:
+                    return diffs, avg_score, len(indexes), indexes
+                else:
+                    return diffs, avg_score, len(indexes)
+
+            if arr == False and avg == True and gap is not None:
+                if success_indexes == True:
+                    return avg_score, len(indexes), indexes
+                else:
+                    return avg_score, len(indexes)
+
+        if gap is not None:
+            indexes = []
+
+            if gap_type == 'exact':
+                for i in range(y_test.shape[0]):
+                    if y_test[i] == y_pred[i]:
+                        indexes.append(i)
+            else:
+                for i in range(y_test.shape[0]):
+                    lowest = None
+                    highest = None
+
+                    if gap_type == 'num':
+                        lowest = y_test[i] - gap
+                        highest = y_test[i] + gap
+                    elif gap_type == 'num+':
+                        lowest = y_test[i]
+                        highest = y_test[i] + gap
+                    elif gap_type == 'num-':
+                        lowest = y_test[i] - gap
+                        highest = y_test[i]
+                    elif gap_type == 'per':
+                        lowest = y_test[i] * (100 - gap) / 100
+                        highest = y_test[i] * (100 + gap) / 100
+                    elif gap_type == 'per+':
+                        lowest = y_test[i]
+                        highest = y_test[i] * (100 + gap) / 100
+                    elif gap_type == 'per-':
+                        lowest = y_test[i] * (100 - gap) / 100
+                        highest = y_test[i]
+
+                    if highest < lowest:
+                        temp = lowest
+                        lowest = highest
+                        highest = temp
+
+                    if lowest <= y_pred[i] <= highest:
+                        indexes.append(i)
+
+            if arr == True and avg == False:
+                if success_indexes == True:
+                    return diffs, len(indexes), indexes
+                else:
+                    return diffs, len(indexes)
+
+            if arr == False and avg == False:
+                if success_indexes == True:
+                    return len(indexes), indexes
+                else:
+                    return len(indexes)
```

### Comparing `wolta-0.2.2/wolta/feature_tools.py` & `wolta-0.2.3/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.2/wolta/model_tools.py` & `wolta-0.2.3/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.2/wolta/progressive_tools.py` & `wolta-0.2.3/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.2/wolta.egg-info/PKG-INFO` & `wolta-0.2.3/wolta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.2.2
+Version: 0.2.3
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -133,14 +133,54 @@
 **Parameters**:
 
 * df, pandas dataframe
 * print_columns, boolean, False by default
 
 ***
 
+### find_deflection
+
+**Returns**:
+
+1. differences, 1D numpy array, if arr parameter is True
+2. average, average difference between predictions and actual values, if avg is True
+3. amount of succeeded predictions, the amount of predictions which in acceptable range, if gap is not None
+4. indexes of succeeded predictions in y_pred, if success_indexes is True
+
+**Parameters**:
+* y_test
+* y_pred
+* arr, True by default
+* avg, False by default
+* gap, None by default, if it is not None then it must be positive
+* gap_type, the type of usage gap value in the creation of accepted range as 'successful'
+
+| value | meaning                                                                     |
+| --- |-----------------------------------------------------------------------------|
+| exact | prediction and actual value must be same                                    |
+| num | for succession must be 'actual - gap <= prediction <= actual + gap'         |
+| num+ | for succession must be 'actual <= prediction <= actual + gap'               |
+| num- | for succession must be 'actual - gap <= prediction <= actual'               |
+| per | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual * (100 + gap) / 100' |
+| per+ | for succession must be 'actual <= prediction <= actual * (100 + gap) / 100' |
+| per- | for succession must be 'actual * (100 - gap) / 100 <= prediction <= actual' |
+
+* dif_type, indicates the way of calculation of difference between prediction and actual value. 'f-i' by default.
+
+| value | meaning |
+| --- | --- |
+| f-i | difference = prediction - actual |
+| i-f | difference = actual - prediction |
+| abs | absolute value |
+
+* avg_w_abs, True by default, indicates the way of calculation of average difference, using difference array with absolute values or not
+* success_indexes, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
```

