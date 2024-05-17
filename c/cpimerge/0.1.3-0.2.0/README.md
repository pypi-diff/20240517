# Comparing `tmp/cpimerge-0.1.3.tar.gz` & `tmp/cpimerge-0.2.0.tar.gz`

## Comparing `cpimerge-0.1.3.tar` & `cpimerge-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.3/src/cpimerge/__init__.py
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 cpimerge-0.1.3/src/cpimerge/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.3/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/__main__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/backup.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/config.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/descriptions.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/exclusions.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/gui.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/ical.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/load.py
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 cpimerge-0.2.0/src/cpimerge/merge.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cpimerge-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.2.0/PKG-INFO
```

### Comparing `cpimerge-0.1.3/.gitignore` & `cpimerge-0.2.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -154,7 +154,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# Test files
+tests/
```

### Comparing `cpimerge-0.1.3/LICENSE` & `cpimerge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.1.3/pyproject.toml` & `cpimerge-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
```

