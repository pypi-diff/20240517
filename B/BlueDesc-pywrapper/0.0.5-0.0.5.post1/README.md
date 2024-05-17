# Comparing `tmp/bluedesc_pywrapper-0.0.5.tar.gz` & `tmp/bluedesc_pywrapper-0.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluedesc_pywrapper-0.0.5.tar", last modified: Fri May 10 17:09:54 2024, max compression
+gzip compressed data, was "bluedesc_pywrapper-0.0.5.post1.tar", last modified: Fri May 17 19:36:08 2024, max compression
```

## Comparing `bluedesc_pywrapper-0.0.5.tar` & `bluedesc_pywrapper-0.0.5.post1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/
--rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3566 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2217 2023-08-11 12:16:36.000000 bluedesc_pywrapper-0.0.5/README.md
--rw-rw-rw-   0        0        0     1361 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.244195 bluedesc_pywrapper-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.244195 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/
--rw-rw-rw-   0        0        0      142 2024-05-10 17:09:07.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    10509 2024-05-09 19:50:00.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
--rw-rw-rw-   0        0        0    36313 2023-07-14 12:26:42.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/descs.json
--rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/dtypes.json
--rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.266806 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3566 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.266806 bluedesc_pywrapper-0.0.5/tests/
--rw-rw-rw-   0        0        0     2021 2023-07-14 13:08:16.000000 bluedesc_pywrapper-0.0.5/tests/test_descriptors.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:08.669275 bluedesc_pywrapper-0.0.5.post1/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5.post1/LICENSE
+-rw-rw-rw-   0        0        0     3572 2024-05-17 19:36:08.669275 bluedesc_pywrapper-0.0.5.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2217 2023-08-11 12:16:36.000000 bluedesc_pywrapper-0.0.5.post1/README.md
+-rw-rw-rw-   0        0        0     1361 2024-05-17 19:36:08.669275 bluedesc_pywrapper-0.0.5.post1/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:08.621976 bluedesc_pywrapper-0.0.5.post1/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:08.637610 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/
+-rw-rw-rw-   0        0        0      148 2024-05-17 19:34:27.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    10470 2024-05-17 19:35:17.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
+-rw-rw-rw-   0        0        0    36313 2023-07-14 12:26:42.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/descs.json
+-rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/dtypes.json
+-rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:08.653641 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3572 2024-05-17 19:36:08.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2024-05-17 19:36:08.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:36:08.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2024-05-17 19:36:08.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-17 19:36:08.000000 bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:08.653641 bluedesc_pywrapper-0.0.5.post1/tests/
+-rw-rw-rw-   0        0        0     2021 2023-07-14 13:08:16.000000 bluedesc_pywrapper-0.0.5.post1/tests/test_descriptors.py
```

### Comparing `bluedesc_pywrapper-0.0.5/LICENSE` & `bluedesc_pywrapper-0.0.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/PKG-INFO` & `bluedesc_pywrapper-0.0.5.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc_pywrapper
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `bluedesc_pywrapper-0.0.5/README.md` & `bluedesc_pywrapper-0.0.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/setup.cfg` & `bluedesc_pywrapper-0.0.5.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/bluedesc_pywrapper.py` & `bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,18 @@
         self.include_3D = not ignore_3D
         # Ensure the jar file exists
         if not os.path.isfile(self._jarfile):
             raise IOError('The required BlueDesc JAR file is not present. Reinstall BlueDesc.')
 
     def calculate(self, mols: Iterable[Chem.Mol], show_banner: bool = True, njobs: int = 1,
                   chunksize: Optional[int] = 1000) -> pd.DataFrame:
-        """Calculate molecular fingerprints.
+        """Calculate molecular descriptors.
 
-        :param mols: RDKit molecules for which fingerprints should be calculated
-        :param show_banner: If True, show notice on fingerprint usage
+        :param mols: RDKit molecules for which descriptors should be calculated
+        :param show_banner: If True, show notice on descriptor usage
         :param njobs: number of concurrent processes
         :param chunksize: number of molecules to be processed by a process; ignored if njobs is 1
         :return: a pandas DataFrame containing all BlueDesc descriptor values
         """
         if show_banner:
             self._show_banner()
         if njobs < 0:
@@ -115,15 +115,14 @@
                     if needsHs(mol):
                         warnings.warn('Molecule lacks hydrogen atoms: this might affect the value of calculated descriptors')
                     # Are molecules 3D
                     if self.include_3D:
                         confs = list(mol.GetConformers())
                         if not (len(confs) > 0 and confs[-1].Is3D()):
                             raise ValueError('Cannot calculate the 3D descriptors of a conformer-less molecule')
-                    mol.SetProp('index', str(i))
                     writer.write(mol)
                 else:
                     self._skipped.append(i)
                 self.n += 1
             writer.close()
             del block
         except ValueError as e:
@@ -155,22 +154,22 @@
             try:
                 values = arff.loadarff(self._out)
                 values = (pd.DataFrame(values[0])
                           .drop("?", axis=1)
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.count.', ''))
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.', ''))
                           )
-                if values.shape[0] != (self.n - self._skipped):
+                if values.shape[0] != (self.n - len(self._skipped)):
                     # Create an empty array
-                    values_ = pd.DataFrame(np.zeros(((self.n - self._skipped), values.shape[1])),
+                    values_ = pd.DataFrame(np.zeros(((self.n - len(self._skipped)), values.shape[1])),
                                            columns=values.columns)
                     # Identify skipped molecules
                     start = process.stdout.find('Sequence of skipped instances:')
                     skipped = pd.Series(process.stdout[start + 30:].split()).astype(int) - 1
-                    for i in range((self.n - self._skipped)):
+                    for i in range((self.n - len(self._skipped))):
                         if i in skipped.tolist():
                             values_.iloc[i, :] = np.NaN
                         else:
                             values_.iloc[i, :] = values.iloc[0, :]
                             values = values.iloc[1:, :]
                     values = values_
             except Exception as e:
@@ -214,15 +213,15 @@
                           .apply(pd.to_numeric, errors='ignore', downcast='float', axis=0)
                    )
         return results
 
     def _multiproc_calculate(self, mols: List[Chem.Mol], nbits: int = 1024) -> pd.DataFrame:
         """Calculate BlueDesc descriptors in thread-safe manner.
 
-        :param mols: RDKit molecules for which BlueDesc fingerprints should be calculated
+        :param mols: RDKit molecules for which BlueDesc descriptors should be calculated
         :return: a pandas DataFrame containing all BlueDesc desciptor values
         """
         # Copy self instance to make thread safe
         bluedesc = deepcopy(self)
         # Run copy
         result = bluedesc.calculate(mols, show_banner=False, njobs=1)
         return result
```

### Comparing `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/descs.json` & `bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/descs.json`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/dtypes.json` & `bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/dtypes.json`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/utils.py` & `bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/PKG-INFO` & `bluedesc_pywrapper-0.0.5.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc_pywrapper
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `bluedesc_pywrapper-0.0.5/tests/test_descriptors.py` & `bluedesc_pywrapper-0.0.5.post1/tests/test_descriptors.py`

 * *Files identical despite different names*

