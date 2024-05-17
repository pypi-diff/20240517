# Comparing `tmp/ru_text_cleaner-1.1.2.tar.gz` & `tmp/ru_text_cleaner-1.1.3.tar.gz`

## Comparing `ru_text_cleaner-1.1.2.tar` & `ru_text_cleaner-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/requirements.txt
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     8551 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/TextCleaner.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_to_lower.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/src/ru_text_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/requirements.txt
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/PKG-INFO
```

### Comparing `ru_text_cleaner-1.1.2/.idea/workspace.xml` & `ru_text_cleaner-1.1.3/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `ru_text_cleaner-1.1.2/.idea/workspace.xml` & `ru_text_cleaner-1.1.3/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Upload settings">
-      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/_spaces_cleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/_spaces_cleaner.py" afterDir="false"/>
+    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Delete empty unicode symbols">
+      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/_punctuation_cleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/_punctuation_cleaner.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -182,23 +182,32 @@
       <option name="closed" value="true"/>
       <created>1715950877729</created>
       <option name="number" value="00014"/>
       <option name="presentableId" value="LOCAL-00014"/>
       <option name="project" value="LOCAL"/>
       <updated>1715950877729</updated>
     </task>
-    <option name="localTasksCounter" value="15"/>
+    <task id="LOCAL-00015" summary="Delete empty unicode symbols">
+      <option name="closed" value="true"/>
+      <created>1715956517131</created>
+      <option name="number" value="00015"/>
+      <option name="presentableId" value="LOCAL-00015"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715956517131</updated>
+    </task>
+    <option name="localTasksCounter" value="16"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="More functions v1.0"/>
     <MESSAGE value="Support only russian language"/>
     <MESSAGE value="README.md"/>
     <MESSAGE value="File configuration"/>
     <MESSAGE value="Prepare for downloading to upload"/>
     <MESSAGE value="Stable version for uploading"/>
     <MESSAGE value="Mirror update"/>
     <MESSAGE value="New README"/>
     <MESSAGE value="Upload settings"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Upload settings"/>
+    <MESSAGE value="Delete empty unicode symbols"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Delete empty unicode symbols"/>
   </component>
 </project>
```

### Comparing `ru_text_cleaner-1.1.2/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-1.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/src/ru_text_cleaner/TextCleaner.py` & `ru_text_cleaner-1.1.3/src/ru_text_cleaner/TextCleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/src/ru_text_cleaner/_clean_stopwords.py` & `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_clean_stopwords.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/src/ru_text_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_spaces_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/src/ru_text_cleaner/_to_morpheme.py` & `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_morpheme.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/LICENSE` & `ru_text_cleaner-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/README.md` & `ru_text_cleaner-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.2/pyproject.toml` & `ru_text_cleaner-1.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     { name="Vildan Nasyrov", email="" },
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
 ]
-description = "Prepare russian text for NLTK"
+description = "Prepare russian text for NLP"
 requires-python = ">=3.10.4"
 readme = "README.md"
 classifiers = [
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent",
 ]
```

### Comparing `ru_text_cleaner-1.1.2/PKG-INFO` & `ru_text_cleaner-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 1.1.2
-Summary: Prepare russian text for NLTK
+Version: 1.1.3
+Summary: Prepare russian text for NLP
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

