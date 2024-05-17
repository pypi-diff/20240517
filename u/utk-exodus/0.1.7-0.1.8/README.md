# Comparing `tmp/utk_exodus-0.1.7.tar.gz` & `tmp/utk_exodus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.7.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.8.tar", max compression
```

## Comparing `utk_exodus-0.1.7.tar` & `utk_exodus-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     3755 2024-05-15 15:33:14.611533 utk_exodus-0.1.7/README.md
--rw-r--r--   0        0        0      654 2024-05-15 15:33:14.611849 utk_exodus-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      656 2024-05-15 15:33:14.612191 utk_exodus-0.1.7/utk_exodus/__init__.py
--rw-r--r--   0        0        0       66 2024-05-15 14:25:18.889957 utk_exodus-0.1.7/utk_exodus/combine/__init__.py
--rw-r--r--   0        0        0     1868 2024-05-15 14:25:18.890339 utk_exodus-0.1.7/utk_exodus/combine/combine.py
--rw-r--r--   0        0        0     2387 2024-05-10 00:17:11.629365 utk_exodus-0.1.7/utk_exodus/config/samvera_default.yml
--rw-r--r--   0        0        0    12260 2024-05-10 00:17:11.629691 utk_exodus-0.1.7/utk_exodus/config/utk_dc.yml
--rw-r--r--   0        0        0    11044 2024-05-10 00:17:11.629996 utk_exodus-0.1.7/utk_exodus/config/utk_dc_no_uris.yml
--rw-r--r--   0        0        0     7824 2024-05-10 00:17:11.630293 utk_exodus-0.1.7/utk_exodus/config/utk_no_uris_no_names.yml
--rw-r--r--   0        0        0       79 2024-05-10 00:17:11.630638 utk_exodus-0.1.7/utk_exodus/controller/__init__.py
--rw-r--r--   0        0        0     6346 2024-05-15 14:25:18.891011 utk_exodus-0.1.7/utk_exodus/controller/controller.py
--rw-r--r--   0        0        0       59 2024-05-10 00:17:11.630872 utk_exodus-0.1.7/utk_exodus/curate/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.7/utk_exodus/curate/curate.py
--rw-r--r--   0        0        0     5724 2024-05-15 15:33:14.612699 utk_exodus-0.1.7/utk_exodus/exodus.py
--rw-r--r--   0        0        0       61 2024-05-10 00:17:11.631361 utk_exodus-0.1.7/utk_exodus/fedora/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-10 16:33:04.511046 utk_exodus-0.1.7/utk_exodus/fedora/fedora.py
--rw-r--r--   0        0        0       63 2024-05-10 00:17:11.631585 utk_exodus-0.1.7/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18702 2024-05-10 00:17:11.631880 utk_exodus-0.1.7/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.7/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.7/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.7/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    47840 2024-05-14 12:54:12.683039 utk_exodus-0.1.7/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0      103 2024-05-10 17:15:08.670786 utk_exodus-0.1.7/utk_exodus/restrict/__init__.py
--rw-r--r--   0        0        0     4324 2024-05-10 17:15:08.671022 utk_exodus-0.1.7/utk_exodus/restrict/restrict.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.7/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0    11179 2024-05-15 14:25:18.891820 utk_exodus-0.1.7/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0       65 2024-05-15 14:25:18.892035 utk_exodus-0.1.7/utk_exodus/template/__init__.py
--rw-r--r--   0        0        0     2361 2024-05-15 14:25:18.892200 utk_exodus-0.1.7/utk_exodus/template/template.py
--rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.7/utk_exodus/validate/__init__.py
--rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.7/utk_exodus/validate/validate.py
--rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 utk_exodus-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4112 2024-05-17 13:07:44.981283 utk_exodus-0.1.8/README.md
+-rw-r--r--   0        0        0      654 2024-05-17 13:07:44.981647 utk_exodus-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      704 2024-05-17 13:07:44.982030 utk_exodus-0.1.8/utk_exodus/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-17 11:39:11.577880 utk_exodus-0.1.8/utk_exodus/checksum/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-17 11:39:11.578202 utk_exodus-0.1.8/utk_exodus/checksum/checksum.py
+-rw-r--r--   0        0        0       66 2024-05-15 14:25:18.889957 utk_exodus-0.1.8/utk_exodus/combine/__init__.py
+-rw-r--r--   0        0        0     1868 2024-05-15 14:25:18.890339 utk_exodus-0.1.8/utk_exodus/combine/combine.py
+-rw-r--r--   0        0        0     2387 2024-05-10 00:17:11.629365 utk_exodus-0.1.8/utk_exodus/config/samvera_default.yml
+-rw-r--r--   0        0        0    12260 2024-05-10 00:17:11.629691 utk_exodus-0.1.8/utk_exodus/config/utk_dc.yml
+-rw-r--r--   0        0        0    11044 2024-05-10 00:17:11.629996 utk_exodus-0.1.8/utk_exodus/config/utk_dc_no_uris.yml
+-rw-r--r--   0        0        0     7824 2024-05-10 00:17:11.630293 utk_exodus-0.1.8/utk_exodus/config/utk_no_uris_no_names.yml
+-rw-r--r--   0        0        0       79 2024-05-10 00:17:11.630638 utk_exodus-0.1.8/utk_exodus/controller/__init__.py
+-rw-r--r--   0        0        0     6346 2024-05-15 14:25:18.891011 utk_exodus-0.1.8/utk_exodus/controller/controller.py
+-rw-r--r--   0        0        0       59 2024-05-10 00:17:11.630872 utk_exodus-0.1.8/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.8/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     6329 2024-05-17 13:07:44.982665 utk_exodus-0.1.8/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       61 2024-05-10 00:17:11.631361 utk_exodus-0.1.8/utk_exodus/fedora/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-17 13:07:44.983072 utk_exodus-0.1.8/utk_exodus/fedora/fedora.py
+-rw-r--r--   0        0        0       63 2024-05-10 00:17:11.631585 utk_exodus-0.1.8/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18702 2024-05-10 00:17:11.631880 utk_exodus-0.1.8/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      857 2024-05-17 11:39:11.578619 utk_exodus-0.1.8/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-05-17 13:07:44.983560 utk_exodus-0.1.8/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.8/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    48565 2024-05-17 11:39:11.578976 utk_exodus-0.1.8/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0      103 2024-05-10 17:15:08.670786 utk_exodus-0.1.8/utk_exodus/restrict/__init__.py
+-rw-r--r--   0        0        0     4324 2024-05-10 17:15:08.671022 utk_exodus-0.1.8/utk_exodus/restrict/restrict.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.8/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0    11179 2024-05-17 13:07:44.983970 utk_exodus-0.1.8/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       65 2024-05-15 14:25:18.892035 utk_exodus-0.1.8/utk_exodus/template/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-15 14:25:18.892200 utk_exodus-0.1.8/utk_exodus/template/template.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.8/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.8/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 utk_exodus-0.1.8/PKG-INFO
```

### Comparing `utk_exodus-0.1.7/README.md` & `utk_exodus-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,26 @@
     * `FEDORA_URI`: the base URI for where Fedora is installed
 2. If you're looking for these values, you can find them in the Exodus `Environment` of this repository in `Settings`.
 
 ## Using
 
 There are several interfaces for the application.
 
