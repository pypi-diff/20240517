# Comparing `tmp/findpeaks-2.6.2.tar.gz` & `tmp/findpeaks-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpeaks-2.6.2.tar", last modified: Sun Feb 18 23:16:06 2024, max compression
+gzip compressed data, was "findpeaks-2.6.3.tar", last modified: Sun Feb 18 23:59:47 2024, max compression
```

## Comparing `findpeaks-2.6.2.tar` & `findpeaks-2.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.981185 findpeaks-2.6.2/
--rw-rw-rw-   0        0        0     1122 2023-09-23 19:57:53.000000 findpeaks-2.6.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9113 2024-02-18 23:16:06.977672 findpeaks-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     8282 2023-11-10 19:54:20.000000 findpeaks-2.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.875243 findpeaks-2.6.2/findpeaks/
--rw-rw-rw-   0        0        0     2347 2024-02-18 23:13:49.000000 findpeaks-2.6.2/findpeaks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.960540 findpeaks-2.6.2/findpeaks/data/
--rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/data/__init__.py
--rw-rw-rw-   0        0        0    23598 2023-11-19 20:16:45.000000 findpeaks-2.6.2/findpeaks/examples.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.972020 findpeaks-2.6.2/findpeaks/filters/
--rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/__init__.py
--rw-rw-rw-   0        0        0     5665 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/frost.py
--rw-rw-rw-   0        0        0     4133 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/kuan.py
--rw-rw-rw-   0        0        0     6429 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/lee.py
--rw-rw-rw-   0        0        0     5248 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/lee_enhanced.py
--rw-rw-rw-   0        0        0    17184 2023-11-10 19:27:38.000000 findpeaks-2.6.2/findpeaks/filters/lee_sigma.py
--rw-rw-rw-   0        0        0     3921 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/mean.py
--rw-rw-rw-   0        0        0     3180 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/filters/median.py
--rw-rw-rw-   0        0        0    57116 2023-11-10 19:28:41.000000 findpeaks-2.6.2/findpeaks/findpeaks.py
--rw-rw-rw-   0        0        0     5995 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/interpolate.py
--rw-rw-rw-   0        0        0    25717 2023-11-10 19:32:10.000000 findpeaks-2.6.2/findpeaks/stats.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.977672 findpeaks-2.6.2/findpeaks/tests/
--rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/tests/__init__.py
--rw-rw-rw-   0        0        0     8801 2023-11-10 19:36:09.000000 findpeaks-2.6.2/findpeaks/tests/test_findpeaks.py
--rw-rw-rw-   0        0        0     2469 2023-09-23 19:57:53.000000 findpeaks-2.6.2/findpeaks/union_find.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:16:06.954907 findpeaks-2.6.2/findpeaks.egg-info/
--rw-rw-rw-   0        0        0     9113 2024-02-18 23:16:06.000000 findpeaks-2.6.2/findpeaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-02-18 23:16:06.000000 findpeaks-2.6.2/findpeaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 23:16:06.000000 findpeaks-2.6.2/findpeaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-02-18 23:16:06.000000 findpeaks-2.6.2/findpeaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-18 23:16:06.000000 findpeaks-2.6.2/findpeaks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-18 23:16:06.981185 findpeaks-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1735 2024-02-18 23:08:54.000000 findpeaks-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.861548 findpeaks-2.6.3/
+-rw-rw-rw-   0        0        0     1122 2023-09-23 19:57:53.000000 findpeaks-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9113 2024-02-18 23:59:47.861548 findpeaks-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8282 2023-11-10 19:54:20.000000 findpeaks-2.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.812717 findpeaks-2.6.3/findpeaks/
+-rw-rw-rw-   0        0        0     2347 2024-02-18 23:34:29.000000 findpeaks-2.6.3/findpeaks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.845748 findpeaks-2.6.3/findpeaks/data/
+-rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/data/__init__.py
+-rw-rw-rw-   0        0        0    23530 2024-02-18 23:29:37.000000 findpeaks-2.6.3/findpeaks/examples.py
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.854267 findpeaks-2.6.3/findpeaks/filters/
+-rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/__init__.py
+-rw-rw-rw-   0        0        0     5665 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/frost.py
+-rw-rw-rw-   0        0        0     4133 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/kuan.py
+-rw-rw-rw-   0        0        0     6429 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/lee.py
+-rw-rw-rw-   0        0        0     5248 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/lee_enhanced.py
+-rw-rw-rw-   0        0        0    17184 2023-11-10 19:27:38.000000 findpeaks-2.6.3/findpeaks/filters/lee_sigma.py
+-rw-rw-rw-   0        0        0     3921 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/mean.py
+-rw-rw-rw-   0        0        0     3180 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/filters/median.py
+-rw-rw-rw-   0        0        0    58483 2024-02-18 23:56:17.000000 findpeaks-2.6.3/findpeaks/findpeaks.py
+-rw-rw-rw-   0        0        0     5995 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/interpolate.py
+-rw-rw-rw-   0        0        0    25717 2023-11-10 19:32:10.000000 findpeaks-2.6.3/findpeaks/stats.py
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.854267 findpeaks-2.6.3/findpeaks/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/tests/__init__.py
+-rw-rw-rw-   0        0        0     9039 2024-02-18 23:58:03.000000 findpeaks-2.6.3/findpeaks/tests/test_findpeaks.py
+-rw-rw-rw-   0        0        0     2469 2023-09-23 19:57:53.000000 findpeaks-2.6.3/findpeaks/union_find.py
+drwxrwxrwx   0        0        0        0 2024-02-18 23:59:47.845748 findpeaks-2.6.3/findpeaks.egg-info/
+-rw-rw-rw-   0        0        0     9113 2024-02-18 23:59:47.000000 findpeaks-2.6.3/findpeaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-02-18 23:59:47.000000 findpeaks-2.6.3/findpeaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-18 23:59:47.000000 findpeaks-2.6.3/findpeaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-02-18 23:59:47.000000 findpeaks-2.6.3/findpeaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-02-18 23:59:47.000000 findpeaks-2.6.3/findpeaks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-18 23:59:47.861548 findpeaks-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2024-02-18 23:54:23.000000 findpeaks-2.6.3/setup.py
```

### Comparing `findpeaks-2.6.2/LICENSE` & `findpeaks-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/PKG-INFO` & `findpeaks-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.6.2
+Version: 2.6.3
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.6.2.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.6.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy==1.11.4
+Requires-Dist: peakdetect==1.1
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: peakdetect==1.1
 Requires-Dist: requests
 Requires-Dist: caerus>=0.1.9
 Requires-Dist: xarray
 Requires-Dist: joblib
 
 # findpeaks
