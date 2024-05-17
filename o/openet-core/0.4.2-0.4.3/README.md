# Comparing `tmp/openet_core-0.4.2.tar.gz` & `tmp/openet_core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet_core-0.4.2.tar", last modified: Tue May  7 22:41:30 2024, max compression
+gzip compressed data, was "openet_core-0.4.3.tar", last modified: Fri May 17 03:14:21 2024, max compression
```

## Comparing `openet_core-0.4.2.tar` & `openet_core-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.663577 openet_core-0.4.2/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-07 22:41:30.663185 openet_core-0.4.2/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2338 2024-03-23 18:48:00.000000 openet_core-0.4.2/README.rst
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.654460 openet_core-0.4.2/openet/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-09-20 21:11:17.000000 openet_core-0.4.2/openet/__init__.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.657144 openet_core-0.4.2/openet/core/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      324 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/__init__.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3346 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/api.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17694 2024-05-07 20:34:56.000000 openet_core-0.4.2/openet/core/common.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4976 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/ensemble.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    49790 2024-03-12 20:16:00.000000 openet_core-0.4.2/openet/core/interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    12654 2024-05-07 20:43:24.000000 openet_core-0.4.2/openet/core/landsat.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.660153 openet_core-0.4.2/openet/core/tests/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet_core-0.4.2/openet/core/tests/conftest.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8123 2024-03-23 18:43:57.000000 openet_core-0.4.2/openet/core/tests/test_a_utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9351 2024-03-05 04:16:51.000000 openet_core-0.4.2/openet/core/tests/test_b_landsat.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8849 2024-05-07 21:05:23.000000 openet_core-0.4.2/openet/core/tests/test_common.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8271 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/tests/test_ensemble.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    51588 2024-03-11 21:03:23.000000 openet_core-0.4.2/openet/core/tests/test_interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    18851 2024-03-24 05:24:24.000000 openet_core-0.4.2/openet/core/utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)   378148 2023-06-06 21:29:21.000000 openet_core-0.4.2/openet/core/wrs2.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.662726 openet_core-0.4.2/openet_core.egg-info/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      604 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/SOURCES.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/dependency_links.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       56 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/requires.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/top_level.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      995 2024-05-07 20:18:43.000000 openet_core-0.4.2/pyproject.toml
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-05-07 22:41:30.663622 openet_core-0.4.2/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-17 03:14:21.509539 openet_core-0.4.3/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-17 03:14:21.509225 openet_core-0.4.3/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2338 2024-03-23 18:48:00.000000 openet_core-0.4.3/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-17 03:14:21.502023 openet_core-0.4.3/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-09-20 21:11:17.000000 openet_core-0.4.3/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-17 03:14:21.504531 openet_core-0.4.3/openet/core/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      324 2024-03-05 04:16:16.000000 openet_core-0.4.3/openet/core/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3346 2024-03-05 04:16:16.000000 openet_core-0.4.3/openet/core/api.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17694 2024-05-07 20:34:56.000000 openet_core-0.4.3/openet/core/common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4976 2024-03-05 04:16:16.000000 openet_core-0.4.3/openet/core/ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    55900 2024-05-16 23:48:19.000000 openet_core-0.4.3/openet/core/interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    12654 2024-05-07 20:43:24.000000 openet_core-0.4.3/openet/core/landsat.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-17 03:14:21.506760 openet_core-0.4.3/openet/core/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet_core-0.4.3/openet/core/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8123 2024-03-23 18:43:57.000000 openet_core-0.4.3/openet/core/tests/test_a_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9351 2024-03-05 04:16:51.000000 openet_core-0.4.3/openet/core/tests/test_b_landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8849 2024-05-07 21:05:23.000000 openet_core-0.4.3/openet/core/tests/test_common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8271 2024-03-05 04:16:16.000000 openet_core-0.4.3/openet/core/tests/test_ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    54535 2024-05-17 02:13:43.000000 openet_core-0.4.3/openet/core/tests/test_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    18851 2024-03-24 05:24:24.000000 openet_core-0.4.3/openet/core/utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)   378148 2023-06-06 21:29:21.000000 openet_core-0.4.3/openet/core/wrs2.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-17 03:14:21.508787 openet_core-0.4.3/openet_core.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-17 03:14:21.000000 openet_core-0.4.3/openet_core.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      604 2024-05-17 03:14:21.000000 openet_core-0.4.3/openet_core.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-05-17 03:14:21.000000 openet_core-0.4.3/openet_core.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       56 2024-05-17 03:14:21.000000 openet_core-0.4.3/openet_core.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-05-17 03:14:21.000000 openet_core-0.4.3/openet_core.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      995 2024-05-16 23:52:28.000000 openet_core-0.4.3/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-05-17 03:14:21.509584 openet_core-0.4.3/setup.cfg
```

### Comparing `openet_core-0.4.2/PKG-INFO` & `openet_core-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: OpenET Core Components
 Author-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-core
 Keywords: OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openet_core-0.4.2/README.rst` & `openet_core-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/api.py` & `openet_core-0.4.3/openet/core/api.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/common.py` & `openet_core-0.4.3/openet/core/common.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/ensemble.py` & `openet_core-0.4.3/openet/core/ensemble.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/interpolate.py` & `openet_core-0.4.3/openet/core/interpolate.py`

 * *Files 8% similar despite different names*

```diff
@@ -487,15 +487,15 @@
     interp_start_date = interp_start_dt.date().isoformat()
     interp_end_date = interp_end_dt.date().isoformat()
 
     # Get reference ET parameters
     # Supporting reading the parameters from both the interp_args and model_args dictionaries
     # Check interp_args then model_args, and eventually drop support for reading from model_args
     # Assume that if source and band are present, factor and resample should also be read
