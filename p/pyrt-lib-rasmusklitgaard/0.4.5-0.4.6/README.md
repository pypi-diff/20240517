# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.5.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.5.tar", last modified: Wed May 15 08:42:03 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.6.tar", last modified: Fri May 17 10:14:41 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.5.tar` & `pyrt_lib_rasmusklitgaard-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-15 08:42:03.263191 pyrt_lib_rasmusklitgaard-0.4.5/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.5/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-15 08:42:03.263191 pyrt_lib_rasmusklitgaard-0.4.5/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.5/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-15 08:41:56.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-15 08:42:03.263191 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11580 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32703 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-15 08:42:01.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-15 08:42:03.263191 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-15 08:42:03.000000 pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-15 08:42:03.263191 pyrt_lib_rasmusklitgaard-0.4.5/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.391729 pyrt_lib_rasmusklitgaard-0.4.6/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.6/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:14:41.387729 pyrt_lib_rasmusklitgaard-0.4.6/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.6/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 10:14:27.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.351729 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11577 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33272 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.383729 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 10:14:41.391729 pyrt_lib_rasmusklitgaard-0.4.6/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.5
+Version: 0.4.6
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/README.md` & `pyrt_lib_rasmusklitgaard-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 import subprocess
 import os
 import tempfile
 import string
 
 
 def calculate_vh(data_array, stepsize=0.1, nsteps = None):
-    data_array = np.array(data_array)
-    full_volume = np.prod(np.shape(data_array))
+	data_array = np.array(data_array)
+	full_volume = np.prod(np.shape(data_array))
 
-    value_array = np.array([0,0])
-    if stepsize != 0:
-        value_array = np.arange(0, np.max(data_array), stepsize)
-
-    if nsteps:
-        value_array = np.linspace(0, np.max(data_array), nsteps)
-    if len(value_array) == 1:
-        value_array = np.append(value_array, stepsize)
-    volume_array = np.zeros_like(value_array)
-    for i,v in enumerate(value_array):
-        sub_volume = np.prod(np.shape(data_array[data_array>v]))
-        volume_array[i] = sub_volume
-    return (value_array, volume_array / full_volume)
+	value_array = np.array([0,0])
+	if stepsize != 0:
+		value_array = np.arange(0, np.max(data_array), stepsize)
+
+	if nsteps:
+		value_array = np.linspace(0, np.max(data_array), nsteps)
+	if len(value_array) == 1:
+		value_array = np.append(value_array, stepsize)
+	volume_array = np.zeros_like(value_array)
+	for i,v in enumerate(value_array):
+		sub_volume = np.prod(np.shape(data_array[data_array>v]))
+		volume_array[i] = sub_volume
+	return (value_array, volume_array / full_volume)
 
 def get_patient_metadata(patient_data_sheet, patient_id):
 	this_patient_row = -1
 	# now we need to find the row with this patient id
 	for row_i in range(1,1500):
 		if str(patient_data_sheet["A{}".format(row_i)].value) == patient_id:
 			this_patient_row = row_i
@@ -104,19 +104,19 @@
 	x = np.linspace(x0+dx/2,x0+nx*dx-dx/2,nx)
 	y = np.linspace(y0+dy/2,y0+ny*dy-dy/2,ny)
 	z = np.linspace(z0,z0+(nz-1)*dz,nz)
 	newgrid = np.array(np.meshgrid(x,y,z,indexing="ij")).T
 	return newgrid
 
 def is_tool(name):
-    """Check whether `name` is on PATH and marked as executable."""
+	"""Check whether `name` is on PATH and marked as executable."""
 
-    # from whichcraft import which
+	# from whichcraft import which
 
-    return which(name) is not None
+	return which(name) is not None
 
 def find_struct_indices_in_rtdose(rtstruct: pd.Dataset, rtdose: pd.Dataset, structure_name: str):
 
 	# Currently has an error!!!
 	# Should be swapped for a better implementation which doesn't overestimate the volume of structures.
 
 	struct_contourXyz = getROIContourSequenceXyz(rtstruct,ROIName2Number(rtstruct, structure_name))