```

### Comparing `findpeaks-2.6.2/README.md` & `findpeaks-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/__init__.py` & `findpeaks-2.6.3/findpeaks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from findpeaks.filters.kuan import kuan_filter
 from findpeaks.filters.frost import frost_filter
 from findpeaks.filters.median import median_filter
 from findpeaks.filters.mean import mean_filter
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.6.2'
+__version__ = '2.6.3'
 
 # module level doc-string
 __doc__ = """
 findpeaks
 =====================================================================
 
 findpeaks is for the detection and vizualization of peaks and valleys in a 1D-vector and 2D-array.
```

### Comparing `findpeaks-2.6.2/findpeaks/examples.py` & `findpeaks-2.6.3/findpeaks/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,26 +53,26 @@
 import numpy as np
 from scipy.ndimage import gaussian_filter
 from findpeaks import findpeaks
 rng = np.random.default_rng(42)
 x = rng.normal(size=(50, 50))
 x = gaussian_filter(x, sigma=10.)
 # peak and valley
-fp = findpeaks(method="topology", whitelist=['peak','valley'], denoise=None, verbose=3)
+fp = findpeaks(method="topology", whitelist=['peak', 'valley'], denoise=None, verbose=3)
 results = fp.fit(x)
 
 fp.plot(figsize=(25, 15), figure_order='horizontal', cmap=plt.cm.hot_r)
 fp.plot_persistence()
 # fp.plot_mesh()
 
 # %%
 
 from findpeaks import findpeaks
 path = r'https://user-images.githubusercontent.com/12035402/274193739-cdfd8986-91eb-4211-bef6-ebad041f47ae.png'
-fp = findpeaks(method='topology', denoise='lee_sigma', params={'window': 5}, whitelist='peak', limit=5)
+fp = findpeaks(method='topology', whitelist='peak', limit=5, denoise='lee_sigma', params={'window': 5})
 X = fp.imread(path)
 results = fp.fit(X)
 
 result_df = results['persistence']
 peak = result_df.index[result_df['peak']==True].tolist()
 print(result_df.loc[peak])
 print(result_df.shape)
@@ -110,15 +110,15 @@
 
 
 
 # %%
 from findpeaks import findpeaks
 X = [1,1,1.1,1,0.9,1,1,1.1,1,0.9,1,1.1,1,1,0.9,1,1,1.1,1,1,1,1,1.1,0.9,1,1.1,1,1,0.9,1,1.1,1,1,1.1,1,0.8,0.9,1,1.2,0.9,1,1,1.1,1.2,1,1.5,1,3,2,5,3,2,1,1,1,0.9,1,1,3,2.6,4,3,3.2,2,1,1,0.8,4,4,2,2.5,1,1,1]
 
-fp = findpeaks(method='peakdetect', lookahead=1, verbose=3, whitelist=['peak', 'valley'], params={'delta': 1})
+fp = findpeaks(method='peakdetect', whitelist=['peak', 'valley'], lookahead=1, params={'delta': 1}, verbose=3)
 # fp = findpeaks(method='topology')
 results = fp.fit(X)
 fp.plot()
 
 
 # %% New functionality:
 import findpeaks as fp
@@ -142,19 +142,15 @@
 
 
 # %%
 # Import library
 from findpeaks import findpeaks
 
 # Initialize
-fp = findpeaks(method='topology',
-               scale=True,
-               togray=True,
-               imsize=(150, 150),
-               denoise='lee_sigma',
+fp = findpeaks(method='topology', imsize=(150, 150), scale=True, togray=True, denoise='lee_sigma',
                params={'window': 17})
 
 # Import example image
 img = fp.import_example('2dpeaks_image')
 
 # Denoising and detecting peaks
 results = fp.fit(img)
@@ -163,15 +159,15 @@
 # Create denoised plot
 fp.plot(limit=80, figure_order='horizontal', cmap=plt.cm.hot_r)
 
 
 # %% Issue 18:
 from findpeaks import findpeaks
     
-fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, params={'window': 15})
+fp = findpeaks(method='topology', imsize=False, scale=False, togray=False, denoise=None, params={'window': 15})
 X = fp.import_example('2dpeaks')
 fp.fit(X)
 # fp.plot_mesh(wireframe=False, title='Test', cmap='RdBu', view=(70,5))
 fp.plot_mesh()
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10])
 fp.plot_mesh(xlim=[10, None], ylim=[4, 10])
 fp.plot_mesh(xlim=[10, None], ylim=[4, None])
@@ -179,29 +175,29 @@
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[0, None])
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[None, 6])
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[2, 6])
 
 # %%
 from findpeaks import findpeaks
 path = r'https://user-images.githubusercontent.com/44827483/221152897-133839bb-7364-492a-921b-c9077ab9930b.png'
-fp = findpeaks(method='topology', denoise='lee_enhanced', params={'window':5}, whitelist='peak')
-fp = findpeaks(method='topology', denoise='lee_sigma', params={'window':5}, whitelist='peak')
+fp = findpeaks(method='topology', whitelist='peak', denoise='lee_enhanced', params={'window': 5})
+fp = findpeaks(method='topology', whitelist='peak', denoise='lee_sigma', params={'window': 5})
 X = fp.imread(path)
 results = fp.fit(X)
 fp.plot_persistence()
 fp.plot()
 # fp.plot_mesh()
 
 fp.results['persistence'].iloc[0:10,:]
 
 # %%
 from findpeaks import findpeaks
 X = [1,1,1.1,1,0.9,1,1,1.1,1,0.9,1,1.1,1,1,0.9,1,1,1.1,1,1,1,1,1.1,0.9,1,1.1,1,1,0.9,1,1.1,1,1,1.1,1,0.8,0.9,1,1.2,0.9,1,1,1.1,1.2,1,1.5,1,3,2,5,3,2,1,1,1,0.9,1,1,3,2.6,4,3,3.2,2,1,1,0.8,4,4,2,2.5,1,1,1]
 
-fp = findpeaks(method='peakdetect', lookahead=1, verbose=3, whitelist=['peak', 'valley'])
+fp = findpeaks(method='peakdetect', whitelist=['peak', 'valley'], lookahead=1, verbose=3)
 results = fp.fit(X)
 fp.plot()
 
 # %%
 from findpeaks import findpeaks
 X = [1,1,1.1,1,0.9,1,1,1.1,1,0.9,1,1.1,1,1,0.9,1,1,1.1,1,1,1,1,1.1,0.9,1,1.1,1,1,0.9,1,1.1,1,1,1.1,1,0.8,0.9,1,1.2,0.9,1,1,1.1,1.2,1,1.5,1,3,2,5,3,2,1,1,1,0.9,1,1,3,2.6,4,3,3.2,2,1,1,0.8,4,4,2,2.5,1,1,1]
 
@@ -225,15 +221,15 @@
 
 
 # %% issue in mail
 import numpy as np
 from findpeaks import findpeaks
 
 # Initialize peakdetect
-fp1 = findpeaks(method='peakdetect', lookahead=200, whitelist='peak')
+fp1 = findpeaks(method='peakdetect', whitelist='peak', lookahead=200)
 
 # Initialize topology
 fp2 = findpeaks(method='topology')
 
 # Example 1d-vector
 i = 10000
 xs = np.linspace(0,3.7*np.pi,i)
@@ -263,27 +259,27 @@
 fp = findpeaks(method='caerus', params={'minperc': 5, 'window': 50})
 results = fp.fit(X)
 
 
 # %% Issue 13
 # https://github.com/erdogant/findpeaks/issues/13
 from findpeaks import findpeaks
-fp = findpeaks(method="mask", denoise=None, params={'window': 3}, limit=None, verbose=0)
+fp = findpeaks(method="mask", limit=None, denoise=None, params={'window': 3}, verbose=0)
 X = fp.import_example("2dpeaks_image")
 results = fp.fit(X)
 fp.plot(figure_order='horizontal')
 
 
 # %%
 # Load library
 from findpeaks import findpeaks
 # Data
 X = [10,11,9,23,21,11,45,20,11,12]
 # Initialize
-fp = findpeaks(method='topology', lookahead=1, verbose=0, whitelist=['valley', 'peak'])
+fp = findpeaks(method='topology', whitelist=['valley', 'peak'], lookahead=1, verbose=0)
 results = fp.fit(X)
 fp.plot()
 results['df']
 
 # %% find peak and valleys in 2d images.
 import numpy as np
 import matplotlib.pyplot as plt
@@ -306,15 +302,15 @@
 # %%
 from findpeaks import findpeaks
 import cv2
 x = cv2.imread('C://temp/LbK2I.png')
 # x = cv2.imread('C://temp/uISO2.png')
 # x = [7193,7539,14310,14364,7414,7353,7557,7184,7188,7550,14330,14414,7480,7400,7582,7205,7140,7546,14356,14462,7533,7426,7618,7224,7192,7550,14371,14494,7558,7436,7634,7231,7172,7556,14390,14545,7616,7491,7669,7260,7123,7557,14404,14590,7671,7532,7698,7281,7172,7578,14396,14624,7703,7555,7718,7283,7214,7597,14407,14659,7729,7574,7742,7280,7219,7599,14414,14702,7764,7594,7743,7284,7217,7604,14414,14729,7794,7604,7740,7283,7233,7655,14430,14782,7853,7647,7779,7306,7207,7663,14444,14831,7895,7676,7808,7326,7292,7673,14427,14848,7889,7653,7769,7313,7330,7711,14433,14883,7909,7654,7772,7322,7343,7732,14442,14934,7969,7706,7807,7341,7315,7735,14450,14987,8043,7771,7837,7360,7330,7759,14458,15032,8083,7791,7857,7386,7364,7790,14464,15063,8106,7804,7859,7397,7364,7799,14474,15097,8161,7838,7873,7413,7374,7803,14468,15139,8212,7858,7891,7432,7391,7836,14478,15181,8258,7900,7927,7462,7405,7840,14459,15195,8278,7932,7950,7476,7389,7849,14454,15224,8321,7965,7978,7494,7470,7860,14445,15230,8322,7972,7979,7497,7430,7895,14454,15267,8344,8006,8020,7518,7420,7898,14440,15276,8332,7996,8015,7516,7482,7918,14410,15265,8332,7988,8005,7519,7536,7956,14404,15279,8339,7998,8026,7539,7523,7949,14410,15289,8329,8005,8047,7564,7501,7945,14403,15283,8329,8009,8049,7562,7533,7970,14392,15283,8321,8017,8068,7577,7515,7980,14409,15297,8319,8031,8078,7600,7508,7967,14396,15286,8331,8047,8072,7590,7582,7967,14362,15257,8336,8041,8072,7583,7650,7956,14344,15229,8318,8015,8060,7580,7570,7945,14342,15223,8314,8015,8059,7599,7529,7966,14355,15229,8321,8041,8085,7628,7578,7959,14352,15212,8322,8048,8089,7632,7546,7932,14332,15181,8306,8055,8078,7615,7494,7943,14325,15160,8291,8057,8069,7616,7547,7962,14296,15126,8253,8031,8053,7606,7646,7953,14239,15066,8203,7985,8015,7570,7539,7955,14249,15057,8196,7989,8031,7602,7447,7967,14276,15059,8191,8024,8069,7646,7532,7942,14258,14998,8145,7994,8046,7633,7543,7932,14220,14927,8073,7949,8011,7594,7491,7943,14190,14869,8019,7919,7992,7583,7505,7897,14183,14822,7985,7907,8007,7593,7470,7858,14176,14778,7940,7889,7991,7584,7478,7823,14152,14706,7876,7857,7960,7567,7549,7832,14111,14618,7783,7795,7915,7526,7456,7792,14132,14556,7723,7756,7910,7515,7336,7745,14149,14517,7669,7719,7881,7503,7309,7725,14143,14448,7587,7676,7840,7476,7350,7701,14117,14364,7496,7624,7798,7432,7295,7653,14114,14298,7440,7572,7746,7394,7282,7643,14100,14236,7350,7527,7704,7368,7296,7626,14081,14174,7284,7491,7688,7345,7217,7588,14086,14110,7205,7440,7655,7310,7174,7557,14086,14038,7139,7387,7613,7283,7209,7512,14081,13995,7087,7351,7578,7274,7178,7472,14078,13950,7029,7318,7549,7255,7110,7441,14066,13878,6954,7259,7489,7222,7076,7420,14076,13839,6896,7223,7485,7225,7127,7390,14050,13784,6831,7186,7469,7187,7013,7332,14083,13760,6783,7164,7458,7183,6996,7308,14078,13712,6725,7128,7417,7170,7024,7302,14077,13676,6668,7081,7392,7135,6996,7283,14071,13635,6613,7034,7363,7121,6940,7247,14067,13593,6553,6998,7349,7102,6892,7258,14098,13599,6539,7006,7384,7119,6894,7222,14086,13558,6483,6972,7346,7096,6920,7193,14064,13510,6437,6926,7301,7050,6937,7191,14053,13506,6422,6914,7295,7047,6928,7176,14060,13499,6393,6894,7292,7056,6855,7155,14077,13482,6384,6899,7281,7061,6861,7159,14069,13479,6372,6881,7266,7057,6935,7164,14063,13461,6334,6857,7253,7047,6935,7140,14047,13443,6303,6828,7218,7027,6897,7114,14054,13439,6296,6822,7200,7030,6801,7123,14090,13475,6316,6861,7245,7069,6763,7123,14087,13484,6316,6870,7268,7087,6961,7130,14023,13420,6250,6812,7202,7032,7013,7148,14022,13406,6231,6804,7201,7025,6947,7131,14057,13437,6247,6835,7236,7053,6806,7094,14081,13461,6263,6848,7262,7070,6828,7101,14059,13453,6250,6822,7240,7070,6870,7118,14054,13451,6256,6817,7249,7073,6882,7106,14045,13464,6253,6827,7237,7063,6925,7101,14028,13443,6243,6817,7216,7047,6954,7111,14036,13458,6254,6831,7224,7050,6924,7091,14038,13461,6253,6837,7221,7054,6868,7082,14049,13474,6257,6828,7214,7051,6866,7107,14052,13495,6271,6838,7231,7069,6866,7121,14046,13510,6284,6858,7243,7086,6868,7107,14023,13503,6260,6851,7216,7070,6976,7097,13991,13465,6223,6817,7162,7037,6980,7117,13999,13479,6244,6822,7191,7044,6827,7093,14059,13534,6302,6867,7234,7099,6831,7094,14064,13540,6302,6854,7217,7102,6876,7114,14052,13551,6290,6858,7231,7108]
 
-fp = findpeaks(method="peakdetect", whitelist=['peak', 'valley'], denoise=None, limit=0, verbose=3)
+fp = findpeaks(method="peakdetect", whitelist=['peak', 'valley'], limit=0, denoise=None, verbose=3)
 results = fp.fit(x)
 
 # results['df']
 fp.plot()
 fp.plot_persistence()
 fp.plot_mesh(view=(90, 0))
 
@@ -326,15 +322,15 @@
 from findpeaks import findpeaks
 rng = np.random.default_rng(42)
 
 x = rng.normal(size=(50, 50))
 x = gaussian_filter(x, sigma=10.)
 
 # Search for peaks/valleys with a minimum value of 0
-fp = findpeaks(method="topology", denoise=None, limit=0, verbose=3)
+fp = findpeaks(method="topology", limit=0, denoise=None, verbose=3)
 results = fp.fit(x)
 
 results['persistence']
 fp.plot(cmap='coolwarm')
 
 # Plot
 plt.imshow(x, cmap="coolwarm", interpolation="none", vmin=0, vmax=255)
@@ -366,29 +362,29 @@
 fp.plot_persistence(fontsize_ax1=4)
 
 fp = findpeaks(method="peakdetect", lookahead=15, verbose=verbose)
 # Make fit
 results = fp.fit(X)
 fp.plot()
 
-fp = findpeaks(method="caerus", params={'minperc':100}, interpolate=None, verbose=verbose)
+fp = findpeaks(method="caerus", interpolate=None, params={'minperc': 100}, verbose=verbose)
 # Make fit
 results = fp.fit(X)
 ax = fp.plot()
 
 
 # %%
 from findpeaks import findpeaks
 import numpy as np
 
 # np.random.seed(100)
 np.random.seed(200)
 X = np.random.randint(200, size=400)
 
-fp = findpeaks(method='topology', interpolate = 10, lookahead = 1, verbose=3)
+fp = findpeaks(method='topology', lookahead=1, interpolate=10, verbose=3)
 results = fp.fit(X)
 
 fig=fp.plot()
 fp.plot_mesh()
 
 # %%
 from findpeaks import findpeaks
@@ -410,45 +406,40 @@
 
 # %%
 # Import library
 from findpeaks import findpeaks
 # Import image example
 img = fp.import_example('2dpeaks_image')
 # Initializatie
-fp = findpeaks(scale=True, denoise='fastnl', params={'window': 31}, togray=True, imsize=(300,300), whitelist=['peak', 'valley'], verbose=3)
+fp = findpeaks(whitelist=['peak', 'valley'], imsize=(300, 300), scale=True, togray=True, denoise='fastnl',
+               params={'window': 31}, verbose=3)
 # Fit
 fp.fit(img)
 fp.plot()
 fp.results["persistence"]
 
 # Take the minimum score for the top peaks off the diagonal.
 limit = fp.results['persistence'][0:5]['score'].min()
 fp.plot(text=True, limit=limit)
 
-fp = findpeaks(scale=True,
-               denoise='fastnl',
-               params={'window': 31},
-               togray=True,
-               imsize=(300,300),
-               limit=limit,
-               whitelist=['peak', 'valley'],
-               verbose=3)
+fp = findpeaks(whitelist=['peak', 'valley'], limit=limit, imsize=(300, 300), scale=True, togray=True, denoise='fastnl',
+               params={'window': 31}, verbose=3)
 fp.fit(img)
 
 fp.results["persistence"]
 fp.plot(text=True)
 
 # Plot
 fp.plot_mesh()
 # Rotate to make a top view
 fp.plot_mesh(view=(90,0))
 
 # %%
 from findpeaks import findpeaks
-fp = findpeaks(method="topology", denoise=None, params={'window': 3}, limit=None, verbose=0)
+fp = findpeaks(method="topology", limit=None, denoise=None, params={'window': 3}, verbose=0)
 X = fp.import_example("2dpeaks_image")
 # X = fp.import_example("2dpeaks")
 results = fp.fit(X)
 
 fp.plot_persistence()
 
 results["persistence"]
@@ -474,26 +465,26 @@
 methods = ['topology', 'peakdetect', None]
 interpolates = [None, 1, 10, 1000]
 lookaheads =[None, 0, 1, 10, 100]
 
 for method in methods:
     for interpolate in interpolates:
         for lookahead in lookaheads:
-            fp = findpeaks(lookahead=lookahead, interpolate=interpolate, method=method)
+            fp = findpeaks(method=method, lookahead=lookahead, interpolate=interpolate)
             results = fp.fit(X)
             # fp.plot()
             # fp.plot_persistence()
 
 # fp.results['df_interp']
 fp.results['df']
 
 # %%
 from findpeaks import findpeaks
 X = [10,11,9,23,21,11,45,20,11,12]
-fp = findpeaks(lookahead=1, method="topology", verbose=3)
+fp = findpeaks(method="topology", lookahead=1, verbose=3)
 results = fp.fit(X)
 fp.plot()
 fp.plot_persistence()
 
 
 # %% Run over all methods and many parameters
 from findpeaks import findpeaks
@@ -502,25 +493,27 @@
 filters = ['fastnl','bilateral','frost','median','mean', None]
 windows = [3, 9, 15, 31, 63]
 cus = [0.25, 0.5, 0.75]
 verbose=3
 
 for getfilter in filters:
     for window in windows:
-            fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window}, togray=True, imsize=(300,300), verbose=verbose)
+            fp = findpeaks(method='topology', imsize=(300, 300), scale=True, togray=True, denoise=getfilter,
+                           params={'window': window}, verbose=verbose)
             img = fp.import_example('2dpeaks_image')
             results = fp.fit(img)
             title = 'Method=' + str(getfilter) + ', window='+str(window)
             _, ax1 = fp.plot_mesh(wireframe=False, title=title, savepath=savepath+title+'.png')
 
 filters = ['lee','lee_enhanced','kuan']
 for getfilter in filters:
     for window in windows:
         for cu in cus:
-            fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window, 'cu': cu}, togray=True, imsize=(300,300), verbose=verbose)
+            fp = findpeaks(method='topology', imsize=(300, 300), scale=True, togray=True, denoise=getfilter,
+                           params={'window': window, 'cu': cu}, verbose=verbose)
             img = fp.import_example('2dpeaks_image')
             results = fp.fit(img)
             title = 'Method=' + str(getfilter) + ', window='+str(window) + ', cu='+str(cu)
             _, ax1 = fp.plot_mesh(wireframe=False, title=title, savepath=savepath+title+'.png')
 
 
 #%% Plot each seperately
@@ -548,15 +541,15 @@
 fp = findpeaks(method='topology', verbose=3)
 X = fp.import_example('1dpeaks')
 fp.fit(X)
 fp.plot()
 fp.plot_persistence()
 
 from findpeaks import findpeaks
-fp = findpeaks(method='topology',  interpolate=10, verbose=3)
+fp = findpeaks(method='topology', interpolate=10, verbose=3)
 X = fp.import_example('1dpeaks')
 fp.fit(X)
 fp.plot()
 fp.plot_persistence()
 
 
 from tabulate import tabulate
@@ -581,15 +574,16 @@
 fp = findpeaks(method='mask', verbose=3)
 img = fp.import_example()
 fp.fit(img)
 fp.plot()
 
 
 # 2dpeaks example with other settings
-fp = findpeaks(method='topology', scale=True, denoise='fastnl', params={'window': 31}, togray=True, imsize=(300,300), verbose=3)
+fp = findpeaks(method='topology', imsize=(300, 300), scale=True, togray=True, denoise='fastnl', params={'window': 31},
+               verbose=3)
 img = fp.import_example('2dpeaks')
 fp.fit(img)
 fp.plot()
 
 # %%
 from findpeaks import findpeaks
 fp = findpeaks(method='topology')
@@ -687,13 +681,13 @@
 plt.figure(); plt.imshow(image_lee, cmap='gray'); plt.title('Lee')
 plt.figure(); plt.imshow(image_lee_enhanced, cmap='gray'); plt.title('Lee Enhanced')
 plt.figure(); plt.imshow(image_mean, cmap='gray'); plt.title('Mean')
 plt.figure(); plt.imshow(image_median, cmap='gray'); plt.title('Median')
 
 
 from findpeaks import findpeaks
-fp = findpeaks(method='topology', scale=False, denoise='fastnl', togray=True, imsize=False, verbose=3)
+fp = findpeaks(method='topology', imsize=False, scale=False, togray=True, denoise='fastnl', verbose=3)
 fp.fit(img)
 fp.plot_persistence()
 fp.plot_mesh(wireframe=False, title='image_lee_enhanced', view=(30,30))
 
 # %%
```

### Comparing `findpeaks-2.6.2/findpeaks/filters/frost.py` & `findpeaks-2.6.3/findpeaks/filters/frost.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/kuan.py` & `findpeaks-2.6.3/findpeaks/filters/kuan.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/lee.py` & `findpeaks-2.6.3/findpeaks/filters/lee.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/lee_enhanced.py` & `findpeaks-2.6.3/findpeaks/filters/lee_enhanced.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/lee_sigma.py` & `findpeaks-2.6.3/findpeaks/filters/lee_sigma.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/mean.py` & `findpeaks-2.6.3/findpeaks/filters/mean.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/filters/median.py` & `findpeaks-2.6.3/findpeaks/filters/median.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/findpeaks.py` & `findpeaks-2.6.3/findpeaks/findpeaks.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 # import stats as stats
 # from stats import disable_tqdm
 # import interpolate as interpolate
 # #####################
 import findpeaks.stats as stats
 from findpeaks.stats import disable_tqdm
 import findpeaks.interpolate as interpolate
+
+
 # #####################
 
 
 # %%
 class findpeaks():
     """Python library for the detection of peaks and valleys.
 