+You can always find out what interfaces exist with:
+
+```shell
+exodus --help
+```
+
+Similarly, you can get help for a specific interface with:
+
+```shell
+exodus <interface> --help
+````
+
 If you want to get works and files, and you have metadata files, use:
 
 ```shell
 exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
 ```
 
 If you want to get works and files, and you don't have metadata files, you need to specify
@@ -70,14 +82,20 @@
 
 If you want to generate a full template for a metadata import, use:
 
 ```shell
 exodus generate_template --model book -o /path/to/sheet.csv
 ```
 
+If you want to generate a sheet of checksums for files that failed to import, you can:
+
+```shell
+exodus hash_errors --path /path/to/directory --output /path/to/sheet.csv
+```
+
 ## What's Missing Here Right Now
 
 * The ability to create pcdm:Collection objects.
 * The ability to create a new metadata import from a previous import
 
 ## Understanding Configs
```

### Comparing `utk_exodus-0.1.7/pyproject.toml` & `utk_exodus-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utk-exodus"
-version = "0.1.7"
+version = "0.1.8"
 description = "A tool for building import sheets from UTK legacy systems"
 authors = ["Mark Baggett <mbagget1@utk.edu>"]
 readme = "README.md"
 include = [
     { path = "utk_exodus/config", format = ["sdist", "wheel"] }
 ]