@@ -147,25 +147,32 @@
 		This function takes an RTSTRUCT and a list of wanted structure names
 		It then tries to find them automagically based on their names,
 		but if unable it will prompt the user for help.
 		If one is not available the user can enter this
 		and the function will return with the ones found.
 		The function returns a list of strings corresponding to the structurenames.
 	"""
+	
 	iii = -1
 	for i, el in enumerate(selections):
 		if el == "body":
 			iii = i
 			break
 	if not iii == -1:
 		del selections[iii]
 
 	return_list = ["NOT_FOUND_YET"] * len(selections)
 	# first we try to find the correct structures. Then only ask for what we need.
-	listOfStructures = [a.ROIName for a in structure.StructureSetROISequence]
+	
+	try:
+		listOfStructures = [a.ROIName for a in structure.StructureSetROISequence]
+	except AttributeError as e:
+		print(e)
+		exit()
+		
 	for j,sel in enumerate(selections):			
 		if sel.lower() in [l.lower() for l in listOfStructures] \
 		or sel.lower() in [l.lower().replace("_"," ") for l in listOfStructures] \
 		or sel.lower().replace("_"," ") in [l.lower() for l in listOfStructures]:
 			sel_indx = -1
 			for i, name in enumerate(listOfStructures):
 				if sel.lower() == name.lower() or sel.lower().replace("_"," ") == name.lower():
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 		except AttributeError as e:
 			print("Attribute error for patient when setting structures: {}".format(self.patient_id))
 			print(str(e))
 		t7=time.time()
 
 		self.set_structure_indices()
 		t8=time.time()
+		
 
 
 	def get_dvh_param(self, structure, model, key) -> float:
 		# in this case, model could also be "let" and is in that case in units 
 		# of kev/um and describes dose averaged let
 
 		# perhaps if patient is missing this specific DVH, we could try to create one 
@@ -373,14 +374,25 @@
 				continue
 			if path.split("/")[-1][:7] == "FLK_Bio":
 				self.rtdose_dose= pd.read_file(path)
 				self.path_to_rtdose_dose = path
 			if path.split("/")[-1][:8] == "RTSTRUCT":
 				self.rtstruct= pd.read_file(path)
 				self.path_to_rtstruct = path
+		not_founds = ""
+		if self.rtstruct == None:
+			not_founds += "RTSTRUCT "
+		if self.rtdose_letd == None:
+			not_founds += "RTDOSE_LETD "
+		if self.rtdose_dose == None:
+			not_founds += "RTDOSE_DOSE "
+		if not_founds != "":
+			raise ValueError("Could not find {} for patient {} ".format(not_founds, self.patient_id))
+		
+        
 	def dvh_above_let_value(self, let_value, structure, pydicom_rtdose="this", relative_volume=True, dose_is_let = False, delta_dose = 0.1):
 		import time
 		t00 = time.time()
 		if self.rtdose_letd == None:
 			self.rtdose_letd = pd.read_file(self.rtdose_letd)
 		if self.rtdose_dose == None:
 			self.rtdose_dose = pd.read_file(self.rtdose_dose)
@@ -578,24 +590,28 @@
 		rbe_rtdose.PixelData = rbe_weighed_dose.astype(np.uint16).tobytes()
 
 
 		self.unkelbach_rbe_weighed_dose = rbe_rtdose
 	
 	def set_structure_indices(self): # sets rectum and bladder structures
 		indices = {}
-		bladder = self.get_indices_in_structure(self.actual_structure_names["Bladder"])
-		bladder_wall = self.get_indices_in_structure(self.actual_structure_names["Bladder Wall"])
-		rectum  = self.get_indices_in_structure(self.actual_structure_names["Rectum"])
-		rectal_wall  = self.get_indices_in_structure(self.actual_structure_names["Rectal Wall"])
-		CTV  = self.get_indices_in_structure(self.actual_structure_names["CTV"])
-		indices[self.actual_structure_names["Bladder"]] = bladder
-		indices[self.actual_structure_names["Bladder Wall"]] = bladder_wall
-		indices[self.actual_structure_names["Rectum"]] = rectum
-		indices[self.actual_structure_names["Rectal Wall"]] = rectal_wall
-		indices[self.actual_structure_names["CTV"]] = CTV
+		for org in self.wanted_structures:
+			if org.lower() not in ["rectum", "bladder wall", "rectum", "rectal wall", "ctv"]:
+				continue
+			indices[org] = self.get_indices_in_structure(self.actual_structure_names[org])
+		# bladder = self.get_indices_in_structure(self.actual_structure_names["Bladder"])
+		# bladder_wall = self.get_indices_in_structure(self.actual_structure_names["Bladder Wall"])
+		# rectum  = self.get_indices_in_structure(self.actual_structure_names["Rectum"])
+		# rectal_wall  = self.get_indices_in_structure(self.actual_structure_names["Rectal Wall"])
+		# CTV  = self.get_indices_in_structure(self.actual_structure_names["CTV"])
+		# indices[self.actual_structure_names["Bladder"]] = bladder
+		# indices[self.actual_structure_names["Bladder Wall"]] = bladder_wall
+		# indices[self.actual_structure_names["Rectum"]] = rectum
+		# indices[self.actual_structure_names["Rectal Wall"]] = rectal_wall
+		# indices[self.actual_structure_names["CTV"]] = CTV
 		self.structure_indices = indices
 
 	def get_indices_in_structure(self, structure):
 		if structure not in self.actual_structure_names.values() and structure in self.actual_structure_names.keys():
 			structure_name = self.actual_structure_names[structure].strip()
 		elif structure in self.actual_structure_names.values():
 			structure_name = structure
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.5
+Version: 0.4.6
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.5/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

