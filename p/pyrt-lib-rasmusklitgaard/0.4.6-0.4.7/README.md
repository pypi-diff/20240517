# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.6.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.6.tar", last modified: Fri May 17 10:14:41 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.7.tar", last modified: Fri May 17 10:46:52 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.6.tar` & `pyrt_lib_rasmusklitgaard-0.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.391729 pyrt_lib_rasmusklitgaard-0.4.6/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.6/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:14:41.387729 pyrt_lib_rasmusklitgaard-0.4.6/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.6/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 10:14:27.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.351729 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11577 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33272 2024-05-17 10:14:31.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 10:14:32.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:14:41.383729 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 10:14:41.000000 pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 10:14:41.391729 pyrt_lib_rasmusklitgaard-0.4.6/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.7/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.7/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 10:46:46.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.063426 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11577 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33505 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.063426 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.6
+Version: 0.4.7
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/README.md` & `pyrt_lib_rasmusklitgaard-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 3% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 		if self.rtdose_letd == None:
 			not_founds += "RTDOSE_LETD "
 		if self.rtdose_dose == None:
 			not_founds += "RTDOSE_DOSE "
 		if not_founds != "":
 			raise ValueError("Could not find {} for patient {} ".format(not_founds, self.patient_id))
 		
-        
+		
 	def dvh_above_let_value(self, let_value, structure, pydicom_rtdose="this", relative_volume=True, dose_is_let = False, delta_dose = 0.1):
 		import time
 		t00 = time.time()
 		if self.rtdose_letd == None:
 			self.rtdose_letd = pd.read_file(self.rtdose_letd)
 		if self.rtdose_dose == None:
 			self.rtdose_dose = pd.read_file(self.rtdose_dose)
@@ -479,25 +479,44 @@
 		if structure not in self.actual_structure_names.values() and structure in self.actual_structure_names.keys():
 			structure_name = self.actual_structure_names[structure].strip()
 		elif structure in self.actual_structure_names.values():
 			structure_name = structure
 		else:
 			raise ValueError("The supplied structure is not found for this patient. You supplied {} and for this patient (patient_ID = {}) the following are valid (both keys and values): {}".format(structure, self.patient_id,self.actual_structure_names))
 
-		if hasattr(self, "{}_indices".format(structure_name)):
-			structure_indices = getattr(self, "{}_indices".format(structure_name))
+		if hasattr(self, "structure_indices"):
+			if structure_name in self.structure_indices:
+			    this_structure_indices = self.structure_indices[structure_name]
+			else:
+				this_structure_indices = self.get_indices_in_structure(structure_name); print("A: Finding {} for {}".format(structure_name, self.patient_id))
+				self.structure_indices[structure_name] = this_structure_indices
 		else:
-			structure_indices = self.get_indices_in_structure(structure_name)
-			setattr(self, "{}_indices".format(structure_name), structure_indices)
-
-		dose_array = self.rtdose_dose.pixel_array * self.rtdose_dose.DoseGridScaling
-		letd_array = self.rtdose_letd.pixel_array * self.rtdose_letd.DoseGridScaling
-		dose_in_structure = dose_array[structure_indices]
-		letd_in_structure = letd_array[structure_indices]
-		letd_above_threshold = letd_in_structure[dose_in_structure > float(dose)]
+			setattr(self, "structure_indices")
+			this_structure_indices = self.get_indices_in_structure(structure_name); print("B: Finding {} for {}".format(structure_name, self.patient_id))
+			self.structure_indices[structure_name] = this_structure_indices
+		
+		if not hasattr(self, "dose_array"):
+			self.dose_array = self.rtdose_dose.pixel_array * self.rtdose_dose.DoseGridScaling
+			
+		if not hasattr(self, "letd_array"):
+			self.letd_array = self.rtdose_letd.pixel_array * self.rtdose_letd.DoseGridScaling
+			
+		if not hasattr(self, "dose_in_structure"):
+			self.dose_in_structure = {structure_name: self.dose_array[this_structure_indices]}
+		else:
+			if not structure_name in self.dose_in_structure:
+				self.dose_in_structure[structure_name] = self.dose_array[this_structure_indices]
+				
+		if not hasattr(self, "letd_in_structure"):
+			self.letd_in_structure = {structure_name:  self.letd_array[this_structure_indices]}
+		else:
+			if not structure_name in self.letd_in_structure:
+				self.letd_in_structure[structure_name] = self.letd_array[this_structure_indices]
+			
+		letd_above_threshold = self.letd_in_structure[structure_name][self.dose_in_structure[structure_name] > float(dose)]
 		if np.prod(letd_above_threshold.shape) == 0:
 			return 0
 		return np.mean(letd_above_threshold)
 	
 	def calculate_dvh_volume(self, structure : str, dvh_parameter : str, percentage=True) -> float:
 		# Volume case
 		# Generalized looks like: V_X_[%,Gy]_Y_[%,kev/um] -- You can omit either dose or LET requirement.
@@ -591,27 +610,17 @@
 
 
 		self.unkelbach_rbe_weighed_dose = rbe_rtdose
 	
 	def set_structure_indices(self): # sets rectum and bladder structures
 		indices = {}
 		for org in self.wanted_structures:
-			if org.lower() not in ["rectum", "bladder wall", "rectum", "rectal wall", "ctv"]:
+			if org.lower() not in ["bladder", "bladder wall", "rectum", "rectal wall", "ctv"]:
 				continue
-			indices[org] = self.get_indices_in_structure(self.actual_structure_names[org])
-		# bladder = self.get_indices_in_structure(self.actual_structure_names["Bladder"])
-		# bladder_wall = self.get_indices_in_structure(self.actual_structure_names["Bladder Wall"])
-		# rectum  = self.get_indices_in_structure(self.actual_structure_names["Rectum"])
-		# rectal_wall  = self.get_indices_in_structure(self.actual_structure_names["Rectal Wall"])
-		# CTV  = self.get_indices_in_structure(self.actual_structure_names["CTV"])
-		# indices[self.actual_structure_names["Bladder"]] = bladder
-		# indices[self.actual_structure_names["Bladder Wall"]] = bladder_wall
-		# indices[self.actual_structure_names["Rectum"]] = rectum
-		# indices[self.actual_structure_names["Rectal Wall"]] = rectal_wall
-		# indices[self.actual_structure_names["CTV"]] = CTV
+			indices[self.actual_structure_names[org]] = self.get_indices_in_structure(self.actual_structure_names[org])
 		self.structure_indices = indices
 
 	def get_indices_in_structure(self, structure):
 		if structure not in self.actual_structure_names.values() and structure in self.actual_structure_names.keys():
 			structure_name = self.actual_structure_names[structure].strip()
 		elif structure in self.actual_structure_names.values():
 			structure_name = structure
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.6
+Version: 0.4.7
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