@@ -39,56 +41,56 @@
     pre-processing by interpolation is possible. Peaks can be detected using various methods, and the results can be
     vizualized, such as the preprocessing steps, the persistence of peaks, the masking plot and a 3d-mesh plot.
 
     Examples
     --------
     >>> from findpeaks import findpeaks
     >>> X = [9,60,377,985,1153,672,501,1068,1110,574,135,23,3,47,252,812,1182,741,263,33]
-    >>> fp = findpeaks(method='peakdetect', interpolate=10, lookahead=1)
+    >>> fp = findpeaks(method='peakdetect',lookahead=1,interpolate=10)
     >>> results = fp.fit(X)
     >>> fp.plot()
     >>>
     >>> # 2D array example
     >>> from findpeaks import findpeaks
     >>> X = fp.import_example('2dpeaks')
     >>> results = fp.fit(X)
     >>> fp.plot()
     >>>
     >>> # Image example
     >>> from findpeaks import findpeaks
-    >>> fp = findpeaks(method='topology', denoise='fastnl', params={'window': 30}, imsize=(300,300))
+    >>> fp = findpeaks(method='topology',imsize=(300,300),denoise='fastnl',params={'window': 30})
     >>> X = fp.import_example('2dpeaks_image')
     >>> results = fp.fit(X)
     >>> fp.plot()
     >>>
     >>> # Plot each seperately
     >>> fp.plot_preprocessing()
     >>> fp.plot_persistence()
     >>> fp.plot_mesh()
 
     References
     ----------
         * https://erdogant.github.io/findpeaks/
 
     """
-
     def __init__(self,
                  method=None,
                  whitelist=['peak', 'valley'],
                  lookahead=200,
                  interpolate=None,
                  limit=None,
                  imsize=None,
                  scale=True,
                  togray=True,
                  denoise='fastnl',
                  window=None,  # DEPRECATED IN LATER VERSIONS: specify in params
                  cu=None,  # DEPRECATED IN LATER VERSIONS: specify in params
                  params_caerus={},  # DEPRECATED IN LATER VERSIONS: use params instead
                  params={'window': 3, 'delta': 0},
+                 # height=None,
                  figsize=(15, 8),
                  verbose=3):
         """Initialize findpeaks parameters.
 
         Parameters
         ----------
         X : array-like (1d-vector or 2d-image)
@@ -153,70 +155,76 @@
         dict()
             See 1dpeaks and 2dpeaks for more details.
 
         Examples
         --------
         >>> from findpeaks import findpeaks
         >>> X = [9,60,377,985,1153,672,501,1068,1110,574,135,23,3,47,252,812,1182,741,263,33]
-        >>> fp = findpeaks(method='peakdetect', interpolate=10, lookahead=1)
+        >>> fp = findpeaks(method='peakdetect',lookahead=1,interpolate=10)
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # 2D array example
         >>> from findpeaks import findpeaks
         >>> X = fp.import_example('2dpeaks')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Image example
         >>> from findpeaks import findpeaks