-    if 'et_reference_source' in interp_args.keys() and 'et_reference_band' in interp_args.keys():
+    if ('et_reference_source' in interp_args.keys()) and ('et_reference_band' in interp_args.keys()):
         et_reference_source = interp_args['et_reference_source']
         et_reference_band = interp_args['et_reference_band']
         if not et_reference_source or not et_reference_band:
             raise ValueError('et_reference_source or et_reference_band were not set')
 
         if 'et_reference_factor' in interp_args.keys():
             et_reference_factor = interp_args['et_reference_factor']
@@ -504,22 +504,22 @@
             logging.debug('et_reference_factor was not set, default to 1.0')
 
         if 'et_reference_resample' in interp_args.keys():
             et_reference_resample = interp_args['et_reference_resample'].lower()
             if not et_reference_resample:
                 et_reference_resample = 'nearest'
                 logging.debug('et_reference_resample was not set, default to nearest')
-            elif et_reference_resample not in ['nearest', 'bilinear', 'bicubic']:
+            elif et_reference_resample not in RESAMPLE_METHODS:
                 raise ValueError(f'unsupported et_reference_resample method: '
                                  f'{et_reference_resample}')
         else:
             et_reference_resample = 'nearest'
             logging.debug('et_reference_resample was not set, default to nearest')
 
-    elif 'et_reference_source' in model_args.keys() and 'et_reference_band' in model_args.keys():
+    elif ('et_reference_source' in model_args.keys()) and ('et_reference_band' in model_args.keys()):
         et_reference_source = model_args['et_reference_source']
         et_reference_band = model_args['et_reference_band']
         if not et_reference_source or not et_reference_band:
             raise ValueError('et_reference_source or et_reference_band were not set')
 
         if 'et_reference_factor' in model_args.keys():
             et_reference_factor = model_args['et_reference_factor']
@@ -528,15 +528,15 @@
             logging.debug('interp_factor was not set, default to 1.0')
 
         if 'et_reference_resample' in model_args.keys():
             et_reference_resample = model_args['et_reference_resample'].lower()
             if not et_reference_resample:
                 et_reference_resample = 'nearest'
                 logging.debug('et_reference_resample was not set, default to nearest')
-            elif et_reference_resample not in ['nearest', 'bilinear', 'bicubic']:
+            elif et_reference_resample not in RESAMPLE_METHODS:
                 raise ValueError(f'unsupported et_reference_resample method: '
                                  f'{et_reference_resample}')
         else:
             et_reference_resample = 'nearest'
             logging.debug('et_reference_resample was not set, default to nearest')
 
     else:
@@ -580,23 +580,67 @@
         interp_vars.append('et_fraction')
 
     # With the current interpolate.daily() function,
     #   something has to be interpolated in order to return et_reference
     if ('et_reference' in variables) and ('et_fraction' not in interp_vars):
         interp_vars.append('et_fraction')
 
-    # The time band is always needed for interpolation
+    # The time band is needed for interpolation
+    # (until interpolate_prep below is added)
     interp_vars.append('time')
 
     # TODO: Look into implementing et_fraction clamping here
     #   (similar to et_actual below)
 
