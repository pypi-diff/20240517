# Comparing `tmp/lime-stable-1.0.3.tar.gz` & `tmp/lime-stable-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-1.0.3.tar", last modified: Thu May  9 05:19:31 2024, max compression
+gzip compressed data, was "lime-stable-1.0.4.tar", last modified: Fri May 17 20:31:12 2024, max compression
```

## Comparing `lime-stable-1.0.3.tar` & `lime-stable-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.146333 lime-stable-1.0.3/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.3/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.3/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-09 05:19:31.146333 lime-stable-1.0.3/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.3/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-09 05:18:45.000000 lime-stable-1.0.3/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-09 05:19:31.146333 lime-stable-1.0.3/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.3/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.142333 lime-stable-1.0.3/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.142333 lime-stable-1.0.3/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.3/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-01 21:07:04.000000 lime-stable-1.0.3/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.3/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.3/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.3/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.3/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    82241 2024-05-06 01:21:46.000000 lime-stable-1.0.3/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.3/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    33847 2024-05-08 16:58:08.000000 lime-stable-1.0.3/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.3/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.142333 lime-stable-1.0.3/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.3/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.3/src/lime/resources/parent_bands_BackUp.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.3/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.3/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-05-04 18:53:12.000000 lime-stable-1.0.3/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.3/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.3/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.146333 lime-stable-1.0.3/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-09 05:19:31.000000 lime-stable-1.0.3/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-09 05:19:31.000000 lime-stable-1.0.3/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-09 05:19:31.000000 lime-stable-1.0.3/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-09 05:19:31.000000 lime-stable-1.0.3/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-09 05:19:31.000000 lime-stable-1.0.3/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:19:31.146333 lime-stable-1.0.3/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.3/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.3/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.3/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.3/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.3/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.3/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.3/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.3/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.3/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.4/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.4/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-17 20:31:12.112697 lime-stable-1.0.4/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.4/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-17 20:01:34.000000 lime-stable-1.0.4/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-17 20:31:12.112697 lime-stable-1.0.4/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.4/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.108698 lime-stable-1.0.4/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.4/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-17 20:01:34.000000 lime-stable-1.0.4/src/lime/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.4/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.4/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.4/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.4/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82245 2024-05-17 14:34:08.000000 lime-stable-1.0.4/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70645 2024-05-17 20:14:58.000000 lime-stable-1.0.4/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    33794 2024-05-17 19:51:29.000000 lime-stable-1.0.4/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.4/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.4/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.4/src/lime/resources/parent_bands_BackUp.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.4/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.4/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    34917 2024-05-17 14:54:27.000000 lime-stable-1.0.4/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.4/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.4/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.4/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.4/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.4/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.4/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.4/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7374 2024-05-17 19:54:25.000000 lime-stable-1.0.4/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.4/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.4/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.4/tests/test_tools.py
```

### Comparing `lime-stable-1.0.3/LICENSE.rst` & `lime-stable-1.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/PKG-INFO` & `lime-stable-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.3
+Version: 1.0.4
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.3/README.rst` & `lime-stable-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/pyproject.toml` & `lime-stable-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lime-stable"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
 dependencies = ["asdf~=3.0",
```

### Comparing `lime-stable-1.0.3/setup.py` & `lime-stable-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/__init__.py` & `lime-stable-1.0.4/src/lime/__init__.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/config.toml` & `lime-stable-1.0.4/src/lime/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'lime-stable'
-version = '1.0.0'
+version = '1.0.4'
 
 [colors] #Default theme
 default.bg = '#FFFFFF'
 default.fg = '#000000'
 default.cont_band = '#8c564b'
 default.line_band = '#b5bd61'
 default.color_cycle = ['#279e68', '#d62728', '#aa40fc', '#8c564b',  '#e377c2', '#7f7f7f',
```

### Comparing `lime-stable-1.0.3/src/lime/io.py` & `lime-stable-1.0.4/src/lime/io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/logo.py` & `lime-stable-1.0.4/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/model.py` & `lime-stable-1.0.4/src/lime/model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/observations.py` & `lime-stable-1.0.4/src/lime/observations.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/plots.py` & `lime-stable-1.0.4/src/lime/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
 
 
 def spatial_mask_plot(ax, masks_dict, mask_color, mask_alpha, units_flux, mask_list=[]):
 
     # Container for the legends
     legend_list = [None] * len(masks_dict)
 
-    cmap_contours = cm.get_cmap(mask_color, len(masks_dict))
+    cmap_contours = plt.get_cmap(mask_color, len(masks_dict))
 
     for idx_mask, items in enumerate(masks_dict.items()):
 
         mask_name, hdu_mask = items
         mask_data, mask_header = hdu_mask
 
         if (len(mask_list) == 0) or (mask_name in mask_list):
@@ -522,15 +522,15 @@
 
         # If only one component or combined
         if n_comps == 1:
             width_i, style, color = theme.colors['single_width'], '-', theme.colors['profile']
 
         # Component
         else:
-            cmap = cm.get_cmap(theme.colors['comps_map'])
+            cmap = plt.get_cmap(theme.colors['comps_map'])
             width_i, style, color = theme.colors['comp_width'], ':', cmap(idx_line/n_comps)
 
     # Case where the line has an error
     else:
         width_i, style, color = theme.colors['err_width'], '-', theme.colors['error']
 
     # Plot the profile
@@ -546,15 +546,15 @@
 
         # If only one component or combined
         if n_comps == 1:
             width_i, style, color = theme.colors['single_width'], '-', theme.colors['profile']
 
         # Component
         else:
-            cmap = cm.get_cmap(theme.colors['comps_map'])
+            cmap = plt.get_cmap(theme.colors['comps_map'])
             width_i, style, color = theme.colors['comp_width'], ':', cmap(idx_line/n_comps)
 
     # Case where the line has an error
     else:
         width_i, style, color = theme.colors['err_width'], '-', 'red'
 
     # Make dictionary with the params
@@ -1025,15 +1025,15 @@
 
                 if detec_obj.confidence is not None:
 
                     # Boundaries array for confidence intervals
                     bounds = np.array([0.0, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
 
                     # Adjust color map to match lower detection limit to fg color
-                    cmap = cm.get_cmap(theme.colors['mask_map'])
+                    cmap = plt.get_cmap(theme.colors['mask_map'])
                     cmaplist = [cmap(i) for i in range(cmap.N)]
                     cmaplist[0] = theme.colors['fg']
                     cmap = colors.LinearSegmentedColormap.from_list('mcm', cmaplist, bounds.size-1)
                     norm = colors.BoundaryNorm(bounds * 100, cmap.N)
 
                     # Iterate through the confidence intervals and plot the step spectrum
                     for i in range(1, len(bounds)):
```

### Comparing `lime-stable-1.0.3/src/lime/plots_interactive.py` & `lime-stable-1.0.4/src/lime/plots_interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
                 # Create sliders grid
                 n_sliders = 1 if self._redshift_log_path is None else 2
                 gs_slicers = gs0[1].subgridspec(1, n_sliders)
                 ax_sliders = gs_slicers.subplots().flatten() if n_sliders > 1 else [gs_slicers.subplots()]
 
                 # Mask sweep slider configuration
                 self._inter_mask = np.median(np.diff(self._spec.wave_rest))
-                mask_slider = Slider(ax_sliders[0], 'Band\n(pixels)', -10, 10, 0, valstep=1)
+                mask_slider = Slider(ax_sliders[0], 'Band\n(pixels)', -10, 10, valinit=0.0, valstep=1)
                 mask_slider.on_changed(self._on_mask_slider_MI)
 
                 # Redshift sweep slider configuration
                 if self._redshift_log_path is not None:
                     if self._obj_ref is None:
                         raise LiMe_Error(f'No object reference was provided for the redshift log.')
 
@@ -354,15 +354,15 @@
 
                     # Add the current value
                     self.z_df.loc[self._obj_ref, self._redshift_column] = self._spec.redshift
                     save_frame(self._redshift_log_path, self.z_df)
 
                     self._z_orig = self._spec.redshift
                     self._inter_z = np.abs(self._spec.redshift - (self._spec.wave/(self._spec.wave_rest + self._inter_mask) - 1).mean())
-                    z_slider = Slider(ax_sliders[1], 'Redshift\n($\Delta z$)', -10, 10, 0, valstep=1)
+                    z_slider = Slider(ax_sliders[1], 'Redshift\n($\Delta z$)', -10, 10, valinit=0, valstep=1)
                     z_slider.on_changed(self._on_z_slider_MI)
 
                 # Connecting the figure to the interactive widgets
                 self._fig.canvas.mpl_connect('button_press_event', self._on_click_MI)
                 self._fig.canvas.mpl_connect('axes_enter_event', self._on_enter_axes_MI)
 
                 # Show the image
```

### Comparing `lime-stable-1.0.3/src/lime/read_fits.py` & `lime-stable-1.0.4/src/lime/read_fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,25 +620,22 @@
 
         # Get data table and header dict lists
         data_list, header_list = load_fits(fits_address, data_ext_list, hdr_ext_list, url_check=False)
 
         # Re-construct spectrum arrays
         wave_array = data_list[0]
         flux_cube = data_list[1]
-        ivar_cube = data_list[1]
+        ivar_cube = data_list[2]
 
         # Convert ivar = 0 to nan
         ivar_cube[ivar_cube == 0] = np.nan
 
         # Get standard deviation cube
         err_cube = np.sqrt(1 / ivar_cube)
 
-        # Pixel mask
-        pixel_mask_cube = None
-
         # WCS from hearder
         wcs = WCS(header_list[0])
 
         # Fits properties
         fits_params = {**CUBE_FITS_PARAMS['manga'], 'wcs': wcs}
 
         return wave_array, flux_cube, err_cube, header_list, fits_params
```

### Comparing `lime-stable-1.0.3/src/lime/recognition.py` & `lime-stable-1.0.4/src/lime/recognition.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/resources/parent_bands.txt` & `lime-stable-1.0.4/src/lime/resources/parent_bands.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/resources/parent_bands_BackUp.txt` & `lime-stable-1.0.4/src/lime/resources/parent_bands_BackUp.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/resources/types_params.txt` & `lime-stable-1.0.4/src/lime/resources/types_params.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/tables.py` & `lime-stable-1.0.4/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/tools.py` & `lime-stable-1.0.4/src/lime/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
             if numer == denom:  # Same line normalization
                 idcs_slice = log.index.get_level_values(sample_levels[-1]) == numer
                 df_slice = log.loc[idcs_slice]
             else:  # Rest cases
                 idcs_slice = log.index.get_level_values(sample_levels[-1]).isin([numer, denom])
                 grouper = log.index.droplevel('line')
-                idcs_slice = pd.Series(idcs_slice).groupby(grouper).transform('sum').ge(2).array
+                idcs_slice = pd.Series(idcs_slice).groupby(grouper).transform('sum').ge(2).to_numpy()
                 df_slice = log.loc[idcs_slice]
 
             # Get fluxes
             if df_slice.size > 0:
                 num_slice = df_slice.xs(numer, level=sample_levels[-1], drop_level=False)
                 numer_flux = num_slice[flux_column].to_numpy()
                 numer_err = num_slice[f'{flux_column}_err'].to_numpy()
```

### Comparing `lime-stable-1.0.3/src/lime/transitions.py` & `lime-stable-1.0.4/src/lime/transitions.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime/workflow.py` & `lime-stable-1.0.4/src/lime/workflow.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-1.0.4/src/lime_stable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.3
+Version: 1.0.4
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.3/src/lime_stable.egg-info/SOURCES.txt` & `lime-stable-1.0.4/src/lime_stable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_astro.py` & `lime-stable-1.0.4/tests/test_astro.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_cube.py` & `lime-stable-1.0.4/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_io.py` & `lime-stable-1.0.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_line.py` & `lime-stable-1.0.4/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_model.py` & `lime-stable-1.0.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_sample.py` & `lime-stable-1.0.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_spectrum.py` & `lime-stable-1.0.4/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.3/tests/test_tools.py` & `lime-stable-1.0.4/tests/test_tools.py`

 * *Files identical despite different names*