-        >>> fp = findpeaks(method='topology', denoise='fastnl', params={'window': 30}, imsize=(300,300))
+        >>> fp = findpeaks(method='topology',imsize=(300,300),denoise='fastnl',params={'window': 30})
         >>> X = fp.import_example('2dpeaks_image')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Plot each seperately
         >>> fp.plot_preprocessing()
         >>> fp.plot_persistence()
         >>> fp.plot_mesh()
 
         References
         ----------
             * https://erdogant.github.io/findpeaks/
         """
-        if window is not None: print('The input parameter "window" will be deprecated in future releases. Please use "params={"window": 5}" instead.')
-        if cu is not None: print('The input parameter "cu" will be deprecated in future releases. Please use "params={"cu": 3}" instead.')
+        if window is not None: print(
+            'The input parameter "window" will be deprecated in future releases. Please use "params={"window": 5}" '
+            'instead.')
+        if cu is not None: print(
+            'The input parameter "cu" will be deprecated in future releases. Please use "params={"cu": 3}" instead.')
 
         # Store in object
-        if isinstance(whitelist, str): whitelist=[whitelist]
-        if lookahead is None: lookahead=1
+        if isinstance(whitelist, str): whitelist = [whitelist]
+        if lookahead is None: lookahead = 1
         lookahead = np.maximum(1, lookahead)
-        # if method is None: raise Exception('[findpeaks] >Specify the desired method="topology", "peakdetect", or "mask".')
+        # if method is None: raise Exception('[findpeaks] >Specify the desired method="topology", "peakdetect",
+        # or "mask".')
         self.method = method
         self.whitelist = whitelist
         self.lookahead = lookahead
         self.interpolate = interpolate
         self.limit = limit
         self.imsize = imsize
         self.scale = scale
         self.togray = togray
         self.denoise = denoise
         self.figsize = figsize
         self.verbose = verbose
+        # self.height = height
 
         # Store parameters for caerus
-        defaults={}
-        if method=='caerus':
-            if len(params_caerus)>0:
-                print('The input parameter "params_caerus" will be deprecated in future releases. Please use "params" instead.')
+        defaults = {}
+        if method == 'caerus':
+            if len(params_caerus) > 0:
+                print(
+                    'The input parameter "params_caerus" will be deprecated in future releases. Please use "params" instead.')
                 params = params_caerus
             defaults = {'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}
-        elif method=='lee_sigma':
+        elif method == 'lee_sigma':
             defaults = {'window': 7, 'sigma': 0.9, 'num_looks': 1, 'tk': 5}
-        elif method=='peakdetect':
+        elif method == 'peakdetect':
             defaults = {'delta': 0}
         defaults = {**{'window': 3}, **defaults}
 
         params = {**defaults, **params}
         self.window = params['window']
         self.cu = params.get('cu', 0.25)
         self.params = params
@@ -244,35 +252,36 @@
         """
         # Check datatype
         if isinstance(X, list):
             X = np.array(X)
         if isinstance(X, type(pd.DataFrame())):
             X = X.values
 
-        if len(X.shape)>1:
+        if len(X.shape) > 1:
             # 2d-array (image)
             results = self.peaks2d(X, method=self.method)
         else:
             # 1d-array (vector)
             results = self.peaks1d(X, x=x, method=self.method)
 
         return results
 
     # Find peaks in 1D vector
-    def peaks1d(self, X, x=None, method='peakdetect'):
+    def peaks1d(self, X, x=None, method='peakdetect', height=0):
         """Detect of peaks in 1D array.
 
         Description
         -----------
         This function only eats the input data. Use the .fit() function for more information regarding the input parameters:
             * method : method to be used for peak detection: 'topology' or 'peakdetect'.
             * lookahead : Looking ahead for peaks. For very small 1d arrays (such as up to 50 datapoints), use low numbers: 1 or 2.
             * interpolate : Interpolation factor. The higher the number, the less sharp the edges will be.
             * limit : Values > limit are set as regions of interest (ROI).
             * verbose : Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
+            * height: required height of the peaks.
 
         Parameters
         ----------
         X : array-like 1D vector.
             Input data.
         x : array-like 1D vector.
             Coordinates of the x-axis.
@@ -297,56 +306,62 @@
             * valley  : Whether the point is marked as valley
             * peak    : Whether the point is marked as peak
 
         Examples
         --------
         >>> from findpeaks import findpeaks
         >>> X = [9,60,377,985,1153,672,501,1068,1110,574,135,23,3,47,252,812,1182,741,263,33]
-        >>> fp = findpeaks(method='peakdetect', interpolate=10, lookahead=1)
+        >>> fp = findpeaks(method='peakdetect',lookahead=1,interpolate=10)
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> fp = findpeaks(method='topology')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>> fp.plot_persistence()
 
         """
-        if method is None: method='peakdetect'
+        if method is None: method = 'peakdetect'
         self.method = method
         self.type = 'peaks1d'
-        if self.verbose>=3: print('[findpeaks] >Finding peaks in 1d-vector using [%s] method..' %(self.method))
+        if self.verbose >= 3: print('[findpeaks] >Finding peaks in 1d-vector using [%s] method..' % (self.method))
         # Make numpy array
         X = np.array(X)
         Xraw = X.copy()
         result = {}
 
         # Interpolation
-        if self.interpolate is not None:
+        if self.interpolate is not None and self.interpolate>0:
             X = interpolate.interpolate_line1d(X, n=self.interpolate, method=2, showfig=False, verbose=self.verbose)
 
         # Compute peaks based on method
-        if method=='peakdetect':
+        if method == 'peakdetect':
             # Peakdetect method
+            # max_peaks, min_peaks = peakdetect(X, lookahead=self.lookahead, delta=self.params['delta'], height=self.height)
             max_peaks, min_peaks = peakdetect(X, lookahead=self.lookahead, delta=self.params['delta'])
             # Post processing for the peak-detect
-            result['peakdetect'] = stats._post_processing(X, Xraw, min_peaks, max_peaks, self.interpolate, self.lookahead)
-        elif method=='topology':
+            result['peakdetect'] = stats._post_processing(X, Xraw, min_peaks, max_peaks, self.interpolate,
+                                                          self.lookahead)
+        elif method == 'topology':
             # Compute persistence using toplogy method
             result = stats.topology(np.c_[X, X], limit=self.limit, verbose=self.verbose)
             # Post processing for the topology method
             result['topology'] = stats._post_processing(X, Xraw, result['valley'], result['peak'], self.interpolate, 1)
-        elif method=='caerus':
+        elif method == 'caerus':
             cs = caerus(**self.params)
             result = cs.fit(X, return_as_dict=True, verbose=self.verbose)
             # Post processing for the caerus method
-            result['caerus'] = stats._post_processing(X, Xraw, np.c_[result['loc_start_best'], result['loc_start_best']], np.c_[result['loc_stop_best'], result['loc_stop_best']], self.interpolate, 1, labxRaw=result['df']['labx'].values)
+            result['caerus'] = stats._post_processing(X, Xraw,
+                                                      np.c_[result['loc_start_best'], result['loc_start_best']],
+                                                      np.c_[result['loc_stop_best'], result['loc_stop_best']],
+                                                      self.interpolate, 1, labxRaw=result['df']['labx'].values)
             result['caerus']['model'] = cs
         else:
-            if self.verbose>=2: print('[findpeaks] >WARNING: [method="%s"] is not supported in 1d-vector data. <return>' %(self.method))
+            if self.verbose >= 2: print(
+                '[findpeaks] >WARNING: [method="%s"] is not supported in 1d-vector data. <return>' % (self.method))
             return None
         # Store
         self.results, self.args = self._store1d(X, Xraw, x, result)
         # Return
         return self.results
 
     # Store 1D vector
@@ -356,24 +371,24 @@
         if xs is None: xs = np.arange(0, len(X))
         results = {}
         # Interpolated data
         dfint = pd.DataFrame()
         dfint['x'] = xs
         dfint['y'] = X
         # Store results for method
-        if self.method=='peakdetect':
+        if self.method == 'peakdetect':
             # peakdetect
             dfint['labx'] = result['peakdetect']['labx_s']
             dfint['valley'] = False
             dfint['peak'] = False
             if result['peakdetect']['min_peaks_s'] is not None:
                 dfint['valley'].iloc[result['peakdetect']['min_peaks_s'][:, 0].astype(int)] = True
             if result['peakdetect']['max_peaks_s'] is not None:
                 dfint['peak'].iloc[result['peakdetect']['max_peaks_s'][:, 0].astype(int)] = True
-        elif self.method=='topology':
+        elif self.method == 'topology':
             # Topology
             dfint['labx'] = result['topology']['labx_s']
             dfint['rank'] = result['Xranked']
             dfint['score'] = result['Xdetect']
             dfint['valley'] = False
             dfint['peak'] = False
             if result['topology']['min_peaks_s'] is not None:
@@ -381,15 +396,15 @@
             if result['topology']['max_peaks_s'] is not None:
                 dfint['peak'].iloc[result['topology']['max_peaks_s'][:, 0].astype(int)] = True
 
             results['persistence'] = result['persistence']
             results['Xdetect'] = result['Xdetect']
             results['Xranked'] = result['Xranked']
             results['groups0'] = result['groups0']
-        elif self.method=='caerus':
+        elif self.method == 'caerus':
             # caerus
             dfint = result['df'].copy()
             dfint['y'] = result['X']
             dfint.drop(labels='X', inplace=True, axis=1)
             dfint['x'] = xs
             # dfint['labx'] = result['caerus']['labx_s']
             # dfint['valley'] = False
@@ -400,44 +415,46 @@
             #     dfint['peak'].iloc[result['caerus']['max_peaks_s'][:, 0].astype(int)] = True
 
         # As for the input data
         if self.interpolate is not None:
             df = pd.DataFrame()
             df['y'] = Xraw
             # Store results for method
-            if self.method=='peakdetect':
+            if self.method == 'peakdetect':
                 # peakdetect
                 df['x'] = result['peakdetect']['xs']
                 df['labx'] = result['peakdetect']['labx']
                 df['valley'] = False
                 df['peak'] = False
                 if result['peakdetect']['min_peaks'] is not None:
                     df['valley'].iloc[result['peakdetect']['min_peaks'][:, 0].astype(int)] = True
                 if result['peakdetect']['max_peaks'] is not None:
                     df['peak'].iloc[result['peakdetect']['max_peaks'][:, 0].astype(int)] = True
-            elif self.method=='topology':
+            elif self.method == 'topology':
                 # Topology
                 df['x'] = result['topology']['xs']
                 df['labx'] = result['topology']['labx']
                 df['valley'] = False
                 df['peak'] = False
                 if result['topology']['min_peaks'] is not None:
                     df['valley'].iloc[result['topology']['min_peaks'][:, 0].astype(int)] = True
                 if result['topology']['max_peaks'] is not None:
                     df['peak'].iloc[result['topology']['max_peaks'][:, 0].astype(int)] = True
 
                 # Store the score and ranking
                 df['rank'] = 0
                 df['score'] = 0
 
-                df['rank'].iloc[result['topology']['max_peaks'][:, 0].astype(int)] = dfint['rank'].iloc[result['topology']['max_peaks_s'][:, 0].astype(int)].values
-                df['score'].iloc[result['topology']['max_peaks'][:, 0].astype(int)] = dfint['score'].iloc[result['topology']['max_peaks_s'][:, 0].astype(int)].values
+                df['rank'].iloc[result['topology']['max_peaks'][:, 0].astype(int)] = dfint['rank'].iloc[
+                    result['topology']['max_peaks_s'][:, 0].astype(int)].values
+                df['score'].iloc[result['topology']['max_peaks'][:, 0].astype(int)] = dfint['score'].iloc[
+                    result['topology']['max_peaks_s'][:, 0].astype(int)].values
                 # df['rank'].loc[df['peak']] = dfint['rank'].loc[dfint['peak']].values
                 # df['score'].loc[df['peak']] = dfint['score'].loc[dfint['peak']].values
-            if self.method=='caerus':
+            if self.method == 'caerus':
                 # caerus
                 df['x'] = result['caerus']['xs']
                 df['labx'] = result['df']['labx']
                 df['valley'] = False
                 df['peak'] = False
                 if result['caerus']['min_peaks'] is not None:
                     df['valley'].iloc[result['caerus']['min_peaks'][:, 0].astype(int)] = True
@@ -446,15 +463,15 @@
 
             # Store in results
             results['df'] = df
             results['df_interp'] = dfint
         else:
             results['df'] = dfint
 
-        if self.method=='caerus':
+        if self.method == 'caerus':
             results['model'] = result['caerus']['model']
         # Arguments
         args = {}
         args['method'] = self.method
         args['params'] = self.params
         args['lookahead'] = self.lookahead
         args['interpolate'] = self.interpolate
