# Comparing `tmp/caluxpy_fi-0.1.52.tar.gz` & `tmp/caluxpy_fi-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.52.tar", last modified: Wed May  8 17:53:13 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.53.tar", last modified: Wed May  8 18:03:28 2024, max compression
```

## Comparing `caluxpy_fi-0.1.52.tar` & `caluxpy_fi-0.1.53.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.997747 caluxpy_fi-0.1.52/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.52/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-05-08 17:53:12.994976 caluxpy_fi-0.1.52/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.52/README.md
--rw-rw-rw-   0        0        0      824 2024-05-08 17:51:47.000000 caluxpy_fi-0.1.52/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 17:53:12.997747 caluxpy_fi-0.1.52/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.870833 caluxpy_fi-0.1.52/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.980121 caluxpy_fi-0.1.52/src/caluxPy_fi/
--rw-rw-rw-   0        0        0    10586 2024-05-08 17:51:33.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.982473 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 18:03:28.600528 caluxpy_fi-0.1.53/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.53/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-08 18:03:28.598502 caluxpy_fi-0.1.53/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.53/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-08 18:01:38.000000 caluxpy_fi-0.1.53/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 18:03:28.601551 caluxpy_fi-0.1.53/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 18:03:28.530197 caluxpy_fi-0.1.53/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 18:03:28.582181 caluxpy_fi-0.1.53/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0     9529 2024-05-08 18:01:08.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.53/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:03:28.596502 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-08 18:03:28.000000 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-08 18:03:28.000000 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 18:03:28.000000 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-08 18:03:28.000000 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 18:03:28.000000 caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.52/LICENSE.txt` & `caluxpy_fi-0.1.53/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/PKG-INFO` & `caluxpy_fi-0.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.52
+Version: 0.1.53
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.52/README.md` & `caluxpy_fi-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/pyproject.toml` & `caluxpy_fi-0.1.53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.52"
+version = "0.1.53"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/Convexity.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,35 +56,36 @@
                                              ytm = ytm2, 
                                              periodicity = periodicity, 
                                              coupon_flow = coupon_flow, 
                                              payment_type = payment_type, 
                                              issuer = issuer, 
                                              notional_value = notional_value, 
                                              gained_coupon = gained_coupon)
-            # Creating lists lists for the table
+            # Append results to lists
             listPBS.append(y) # List of basis points
             listDirtyPrice.append(resValuation[1] * 100) # List of dirty prices
             listDuration.append(resValuation[4] if y != 0 else 0)
             listConvexity.append(resValuation[7] if y != 0 else 0)
             y += 1 # Marginal increase
         
         # Conversion of lists into numpy arrays for ease of use
         listPBS = np.array(listPBS)
         listDirtyPrice = np.array(listDirtyPrice)
         listDuration = np.array(listDuration)
         listConvexity = np.array(listConvexity)
         
         # Creation of DataFrame
-        self.df_convex = pd.DataFrame({'pbs': listPBS, 
-                                       'Price': listDirtyPrice,
-                                       'Duration': listDuration,
-                                       'Convexity': listConvexity
-                                       })
+        self.df_convex = pd.DataFrame({
+            'pbs': listPBS, 
+            'Price': listDirtyPrice,
+            'Duration': listDuration,
+            'Convexity': listConvexity
+        })
         
-        # Treatment of the negatives in the df
+        # Process negative PBS values
         negatives = self.df_convex[self.df_convex['pbs'] <= 0].copy() # Copy the DataFrame for ease of use
         negatives.sort_values(by = 'pbs', ascending = False, inplace = True) # Sort descending
         negatives['dv01'] = negatives['Price'].diff().fillna(0) * 10000 # Calculate the difference and fill first with 0
         negatives['Cummulative'] = negatives['dv01'].cumsum() # Perform Cummulative Sum
         negatives[['Duration', 'Convexity']] = negatives[['Duration', 'Convexity']].cumsum()
         negatives.sort_values(by = 'pbs', ascending = True, inplace = True) # Sort Ascending
         first_neg = negatives.iloc[-2]['dv01'] # Get the first negative (the one after 0)
@@ -93,64 +94,35 @@
         positives = self.df_convex[self.df_convex['pbs'] >= 0].copy() # Copy the DataFrame for ease of use
         positives.sort_values(by = 'pbs', ascending = True, inplace = True) # Sort Ascending
         positives['dv01'] = positives['Price'].diff().fillna(0) * -10000 # Calculate the difference and fill first with 0
         positives['Cummulative'] = positives['dv01'].cumsum() # Perform Cummulative Sum
         positives[['Duration', 'Convexity']] = positives[['Duration', 'Convexity']].cumsum()
         first_pos = positives.iloc[1]['dv01'] # Get the first positive (the one after 0)
         
