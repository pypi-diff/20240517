# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.7.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.7.tar", last modified: Fri May 17 10:46:52 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.8.tar", last modified: Fri May 17 11:34:12 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.7.tar` & `pyrt_lib_rasmusklitgaard-0.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.7/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.7/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 10:46:46.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.063426 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11577 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33505 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 10:46:49.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 10:46:52.063426 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 10:46:52.000000 pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 10:46:52.067426 pyrt_lib_rasmusklitgaard-0.4.7/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.8/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.8/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-17 11:34:04.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.110088 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11650 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    33769 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-17 11:34:07.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-17 11:34:12.000000 pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-17 11:34:12.114088 pyrt_lib_rasmusklitgaard-0.4.8/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.7
+Version: 0.4.8
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/README.md` & `pyrt_lib_rasmusklitgaard-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.7"
+version = "0.4.8"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 	code.InteractiveConsole(vars).interact()	
 
 def printStructures(structure):
 	print("There are the following structures available in your RTSTRUCT:")
 	for i, name in enumerate([a.ROIName for a in structure.StructureSetROISequence]):
 		print("{0:2}: {1}".format(i,name))
 
-def selectStructures(structure, selections, ctvfallback=None):
+def selectStructures(structure, selections, ctvfallback=None, prompt_if_not_found = True):
 	"""
 		This function takes an RTSTRUCT and a list of wanted structure names
 		It then tries to find them automagically based on their names,
 		but if unable it will prompt the user for help.
 		If one is not available the user can enter this
 		and the function will return with the ones found.
 		The function returns a list of strings corresponding to the structurenames.
@@ -190,14 +190,17 @@
 					break
 			if sel_indx != -1:
 				return_list[sel_indx] = name
 				
 	if "NOT_FOUND_YET" not in return_list:
 		return return_list
 	
+	if not prompt_if_not_found:
+		return None
+	
 	missing_indices = []
 	for i, struct in enumerate(return_list):
 		if struct == "NOT_FOUND_YET":
 			missing_indices.append(i)
 	
 	missing_structs = [selections[i] for i in missing_indices]
 	printStructures(structure)
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,27 @@
 		self.structures_with_gamma_passes	= self.get_structures_with_gamma_passes()
 		t4=time.time()
 		self.dict_of_gamma_passes			= self.get_gamma_pass_dict()
 		self.all_dvhs_by_model				= self.get_all_dvhs_by_model()
 		self.all_dvhs_by_structure			= self.get_all_dvhs_by_structure()
 		self.patient_id						= self.get_patient_id()
 		self.metadata						= self.collect_metadata(xlsx_workbook)
+		if self.metadata == {}:
+			return None
 
 		t5=time.time()
 		self.set_default_rtdoses()
 		t6=time.time()
 
 		try:
 			if self.wanted_structures == "default":
 				self.wanted_structures = ["ctv", "bladder", "bladder wall", "rectum", "rectal wall", "Bladder Wall", "Rectal Wall", "Rectum", "Bladder", "CTV", "Rectal_Wall", "Bladder_Wall"]
 			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures , *args, **kwargs)
+			if self.actual_structure_names == None:
+				raise ValueError("No structures names set for patient {}".format(self.patient_id))
 		except AttributeError as e:
 			print("Attribute error for patient when setting structures: {}".format(self.patient_id))
 			print(str(e))
 		t7=time.time()
 
 		self.set_structure_indices()
 		t8=time.time()
@@ -342,24 +346,28 @@
 				for line in f:
 					key = line.split(":")[0]
 					val = line.split(":")[-1].replace("\n","")
 					actual_structurenames_dict[key] = val
 			for wanted_struct in wanted_structures: 
 				if wanted_struct not in list(actual_structurenames_dict.keys()):
 					act_struct = selectStructures(self.rtstruct, [wanted_struct], *args, **kwargs)[0]
+					if act_struct == None:
+						return None
 					actual_structurenames_dict[wanted_struct] = act_struct
 					with open(actual_structurenames_file, "a") as f:
 						f.write("{}:{}\n".format(wanted_struct, act_struct))
 			add_these = list(actual_structurenames_dict.values())
 			for value in add_these:
 				actual_structurenames_dict[value] = value
 			return actual_structurenames_dict
 
 
 		actual_structures = selectStructures(self.rtstruct, wanted_structures, *args, **kwargs)
+		if actual_structures == None:
+			return None
 		writepath = ""
 		writepath = writepath + self.patient_folder_path
 		if not self.patient_folder_path[-1] == "/":
 			writepath = writepath + "/"
 		writepath = writepath + "actual_structure_names.txt"
 		with open(writepath, "w") as f:
 			for key, value in zip(wanted_structures, actual_structures):
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.7
+Version: 0.4.8
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.7/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.8/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