@@ -515,67 +532,70 @@
         >>> X = fp.import_example('2dpeaks')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Image example
         >>> from findpeaks import findpeaks
         >>> X = fp.import_example('2dpeaks_image')
-        >>> fp = findpeaks(denoise='fastnl', params={'window': 30}, imsize=(300,300))
+        >>> fp = findpeaks(imsize=(300,300),denoise='fastnl',params={'window': 30})
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Plot each seperately
         >>> fp.plot_preprocessing()
         >>> fp.plot_persistence()
         >>> fp.plot_mesh()
 
         """
-        if method is None: method='topology'
+        if method is None: method = 'topology'
         self.method = method
         self.type = 'peaks2d'
-        if self.verbose>=3: print('[findpeaks] >Finding peaks in 2d-array using %s method..' %(self.method))
-        if (not self.togray) and (len(X.shape)==3) and (self.method=='topology'): raise Exception('[findpeaks] >Error: Topology method requires 2d-array. Your input is 3d. Hint: set togray=True.')
+        if self.verbose >= 3: print('[findpeaks] >Finding peaks in 2d-array using %s method..' % (self.method))
+        if (not self.togray) and (len(X.shape) == 3) and (self.method == 'topology'): raise Exception(
+            '[findpeaks] >Error: Topology method requires 2d-array. Your input is 3d. Hint: set togray=True.')
 
         # Preprocessing the image
         Xproc = self.preprocessing(X, showfig=False)
         # Compute peaks based on method
-        if method=='topology':
+        if method == 'topology':
             # Compute persistence based on topology method
             result = stats.topology2d(Xproc, limit=self.limit, whitelist=self.whitelist, verbose=self.verbose)
             # result = stats.topology(Xproc, limit=self.limit, verbose=self.verbose)
-        elif method=='mask':
+        elif method == 'mask':
             # Compute peaks using local maximum filter.
             result = stats.mask(Xproc, limit=self.limit, verbose=self.verbose)
         else:
-            if self.verbose>=2: print('[findpeaks] >WARNING: [method="%s"] is not supported in 2d-array (image) data. <return>' %(self.method))
+            if self.verbose >= 2: print(
+                '[findpeaks] >WARNING: [method="%s"] is not supported in 2d-array (image) data. <return>' % (
+                    self.method))
             return None
 
         # Store
         self.results, self.args = self._store2d(X, Xproc, result)
         # Return
-        if self.verbose>=3: print('[findpeaks] >Fin.')
+        if self.verbose >= 3: print('[findpeaks] >Fin.')
         return self.results
 
     # Store 2D-array
     def _store2d(self, X, Xproc, result):
         # Store results
         results = {}
         results['Xraw'] = X
         results['Xproc'] = Xproc
 
         # Store method specific results
-        if self.method=='topology':
+        if self.method == 'topology':
             # results['topology'] = result
             results['Xdetect'] = result['Xdetect']
             results['Xranked'] = result['Xranked']
             results['persistence'] = result['persistence']
             # results['peak'] = result['peak'] # These values are incorrect when using 2d
             # results['valley'] = result['valley'] # These values are incorrect when using 2d
             results['groups0'] = result['groups0']
-        if self.method=='mask':
+        if self.method == 'mask':
             results['Xdetect'] = result['Xdetect']
             results['Xranked'] = result['Xranked']
 
         # Store arguments
         args = {}
         args['limit'] = self.limit
         args['scale'] = self.scale
@@ -615,35 +635,35 @@
             nplots = 1 + (self.imsize is not None) + self.scale + self.togray + (self.denoise is not None)
             fig, ax = plt.subplots(1, nplots, figsize=self.figsize)
             iax = 0
 
             # Plot RAW input image
             ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
             ax[iax].grid(False)
-            ax[iax].set_title('Input\nRange: [%.3g,%.3g]' %(X.min(), X.max()))
+            ax[iax].set_title('Input\nRange: [%.3g,%.3g]' % (X.min(), X.max()))
             iax = iax + 1
             # plt.show()
 
         # Resize
         if self.imsize:
             X = stats.resize(X, size=self.imsize, verbose=self.verbose)
             if showfig:
                 # plt.figure(figsize=self.figsize)
                 ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
                 ax[iax].grid(False)
-                ax[iax].set_title('Resize\n(%s,%s)' %(self.imsize))
+                ax[iax].set_title('Resize\n(%s,%s)' % (self.imsize))
                 iax = iax + 1
         # Scaling color range between [0,255]
         if self.scale:
             X = stats.scale(X, verbose=self.verbose)
             if showfig:
                 # plt.figure(figsize=self.figsize)
                 ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
                 ax[iax].grid(False)
-                ax[iax].set_title('Scale\nRange: [%.3g %.3g]' %(X.min(), X.max()))
+                ax[iax].set_title('Scale\nRange: [%.3g %.3g]' % (X.min(), X.max()))
                 iax = iax + 1
         # Convert to gray image
         if self.togray:
             X = stats.togray(X, verbose=self.verbose)
             if showfig:
                 # plt.figure(figsize=self.figsize)
                 ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
@@ -674,20 +694,20 @@
         Returns
         -------
         X : Numpy array
 
         """
         cv2 = stats._import_cv2()
         if is_url(path):
-            if verbose>=3: print('[findpeaks] >Downloading from github source: [%s]' %(path))
+            if verbose >= 3: print('[findpeaks] >Downloading from github source: [%s]' % (path))
             response = requests.get(path)
             img_array = np.asarray(bytearray(response.content), dtype=np.uint8)
             X = cv2.imdecode(img_array, cv2.IMREAD_COLOR)
         elif os.path.isfile(path):