-        # Getting the average
+        # Calculate average dv01
         self.avg_dv01 = (first_neg + first_pos) / 2 # Get an averaged dv01 with the first occurrence of a marginal increase, because it can go both ways
         
         #Concatenating the dfs to form the complete one
         final = pd.concat([negatives, positives[1:]]) # Concatenate both results of gains and losses
         final.reset_index(drop = True, inplace = True) # Reset indexes so it can be incorporated into the original DataFrame
-        self.df_convex[['dv01', 'Cummulative', 'Duration', 'Convexity']] = final['dv01', 'Cummulative', 'Duration', 'Convexity'] # Incorporate gains and losses into the original DataFrame
+        self.df_convex[['dv01', 'Cummulative', 'Duration', 'Convexity']] = final[['dv01', 'Cummulative', 'Duration', 'Convexity']] # Incorporate gains and losses into the original DataFrame
         
         final['Negative'] = final['pbs'] < 0 # Add a boolean column where True is if value of pbs is negative
         max_values_by_category = final.groupby('Negative')['dv01'].max() # Group the data by the boolean column, having 2 groups (True and False) then getting max values of box, resulting into a list
         avg_values_by_category = final.groupby('Negative')['dv01'].mean() # Get a list with the average means of both groups
         std_values_by_category = final.groupby('Negative')['dv01'].std() # Get a list with the standard deviations of both groups
 
         # Assigning values to the usable variables
         self.max_gain = max_values_by_category[True] 
         self.max_loss = max_values_by_category[False]
         self.avg_gain = avg_values_by_category[True]
         self.avg_loss = avg_values_by_category[False]
         self.std_gain = std_values_by_category[True]
         self.std_loss = std_values_by_category[False]
-
-        '''# Preparing the informations for the chart
-        i = 0
-        while i <= int(bps):
-            if i == 0:
-                listConvexity.append(0)
-            else:
-                listConvexity.append(listConvexity[i - 1] - final['dv01'][i])
-            i += 1
-            
-        i = -1
-        while i >= -int(bps):
-            if i == -1:
-                listConvexity.append(final['dv01'][i])
-            else:
-                listConvexity.append(listConvexity[-1] + final['dv01'][i])
-            i -= 1
-        listConvexity = np.array(listConvexity)
-        listConvexity[::-1].sort()
-        
-        i = -int(bps)
-        while i <= int(bps):
-            listDuration2.append(final['dv01'][0] * (0 - i))
-            i += 1
-        listDuration2 = np.array(listDuration2)
-
-        self.chart_data['x_pbs'] = listPBS
-        self.chart_data['y1_dur'] = listDuration2
-        self.chart_data['y2_cvx'] = listConvexity'''
-        
+       
     def showGraph(self):
         plt.figure(figsize=(10,6))
         plt.plot(self.chart_data['x_pbs'], self.chart_data['y1_dur'])
         plt.plot(self.chart_data['x_pbs'], self.chart_data['y2_cvx'], linestyle='--')
         title = 'Gráfico de Duración-Convexidad' if self._lang == 'esp' else 'Duration-Convexity Graph' if self._lang == 'eng' else ''
         basis_points = 'Puntos Básicos' if self._lang == 'esp' else 'Basis Points' if self._lang == 'eng' else ''
         values = 'Valores Duración y Convexidad' if self._lang == 'esp' else 'Duration and Convexity Values' if self._lang == 'eng' else ''
@@ -169,15 +141,15 @@
                    'max_loss': self.max_loss, 
                    'avg_gain': self.avg_gain, 
                    'avg_loss': self.avg_loss, 
                    'sd_gain': self.std_gain, 
                    'sd_loss': self.std_loss,
                    'dv01': self.avg_dv01,
                    'df': self.df_convex,
-                   'chart_data': self.chart_data
+                   #'chart_data': self.chart_data
                    }
         return results
 
     def __str__(self):
         return f'\
 {'Max Gain' if self._lang == 'eng' else 'Max Ganancia'}: {self.max_gain} \n \
 {'Max Loss' if self._lang == 'eng' else 'Max Perdida'}: {self.max_loss} \n \
```

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/FixedIncome.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.53/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.53/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.52
+Version: 0.1.53
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

