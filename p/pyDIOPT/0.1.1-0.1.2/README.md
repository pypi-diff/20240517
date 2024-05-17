# Comparing `tmp/pydiopt-0.1.1.tar.gz` & `tmp/pydiopt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiopt-0.1.1.tar", last modified: Wed May 15 09:27:24 2024, max compression
+gzip compressed data, was "pydiopt-0.1.2.tar", last modified: Fri May 17 04:11:13 2024, max compression
```

## Comparing `pydiopt-0.1.1.tar` & `pydiopt-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:27:24.775798 pydiopt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-15 09:27:16.000000 pydiopt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 09:27:24.775798 pydiopt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 09:27:16.000000 pydiopt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:27:24.771798 pydiopt-0.1.1/pyDIOPT/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 09:27:16.000000 pydiopt-0.1.1/pyDIOPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:27:24.775798 pydiopt-0.1.1/pyDIOPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 09:27:24.000000 pydiopt-0.1.1/pyDIOPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:27:24.775798 pydiopt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 09:27:16.000000 pydiopt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:11:13.370831 pydiopt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-17 04:11:07.000000 pydiopt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-17 04:11:13.370831 pydiopt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-17 04:11:07.000000 pydiopt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:11:13.370831 pydiopt-0.1.2/pyDIOPT/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-17 04:11:07.000000 pydiopt-0.1.2/pyDIOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-17 04:11:07.000000 pydiopt-0.1.2/pyDIOPT/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-17 04:11:07.000000 pydiopt-0.1.2/pyDIOPT/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-17 04:11:07.000000 pydiopt-0.1.2/pyDIOPT/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 04:11:07.000000 pydiopt-0.1.2/pyDIOPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:11:13.370831 pydiopt-0.1.2/pyDIOPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 04:11:13.000000 pydiopt-0.1.2/pyDIOPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:11:13.370831 pydiopt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-17 04:11:07.000000 pydiopt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:11:13.370831 pydiopt-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 04:11:07.000000 pydiopt-0.1.2/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-17 04:11:07.000000 pydiopt-0.1.2/tests/test_species.py
```

### Comparing `pydiopt-0.1.1/LICENSE` & `pydiopt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiopt-0.1.1/PKG-INFO` & `pydiopt-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDIOPT
-Version: 0.1.1
+Version: 0.1.2
 Summary: pyDIOPT - Python Wrapper for DIOPT
 Home-page: https://github.com/akmazian/pyDIOPT
 Author: AZ Zhang
 Author-email: azz@berkeley.edu
 License: Apache 2.0
 Keywords: wrapper bioinformatics biology
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,20 @@
 Requires-Dist: aiohttp
 Requires-Dist: gprofiler-official
 
 # pyDIOPT
 
 This is the unofficial, opinionated DIOPT python wrapper for the [DIOPT](https://www.flyrnai.org/cgi-bin/DRSC_orthologs.pl) ortholog finder.
 
+## Installation
+
+```shell
+pip install pyDIOPT
+```
+
 ## Example
 
 A couple examples of how to run the wrapper. The standard output is organized into pd.DataFrame for easier downstream manipulations and whatever you want (or can) do with ortholog data (?).
 
 ```python
 from pyDIOPT import DIOPTRelease
```

### Comparing `pydiopt-0.1.1/README.md` & `pydiopt-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # pyDIOPT
 
 This is the unofficial, opinionated DIOPT python wrapper for the [DIOPT](https://www.flyrnai.org/cgi-bin/DRSC_orthologs.pl) ortholog finder.
 
+## Installation
+
+```shell
+pip install pyDIOPT
+```
+
 ## Example
 
 A couple examples of how to run the wrapper. The standard output is organized into pd.DataFrame for easier downstream manipulations and whatever you want (or can) do with ortholog data (?).
 
 ```python
 from pyDIOPT import DIOPTRelease
```

### Comparing `pydiopt-0.1.1/pyDIOPT/fetch.py` & `pydiopt-0.1.2/pyDIOPT/fetch.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,32 +15,37 @@
 
 
 class DIOPTRelease:
     """
     Util class for fetching orthologs.
     """
 
-    gp = GProfiler(return_dataframe=True)
+    _gp = GProfiler(return_dataframe=True)
 
     def __init__(
         self, version: Literal["v8", "v9"] = "v8", input_species: str | int = "human"
     ) -> None:
         if version not in ["v8", "v9"]:
             if version in [8, 9]:
-                self.version = "v" + version
+                self.version = f"v{version}"
             else:
-                raise TypeError("The")
+                raise TypeError("The version annot be parsed. Please indicate whether v8 or v9 is to be used")
         else:
             if version == "v9":
                 print(
                     "Please note that v9 is currently in beta testing. Use v8 if you prefer the stable version."
                 )
             self.version = version
 
-        self.input_species = Species.parse_species(input_species)
+        try:
+            self.input_species = Species.parse_species(input_species, error=True)
+        except:
+            raise ValueError(
+                "The input species cannot be parsed. Refer to pyDIOPT.Species.available() for a complete list of supported species."
+            )
 
     def fetch(
         self,
         genes: Sequence[str],
         target_species: Optional[Species | str | int],
         filter: Optional[
             Literal["best_match", "exclude_score_less_1", "exclude_score_less_2"]
@@ -74,15 +79,15 @@
         base = url_builder(
             self.version,
             self.input_species.ncbi_taxonomy_id,
             target_species_id,
             filter if filter else "none",
         )
 
-        genes = self.convert_to_entrez_acc(np.array(genes).tolist())
+        genes = self.convert_to_entrez_acc(genes)
 
         async def _fetch(session, url):
             async with session.get(url) as response:
                 try:
                     return await response.json()
                 except:
                     raise ValueError(
@@ -100,18 +105,22 @@
 
         results = asyncio.run(_fetch_all([base(gene) for gene in genes]))
 
         unmatched = []
         chunks = []
 
         for entry in results:
-            gene_details = entry["search_details"]["gene_details"][0]
+            try:
+                gene_details = entry["search_details"]["gene_details"][0]
+            except:
+                print(
+                    f'entry["search_details"]["gene_details"] is {entry["search_details"]["gene_details"]}. entry is {entry}'
+                )
 
             if not entry["results"]:
-                print(entry)
                 unmatched.append(gene_details["symbol"])
                 continue
 
             for i in entry["results"].values():
                 if condensed:
                     chunk = pd.DataFrame(i.values())[
                         [
@@ -133,34 +142,40 @@
                     chunk = chunk.add_prefix("target_")
                     chunk = chunk.assign(
                         **{f"input_{key}": value for key, value in gene_details.items()}
                     )
                 chunks.append(chunk)
 
         if unmatched:
-            print(f"Some of the queries are returned unmatched:\n{unmatched}")
+            print(
+                f"{np.ceil(len(unmatched) / len(genes) * 100)}% of the queries are returned unmatched:\n{unmatched}"
+            )
 
-        return pd.concat(chunks, axis=0, ignore_index=True)
+        return (
+            pd.concat(chunks, axis=0, ignore_index=True) if chunks else pd.DataFrame()
+        )
 
     def convert_to_entrez_acc(self, genes: Sequence[str]) -> np.array:
         """
         Helper function that converts a list of arbitrary gene identifiers to Entrez IDs using the gprofiler library.
 
         Theoretically the list of genes can be in any format but it should preferabbly be passed in as a list, np.ndarray, or pd.Series.
 
         Returns an np.array of the Entrez IDs. If the full pd.DataFrame is desired, use the gprofiler library directly.
         """
         organism = self.input_species.latin_name.split(" ")
-        organism = organism[0][0] + organism[1]
+        organism = (organism[0][0] + organism[1]).lower()
 
-        result = self.gp.convert(
+        result = self._gp.convert(
             organism=organism.lower(),
-            query=np.array(genes).tolist(),
-            target_namespace="ENTREZGENE_ACC",
+            query=list(np.array(genes).tolist()),
+            target_namespace=(
+                "ENTREZGENE_ACC" if organism != "dmelanogaster" else "ENTREZGENE"
+            ),
         )
 
         if result[result["converted"] == "None"].shape[0]:
             print(
-                f'The following queries returned None when trying to get Entrez Acc Number:\n{result[result["converted"] == "None"]["incoming"].tolist()}'
+                f'The following queries ({np.ceil(result[result["converted"] == "None"].shape[0] / len(genes) * 100)}%) returned None when trying to get Entrez Acc Number:\n{result[result["converted"] == "None"]["incoming"].tolist()}'
             )
 
         return result[result["converted"] != "None"]["converted"].to_numpy()
```

### Comparing `pydiopt-0.1.1/pyDIOPT/species.py` & `pydiopt-0.1.2/pyDIOPT/species.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         return self.latin_name
 
     latin_name_map: dict[str, "Species"] = {}
     common_name_map: dict[str, "Species"] = {}
     ncbi_taxonomy_id_map: dict[int, "Species"] = {}
 
     @staticmethod
-    def Register(species: "Species") -> None:
+    def _register(species: "Species") -> None:
+        """Intended for internal use only. Registers a species"""
         Species.latin_name_map[species.latin_name] = species
         if species.common_name:
             if type(species.common_name) == list:
                 for common_name in species.common_name:
                     Species.common_name_map[common_name] = species
             else:
                 Species.common_name_map[species.common_name] = species
@@ -34,14 +35,18 @@
         species.registered = True
 
     @staticmethod
     def parse_species(
         search_query: Union["Species", str, int], error: bool = False
     ) -> "Species":
         """
+        Returns the appropriate species object based on search query.
+
+        A species object can also be passed in and the registered copy will be returned.
+
         Parameters:
             search_query: str | int | Species - any input that points to a species
             error: bool - whether to throw error if unable to parse species from search_query
         """
 
         if type(search_query) == int:
             if search_query in Species.ncbi_taxonomy_id_map:
@@ -63,15 +68,15 @@
             if search_string in Species.common_name_map:
                 return Species.common_name_map[search_string]
 
             # try matching latin names directly
             search_string = search_string.capitalize()
 
             if search_string in Species.latin_name_map:
-                return Species.common_name_map[search_string]
+                return Species.latin_name_map[search_string]
 
             # try matching abbreviated latin names
             species_query = search_string.split(" ")[-1]
             for genus_species in Species.latin_name_map.keys():
                 if species_query == genus_species.split(" ")[-1]:
                     return Species.latin_name_map[genus_species]
 
@@ -84,19 +89,19 @@
     @staticmethod
     def available() -> None:
         print("Available species through DIOPT:")
         for ncbi_taxnomoy_id, species in Species.ncbi_taxonomy_id_map.items():
             print(f"{ncbi_taxnomoy_id}\t{species.latin_name}")
 
 
-Species.Register(Species("Escherichia coli", common_name=None, ncbi_taxonomy_id=83333))
-Species.Register(Species("Arabidopsis thaliana", ["thale cress", "cress"], 3702))
-Species.Register(Species("Schizosaccharomyces pombe", "fission yeast", 4896))
-Species.Register(Species("Saccharomyces cerevisiae", ["budding yeast", "yeast"], 4932))
-Species.Register(Species("Caenorhabditis elegans", ["worm", "nematode"], 6239))
-Species.Register(Species("Anopheles gambiae", "mosquito", 7165))
-Species.Register(Species("Drosophila melanogaster", ["fly", "fruit fly"], 7227))
-Species.Register(Species("Danio rerio", "zebrafish", 7955))
-Species.Register(Species("Xenopus tropicalis", "western clawed frog", 8364))
-Species.Register(Species("Rattus norvegicus", ["rat", "brown rat"], 10116))
-Species.Register(Species("Mus musculus", "mouse", 10090))
-Species.Register(Species("Homo sapiens", "human", 9606))
+Species._register(Species("Escherichia coli", common_name=None, ncbi_taxonomy_id=83333))
+Species._register(Species("Arabidopsis thaliana", ["thale cress", "cress"], 3702))
+Species._register(Species("Schizosaccharomyces pombe", "fission yeast", 4896))
+Species._register(Species("Saccharomyces cerevisiae", ["budding yeast", "yeast"], 4932))
+Species._register(Species("Caenorhabditis elegans", ["worm", "nematode"], 6239))
+Species._register(Species("Anopheles gambiae", "mosquito", 7165))
+Species._register(Species("Drosophila melanogaster", ["fly", "fruit fly"], 7227))
+Species._register(Species("Danio rerio", "zebrafish", 7955))
+Species._register(Species("Xenopus tropicalis", "western clawed frog", 8364))
+Species._register(Species("Rattus norvegicus", ["rat", "brown rat"], 10116))
+Species._register(Species("Mus musculus", "mouse", 10090))
+Species._register(Species("Homo sapiens", "human", 9606))
```

### Comparing `pydiopt-0.1.1/pyDIOPT/utils.py` & `pydiopt-0.1.2/pyDIOPT/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     print(
         "It would be appreciated if you also cited pyDIOPT :) though it is not required."
     )
 
 
 def help() -> None:
     print("The documentations for pyDIOPT can be found at:")
-    print("*not quite ready yet*")
+    print("[pyDIOT](https://github.com/akmazian/pyDIOPT)")
     print()
     print("The documentations for DIOPT can be found at:")
     print("[DIOPT](https://fgr.hms.harvard.edu/diopt-documentation)")
```

### Comparing `pydiopt-0.1.1/pyDIOPT.egg-info/PKG-INFO` & `pydiopt-0.1.2/pyDIOPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDIOPT
-Version: 0.1.1
+Version: 0.1.2
 Summary: pyDIOPT - Python Wrapper for DIOPT
 Home-page: https://github.com/akmazian/pyDIOPT
 Author: AZ Zhang
 Author-email: azz@berkeley.edu
 License: Apache 2.0
 Keywords: wrapper bioinformatics biology
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,20 @@
 Requires-Dist: aiohttp
 Requires-Dist: gprofiler-official
 
 # pyDIOPT
 
 This is the unofficial, opinionated DIOPT python wrapper for the [DIOPT](https://www.flyrnai.org/cgi-bin/DRSC_orthologs.pl) ortholog finder.
 
+## Installation
+
+```shell
+pip install pyDIOPT
+```
+
 ## Example
 
 A couple examples of how to run the wrapper. The standard output is organized into pd.DataFrame for easier downstream manipulations and whatever you want (or can) do with ortholog data (?).
 
 ```python
 from pyDIOPT import DIOPTRelease
```

### Comparing `pydiopt-0.1.1/setup.py` & `pydiopt-0.1.2/setup.py`

 * *Files identical despite different names*