```

### Comparing `utk_exodus-0.1.7/utk_exodus/__init__.py` & `utk_exodus-0.1.8/utk_exodus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from .metadata import MetadataMapping
 from .risearch import ResourceIndexSearch
 from .finder import FileOrganizer
 from .curate import FileCurator
 from .validate import ValidateMigration
 from .fedora import FedoraObject
+from.checksum import HashSheet
 from .controller import InterfaceController
 from .combine import ImportRefactor
 from .template import ImportTemplate
 from .restrict import Restrictions, RestrictionsSheet
 
 __all__ = [
     "FedoraObject",
     "FileCurator",
     "FileOrganizer",
+    "HashSheet",
     "ImportRefactor",
     "ImportTemplate",
     "InterfaceController",
     "MetadataMapping",
     "ResourceIndexSearch",
     "Restrictions",
     "RestrictionsSheet",
```

### Comparing `utk_exodus-0.1.7/utk_exodus/combine/combine.py` & `utk_exodus-0.1.8/utk_exodus/combine/combine.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/config/samvera_default.yml` & `utk_exodus-0.1.8/utk_exodus/config/samvera_default.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/config/utk_dc.yml` & `utk_exodus-0.1.8/utk_exodus/config/utk_dc.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/config/utk_dc_no_uris.yml` & `utk_exodus-0.1.8/utk_exodus/config/utk_dc_no_uris.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/config/utk_no_uris_no_names.yml` & `utk_exodus-0.1.8/utk_exodus/config/utk_no_uris_no_names.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/controller/controller.py` & `utk_exodus-0.1.8/utk_exodus/controller/controller.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/curate/curate.py` & `utk_exodus-0.1.8/utk_exodus/curate/curate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/exodus.py` & `utk_exodus-0.1.8/utk_exodus/exodus.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from utk_exodus.finder import FileOrganizer
 from utk_exodus.metadata import MetadataMapping
 from utk_exodus.validate import ValidateMigration
 from utk_exodus.controller import InterfaceController
 from utk_exodus.template import ImportTemplate
 from utk_exodus.combine import ImportRefactor
+from utk_exodus.checksum import HashSheet
 import click
 import requests
 
 
 @click.group()
 def cli() -> None:
     pass
@@ -209,7 +210,33 @@
     sheet: str,
     old_sheet: str,
     new_sheet: str,
 ) -> None:
     ir = ImportRefactor(sheet, old_sheet)
     ir.create_csv_with_fields_to_nuke(sheet, new_sheet)
     print(f"Refactored sheet written to {new_sheet}.")