-    # Filter scene collection to the interpolation range
-    # This probably isn't needed since scene_coll was built to this range
-    scene_coll = scene_coll.filterDate(interp_start_date, interp_end_date)
+    # ############
+    # def interpolate_prep(img):
+    #     """Prep WRS2 scene images for interpolation
+    #
+    #     "Unscale" the images using the "scale_factor" property and convert to double.
+    #     Add a mask and time band to each image in the scene_coll since
+    #         interpolator is assuming time and mask bands exist.
+    #     The interpolation could be modified to get the mask from the
+    #         time band instead of setting it here.
+    #     The time image must be the 0 UTC time
+    #
+    #     """
+    #     mask_img = (
+    #         img.select(['et_fraction']).multiply(0).add(1).updateMask(1).uint8()
+    #         .rename('mask')
+    #     )
+    #     time_img = (
+    #         img.select(['et_fraction']).double().multiply(0)
+    #         .add(utils.date_0utc(ee.Date(img.get('system:time_start'))).millis())
+    #         .rename('time')
+    #     )
+    #
+    #     # Set the default scale factor to 1 if the image does not have the property
+    #     scale_factor = (
+    #         ee.Dictionary({'scale_factor': img.get('scale_factor')})
+    #         .combine({'scale_factor': 1.0}, overwrite=False)
+    #     )
+    #
+    #     return (
+    #         img.select(interp_vars)
+    #         .double().multiply(ee.Number(scale_factor.get('scale_factor')))
+    #         .addBands([mask_img, time_img])
+    #         .set({
+    #             'system:time_start': ee.Number(img.get('system:time_start')),
+    #             'image_id': ee.String(img.get('system:index')),
+    #         })
+    #     )
+    #
+    # # Filter scene collection to the interpolation range
+    # #   This probably isn't needed since scene_coll was built to this range
+    # # Then add the time and mask bands needed for interpolation
+    # scene_coll = ee.ImageCollection(
+    #     scene_coll.filterDate(interp_start_date, interp_end_date)
+    #     .map(interpolate_prep)
+    # )
+    # ############
 
     # For count, compute the composite/mosaic image for the mask band only
     if 'count' in variables:
         aggregate_coll = aggregate_to_daily(
             image_coll=scene_coll.select(['mask']),
             start_date=start_date,
             end_date=end_date,
@@ -608,14 +652,22 @@
         # Without this the count image will not be built but the other
         #   bands will be which causes a non-homogeneous image collection.
         aggregate_coll = aggregate_coll.merge(
             ee.Image.constant(0).rename(['mask'])
             .set({'system:time_start': ee.Date(start_date).millis()})
         )
 
+    # import pprint
+    # print('Prep Collection')
+    # pprint.pprint(scene_coll.select(['et_fraction']).getInfo())
+    # pprint.pprint(scene_coll.select(['ndvi']).getInfo())
+    # pprint.pprint(scene_coll.select(['time']).getInfo())
+    # pprint.pprint(scene_coll.select(['mask']).getInfo())
+    # print('DEADBEEF 3')
+
     # Interpolate to a daily time step
     daily_coll = daily(
         target_coll=daily_et_ref_coll,
         source_coll=scene_coll.select(interp_vars),
         interp_method=interp_method,
         interp_days=interp_days,
         use_joins=use_joins,
@@ -688,17 +740,15 @@
         image_list = []
         if 'et' in variables:
             image_list.append(et_img.float())
         if 'et_reference' in variables:
             image_list.append(et_reference_img.float())
         if 'et_fraction' in variables:
             # Compute average et fraction over the aggregation period
-            image_list.append(
-                et_img.divide(et_reference_img).rename(['et_fraction']).float()
-            )
+            image_list.append(et_img.divide(et_reference_img).rename(['et_fraction']).float())
         if 'ndvi' in variables:
             # Compute average NDVI over the aggregation period
             ndvi_img = (
                 daily_coll
                 .filterDate(agg_start_date, agg_end_date)
                 .mean().select(['ndvi']).float()
             )
@@ -920,44 +970,86 @@
     else:
         interp_resample = 'nearest'
         logging.debug('interp_resample was not set, default to nearest')
     if interp_resample and (interp_resample not in RESAMPLE_METHODS):
         raise ValueError(f'unsupported interp_resample: {interp_resample}')
 
     # Get reference ET collection
-    if 'et_reference' in variables or 'et_fraction' in variables:
-        if 'et_reference_source' not in model_args.keys():
-            raise ValueError('et_reference_source was not set')
+    if ('et_reference' in variables) or ('et_fraction' in variables):
 
-        if 'et_reference_band' not in model_args.keys():
-            raise ValueError('et_reference_band was not set')
+        # Supporting reading the parameters from both the interp_args and model_args dictionaries
+        # Check interp_args then model_args, and eventually drop support for reading from model_args
+        # Assume that if source and band are present, factor and resample should also be read
+        if (('et_reference_source' in interp_args.keys()) and
+                ('et_reference_band' in interp_args.keys())):
+            et_reference_source = interp_args['et_reference_source']
+            et_reference_band = interp_args['et_reference_band']
+
+            if 'et_reference_factor' in interp_args.keys():
+                et_reference_factor = interp_args['et_reference_factor']
+            else:
+                et_reference_factor = 1.0
+                logging.debug('et_reference_factor was not set, default to 1.0')
+
+            if 'et_reference_resample' in interp_args.keys():
+                et_reference_resample = interp_args['et_reference_resample'].lower()
+                if not et_reference_resample:
+                    et_reference_resample = 'nearest'
+                    logging.debug('et_reference_resample was not set, default to nearest')
+                elif et_reference_resample not in RESAMPLE_METHODS:
+                    raise ValueError(f'unsupported et_reference_resample method: '
+                                     f'{et_reference_resample}')
+            else:
+                et_reference_resample = 'nearest'
+                logging.debug('et_reference_resample was not set, default to nearest')
 
-        # TODO: Check if model_args can be modified instead of making new variables
-        if 'et_reference_factor' in model_args.keys():
-            et_reference_factor = model_args['et_reference_factor']
-        else:
-            et_reference_factor = 1.0
-            logging.debug('et_reference_factor was not set, default to 1.0')
+            if et_reference_resample and (et_reference_resample not in RESAMPLE_METHODS):
+                raise ValueError(f'unsupported et_reference_resample: {et_reference_resample}')
 
-        if 'et_reference_resample' in model_args.keys():
-            et_reference_resample = model_args['et_reference_resample'].lower()
-        else:
-            et_reference_resample = 'nearest'
-            logging.debug('et_reference_resample was not set, default to nearest')
+        elif (('et_reference_source' in model_args.keys()) and
+                ('et_reference_band' in model_args.keys())):
+            et_reference_source = model_args['et_reference_source']
+            et_reference_band = model_args['et_reference_band']
+
+            if 'et_reference_factor' in model_args.keys():
+                et_reference_factor = model_args['et_reference_factor']
+            else:
+                et_reference_factor = 1.0
+                logging.debug('et_reference_factor was not set, default to 1.0')
+
+            if 'et_reference_resample' in model_args.keys():
+                et_reference_resample = model_args['et_reference_resample'].lower()
+                if not et_reference_resample:
+                    et_reference_resample = 'nearest'
+                    logging.debug('et_reference_resample was not set, default to nearest')
+                elif et_reference_resample not in RESAMPLE_METHODS:
+                    raise ValueError(f'unsupported et_reference_resample method: '
+                                     f'{et_reference_resample}')
+            else:
+                et_reference_resample = 'nearest'
+                logging.debug('et_reference_resample was not set, default to nearest')
 
-        if et_reference_resample and (et_reference_resample not in RESAMPLE_METHODS):
-            raise ValueError(f'unsupported et_reference_resample: {et_reference_resample}')
+            if et_reference_resample and (et_reference_resample not in RESAMPLE_METHODS):
+                raise ValueError(f'unsupported et_reference_resample: {et_reference_resample}')
 
-        # Assume a string source is a single image collection ID
-        #   not a list of collection IDs or ee.ImageCollection
-        daily_et_ref_coll = (
-            ee.ImageCollection(model_args['et_reference_source'])
-            .filterDate(start_date, end_date)
-            .select([model_args['et_reference_band']], ['et_reference'])
-        )
+        else:
+            raise ValueError('et_reference_source or et_reference_band were not set')
+
+        if type(et_reference_source) is str:
+            # Assume a string source is a single image collection ID
+            #   not a list of collection IDs or ee.ImageCollection
+            daily_et_ref_coll = (
+                ee.ImageCollection(et_reference_source)
+                .filterDate(start_date, end_date)
+                .select([et_reference_band], ['et_reference'])
+            )
+        # elif isinstance(et_reference_source, computedobject.ComputedObject):
+        #     # Interpret computed objects as image collections
+        else:
+            raise ValueError(f'unsupported et_reference_source: {et_reference_source}')
 
         # Scale reference ET images (if necessary)
         if et_reference_factor and (et_reference_factor != 1):
             def et_reference_adjust(input_img):
                 return (
                     input_img.multiply(et_reference_factor)
                     .copyProperties(input_img)
@@ -971,14 +1063,55 @@
     #   interpolate.daily()
     daily_target_coll = (
         ee.ImageCollection(interp_args['interp_source'])
         .filterDate(interp_start_date, interp_end_date)
         .select([interp_args['interp_band']])
     )
 
+    # ############
+    # def interpolate_prep(img):
+    #     """Prep WRS2 scene images for interpolation
+    #
+    #     "Unscale" the images using the "scale_factor" property and convert to double.
+    #     Add a mask and time band to each image in the scene_coll since
+    #         interpolator is assuming time and mask bands exist.
+    #     The interpolation could be modified to get the mask from the
+    #         time band instead of setting it here.
+    #     The time image must be the 0 UTC time
+    #
+    #     """
+    #     mask_img = (
+    #         img.select(['et']).multiply(0).add(1).updateMask(1).uint8()
+    #         .rename('mask')
+    #     )
+    #     time_img = (
+    #         img.select(['et']).double().multiply(0)
+    #         .add(utils.date_0utc(ee.Date(img.get('system:time_start'))).millis())
+    #         .rename('time')
+    #     )
+    #
+    #     # Set the default scale factor to 1 if the image does not have the property
+    #     scale_factor = (
+    #         ee.Dictionary({'scale_factor': img.get('scale_factor')})
+    #         .combine({'scale_factor': 1.0}, overwrite=False)
+    #     )
+    #
+    #     return (
+    #         img.select(['et'])
+    #         .double().multiply(ee.Number(scale_factor.get('scale_factor')))
+    #         .addBands([mask_img, time_img])
+    #         .set({
+    #             'system:time_start': ee.Number(img.get('system:time_start')),
+    #             'system:index': ee.String(img.get('system:index')),
+    #         })
+    #     )
+    #
+    # scene_coll = scene_coll.map(interpolate_prep)
+    # ###########
+
     # For count, compute the composite/mosaic image for the mask band only
     if 'count' in variables:
         aggregate_coll = aggregate_to_daily(
             image_coll=scene_coll.select(['mask']),
             start_date=start_date,
             end_date=end_date,
         )
```

### Comparing `openet_core-0.4.2/openet/core/landsat.py` & `openet_core-0.4.3/openet/core/landsat.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/conftest.py` & `openet_core-0.4.3/openet/core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/test_a_utils.py` & `openet_core-0.4.3/openet/core/tests/test_a_utils.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/test_b_landsat.py` & `openet_core-0.4.3/openet/core/tests/test_b_landsat.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/test_common.py` & `openet_core-0.4.3/openet/core/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/test_ensemble.py` & `openet_core-0.4.3/openet/core/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/tests/test_interpolate.py` & `openet_core-0.4.3/openet/core/tests/test_interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,38 +74,53 @@
     img = (
         ee.Image('LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716')
         .select(['SR_B3']).double().multiply(0)
     )
     mask = img.add(1).updateMask(1).uint8()
 
     # The "date" is used for the time band since it needs to be the 0 UTC time
-    # The "time" is advanced to match the typical Landsat overpass time
     date1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).millis())
     date2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).millis())
     date3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).millis())
