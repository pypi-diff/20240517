# Comparing `tmp/bibla-2.0.4.tar.gz` & `tmp/bibla-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibla-2.0.4.tar", last modified: Sun May 12 13:53:33 2024, max compression
+gzip compressed data, was "bibla-2.0.5.tar", last modified: Fri May 17 21:30:29 2024, max compression
```

## Comparing `bibla-2.0.4.tar` & `bibla-2.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.398084 bibla-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-12 13:53:28.000000 bibla-2.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.390084 bibla-2.0.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-12 13:53:28.000000 bibla-2.0.4/.idea/biblint.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.390084 bibla-2.0.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 13:53:28.000000 bibla-2.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 13:53:28.000000 bibla-2.0.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-12 13:53:28.000000 bibla-2.0.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 13:53:28.000000 bibla-2.0.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-12 13:53:28.000000 bibla-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-12 13:53:28.000000 bibla-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-12 13:53:33.398084 bibla-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-12 13:53:28.000000 bibla-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.390084 bibla-2.0.4/bibla/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.394084 bibla-2.0.4/bibla/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/database_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13271 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/entry_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/field_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/specification_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/rules/text_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-12 13:53:28.000000 bibla-2.0.4/bibla/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.398084 bibla-2.0.4/bibla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 13:53:33.000000 bibla-2.0.4/bibla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:53:33.398084 bibla-2.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-12 13:53:28.000000 bibla-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.394084 bibla-2.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:28.000000 bibla-2.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 13:53:28.000000 bibla-2.0.4/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:33.398084 bibla-2.0.4/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/.bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/authorNameFormatting.bib
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/bibLaTeX.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/dateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/emptyEntries.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/mit.bib
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/noHomepages.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/nodirectives.bib
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/nokeys.bib
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/originalOverAlias.bib
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/pages.bib
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/required.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/shouldUseDateInsteadOfYearMonthDay.bib
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/suggestedFields.bib
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/syntax.bib
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/unique.bib
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/wrongDateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-12 13:53:28.000000 bibla-2.0.4/test_data/wrongFormatKey.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 21:30:22.000000 bibla-2.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.484213 bibla-2.0.5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/biblint.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.484213 bibla-2.0.5/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-17 21:30:22.000000 bibla-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-17 21:30:22.000000 bibla-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-17 21:30:29.496213 bibla-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-17 21:30:22.000000 bibla-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.488213 bibla-2.0.5/bibla/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.492213 bibla-2.0.5/bibla/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/database_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/entry_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/field_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/specification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/text_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/bibla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:30:29.496213 bibla-2.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-17 21:30:22.000000 bibla-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.492213 bibla-2.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:22.000000 bibla-2.0.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-17 21:30:22.000000 bibla-2.0.5/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/.bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/authorNameFormatting.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/bibLaTeX.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/dateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/emptyEntries.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/mit.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/noHomepages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/nodirectives.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/nokeys.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/originalOverAlias.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/pages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/required.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/shouldUseDateInsteadOfYearMonthDay.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/suggestedFields.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/syntax.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/unique.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/wrongDateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/wrongFormatKey.bib
```

### Comparing `bibla-2.0.4/.idea/biblint.iml` & `bibla-2.0.5/.idea/biblint.iml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/LICENSE` & `bibla-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/PKG-INFO` & `bibla-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.4
+Version: 2.0.5
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bibla-2.0.4/README.md` & `bibla-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/__main__.py` & `bibla-2.0.5/bibla/__main__.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/bibla.yml` & `bibla-2.0.5/bibla/bibla.yml`

 * *Files 6% similar despite different names*

```diff
@@ -78,8 +78,11 @@
     misc: [software]
     online: [electronic, www]
     inproceedings: [conference]
     report: [techreport]
     thesis: [mastersthesis, phdthesis]
 
 alternate_fields:
+  # preferred: [other]
   date: [year] # Month and day will not be used alone, so when we just check for the year, that'll be fine.
+  journaltitle: [journal]
+  institution: [school]
```

### Comparing `bibla-2.0.4/bibla/config.py` & `bibla-2.0.5/bibla/config.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/lint.py` & `bibla-2.0.5/bibla/lint.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/rule.py` & `bibla-2.0.5/bibla/rule.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/rules/database_rules.py` & `bibla-2.0.5/bibla/rules/database_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/rules/entry_rules.py` & `bibla-2.0.5/bibla/rules/entry_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,37 @@
 
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
     :return: True if the current entry's key has the specified format or
     year or author are not specified, False otherwise.
     """
-    if 'date' not in entry.fields or list(
-            itertools.chain(*entry.persons.values())).count == 0:
+    if 'date' not in entry.fields or len(entry.persons.get('author', [])) == 0:
         return True
-    author = entry.persons['author'][0]
-    names = author.rich_prelast_names + author.rich_last_names
+    try:
+        author = entry.persons['author'][0]
+    except KeyError:
+        try:
+            author = entry.persons['editor'][0]
+        except KeyError:
+            return True
+    names = author.rich_prelast_names + [name for last_name in author.rich_last_names for name in last_name.split('-')]
     date = entry.fields['date']
     year = re.search(r'\d{4}', date).group()
-    correct_key_unicode = "".join([str(name) for name in names]) + year
-    correct_key_ascii = unidecode(correct_key_unicode)
+
+    # Check for 'EtAl' in the key when there are more than 3 authors
+    if len(entry.persons.get('author', [])) >= 3 and 'EtAl' in key.lower():
+        correct_key_unicode = names[0] + 'EtAl' + year
+    # Check for two names in the key when there are exactly 2 authors
+    elif len(entry.persons.get('author', [])) == 2:
+        correct_key_unicode = "".join([str(name) for name in names[:2]]) + year
+    else:
+        correct_key_unicode = "".join([str(name) for name in names]) + year
+
+    correct_key_ascii = unidecode(str(correct_key_unicode))
     regex = re.compile(correct_key_ascii + r'[a-zA-Z]?')
     return bool(regex.match(key))
 
 
 @register_entry_rule('E01', 'Author first names should not be abbreviated')
 def author_first_name_abbr(key, entry, database):
     """Raise a linter warning when an author/editor first name is abbreviated.
```

### Comparing `bibla-2.0.4/bibla/rules/field_rules.py` & `bibla-2.0.5/bibla/rules/field_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/rules/specification_rules.py` & `bibla-2.0.5/bibla/rules/specification_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/rules/text_rules.py` & `bibla-2.0.5/bibla/rules/text_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla/text_utils.py` & `bibla-2.0.5/bibla/text_utils.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/bibla.egg-info/PKG-INFO` & `bibla-2.0.5/bibla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.4
+Version: 2.0.5
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bibla-2.0.4/bibla.egg-info/SOURCES.txt` & `bibla-2.0.5/bibla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/setup.py` & `bibla-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/test_data/bibLaTeX.bib` & `bibla-2.0.5/test_data/bibLaTeX.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/test_data/mit.bib` & `bibla-2.0.5/test_data/mit.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/test_data/nodirectives.bib` & `bibla-2.0.5/test_data/nodirectives.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/test_data/originalOverAlias.bib` & `bibla-2.0.5/test_data/originalOverAlias.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.4/test_data/wrongDateFormat.bib` & `bibla-2.0.5/test_data/wrongDateFormat.bib`

 * *Files identical despite different names*