+
+
+@cli.command(
+    "hash_errors",
+    help="Create sheet from a directory of errored import sheets.",
+)
+@click.option(
+    "--path",
+    "-p",
+    required=True,
+    help="Specify the path to the directory of sheets.",
+)
+@click.option(
+    "--output",
+    "-o",
+    required=True,
+    help="Specify where you want to write your sheets.",
+)
+def hash_errors(
+    path: str,
+    output: str,
+) -> None:
+    print(f"Generating checksums for bad files in csvs in {path}.")
+    hs = HashSheet(path, output)
+    hs.write()
+    print(f"Hash sheet written to {output}.")
```

### Comparing `utk_exodus-0.1.7/utk_exodus/fedora/fedora.py` & `utk_exodus-0.1.8/utk_exodus/fedora/fedora.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/finder/finder.py` & `utk_exodus-0.1.8/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.8/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.8/utk_exodus/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,22 @@
         titles_data = {
             "plain": self.__get_titles_from_xpath(
                 'mods:titleInfo[not(@supplied)][not(@type="alternative")]/mods:title'
             ),
             "supplied": self.__get_titles_from_xpath(
                 "mods:titleInfo[@supplied]/mods:title"
             ),
-            "part_names": self.__get_titles_from_xpath(
-                "mods:titleInfo/mods:partName"
-            ),
+            "part_names": self.__get_titles_from_xpath("mods:titleInfo/mods:partName"),
             "part_numbers": self.__get_titles_from_xpath(
                 "mods:titleInfo/mods:partNumber"
             ),
-            "non_sorts": self.__get_titles_from_xpath(
-                "mods:titleInfo/mods:nonSort"
-            ),
+            "non_sorts": self.__get_titles_from_xpath("mods:titleInfo/mods:nonSort"),
             "alternatives": self.__get_titles_from_xpath(
                 'mods:titleInfo[@type="alternative"]/mods:title'
-            )
+            ),
         }
         return titles_data
 
     def __get_titles_from_xpath(self, xpath_expr):
         # Retrieve text content based on the given xpath expression.
         return [
             element.text
@@ -79,18 +75,15 @@
             alternatives.extend(titles_data["plain"])
         else:
             titles.extend(titles_data["supplied"] + titles_data["plain"])
 
         # Handle alternative titles mapping to dcterms:alternative.
         alternatives.extend(titles_data["alternatives"])
 
-        return {
-            "title": titles,
-            "alternative_title": alternatives
-        }
+        return {"title": titles, "alternative_title": alternatives}
 
 
 class RoleAndNameProperty(XMLtoDictProperty):
     def __init__(self, file):
         super().__init__(file)
         self.all_names = self.__find_all_names()
 
@@ -141,15 +134,15 @@
                 if isinstance(name_value, list):
                     for part in name_value:
                         if isinstance(part, dict) and part.get("mods:namePart"):
                             if role not in roles_and_names:
                                 roles_and_names[role] = [part["mods:namePart"]]
                             else:
                                 roles_and_names[role].append([part["mods:namePart"]])
-                        if  isinstance(part, str) and not part.startswith("http"):
+                        if isinstance(part, str) and not part.startswith("http"):
                             if role not in roles_and_names:
                                 roles_and_names[role] = [part]
                             else:
                                 roles_and_names[role].append(part)
                 elif role not in roles_and_names and not name_value.startswith("http"):
                     roles_and_names[role] = [name_value]
                 elif not name_value.startswith("http"):
@@ -157,29 +150,30 @@
         return roles_and_names
 
 
 class NameProperty(XMLtoDictProperty):
     """
     Used for names.
     """
+
     def __init__(self, file):
         super().__init__(file)
         self.all_names = self.__find_all_names()
 
     def __find_all_names(self):
-        if 'mods:name' in self.doc['mods:mods']:
-            all_names = self.doc['mods:mods']['mods:name']
-            if  isinstance(all_names, list):
+        if "mods:name" in self.doc["mods:mods"]:
+            all_names = self.doc["mods:mods"]["mods:name"]
+            if isinstance(all_names, list):
                 return all_names
             elif isinstance(all_names, dict):
                 return [all_names]
             elif isinstance(all_names, str):
                 return [all_names]
             else:
-                return ['Problem']
+                return ["Problem"]
         else:
             return []
 
     def find(self):
         """
         Find all names in the XML file.
 
@@ -192,70 +186,89 @@
             {'composer': ['http://id.loc.gov/authorities/names/no2002022963', 'http://id.loc.gov/authorities/names/n78013127'], 'compiler': ['http://id.loc.gov/authorities/names/no2002022963', 'http://id.loc.gov/authorities/names/n78013127']}
         """
         roles_and_names = {}
         for name in self.all_names:
             roles = []
             local_roles = []
             try:
-                roles.append(name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_'))
-                local_roles.append(f"utk_{name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_')}")
+                roles.append(
+                    name["mods:role"]["mods:roleTerm"]["#text"]
+                    .lower()
+                    .replace(" ", "_")
+                )
+                local_roles.append(
+                    f"utk_{name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_')}"
+                )
             except KeyError:
                 print(name)
             # TODO: A name can have multiple roles
             except TypeError:
-                if isinstance(name['mods:role'], list):
-                    for role in name['mods:role']:
-                        if '#text' in role['mods:roleTerm']:
-                            roles.append(role['mods:roleTerm']['#text'].lower().replace(' ', '_'))
-                            local_roles.append(f"utk_{role['mods:roleTerm']['#text'].lower().replace(' ', '_')}")
+                if isinstance(name["mods:role"], list):
+                    for role in name["mods:role"]:
+                        if "#text" in role["mods:roleTerm"]:
+                            roles.append(
+                                role["mods:roleTerm"]["#text"].lower().replace(" ", "_")
+                            )
+                            local_roles.append(
+                                f"utk_{role['mods:roleTerm']['#text'].lower().replace(' ', '_')}"
+                            )
                         else:
-                            roles.append(role['mods:roleTerm'].lower().replace(' ', '_'))
-                            local_roles.append(f"utk_{role['mods:roleTerm'].lower().replace(' ', '_')}")
+                            roles.append(
+                                role["mods:roleTerm"].lower().replace(" ", "_")
+                            )
+                            local_roles.append(
+                                f"utk_{role['mods:roleTerm'].lower().replace(' ', '_')}"
+                            )
                 else:
-                    roles.append(name['mods:role']['mods:roleTerm'].lower().replace(' ', '_'))
-                    local_roles.append(f"utk_{name['mods:role']['mods:roleTerm'].lower().replace(' ', '_')}")
+                    roles.append(
+                        name["mods:role"]["mods:roleTerm"].lower().replace(" ", "_")
+                    )
+                    local_roles.append(
+                        f"utk_{name['mods:role']['mods:roleTerm'].lower().replace(' ', '_')}"
+                    )
             # TODO: Rework this.  It's not pretty but it works.
-            name_value = name['mods:namePart']
-            if '@valueURI' in name:
-                name_value = name['@valueURI']
+            name_value = name["mods:namePart"]
+            if "@valueURI" in name:
+                name_value = name["@valueURI"]
             for role in roles:
                 if isinstance(name_value, list):
                     for part in name_value:
-                        if isinstance(part, dict) and '@valueURI' in part:
+                        if isinstance(part, dict) and "@valueURI" in part:
                             if role not in roles_and_names:
-                                roles_and_names[role] = [part['@valueURI']]
+                                roles_and_names[role] = [part["@valueURI"]]
                             else:
-                                roles_and_names[role].append([part['@valueURI']])
-                elif role not in roles_and_names and name_value.startswith('http'):
+                                roles_and_names[role].append([part["@valueURI"]])
+                elif role not in roles_and_names and name_value.startswith("http"):
                     roles_and_names[role] = [name_value]
-                elif name_value.startswith('http'):
+                elif name_value.startswith("http"):
                     roles_and_names[role].append(name_value)
             for role in local_roles:
                 if isinstance(name_value, list):
                     for part in name_value:
-                        if isinstance(part, str) and not part.startswith('http'):
+                        if isinstance(part, str) and not part.startswith("http"):
                             if role not in roles_and_names:
                                 roles_and_names[role] = [part]
                             else:
                                 roles_and_names[role].append(part)
-                elif role not in roles_and_names and not name_value.startswith('http'):
+                elif role not in roles_and_names and not name_value.startswith("http"):
                     roles_and_names[role] = [name_value]
-                elif not name_value.startswith('http'):
+                elif not name_value.startswith("http"):
                     roles_and_names[role].append(name_value)
         return roles_and_names
 
 
 class GeoNamesProperty(BaseProperty):
     """
     Handles the mapping of different types of geonames based on the provided XML data.
 
     Args:
         path (str): The path to the XML file.
         namespaces (dict): A dictionary containing the namespaces used in the XML file.
     """
+
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self, name):
         """
         Find all geonames in the XML file.
 
@@ -263,15 +276,15 @@
             name (str): The name of the geoname.
 
         Returns:
             dict: A dictionary containing the geoname mappings.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> geonames = GeoNamesProperty("tests/fixtures/webster_1127.xml", NAMESPACES)
             >>> geonames.find("spatial")
             {'spatial': ['http://sws.geonames.org/4050810', 'http://sws.geonames.org/4609260', 'http://id.loc.gov/authorities/subjects/sh85057008']}
         """
         uris = [
             uri.replace("about.rdf", "")
@@ -329,15 +342,15 @@
         Find all locations properties in the XML file.
 
         Returns:
             dict: A dictionary containing location properties.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> physical_location = PhysicalLocationsProperties("tests/fixtures/civilwar_1438.xml", NAMESPACES)
             >>> physical_location.find()
             {'repository': ['University of Tennessee, Knoxville. Special Collections'], 'archival_collection': ['O. P. Temple Papers,1862']}
         """
         return {
             "repository": self.__find_repositories(),
@@ -394,15 +407,15 @@
         Find all data providers in the XML file.
 
         Returns:
             dict: A dictionary containing data provider information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> dataProvider = DataProvider("tests/fixtures/egypt_224.xml", NAMESPACES)
             >>> dataProvider.find()
             {'provider': ['University of Tennessee, Knoxville. Libraries'], 'intermediate_provider': ['Frank H. McClung Museum of Natural History and Culture']}
         """
         values = [
             value.text
@@ -429,15 +442,15 @@
         Find all machine date information in the XML file.
 
         Returns:
             dict: A dictionary containing machine date information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> machineDate = MachineDate("tests/fixtures/volvoices_2993.xml", NAMESPACES)
             >>> machineDate.find()
             {'date_created_d': ['1948-01'], 'date_issued_d': ['1948'], 'date_other_d': []}
         """
         date_created = [
             value.text
@@ -476,83 +489,74 @@
                 if value is not None:
                     return [value]
         else:
             return values
 
 
 class SubjectProperty(BaseProperty):
-    # TODO: Should this even exist? Can't this just be BaseProperty?
+    """Get subjects from the MODS XML file."""
+
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find_topic(self):
-        subject_topic_value_uris = [
-            uri
-            for uri in self.root.xpath(
-                "mods:subject[mods:topic]/@valueURI", namespaces=self.namespaces
-            )
-        ]
-        topic_value_uris = [
-            uri
-            for uri in self.root.xpath(
-                "mods:subject/mods:topic/@valueURI", namespaces=self.namespaces
-            )
-        ]
-        subject_name_value_uris = [
-            uri
-            for uri in self.root.xpath(
-                "mods:subject[mods:name/mods:namePart]/@valueURI",
-                namespaces=self.namespaces,
-            )
-        ]
-        name_value_uris = [
-            uri
-            for uri in self.root.xpath(
-                "mods:subject/mods:name/@valueURI", namespaces=self.namespaces
-            )
-        ]
-        aat_genres = [
-            uri
-            for uri in self.root.xpath(
-                'mods:genre[@authority="aat"]/@valueURI', namespaces=self.namespaces
-            )
-        ]
-        lcmpt_genres = [
-            uri
-            for uri in self.root.xpath(
-                'mods:genre[@authority="lcmpt"]/@valueURI', namespaces=self.namespaces
-            )
-        ]
-        lcsh_genres = [
-            uri
-            for uri in self.root.xpath(
-                'mods:genre[@authority="lcsh"]/@valueURI', namespaces=self.namespaces
-            )
-        ]
-        all_initial_values = [
-            subject_topic_value_uris,
-            topic_value_uris,
-            subject_name_value_uris,
-            name_value_uris,
-            aat_genres,
-            lcmpt_genres,
-            lcsh_genres,
+        """Find all topics in the XML file.
+
+        Returns:
+            dict: A dictionary containing topics information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3',
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> subjects = SubjectProperty("tests/fixtures/knoxgardens_125.xml", NAMESPACES)
+            >>> subjects.find_topic()
+            {'subject': ['http://id.loc.gov/authorities/subjects/sh85101348', 'http://id.loc.gov/authorities/subjects/sh85053123', 'http://id.loc.gov/authorities/subjects/sh85103022', 'http://id.loc.gov/authorities/subjects/sh2008120720']}
+
+        """
+        xpaths = [
+            "mods:subject[mods:topic]/@valueURI",
+            "mods:subject/mods:topic/@valueURI",
+            "mods:subject[mods:name/mods:namePart]/@valueURI",
+            "mods:subject/mods:name/@valueURI",
+            'mods:genre[@authority="aat"]/@valueURI',
+            'mods:genre[@authority="lcmpt"]/@valueURI',
+            'mods:genre[@authority="lcsh"]/@valueURI',
         ]
+
+        # Execute each XPath query and collect results
         return_values = []
-        for iterable in all_initial_values:
-            for value in iterable:
-                return_values.append(value)
+        for xpath in xpaths:
+            uris = self.root.xpath(xpath, namespaces=self.namespaces)
+            return_values.extend(uri.strip() for uri in uris)
+
         return {"subject": return_values}
 
 
 class KeywordProperty(BaseProperty):
+    """Get keywords from the MODS XML file."""
+
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find_topic(self):
+        """Find all topics in the XML file.
+
+        Returns:
+            dict: A dictionary containing topics information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3',
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> keywords = KeywordProperty("tests/fixtures/civilwar_1438.xml", NAMESPACES)
+            >>> keywords.find_topic()
+            {'keyword': ['Jurisdiction -- Tennessee, East -- History -- Civil War, 1861-1865', 'Actions and defenses -- Tennessee, East -- History -- Civil War, 1861-1865', 'Tennessee, East -- Politics and government -- 19th century', 'Wallace, Jesse G. -- Correspondence', 'Temple, Oliver Perry, 1820-1907 -- Correspondence']}
+
+        """
         non_uris_topics = [
             value.text
             for value in self.root.xpath(
                 "mods:subject[not(@valueURI)]/mods:topic[not(@valueURI)]",
                 namespaces=self.namespaces,
             )
         ]
@@ -580,15 +584,15 @@
         Find all types properties information in the XML file.
 
         Returns:
             dict: A dictionary containing types properties information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> types = TypesProperties("tests/fixtures/utsmc_17870.xml", NAMESPACES)
             >>> types.find()
             {'form': ['http://vocab.getty.edu/aat/300026430'], 'resource_type': ['http://id.loc.gov/vocabulary/resourceTypes/not', 'http://id.loc.gov/vocabulary/resourceTypes/txt'], 'form_local': []}
         """
         return {
             "form": self.__find_edm_has_type(),
@@ -735,15 +739,15 @@
         Find all local types properties information in the XML file.
 
         Returns:
             dict: A dictionary containing local types properties information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> local_types = LocalTypesProperties("tests/fixtures/egypt_224.xml", NAMESPACES)
             >>> local_types.find()
             {'resource_type_local': ['still image'], 'form_local': ['platinum prints']}
         """
         return {
             "resource_type_local": self.__find_dcterms_type(),
@@ -868,15 +872,15 @@
         Find all publisher property information in the XML file.
 
         Returns:
             dict: A dictionary containing publisher property information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> publisher = PublisherProperty("tests/fixtures/playbills:1052.xml", NAMESPACES)
             >>> publisher.find()
             {'publisher': []}
         """
         return {
             "publisher": [
@@ -898,15 +902,15 @@
         Find all rights or liscense property information in the XML file.
 
         Returns:
             dict: A dictionary containing rights or license property information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> rights = RightsOrLicenseProperties("tests/fixtures/heilman:1010.xml", NAMESPACES)
             >>> rights.find()
             {'license': ['http://creativecommons.org/licenses/by-nc-nd/3.0/'], 'rights_statement': ['http://rightsstatements.org/vocab/InC/1.0/']}
         """
         final = {}
         rights = [
@@ -950,15 +954,15 @@
         Find all publication place property information in the XML file.
 
         Returns:
             dict: A dictionary containing publication place property information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> publication_place = PublicationPlaceProperty("tests/fixtures/volvoices_2495.xml", NAMESPACES)
             >>> publication_place.find()
             {'publication_place': ['http://id.loc.gov/authorities/names/n82063401']}
         """
         return {
             "publication_place": [
@@ -980,15 +984,15 @@
         Find all language URI properties in the XML file.
 
         Returns:
             dict: A dictionary containing language URI property information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> language_uri = LanguageURIProperty("tests/fixtures/utsmc:725.xml", NAMESPACES)
             >>> language_uri.find_term()
             {'language': ['http://id.loc.gov/vocabulary/iso639-2/fre', 'http://id.loc.gov/vocabulary/iso639-2/ita']}
         """
         terms_and_uris = {
             "English": "http://id.loc.gov/vocabulary/iso639-2/eng",
@@ -1019,27 +1023,28 @@
     """
     Class to Handle Extent Information.
 
     Args:
         path (str): The path to the file.
         namespaces (dict): Namespaces to be used in the XPath queries.
     """
+
     def __init__(self, path: str, namespaces: dict):
         super().__init__(path, namespaces)
 
     def find(self):
         """
         Finds and returns a dictionary containing the extent information of a record.
 
         Returns:
             dict: A dictionary containing the extent information.
 
         Examples:
             >>> NAMESPACES = {
-            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'mods': 'http://www.loc.gov/mods/v3',
             ... 'xlink': 'http://www.w3.org/1999/xlink' }
             >>> extent_property = ExtentProperty("tests/fixtures/knoxgardens_125.xml", NAMESPACES)
             >>> extent_property.find()
             {'extent': ['3 1/4 x 5 inches']}
 
         """
         extents_without_units = [
@@ -1052,15 +1057,15 @@
 
         extents_with_units = [
             f"{node.text} {node.attrib['unit']}"
             for node in self.root.xpath(
                 "mods:physicalDescription/mods:extent[@unit]",
                 namespaces=self.namespaces,
             )
-            if node.text is not None and 'unit' in node.attrib
+            if node.text is not None and "unit" in node.attrib
         ]
 
         # Combine extents with and without units into a single list
         final_extent = extents_with_units + extents_without_units
 
         return {"extent": final_extent}
 
@@ -1093,15 +1098,15 @@
             # TODO: Ultimately, parents should be populated based on relationship.
             model = self.__dereference_islandora_type(file)
             output_data = {
                 "source_identifier": file.split("/")[-1]
                 .replace("_MODS.xml", "")
                 .replace(".xml", ""),
                 "model": model,
-                'sequence': '',
+                "sequence": "",
                 "remote_files": "",
                 "parents": " | ".join(
                     ResourceIndexSearch().get_parent_collections(
                         file.split("/")[-1].replace("_MODS.xml", "").replace(".xml", "")
                     ),
                 ),
                 "has_work_type": self.__get_utk_ontology_value(model),
@@ -1133,26 +1138,26 @@
                                 print(f"{TypeError}: {file}")
             self.__find_unique_fieldnames(output_data)
             all_file_data.append(output_data)
         for item in all_file_data:
             pages = self.look_for_pages(item)
             for page in pages:
                 new_page = item.copy()
-                new_page['source_identifier'] = page['pid'].replace('info:fedora/', '')
-                new_page['parents'] = item['source_identifier']
-                new_page['model'] = 'Page'
-                new_page['sequence'] = page['page']
+                new_page["source_identifier"] = page["pid"].replace("info:fedora/", "")
+                new_page["parents"] = item["source_identifier"]
+                new_page["model"] = "Page"
+                new_page["sequence"] = page["page"]
                 all_pages.append(new_page)
         for page in all_pages:
             all_file_data.append(page)
         return all_file_data
 
     def look_for_pages(self, data):
-        if data['model'] == 'Book':
-            return ResourceIndexSearch().find_pages_in_book(data['source_identifier'])
+        if data["model"] == "Book":
+            return ResourceIndexSearch().find_pages_in_book(data["source_identifier"])
         return []
 
     def __find_unique_fieldnames(self, data):
         for k, v in data.items():
             if k not in self.fieldnames:
                 self.fieldnames.append(k)
         return
@@ -1164,15 +1169,18 @@
             "info:fedora/islandora:binaryObjectCModel": "Generic",
             "info:fedora/islandora:sp_large_image_cmodel": "Image",
             "info:fedora/islandora:sp_basic_image": "Image",
             "info:fedora/islandora:sp_pdf": "Pdf",
             "info:fedora/islandora:sp_videoCModel": "Video",
         }
         x = ResourceIndexSearch().get_islandora_work_type(
-            file.split("/")[-1].replace("_MODS.xml", "").replace(".xml", "").replace("_", ":")
+            file.split("/")[-1]
+            .replace("_MODS.xml", "")
+            .replace(".xml", "")
+            .replace("_", ":")
         )
         return islandora_types[x]
 
     @staticmethod
     def __get_utk_ontology_value(model):
         ontology_values = {
             "Audio": "https://ontology.lib.utk.edu/works#AudioWork",
```

### Comparing `utk_exodus-0.1.7/utk_exodus/restrict/restrict.py` & `utk_exodus-0.1.8/utk_exodus/restrict/restrict.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.8/utk_exodus/risearch/risearch.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/template/template.py` & `utk_exodus-0.1.8/utk_exodus/template/template.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/utk_exodus/validate/validate.py` & `utk_exodus-0.1.8/utk_exodus/validate/validate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.7/PKG-INFO` & `utk_exodus-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utk-exodus
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for building import sheets from UTK legacy systems
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,14 +57,26 @@
     * `FEDORA_URI`: the base URI for where Fedora is installed
 2. If you're looking for these values, you can find them in the Exodus `Environment` of this repository in `Settings`.
 
 ## Using
 
 There are several interfaces for the application.
 
+You can always find out what interfaces exist with:
+
+```shell
+exodus --help
+```
+
+Similarly, you can get help for a specific interface with:
+
+```shell
+exodus <interface> --help
+````
+
 If you want to get works and files, and you have metadata files, use:
 
 ```shell
 exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
 ```
 
 If you want to get works and files, and you don't have metadata files, you need to specify
@@ -94,14 +106,20 @@
 
 If you want to generate a full template for a metadata import, use:
 
 ```shell
 exodus generate_template --model book -o /path/to/sheet.csv
 ```
 
+If you want to generate a sheet of checksums for files that failed to import, you can:
+
+```shell
+exodus hash_errors --path /path/to/directory --output /path/to/sheet.csv
+```
+
 ## What's Missing Here Right Now
 
 * The ability to create pcdm:Collection objects.
 * The ability to create a new metadata import from a previous import
 
 ## Understanding Configs
```