+
+    # The "time" is advanced to match the typical Landsat overpass time
     time1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).advance(18, 'hours').millis())
     time2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).advance(18, 'hours').millis())
     time3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).advance(18, 'hours').millis())
 
     # TODO: Add code to convert et, et_fraction, and ndvi to lists if they
     #   are set as a single value
 
+    # # Don't add mask or time band to scene collection
+    # # since they are now added in the interpolation calls
+    # scene_coll = ee.ImageCollection.fromImages([
+    #     ee.Image([img.add(etf[0]), img.add(et[0]), img.add(ndvi[0])])
+    #     .rename(['et_fraction', 'et', 'ndvi'])
+    #     .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
+    #     ee.Image([img.add(etf[1]), img.add(et[1]), img.add(ndvi[1])])
+    #     .rename(['et_fraction', 'et', 'ndvi'])
+    #     .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
+    #     ee.Image([img.add(etf[2]), img.add(et[2]), img.add(ndvi[2])])
+    #     .rename(['et_fraction', 'et', 'ndvi'])
+    #     .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
+    # ])
     # Mask and time bands currently get added on to the scene collection
     #   and images are unscaled just before interpolating in the export tool
     scene_coll = ee.ImageCollection.fromImages([
         ee.Image([img.add(etf[0]), img.add(et[0]), img.add(ndvi[0]), img.add(date1), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
+        .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+        .set({'system:index': 'LE07_044033_20170708', 'system:time_start': time1}),
         ee.Image([img.add(etf[1]), img.add(et[1]), img.add(ndvi[1]), img.add(date2), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
+        .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+        .set({'system:index': 'LC08_044033_20170716', 'system:time_start': time2}),
         ee.Image([img.add(etf[2]), img.add(et[2]), img.add(ndvi[2]), img.add(date3), mask])
-            .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
+        .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
+        .set({'system:index': 'LE07_044033_20170724', 'system:time_start': time3}),
     ])
+
     return scene_coll.select(variables)
 
 
 @pytest.mark.parametrize(
     # GRIDMET start times are 7 UTC
     #   1439532000000 - 2015-08-14
     #   1439618400000 - 2015-08-15
@@ -425,26 +440,26 @@
     assert abs(output['etrf'] - expected[0]) <= tol
     assert abs(output['etof'] - expected[1]) <= tol
     assert output['time'] == 0.5 * sum(time_list)
 
 
 def test_aggregate_to_daily_properties():
     """Test daily aggregation image properties"""
-    source_coll = ee.ImageCollection('LANDSAT/LC08/C01/T1_RT_TOA')\
+    source_coll = ee.ImageCollection('LANDSAT/LC08/C02/T1_TOA')\
         .filterDate('2017-06-30', '2017-08-02')\
         .filterBounds(ee.Geometry.Point(-121.9, 39))
     output = utils.get_info(interpolate.aggregate_to_daily(source_coll).first())
     assert set(output['properties'].keys()) == {
         'date', 'system:index', 'system:time_start'}
     assert output['properties']['date'] == '2017-06-30'
 
 
 def test_aggregate_to_daily_date_filtering():
     """Test daily aggregation start/end date filtering"""
-    source_coll = ee.ImageCollection('LANDSAT/LC08/C01/T1_RT_TOA')\
+    source_coll = ee.ImageCollection('LANDSAT/LC08/C02/T1_TOA')\
         .filterDate('2017-01-01', '2018-01-01')\
         .filterBounds(ee.Geometry.Point(-121.9, 39))\
         .select(['B1'])
 
     # First test if both start and end date are set
     output = utils.get_info(interpolate.aggregate_to_daily(
         source_coll, '2017-06-30', '2017-08-02').aggregate_array('date'))
@@ -460,14 +475,15 @@
     output = utils.get_info(interpolate.aggregate_to_daily(
         source_coll, end_date='2017-08-02').aggregate_array('date'))
     assert max(output) < '2017-08-02'
 
 
 def test_from_scene_et_fraction_t_interval_daily_values_interpolated(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi'], ndvi=[0.2, 0.4, 0.6]),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask'], ndvi=[0.2, 0.4, 0.6]),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
@@ -496,14 +512,15 @@
         ['eto', '2017-07-10', 8],
         ['etr', '2017-07-10', 10.5],
     ]
 )
 def test_from_scene_et_fraction_t_interval_daily_values_et_reference(
         et_reference_band, et_reference_date, et_reference, tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi'], ndvi=[0.2, 0.4, 0.6]),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask'], ndvi=[0.2, 0.4, 0.6]),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': et_reference_band,
                     'et_reference_factor': 1.0,
@@ -522,14 +539,15 @@
         ['eto', 236.5],
         ['etr', 310.3],
     ]
 )
 def test_from_scene_et_fraction_t_interval_monthly_values(
         et_reference_band, et_reference, tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi']),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': et_reference_band,
                     'et_reference_factor': 1.0,
@@ -543,14 +561,15 @@
     assert abs(output['et_reference']['2017-07-01'] - et_reference) <= tol
     assert abs(output['et']['2017-07-01'] - (et_reference * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_custom_values(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi']),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'etr',
                     'et_reference_factor': 1.0,
@@ -564,14 +583,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
     assert abs(output['et']['2017-07-01'] - (310.3 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_et_reference_factor(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi']),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'etr',
                     'et_reference_factor': 0.5,
@@ -593,14 +613,15 @@
         ['eto', 236.05609131],
         ['etr', 309.4239807128906],
     ]
 )
 def test_from_scene_et_fraction_t_interval_monthly_et_reference_resample(
         et_reference_band, et_reference, tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi']),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': et_reference_band,
                     'et_reference_factor': 1.0,
@@ -617,14 +638,15 @@
     assert abs(output['et']['2017-07-01'] - (et_reference * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_monthly_interp_args_et_reference(tol=0.0001):
     # Check that the et_reference parameters can be set through the interp_args
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction', 'ndvi']),
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                      'et_reference_band': 'etr',
                      'et_reference_factor': 1.0,
@@ -639,14 +661,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
     assert abs(output['et']['2017-07-01'] - (310.3 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_t_interval_daily_values_eto(tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': 'eto',
                      'interp_resample': 'nearest'},
@@ -665,14 +688,15 @@
     assert abs(output['et']['2017-07-31'] - 5.0) <= tol
     assert '2017-08-01' not in output['et'].keys()
     # assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_t_interval_daily_values_etr(tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': 'etr',
                      'interp_resample': 'nearest'},
@@ -699,14 +723,15 @@
         ['eto', 236.5, 145.9705047607422],
         ['etr', 310.3, 142.9622039794922],
     ]
 )
 def test_from_scene_et_actual_t_interval_monthly_values(
         et_reference_band, et_reference, et, tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': et_reference_band,
                      'interp_resample': 'nearest'},
@@ -723,14 +748,15 @@
     assert abs(output['et_fraction']['2017-07-01'] - et / et_reference) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_t_interval_custom_values_monthly(tol=0.0001):
     # Check that the custom time interval and monthly time interval match
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': 'etr',
                      'interp_resample': 'nearest'},
@@ -746,14 +772,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - 142.9622039794922 / 310.3) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_t_interval_monthly_et_reference_factor(tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': 'etr',
                      'interp_resample': 'nearest'},
@@ -777,14 +804,15 @@
         ['eto', 236.05609131, 145.86253356933594],
         ['etr', 309.4239807128906, 142.99319458007812],
     ]
 )
 def test_from_scene_et_actual_t_interval_monthly_et_reference_resample(
         et_reference_band, et_reference, et, tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': et_reference_band,
                      'interp_resample': 'bilinear'},
@@ -798,16 +826,42 @@
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=30)
     assert abs(output['et']['2017-07-01'] - et) <= tol
     assert abs(output['et_reference']['2017-07-01'] - et_reference) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - et / et_reference) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
+def test_from_scene_et_actual_t_interval_monthly_interp_args_et_reference(tol=0.0001):
+    output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
+        scene_coll(['et', 'time', 'mask']),
+        start_date='2017-07-01', end_date='2017-08-01',
+        variables=['et', 'et_reference', 'et_fraction', 'count'],
+        interp_args={'interp_method': 'linear', 'interp_days': 32,
+                     'interp_source': 'IDAHO_EPSCOR/GRIDMET',
+                     'interp_band': 'etr',
+                     'interp_resample': 'nearest',
+                     'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
+                     'et_reference_band': 'etr',
+                     'et_reference_factor': 1.0,
+                     'et_reference_resample': 'nearest'},
+        model_args={},
+        t_interval='monthly')
+
+    TEST_POINT = (-121.5265, 38.7399)
+    output = utils.point_coll_value(output_coll, TEST_POINT, scale=30)
+    assert abs(output['et']['2017-07-01'] - 142.9622039794922) <= tol
+    assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
+    assert abs(output['et_fraction']['2017-07-01'] - 142.9622039794922 / 310.3) <= tol
+    assert output['count']['2017-07-01'] == 3
+
+
 def test_from_scene_et_actual_t_interval_daily_et_fraction_max(tol=0.0001):
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et'], et=[100, 100, 100]),
         scene_coll(['et', 'time', 'mask'], et=[100, 100, 100]),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                      'interp_band': 'etr',
                      'interp_resample': 'nearest',