-            if verbose>=3: print('[findpeaks] >Import [%s]' %(path))
+            if verbose >= 3: print('[findpeaks] >Import [%s]' % (path))
             X = cv2.imread(path)
         # Return
         return X
 
     # %% Plotting
     def plot(self,
              limit=None,
@@ -723,26 +743,27 @@
 
         Returns
         -------
         fig_axis : tuple containing (fig, ax)
 
         """
         if not hasattr(self, 'results'):
-            if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot. <return>')
+            if self.verbose >= 2: print('[findpeaks] >WARNING: Nothing to plot. <return>')
             return None
 
         figsize = figsize if figsize is not None else self.args['figsize']
 
-        if self.args['type']=='peaks1d':
+        if self.args['type'] == 'peaks1d':
             fig_axis = self.plot1d(legend=legend, figsize=figsize, xlabel=xlabel, ylabel=ylabel)
-        elif self.args['type']=='peaks2d':
+        elif self.args['type'] == 'peaks2d':
             # fig_axis = self.plot2d(figsize=figsize)
-            fig_axis = self.plot_mask(figsize=figsize, cmap=cmap, text=text, limit=limit, s=s, marker=marker, color=color, figure_order=figure_order)
+            fig_axis = self.plot_mask(figsize=figsize, cmap=cmap, text=text, limit=limit, s=s, marker=marker,
+                                      color=color, figure_order=figure_order)
         else:
-            if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot for %s' %(self.args['type']))
+            if self.verbose >= 2: print('[findpeaks] >WARNING: Nothing to plot for %s' % (self.args['type']))
             return None
 
         # Return
         return fig_axis
 
     def plot1d(self, legend=True, figsize=None, xlabel='x-axis', ylabel='y-axis'):
         """Plot the 1D results.
@@ -755,47 +776,51 @@
             (width, height) in inches.
 
         Returns
         -------
         fig_axis : tuple containing axis for each figure.
 
         """
-        if not self.args['type']=='peaks1d':
-            if self.verbose>=3: print('[findpeaks] >Requires results of 1D data <return>.')
+        if not self.args['type'] == 'peaks1d':
+            if self.verbose >= 3: print('[findpeaks] >Requires results of 1D data <return>.')
             return None
 
         figsize = figsize if figsize is not None else self.args['figsize']
         ax1, ax2 = None, None
         title = self.method
 
-        if self.method=='caerus':
+        if self.method == 'caerus':
             if self.results.get('model', None) is not None:
                 ax = self.results['model'].plot(figsize=self.figsize)
                 csplots._plot_graph(self.results['model'].results, figsize=self.figsize, xlabel=xlabel, ylabel=ylabel)
                 # Return axis
                 return ax
         else:
             # Make plot
             min_peaks, max_peaks = np.array([]), np.array([])
             df = self.results['df']
             if np.any('valley' in self.whitelist):
                 min_peaks = df['x'].loc[df['valley']].values
             if np.any('peak' in self.whitelist):
                 max_peaks = df['x'].loc[df['peak']].values
-            ax1 = _plot_original(df['y'].values, df['x'].values, df['labx'].values, min_peaks.astype(int), max_peaks.astype(int), title=title, figsize=figsize, legend=legend, xlabel=xlabel, ylabel=ylabel)
+            ax1 = _plot_original(df['y'].values, df['x'].values, df['labx'].values, min_peaks.astype(int),
+                                 max_peaks.astype(int), title=title, figsize=figsize, legend=legend, xlabel=xlabel,
+                                 ylabel=ylabel)
 
             # Make interpolated plot
             if self.interpolate is not None:
                 min_peaks, max_peaks = np.array([]), np.array([])
                 df_interp = self.results['df_interp']
                 if np.any('valley' in self.whitelist):
                     min_peaks = df_interp['x'].loc[df_interp['valley']].values
                 if np.any('peak' in self.whitelist):
                     max_peaks = df_interp['x'].loc[df_interp['peak']].values
-                ax2 = _plot_original(df_interp['y'].values, df_interp['x'].values, df_interp['labx'].values, min_peaks.astype(int), max_peaks.astype(int), title=title + ' (interpolated)', figsize=figsize, legend=legend, xlabel=xlabel, ylabel=ylabel)
+                ax2 = _plot_original(df_interp['y'].values, df_interp['x'].values, df_interp['labx'].values,
+                                     min_peaks.astype(int), max_peaks.astype(int), title=title + ' (interpolated)',
+                                     figsize=figsize, legend=legend, xlabel=xlabel, ylabel=ylabel)
             # Return axis
             return (ax2, ax1)
 
     def plot2d(self, figsize=None, limit=None, figure_order='vertical'):
         """Plot the 2d results.
 
         Parameters
@@ -804,26 +829,26 @@
             (width, height) in inches.
 
         Returns
         -------
         fig_axis : tuple containing axis for each figure.
 
         """
-        if not self.args['type']=='peaks2d':
-            if self.verbose>=3: print('[findpeaks] >Requires results of 2D data <return>.')
+        if not self.args['type'] == 'peaks2d':
+            if self.verbose >= 3: print('[findpeaks] >Requires results of 2D data <return>.')
             return None
         ax_method, ax_mesh = None, None
         figsize = figsize if figsize is not None else self.args['figsize']
         # Plot preprocessing steps
         self.plot_preprocessing()
 
         # Setup figure
-        if self.method=='mask':
+        if self.method == 'mask':
             ax_method = self.plot_mask(figsize=figsize, limit=limit, figure_order=figure_order)
-        if self.method=='topology':
+        if self.method == 'topology':
             # Plot topology/persistence
             ax_method = self.plot_persistence(figsize=figsize)
 
         # Plot mesh
         ax_mesh = self.plot_mesh(figsize=figsize)
 
         # Return axis
@@ -833,21 +858,23 @@
         """Plot the pre-processing steps.
 
         Returns
         -------
         None.
 
         """
-        if (not hasattr(self, 'results')) or (self.type=='peaks1d'):
-            if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot. Hint: run fit(X), where X is the (image) data. <return>')
+        if (not hasattr(self, 'results')) or (self.type == 'peaks1d'):
+            if self.verbose >= 2: print(
+                '[findpeaks] >WARNING: Nothing to plot. Hint: run fit(X), where X is the (image) data. <return>')
             return None
 
         _ = self.preprocessing(X=self.results['Xraw'], showfig=True)
 
-    def plot_mask(self, limit=None, figsize=None, cmap=None, text=True, s=None, marker='x', color='#FF0000', figure_order='vertical'):
+    def plot_mask(self, limit=None, figsize=None, cmap=None, text=True, s=None, marker='x', color='#FF0000',
+                  figure_order='vertical'):
         """Plot the masking.
 
         Parameters
         ----------
         limit : float, (default : None)
             Values > limit are set as regions of interest (ROI).
         figsize : (int, int), (default: None)
@@ -856,16 +883,17 @@
             Colormap. The default is derived wether image is convert to grey or not. Other options are: plt.cm.hot_r.
 
         Returns
         -------
         fig_axis : tuple containing axis for each figure.
 
         """
-        if (self.type=='peaks1d'):
-            if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot. Hint: run fit(X), where X is the 2d-array (image). <return>')
+        if (self.type == 'peaks1d'):
+            if self.verbose >= 2: print(
+                '[findpeaks] >WARNING: Nothing to plot. Hint: run fit(X), where X is the 2d-array (image). <return>')
             return None
 
         if limit is None: limit = self.limit
         # Only show above the limit
         Xdetect = self.results['Xdetect'].copy()
         if limit is not None:
             Xdetect[np.abs(Xdetect) < limit] = 0
@@ -874,15 +902,15 @@
             cmap = cmap + '_r'
         # Get the index for the detected peaks/valleys
         idx_peaks = np.where(Xdetect > 0)
         idx_valleys = np.where(Xdetect < 0)
 
         # Setup figure
         figsize = figsize if figsize is not None else self.args['figsize']
-        if figure_order=='vertical':
+        if figure_order == 'vertical':
             fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=figsize)
         else:
             fig, (ax1, ax2, ax3) = plt.subplots(1, 3, figsize=figsize)
 
         # Plot input image
         ax1.imshow(self.results['Xraw'], cmap, interpolation="nearest")
         ax1.set_title('Input')
@@ -894,15 +922,16 @@
         Xproc[idx_valleys] = 1
         ax2.imshow(Xproc, cmap, interpolation="nearest")
         ax2.set_title('Processed image')
         ax2.grid(False)
 
         # Masking
         ax3.imshow(np.abs(Xdetect), 'gray_r', interpolation="nearest")
-        ax3.set_title(self.method + ' (' + str(len(np.where(Xdetect > 0)[0])) + ' peaks and ' + str(len(np.where(Xdetect < 0)[0])) + ' valleys)')
+        ax3.set_title(self.method + ' (' + str(len(np.where(Xdetect > 0)[0])) + ' peaks and ' + str(
+            len(np.where(Xdetect < 0)[0])) + ' valleys)')
         ax3.grid(False)
 
         if self.results.get('persistence', None) is not None:
             X = self.results['persistence'].loc[self.results['persistence']['score'] > limit, :]
             for i in range(X.shape[0]):
                 if s is None:
                     X['score'] = stats.normalize(X['score'].values, minscale=2, maxscale=10, scaler='minmax')
@@ -912,15 +941,15 @@
                 ax2.plot(X['x'].iloc[i], X['y'].iloc[i], markersize=X['score'].iloc[i], color=color, marker=marker)
                 ax3.plot(X['x'].iloc[i], X['y'].iloc[i], markersize=X['score'].iloc[i], color=color, marker=marker)
 
             if text:
                 for idx in tqdm(zip(idx_peaks[0], idx_peaks[1]), disable=disable_tqdm(self.verbose)):
                     ax2.text(idx[1], idx[0], 'p' + self.results['Xranked'][idx].astype(str))
                     ax3.text(idx[1], idx[0], 'p' + self.results['Xranked'][idx].astype(str))
-    
+
                 for idx in tqdm(zip(idx_valleys[0], idx_valleys[1]), disable=disable_tqdm(self.verbose)):
                     ax2.text(idx[1], idx[0], 'v' + self.results['Xranked'][idx].astype(str))
                     ax3.text(idx[1], idx[0], 'v' + self.results['Xranked'][idx].astype(str))
 
         # Show plot
         plt.show()
         # Return
@@ -988,15 +1017,15 @@
         
         Example
         -------
         >>> # Import library
         >>> from findpeaks import findpeaks
         >>> #
         >>> # Initialize
-        >>> fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, params={'window': 15})
+        >>> fp = findpeaks(method='topology',imsize=False,scale=False,togray=False,denoise=None,params={'window': 15})
         >>> #
         >>> # Load example data set
         >>> X = fp.import_example('2dpeaks')
         >>> #
         >>> # Fit model
         >>> fp.fit(X)
         >>> #
@@ -1007,40 +1036,41 @@
 
         Returns
         -------
         fig_axis : tuple containing axis for each figure.
 
         """
         if not hasattr(self, 'results'):
-            if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot. Hint: run the fit() function. <return>')
+            if self.verbose >= 2: print('[findpeaks] >WARNING: Nothing to plot. Hint: run the fit() function. <return>')
             return None
         if self.results.get('Xproc', None) is None:
-            if self.verbose>=3: print('[findpeaks] >These analysis do not support mesh plotting. This may be caused because your are analysing 1D.')
+            if self.verbose >= 3: print(
+                '[findpeaks] >These analysis do not support mesh plotting. This may be caused because your are analysing 1D.')
             return None
 
         figsize = figsize if figsize is not None else self.args['figsize']
-        if self.verbose>=3: print('[findpeaks] >Plotting 3d-mesh..')
+        if self.verbose >= 3: print('[findpeaks] >Plotting 3d-mesh..')
         ax1, ax2 = None, None
         if savepath is not None:
             savepath = str.replace(savepath, ',', '_')
             savepath = str.replace(savepath, '=', '_')
 
         # Compute meshgrid
         Z = self.results['Xproc'].copy()
         X, Y = np.mgrid[0:Z.shape[0], 0:Z.shape[1]]
         # To limit on the X and Y axis, we need to create a trick by setting all values to nan in the Z-axis that should be limited.
         if xlim is not None:
-            if xlim[0] is not None: Z[X<xlim[0]]=np.nan
-            if xlim[1] is not None: Z[X>xlim[1]]=np.nan
+            if xlim[0] is not None: Z[X < xlim[0]] = np.nan
+            if xlim[1] is not None: Z[X > xlim[1]] = np.nan
         if ylim is not None:
-            if ylim[0] is not None: Z[Y<ylim[0]]=np.nan
-            if ylim[1] is not None: Z[Y>ylim[1]]=np.nan
+            if ylim[0] is not None: Z[Y < ylim[0]] = np.nan
+            if ylim[1] is not None: Z[Y > ylim[1]] = np.nan
         if zlim is not None:
-            if zlim[0] is not None: Z[Z<zlim[0]]=np.nan
-            if zlim[1] is not None: Z[Z>zlim[1]]=np.nan
+            if zlim[0] is not None: Z[Z < zlim[0]] = np.nan
+            if zlim[1] is not None: Z[Z > zlim[1]] = np.nan
 
         # Plot the figure
         if wireframe:
             fig = plt.figure(figsize=figsize)
             ax1 = fig.add_subplot(projection='3d')
             ax1 = fig.gca()
             ax1.plot_wireframe(X, Y, Z, rstride=rstride, cstride=cstride, linewidth=0.8)
@@ -1053,49 +1083,51 @@
             ax1.set_title(title)
             if xlim is not None: ax1.set_xlim3d(xlim[0], xlim[1])
             if ylim is not None: ax1.set_ylim3d(ylim[0], ylim[1])
             if zlim is not None: ax1.set_zlim3d(zlim[0], zlim[1])
 
             plt.show()
             if savepath is not None:
-                if self.verbose>=3: print('[findpeaks] >Saving wireframe to disk..')
+                if self.verbose >= 3: print('[findpeaks] >Saving wireframe to disk..')
                 fig.savefig(savepath)
 
         if surface:
             # Plot the figure
             fig = plt.figure(figsize=figsize)
             ax2 = fig.add_subplot(projection='3d')
             ax2 = fig.gca()
-            ax2.plot_surface(X, Y, Z, rstride=rstride, cstride=cstride, cmap=cmap, linewidth=0, shade=True, antialiased=False)
+            ax2.plot_surface(X, Y, Z, rstride=rstride, cstride=cstride, cmap=cmap, linewidth=0, shade=True,
+                             antialiased=False)
             if view is not None:
                 ax2.view_init(view[0], view[1])
             ax2.set_xlabel('x-axis')
             ax2.set_ylabel('y-axis')
             ax2.set_zlabel('z-axis')
             ax2.set_title(title)
             if xlim is not None: ax2.set_xlim3d(xlim[0], xlim[1])
             if ylim is not None: ax2.set_ylim3d(ylim[0], ylim[1])
             if zlim is not None: ax2.set_zlim3d(zlim[0], zlim[1])
             plt.show()
             if savepath is not None:
-                if self.verbose>=3: print('[findpeaks] >Saving surface to disk..')
+                if self.verbose >= 3: print('[findpeaks] >Saving surface to disk..')
                 fig.savefig(savepath)
 
         # Plot with contours
         # fig = plt.figure(figsize=figsize)
         # ax3 = fig.gca(projection='3d')
         # X, Y, Z = results['xx'], results['yy'], results['Xproc']
         # ax3.plot_surface(results['xx'], results['yy'], results['Xproc'], rstride=rstride, cstride=cstride, cmap=plt.cm.coolwarm, linewidth=0, shade=True, alpha=0.3)
         # cset = ax3.contour(X, Y, Z, zdir='z', offset=-100, cmap=plt.cm.coolwarm)
         # cset = ax3.contour(X, Y, Z, zdir='x', offset=-40, cmap=plt.cm.coolwarm)
         # cset = ax3.contour(X, Y, Z, zdir='y', offset=40, cmap=plt.cm.coolwarm)
         # plt.show()
         return ax1, ax2
 
-    def plot_persistence(self, figsize=(20, 8), fontsize_ax1=14, fontsize_ax2=14, xlabel='x-axis', ylabel='y-axis', verbose=None):
+    def plot_persistence(self, figsize=(20, 8), fontsize_ax1=14, fontsize_ax2=14, xlabel='x-axis', ylabel='y-axis',
+                         verbose=None):
         """Plot the homology-peristence.
 
         Parameters
         ----------
         figsize : (int, int), (default: None)
             (width, height) in inches.
         fontsize_ax1 : int, (default: 14)
@@ -1109,17 +1141,19 @@
         -------
         ax1 : object
             Figure axis 1.
         ax2 : object
             Figure axis 2.
 
         """
-        if verbose is None: verbose=self.verbose
-        if (self.method!='topology') or (not hasattr(self, 'results')) or len(self.results['persistence']['birth_level'].values)<=0:
-            if verbose>=3: print('[findpeaks] >WARNING: Nothing to plot. Hint: run the .fit(method="topology") function. <return>')
+        if verbose is None: verbose = self.verbose
+        if (self.method != 'topology') or (not hasattr(self, 'results')) or len(
+                self.results['persistence']['birth_level'].values) <= 0:
+            if verbose >= 3: print(
+                '[findpeaks] >WARNING: Nothing to plot. Hint: run the .fit(method="topology") function. <return>')
             return None
 
         # Setup figure
         figsize = figsize if figsize is not None else self.args['figsize']
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
 
         # Create the persistence ax2
@@ -1128,43 +1162,47 @@
         ax1, ax2 = self._plot_persistence_ax1(fontsize_ax1, ax1, ax2, figsize, xlabel, ylabel, verbose)
         # Plot
         plt.show()
         # Return
         return ax1, ax2
 
     def _plot_persistence_ax1(self, fontsize, ax1, ax2, figsize, xlabel, ylabel, verbose):
-        if self.args['type']=='peaks1d':
+        if self.args['type'] == 'peaks1d':
             # Attach the ranking-labels
             if fontsize is not None:
                 y = self.results['df']['y'].values
                 x = self.results['df']['x'].values
-                idx = np.where(self.results['df']['rank']>0)[0]
+                idx = np.where(self.results['df']['rank'] > 0)[0]
                 for i in tqdm(idx, disable=disable_tqdm(verbose)):
-                    ax1.text(x[i], (y[i] + y[i] * 0.01), str(self.results['df']['rank'].iloc[i]), color='b', fontsize=fontsize)
+                    ax1.text(x[i], (y[i] + y[i] * 0.01), str(self.results['df']['rank'].iloc[i]), color='b',
+                             fontsize=fontsize)
 
             # minpers = 0
             min_peaks, max_peaks = np.array([]), np.array([])
             if np.any('valley' in self.whitelist):
                 min_peaks = self.results['df']['x'].loc[self.results['df']['valley']].values
             if np.any('peak' in self.whitelist):
                 max_peaks = self.results['df']['x'].loc[self.results['df']['peak']].values
             # Make the plot
-            ax1 = _plot_original(self.results['df']['y'].values, self.results['df']['x'].values, self.results['df']['labx'].values, min_peaks.astype(int), max_peaks.astype(int), title='Persistence', figsize=figsize, legend=True, ax=ax1, xlabel=xlabel, ylabel=ylabel)
+            ax1 = _plot_original(self.results['df']['y'].values, self.results['df']['x'].values,
+                                 self.results['df']['labx'].values, min_peaks.astype(int), max_peaks.astype(int),
+                                 title='Persistence', figsize=figsize, legend=True, ax=ax1, xlabel=xlabel,
+                                 ylabel=ylabel)
             # Set limits
             X = np.c_[self.results['df']['x'].values, self.results['df']['y'].values]
             ax1.set_xlim((np.min(X), np.max(X)))
             ax1.set_ylim((np.min(X), np.max(X)))
         else:
             # X = self.results['Xproc']
             # Make the figure
             Xdetect = np.zeros_like(self.results['Xproc']).astype(int)
             # fig, ax1 = plt.subplots()
             # minpers = 1
             # Plot the detected loci
-            if verbose>=3: print('[findpeaks] >Plotting loci of birth..')
+            if verbose >= 3: print('[findpeaks] >Plotting loci of birth..')
             ax1.set_title("Loci of births")
             for i, homclass in tqdm(enumerate(self.results['groups0']), disable=disable_tqdm(verbose)):
                 p_birth, bl, pers, p_death = homclass
                 if (self.limit is None):
                     y, x = p_birth
                     Xdetect[y, x] = i + 1
                     ax1.plot([x], [y], '.', c='b')
@@ -1183,16 +1221,16 @@
             # Set the axis to 255-255 in ax2 because it is an image.
             ax2.plot([0, 255], [0, 255], '-', c='grey')
         return ax1, ax2
 
     def _plot_persistence_ax2(self, fontsize, ax2, verbose=3):
         x = self.results['persistence']['birth_level'].values
         y = self.results['persistence']['death_level'].values
-        if len(x)<=0:
-            if verbose>=3: print('[[findpeaks]> Nothing to plot.')
+        if len(x) <= 0:
+            if verbose >= 3: print('[[findpeaks]> Nothing to plot.')
             return None
         ax2.plot(x, y, '.', c='b')
         if fontsize is not None:
             for i in tqdm(range(0, len(x)), disable=disable_tqdm(verbose)):
                 ax2.text(x[i], (y[i] + y[i] * 0.01), str(i + 1), color='b', fontsize=fontsize)
 
         X = np.c_[x, y]
@@ -1230,33 +1268,34 @@
 
         """
         X = import_example(data=data, url=url, sep=sep, verbose=self.verbose, datadir=datadir)
         return X
 
 
 # %%
-def _plot_original(X, xs, labx, min_peaks, max_peaks, title=None, legend=True, ax=None, figsize=(15, 8), xlabel=None, ylabel=None):
+def _plot_original(X, xs, labx, min_peaks, max_peaks, title=None, legend=True, ax=None, figsize=(15, 8), xlabel=None,
+                   ylabel=None):
     uilabx = np.unique(labx)
     uilabx = uilabx[~np.isnan(uilabx)]
 
     if ax is None: fig, ax = plt.subplots(figsize=figsize)
     ax.plot(xs, X, 'k')
     if np.any(max_peaks):
         ax.plot(max_peaks, X[max_peaks], "x", label='Peak')
         # for i in max_peaks:
-            # ax.plot(i, X[i])
+        # ax.plot(i, X[i])
     if np.any(min_peaks):
         ax.plot(min_peaks, X[min_peaks], "o", label='Valley')
         # for i in min_peaks:
-            # ax.plot(i, X[i])
+        # ax.plot(i, X[i])
 
     # Color each detected label
-    s=np.arange(0, len(X))
+    s = np.arange(0, len(X))
     for i in uilabx:
-        idx=(labx==i)
+        idx = (labx == i)
         ax.plot(s[idx], X[idx])
         # plt.plot(s[idx], X[idx], label='peak' + str(i))
 
     if legend: ax.legend(loc=0)
     ax.set_title(title)
     if xlabel is not None: ax.set_xlabel(xlabel)
     if ylabel is not None: ax.set_ylabel(ylabel)
@@ -1290,53 +1329,53 @@
     pd.DataFrame()
         Dataset containing mixed features.
 
     """
     if url is not None:
         fn = os.path.basename(urlparse(url).path).strip()
         if not fn:
-            if verbose>=3: print('[findpeaks] >Could not determine filename to download <return>.')
+            if verbose >= 3: print('[findpeaks] >Could not determine filename to download <return>.')
             return None
         data, _ = os.path.splitext(fn)
-    elif data=='2dpeaks_image' or data=='2dpeaks_image_2':
-        url='https://erdogant.github.io/datasets/' + data + '.png'
+    elif data == '2dpeaks_image' or data == '2dpeaks_image_2':
+        url = 'https://erdogant.github.io/datasets/' + data + '.png'
         fn = data + '.png'
-    elif data=='2dpeaks':
-        url='https://erdogant.github.io/datasets/' + data + '.zip'
+    elif data == '2dpeaks':
+        url = 'https://erdogant.github.io/datasets/' + data + '.zip'
         fn = "2dpeaks.zip"
-    elif data=='1dpeaks':
+    elif data == '1dpeaks':
         # x = [0,   13,  22,  30,  35,  38,   42,   51,   57,   67,  73,   75,  89,   126,  141,  150,  200 ]
         y = [1.5, 0.8, 1.2, 0.2, 0.4, 0.39, 0.42, 0.22, 0.23, 0.1, 0.11, 0.1, 0.14, 0.09, 0.04, 0.02, 0.01]
         # X = np.c_[x, y]
         return y
-    elif (data=='btc') or (data=='facebook'):
+    elif (data == 'btc') or (data == 'facebook'):
         from caerus import caerus
         cs = caerus()
         X = cs.download_example(name=data, verbose=verbose)
         return X
     else:
-        if verbose>=2: print('[findpeaks] >WARNING: Nothing to download. <return>')
+        if verbose >= 2: print('[findpeaks] >WARNING: Nothing to download. <return>')
         return None
 
     if datadir is None: datadir = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     PATH_TO_DATA = os.path.join(datadir, fn)
     if not os.path.isdir(datadir):
         os.makedirs(datadir, exist_ok=True)
 
     # Check file exists.
     if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('[findpeaks] >Downloading from github source: [%s]' %(url))
+        if verbose >= 3: print('[findpeaks] >Downloading from github source: [%s]' % (url))
         r = requests.get(url, stream=True)
         with open(PATH_TO_DATA, "wb") as fd:
             for chunk in r.iter_content(chunk_size=1024):
                 fd.write(chunk)
 
     # Import local dataset
-    if verbose>=3: print('[findpeaks] >Import [%s]' %(PATH_TO_DATA))
-    if data=='2dpeaks_image' or data=='2dpeaks_image_2':
+    if verbose >= 3: print('[findpeaks] >Import [%s]' % (PATH_TO_DATA))
+    if data == '2dpeaks_image' or data == '2dpeaks_image_2':
         cv2 = stats._import_cv2()
         X = cv2.imread(PATH_TO_DATA)
     else:
         X = pd.read_csv(PATH_TO_DATA, sep=sep).values
     # Return
     return X
 
@@ -1347,9 +1386,9 @@
         _ = urlparse(url)
         return True
     except ValueError:
         return False
 
 # %%
 # def disable_tqdm(verbose):
-    # """Set the verbosity messages."""
-    # return  (True if ((verbose==0 or verbose is None) or verbose>3) else False)
+# """Set the verbosity messages."""
+# return  (True if ((verbose==0 or verbose is None) or verbose>3) else False)
```

### Comparing `findpeaks-2.6.2/findpeaks/interpolate.py` & `findpeaks-2.6.3/findpeaks/interpolate.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/stats.py` & `findpeaks-2.6.3/findpeaks/stats.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks/tests/test_findpeaks.py` & `findpeaks-2.6.3/findpeaks/tests/test_findpeaks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from findpeaks import findpeaks
 import numpy as np
 import unittest
 
+
 class TestFINDPEAKS(unittest.TestCase):
 
     def test_fit(self):
         # CHECK OUTPUT METHOD TOPOLOGY
         import numpy as np
-        import matplotlib.pyplot as plt
         from findpeaks import findpeaks
         fp = findpeaks(method="topology", whitelist=['peak'])
         X = fp.import_example('2dpeaks')
         results = fp.fit(X)
-        assert fp.type=='peaks2d'
-        assert [*results.keys()]==['Xraw', 'Xproc', 'Xdetect', 'Xranked', 'persistence', 'groups0']
-        assert [*fp.args]==['limit', 'scale', 'denoise', 'togray', 'imsize', 'figsize', 'type']
-        assert results['Xraw'].shape==results['Xdetect'].shape
-        assert results['Xproc'].shape==results['Xdetect'].shape
+        assert fp.type == 'peaks2d'
+        assert [*results.keys()] == ['Xraw', 'Xproc', 'Xdetect', 'Xranked', 'persistence', 'groups0']
+        assert [*fp.args] == ['limit', 'scale', 'denoise', 'togray', 'imsize', 'figsize', 'type']
+        assert results['Xraw'].shape == results['Xdetect'].shape
+        assert results['Xproc'].shape == results['Xdetect'].shape
 
         fp.plot(figsize=(25, 15), figure_order='horizontal')
 
         # CHECK RESULTS METHOD TOPOLOGY
-        assert len(results['Xdetect'][results['Xdetect']!=0])>18
-        assert len(results['Xranked'][results['Xranked']!=0])>18
+        assert len(results['Xdetect'][results['Xdetect'] != 0]) > 18
+        assert len(results['Xranked'][results['Xranked'] != 0]) > 18
 
         # CHECK RESULTS METHOD with LIMIT functionality
-        fp = findpeaks(method="topology", limit=0, whitelist=['peak'])
+        fp = findpeaks(method="topology", whitelist=['peak'], limit=0)
         X = fp.import_example('2dpeaks')
         results = fp.fit(X)
         fp.plot(figsize=(25, 15), figure_order='horizontal')
-        assert len(results['Xdetect'][results['Xdetect']!=0])>18
-        assert len(results['Xranked'][results['Xranked']!=0])>18
+        assert len(results['Xdetect'][results['Xdetect'] != 0]) > 18
+        assert len(results['Xranked'][results['Xranked'] != 0]) > 18
 
         # CHECK OUTPUT METHOD MASK
         fp = findpeaks(method="mask", verbose=3)
         X = fp.import_example('2dpeaks')
         results = fp.fit(X)
-        assert fp.type=='peaks2d'
-        assert [*results.keys()]==['Xraw', 'Xproc', 'Xdetect','Xranked']
-        assert [*fp.args]==['limit', 'scale', 'denoise', 'togray', 'imsize', 'figsize', 'type']
+        assert fp.type == 'peaks2d'
+        assert [*results.keys()] == ['Xraw', 'Xproc', 'Xdetect', 'Xranked']
+        assert [*fp.args] == ['limit', 'scale', 'denoise', 'togray', 'imsize', 'figsize', 'type']
         fp.plot(figsize=(25, 15), figure_order='horizontal')
-    
+
         # CHECK RESULTS METHOD TOPOLOGY
-        assert np.sum(results['Xdetect'])==20
-        assert results['Xraw'].shape==results['Xdetect'].shape
-        assert results['Xproc'].shape==results['Xdetect'].shape
-    
+        assert np.sum(results['Xdetect']) == 20
+        assert results['Xraw'].shape == results['Xdetect'].shape
+        assert results['Xproc'].shape == results['Xdetect'].shape
+
         # CHECK WHITELIST
         import numpy as np
         from scipy.ndimage import gaussian_filter
         from findpeaks import findpeaks
         rng = np.random.default_rng(42)
         x = rng.normal(size=(50, 50))
         x = gaussian_filter(x, sigma=10.)
@@ -57,141 +57,143 @@
         fp = findpeaks(method="topology", whitelist=['peak', 'valley'], denoise=None, verbose=3)
         results = fp.fit(x)
 
         fp.plot(figsize=(25, 15), figure_order='horizontal')
         fp.plot_persistence()
         fp.plot_mesh()
 
-        Iloc = results['persistence']['score']>1
-        assert results['persistence']['peak'][Iloc].sum()==3
-        assert results['persistence']['valley'][Iloc].sum()==4
+        Iloc = results['persistence']['score'] > 1
+        assert results['persistence']['peak'][Iloc].sum() == 3
+        assert results['persistence']['valley'][Iloc].sum() == 4
 
         # peaks
         fp = findpeaks(method="topology", whitelist='peak', denoise=None, verbose=3)
         fp.plot()
         results = fp.fit(x)
-        Iloc = results['persistence']['score']>1
-        assert results['persistence']['peak'][Iloc].shape[0]==results['persistence']['peak'][Iloc].sum()
+        Iloc = results['persistence']['score'] > 1
+        assert results['persistence']['peak'][Iloc].shape[0] == results['persistence']['peak'][Iloc].sum()
 
         fp = findpeaks(method="topology", whitelist='valley', denoise=None, verbose=3)
         results = fp.fit(x)
-        Iloc = results['persistence']['score']>1
-        assert results['persistence']['valley'].shape[0]==results['persistence']['valley'].sum()
-    
+        Iloc = results['persistence']['score'] > 1
+        assert results['persistence']['valley'].shape[0] == results['persistence']['valley'].sum()
+
         # CHECK OUTPUT METHOD TOPOLOGY
         fp = findpeaks(method="topology")
         X = fp.import_example('1dpeaks')
         results = fp.fit(X)
-        assert fp.type=='peaks1d'
-        assert [*results.keys()]==['persistence', 'Xdetect', 'Xranked', 'groups0', 'df']
-        assert [*fp.args]==['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
-        assert len(X)==len(results['Xdetect'])
-        assert len(X)==len(results['Xranked'])
-        assert len(X)==results['df'].shape[0]
+        assert fp.type == 'peaks1d'
+        assert [*results.keys()] == ['persistence', 'Xdetect', 'Xranked', 'groups0', 'df']
+        assert [*fp.args] == ['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
+        assert len(X) == len(results['Xdetect'])
+        assert len(X) == len(results['Xranked'])
+        assert len(X) == results['df'].shape[0]
         assert np.all(np.isin(results['df'].columns, ['x', 'y', 'labx', 'rank', 'score', 'valley', 'peak']))
         assert np.all(np.isin(results['persistence'].columns, ['x', 'y', 'birth_level', 'death_level', 'score']))
-        
+
         # CHECK RESULTS METHOD TOPOLOGY
-        assert results['persistence'].shape[0]==7
-    
+        # Let op, soms gaat deze ook op 6 vanwege een stochastic components
+        assert results['persistence'].shape[0] == 7
+
         # CHECK RESULTS METHOD with LIMIT functionality
         X = fp.import_example('1dpeaks')
         fp = findpeaks(method="topology", limit=0.02)
         results = fp.fit(X)
-        assert len(results['Xdetect'][results['Xdetect']!=0])==len(results['Xranked'][results['Xranked']!=0])
-    
-        
+        assert len(results['Xdetect'][results['Xdetect'] != 0]) == len(results['Xranked'][results['Xranked'] != 0])
+
         # CHECK OUTPUT METHOD PEAKDETECT
+        # fp = findpeaks(method="peakdetect", lookahead=1, verbose=3, height=0)
         fp = findpeaks(method="peakdetect", lookahead=1, verbose=3)
         X = fp.import_example('1dpeaks')
         results = fp.fit(X)
-        assert fp.type=='peaks1d'
-        assert [*results.keys()]==['df']
-        assert [*fp.args]==['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
-        assert len(X)==results['df'].shape[0]
+        assert fp.type == 'peaks1d'
+        assert [*results.keys()] == ['df']
+        assert [*fp.args] == ['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
+        assert len(X) == results['df'].shape[0]
         assert np.all(np.isin(results['df'].columns, ['x', 'y', 'labx', 'valley', 'peak', 'rank', 'score']))
-        
+
         # CHECK RESULTS METHOD TOPOLOGY
-        assert results['df']['peak'].sum()==2
-        assert results['df']['valley'].sum()==4
-    
+        assert results['df']['peak'].sum() == 2
+        assert results['df']['valley'].sum() == 4
+
         # Run over all combinations and make sure no errors are made
-        X = [10,11,9,23,21,11,45,20,11,12]
+        X = [10, 11, 9, 23, 21, 11, 45, 20, 11, 12]
         methods = ['topology', 'peakdetect', None]
         interpolates = [None, 1, 10, 1000]
-        lookaheads =[None, 0, 1, 10, 100]
+        lookaheads = [None, 0, 1, 10, 100]
         for method in methods:
             for interpolate in interpolates:
                 for lookahead in lookaheads:
-                    fp = findpeaks(lookahead=lookahead, interpolate=interpolate, method=method, verbose=0)
+                    fp = findpeaks(method=method, lookahead=lookahead, interpolate=interpolate, verbose=0)
                     assert fp.fit(X)
-    
-    
+
     def test_denoising(self):
 
         # DENOISING METHODS TEST
         from findpeaks import findpeaks
         fp = findpeaks()
         img = fp.import_example('2dpeaks_image')
         import findpeaks
-        
+
         # filters parameters
         # window size
         winsize = 15
         # damping factor for frost
         k_value1 = 2.0
         # damping factor for lee enhanced
         k_value2 = 1.0
         # coefficient of variation of noise
         cu_value = 0.25
         # coefficient of variation for lee enhanced of noise
         cu_lee_enhanced = 0.523
         # max coefficient of variation for lee enhanced
         cmax_value = 1.73
-        
+
         # Some pre-processing
         # Resize
-        img = findpeaks.stats.resize(img, size=(300,300))
+        img = findpeaks.stats.resize(img, size=(300, 300))
         # Make grey image
         img = findpeaks.stats.togray(img)
         # Scale between [0-255]
         img = findpeaks.stats.scale(img)
-        
+
         # Denoising
         # fastnl
         img_fastnl = findpeaks.stats.denoise(img.copy(), method='fastnl', window=winsize)
         # bilateral
         img_bilateral = findpeaks.stats.denoise(img.copy(), method='bilateral', window=winsize)
         # frost filter
         image_frost = findpeaks.stats.frost_filter(img.copy(), damping_factor=k_value1, win_size=winsize)
         # kuan filter
         image_kuan = findpeaks.stats.kuan_filter(img.copy(), win_size=winsize, cu=cu_value)
         # lee filter
         image_lee = findpeaks.stats.lee_filter(img.copy(), win_size=winsize, cu=cu_value)
         # lee enhanced filter
-        image_lee_enhanced = findpeaks.stats.lee_enhanced_filter(img.copy(), win_size=winsize, k=k_value2, cu=cu_lee_enhanced, cmax=cmax_value)
+        image_lee_enhanced = findpeaks.stats.lee_enhanced_filter(img.copy(), win_size=winsize, k=k_value2,
+                                                                 cu=cu_lee_enhanced, cmax=cmax_value)
         # lee sigma filter
         image_lee_sigma = findpeaks.stats.lee_sigma_filter(img.copy())
         # mean filter
         image_mean = findpeaks.stats.mean_filter(img.copy(), win_size=winsize)
         # median filter
         image_median = findpeaks.stats.median_filter(img.copy(), win_size=winsize)
 
         # Loop throughout many combinations of parameter settings
         from findpeaks import findpeaks
-        methods = ['caerus', 'mask','topology', None]
-        filters = ['lee','lee_enhanced','lee_sigma','kuan','fastnl','bilateral','frost','median','mean', None]
+        methods = ['caerus', 'mask', 'topology', None]
+        filters = ['lee', 'lee_enhanced', 'lee_sigma', 'kuan', 'fastnl', 'bilateral', 'frost', 'median', 'mean', None]
         windows = [None, 3, 63]
         cus = [None, 0, 0.75]
         img = fp.import_example('2dpeaks')
-    
+
         for getfilter in filters:
             for window in windows:
                 for cu in cus:
-                    fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window, 'cu': cu}, togray=True, imsize=None, verbose=3)
+                    fp = findpeaks(method='topology', imsize=None, scale=True, togray=True, denoise=getfilter,
+                                   params={'window': window, 'cu': cu}, verbose=3)
                     assert fp.fit(img)
                     # assert fp.plot_mesh(wireframe=False)
                     # plt.close('all')
                     # assert fp.plot_persistence()
                     # plt.close('all')
                     # assert fp.plot()
                     # plt.close('all')
```

### Comparing `findpeaks-2.6.2/findpeaks/union_find.py` & `findpeaks-2.6.3/findpeaks/union_find.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/findpeaks.egg-info/PKG-INFO` & `findpeaks-2.6.3/findpeaks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.6.2
+Version: 2.6.3
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.6.2.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.6.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy==1.11.4
+Requires-Dist: peakdetect==1.1
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: peakdetect==1.1
 Requires-Dist: requests
 Requires-Dist: caerus>=0.1.9
 Requires-Dist: xarray
 Requires-Dist: joblib
 
 # findpeaks
```

### Comparing `findpeaks-2.6.2/findpeaks.egg-info/SOURCES.txt` & `findpeaks-2.6.3/findpeaks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findpeaks-2.6.2/setup.py` & `findpeaks-2.6.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,24 @@
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['scipy==1.11.4',
+                       'peakdetect==1.1',
                        'matplotlib',
                        'numpy',
                        'pandas',
                        'tqdm',
-                       'peakdetect==1.1',
                        'requests',
                        'caerus>=0.1.9',
                        'xarray',
                        'joblib'],
+     # dependency_links=['https://github.com/arvinnick/peakdetect/tarball/master#egg=peakdetect-1.2'],
      python_requires='>=3',
      name='findpeaks',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).",
      long_description=long_description,
```