@@ -826,42 +880,45 @@
     assert abs(output['et_fraction']['2017-07-10'] - 1.4) <= tol
 
 
 def test_from_scene_et_fraction_t_interval_bad_value():
     # Function should raise a ValueError if t_interval is not supported
     with pytest.raises(ValueError):
         interpolate.from_scene_et_fraction(
+            # scene_coll(['et']),
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01', variables=['et'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
                         'et_reference_resample': 'nearest'},
             t_interval='deadbeef')
 
 
 def test_from_scene_et_fraction_t_interval_no_value():
     # Function should raise an Exception if t_interval is not set
     with pytest.raises(TypeError):
         interpolate.from_scene_et_fraction(
+            # scene_coll(['et']),
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01',
             variables=['et', 'et_reference', 'et_fraction', 'count'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
                         'et_reference_resample': 'nearest'})
 
 
 def test_from_scene_et_actual_t_interval_bad_value():
     # Function should raise a ValueError if t_interval is not supported
     with pytest.raises(ValueError):
         interpolate.from_scene_et_actual(
+            # scene_coll(['et']),
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01', variables=['et'],
             interp_args={'interp_method': 'linear', 'interp_days': 32,
                          'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                          'interp_band': 'etr', 'interp_resample': 'nearest'},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
@@ -870,14 +927,15 @@
             t_interval='deadbeef')
 
 
 def test_from_scene_et_actual_t_interval_no_value():
     # Function should raise an Exception if t_interval is not set
     with pytest.raises(TypeError):
         interpolate.from_scene_et_actual(
+            # scene_coll(['et']),
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01', variables=['et'],
             interp_args={'interp_method': 'linear', 'interp_days': 32,
                          'interp_source': 'IDAHO_EPSCOR/GRIDMET',
                          'interp_band': 'etr',
                          'interp_resample': 'nearest'},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
@@ -885,14 +943,15 @@
                         'et_reference_factor': 1.0,
                         'et_reference_resample': 'nearest'})
 
 
 def test_from_scene_et_fraction_interp_args_use_joins_true(tol=0.01):
     # Check that the use_joins interp_args parameter works
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction']),
         scene_coll(['et_fraction', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32, 'use_joins': True},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'etr',
                     'et_reference_factor': 1.0,
@@ -905,14 +964,15 @@
     assert abs(output['et']['2017-07-01'] - (310.3 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_interp_args_use_joins_false(tol=0.01):
     # Check that the use_joins interp_args parameter works
     output_coll = interpolate.from_scene_et_fraction(
+        # scene_coll(['et_fraction']),
         scene_coll(['et_fraction', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32, 'use_joins': False},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'etr',
                     'et_reference_factor': 1.0,
@@ -925,14 +985,15 @@
     assert abs(output['et']['2017-07-01'] - (310.3 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_interp_args_use_joins_true(tol=0.01):
     # Check that the use_joins interp_args parameter works
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET', 'interp_band': 'etr',
                      'use_joins': True},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
@@ -947,14 +1008,15 @@
     assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_actual_interp_args_use_joins_false(tol=0.01):
     # Check that the use_joins interp_args parameter works
     output_coll = interpolate.from_scene_et_actual(
+        # scene_coll(['et']),
         scene_coll(['et', 'time', 'mask']),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32,
                      'interp_source': 'IDAHO_EPSCOR/GRIDMET', 'interp_band': 'etr',
                      'use_joins': True},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
@@ -966,35 +1028,38 @@
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=30)
     assert abs(output['et']['2017-07-01'] - 142.9622039794922) <= tol
     assert abs(output['et_reference']['2017-07-01'] - 310.3) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
-
 """
 These tests were attempts at making "full" interpolation calls.
 They could be removed but are being left in case we want to explore this again
 at some point in the future.
 """
 # def test_daily_values_collection_a():
 #     """Test the daily interpolation using real images"""
-#     target_coll = ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')\
-#         .filterDate('2017-06-30', '2017-08-02')\
+#     target_coll = (
+#         ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')
+#         .filterDate('2017-06-30', '2017-08-02')
 #         .select(['etr'])
-#     source_coll = ee.ImageCollection('LANDSAT/LC08/C01/T1_RT_TOA')\
-#         .filterDate('2017-06-30', '2017-08-02')\
-#         .filterBounds(ee.Geometry.Point(-121.9, 39))\
-#         .select(['B1'])
+#     )
+#     source_coll = (
+#         ee.ImageCollection('LANDSAT/LC08/C02/T1_L2')
+#         .filterDate('2017-06-30', '2017-08-02')
+#         .filterBounds(ee.Geometry.Point(-121.9, 39))
+#         .select(['SR_B2'])
+#     )
 #
 #     def add_time_band(image):
 #         date_0utc = utils.date_0utc(ee.Date(image.get('system:time_start')))
 #         return image.addBands([
-#             image.select([0]).double().multiply(0).add(date_0utc.millis())\
-#                 .rename(['time'])])
+#             image.select([0]).double().multiply(0).add(date_0utc.millis()).rename(['time'])
+#         ])
 #     source_coll = ee.ImageCollection(source_coll.map(add_time_band))
 #
 #     # print('\nTARGET')
 #     # target_info = utils.point_coll_value(
 #     #     target_coll, xy=(-121.5265, 38.7399), scale=30)
 #     # pprint.pprint(target_info)
 #
@@ -1003,34 +1068,38 @@
 #         source_coll, xy=(-121.5265, 38.7399), scale=30)
 #     pprint.pprint(source_info)
 #
 #     print('\nOUTPUT')
 #     output = utils.point_coll_value(
 #         interpolate.daily(target_coll, source_coll, interp_days=32),
 #         xy=(-121.5265, 38.7399), scale=30)
-#     pprint.pprint(output['B1'])
+#     pprint.pprint(output['SR_B2'])
 #
 #     assert True
 #
 #
 # def test_daily_values_collection_b():
 #     """Test the daily interpolation for short interp_days values"""
-#     target_coll = ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')\
-#         .filterDate('2017-06-30', '2017-08-02')\
+#     target_coll = (
+#         ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')
+#         .filterDate('2017-06-30', '2017-08-02')
 #         .select(['etr'])
-#     source_coll = ee.ImageCollection('LANDSAT/LC08/C01/T1_RT_TOA')\
-#         .filterDate('2017-06-30', '2017-08-02')\
-#         .filterBounds(ee.Geometry.Point(-121.9, 39))\
-#         .select(['B1'])
+#     )
+#     source_coll = (
+#         ee.ImageCollection('LANDSAT/LC08/C02/T1_L2')
+#         .filterDate('2017-06-30', '2017-08-02')
+#         .filterBounds(ee.Geometry.Point(-121.9, 39))
+#         .select(['SR_B2'])
+#     )
 #
 #     def add_time_band(image):
 #         date_0utc = utils.date_0utc(ee.Date(image.get('system:time_start')))
 #         return image.addBands([
-#             image.select([0]).double().multiply(0).add(date_0utc.millis())\
-#                 .rename(['time'])])
+#             image.select([0]).double().multiply(0).add(date_0utc.millis()).rename(['time'])
+#         ])
 #     source_coll = ee.ImageCollection(source_coll.map(add_time_band))
 #
 #     # print('\nTARGET')
 #     # target_info = utils.point_coll_value(
 #     #     target_coll, xy=(-121.5265, 38.7399), scale=30)
 #     # pprint.pprint(target_info)
 #
@@ -1039,34 +1108,38 @@
 #         source_coll, xy=(-121.5265, 38.7399), scale=30)
 #     pprint.pprint(source_info)
 #
 #     print('\nOUTPUT')
 #     output = utils.point_coll_value(
 #         interpolate.daily(target_coll, source_coll, interp_days=4),
 #         xy=(-121.5265, 38.7399), scale=30)
-#     pprint.pprint(output['B1'])
+#     pprint.pprint(output['SR_B2'])
 #
 #     assert True
 #
 #
 # def test_daily_values_collection_c():
 #     """Test if the daily interpolation holds the last known value"""
-#     target_coll = ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')\
-#         .filterDate('2017-07-01', '2017-08-05')\
+#     target_coll = (
+#         ee.ImageCollection('IDAHO_EPSCOR/GRIDMET')
+#         .filterDate('2017-07-01', '2017-08-05')
 #         .select(['etr'])
-#     source_coll = ee.ImageCollection('LANDSAT/LC08/C01/T1_RT_TOA')\
-#         .filterDate('2017-06-30', '2017-07-17')\
-#         .filterBounds(ee.Geometry.Point(-121.9, 39))\
-#         .select(['B1'])
+#     )
+#     source_coll = (
+#         ee.ImageCollection('LANDSAT/LC08/C02/T1_L2')
+#         .filterDate('2017-06-30', '2017-07-17')
+#         .filterBounds(ee.Geometry.Point(-121.9, 39))
+#         .select(['SR_B2'])
+#     )
 #
 #     def add_time_band(image):
 #         date_0utc = utils.date_0utc(ee.Date(image.get('system:time_start')))
 #         return image.addBands([
-#             image.select([0]).double().multiply(0).add(date_0utc.millis())\
-#                 .rename(['time'])])
+#             image.select([0]).double().multiply(0).add(date_0utc.millis()).rename(['time'])
+#         ])
 #     source_coll = ee.ImageCollection(source_coll.map(add_time_band))
 #
 #     # print('\nTARGET')
 #     # target_info = utils.point_coll_value(
 #     #     target_coll, xy=(-121.5265, 38.7399), scale=30)
 #     # pprint.pprint(target_info)
 #
@@ -1075,10 +1148,10 @@
 #         source_coll, xy=(-121.5265, 38.7399), scale=30)
 #     pprint.pprint(source_info)
 #
 #     print('\nOUTPUT')
 #     output = utils.point_coll_value(
 #         interpolate.daily(target_coll, source_coll, interp_days=16),
 #         xy=(-121.5265, 38.7399), scale=30)
-#     pprint.pprint(output['B1'])
+#     pprint.pprint(output['SR_B2'])
 #
 #     assert True
```

### Comparing `openet_core-0.4.2/openet/core/utils.py` & `openet_core-0.4.3/openet/core/utils.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet/core/wrs2.py` & `openet_core-0.4.3/openet/core/wrs2.py`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/openet_core.egg-info/PKG-INFO` & `openet_core-0.4.3/openet_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: OpenET Core Components
 Author-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-core
 Keywords: OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openet_core-0.4.2/openet_core.egg-info/SOURCES.txt` & `openet_core-0.4.3/openet_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openet_core-0.4.2/pyproject.toml` & `openet_core-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openet-core"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
     { name="Charles Morton", email="charles.morton@dri.edu" },
 ]
 description = "OpenET Core Components"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["OpenET", "Earth Engine", "Evapotranspiration", "Landsat"]
```

