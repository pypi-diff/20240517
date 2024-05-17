# Comparing `tmp/nothingpy-0.1.2.tar.gz` & `tmp/nothingpy-0.1.3.tar.gz`

## Comparing `nothingpy-0.1.2.tar` & `nothingpy-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/nothingpy.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nothingpy-0.1.2/research/test_code.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nothingpy-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nothingpy-0.1.2/src/nothingpy/__init__.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nothingpy-0.1.2/src/nothingpy/nothing.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nothingpy-0.1.2/tests/test_nothing.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nothingpy-0.1.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nothingpy-0.1.2/LICENSE
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nothingpy-0.1.2/README.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nothingpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 nothingpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/nothingpy.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nothingpy-0.1.3/research/test_code.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nothingpy-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nothingpy-0.1.3/src/nothingpy/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nothingpy-0.1.3/src/nothingpy/nothing.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nothingpy-0.1.3/tests/test_nothing.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nothingpy-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nothingpy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 nothingpy-0.1.3/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nothingpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 nothingpy-0.1.3/PKG-INFO
```

### Comparing `nothingpy-0.1.2/.idea/workspace.xml` & `nothingpy-0.1.3/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `nothingpy-0.1.2/.idea/workspace.xml` & `nothingpy-0.1.3/.idea/workspace.xml`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="c99d3dba-5e42-43ed-82b8-79771bbb20da" name="Changes" comment="first checkin">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-    </list>
+    <list default="true" id="c99d3dba-5e42-43ed-82b8-79771bbb20da" name="Changes" comment="updated README.md"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -27,26 +24,27 @@
   &quot;associatedIndex&quot;: 5
 }</component>
   <component name="ProjectId" id="2gWNMSuwESURFguHOF8n16niuUS"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;ASKED_SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
-    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
-    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
-    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
-    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
-    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "ASKED_SHARE_PROJECT_CONFIGURATION_FILES": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "reference.settingsdialog.IDE.editor.colors.Python",
+    "vue.rearranger.settings.migration": "true"
   }
-}</component>
+}]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/nothingpy"/>
     </key>
   </component>
   <component name="SharedIndexes">
     <attachedChunks>
@@ -61,28 +59,37 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="c99d3dba-5e42-43ed-82b8-79771bbb20da" name="Changes" comment=""/>
       <created>1715809325353</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1715809325353</updated>
       <workItem from="1715809326394" duration="6150000"/>
-      <workItem from="1715817179021" duration="1805000"/>
+      <workItem from="1715817179021" duration="2573000"/>
     </task>
     <task id="LOCAL-00001" summary="first checkin">
       <option name="closed" value="true"/>
       <created>1715817854763</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1715817854763</updated>
     </task>
-    <option name="localTasksCounter" value="2"/>
+    <task id="LOCAL-00002" summary="updated README.md">
+      <option name="closed" value="true"/>
+      <created>1715819003709</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715819003709</updated>
+    </task>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="first checkin"/>
-    <option name="LAST_COMMIT_MESSAGE" value="first checkin"/>
+    <MESSAGE value="updated README.md"/>
+    <option name="LAST_COMMIT_MESSAGE" value="updated README.md"/>
   </component>
 </project>
```

### Comparing `nothingpy-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `nothingpy-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/research/test_code.py` & `nothingpy-0.1.3/research/test_code.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/src/nothingpy/__init__.py` & `nothingpy-0.1.3/src/nothingpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/src/nothingpy/nothing.py` & `nothingpy-0.1.3/src/nothingpy/nothing.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/tests/test_nothing.py` & `nothingpy-0.1.3/tests/test_nothing.py`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/.gitignore` & `nothingpy-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/LICENSE` & `nothingpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nothingpy-0.1.2/README.md` & `nothingpy-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # nothingpy
-Nothing is a replacement for None that eliminates the need for many if statements.  I am tried of writing code like this:
+Nothing is a replacement for None that eliminates the need for many if statements.  I am tired of writing code like this:
 
 ```python
-if some_list is not None:
+if some_list:
     for item in some_list:
         do_something(item)
 ```
 
 If you use Nothing instead of None, you can write code like this:
 
 ```python
-some_list = Nothing
 for item in some_list:
     do_something(item)
 ```
 
 **Nothing** is a global variable of the class NothingClass.  **Nothing** has a len of 0, is False, returns an empty iterable,
 converts to an empty string, and responds to values(), keys() and items() like an empty dictionary.  **Nothing** equals
 other NothingClass instances, None and False.
```

### Comparing `nothingpy-0.1.2/pyproject.toml` & `nothingpy-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "nothingpy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Tom Burns", email="public@llmonpy.ai" },
 ]
 description = "A None alternative for Python that reduces the need for None checks."
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
```

### Comparing `nothingpy-0.1.2/PKG-INFO` & `nothingpy-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.3
 Name: nothingpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A None alternative for Python that reduces the need for None checks.
 Project-URL: Homepage, https://github.com/llmonpy/nothingpy
 Project-URL: Issues, https://github.com/llmonpy/nothingpy/issues
 Author-email: Tom Burns <public@llmonpy.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
 # nothingpy
-Nothing is a replacement for None that eliminates the need for many if statements.  I am tried of writing code like this:
+Nothing is a replacement for None that eliminates the need for many if statements.  I am tired of writing code like this:
 
 ```python
-if some_list is not None:
+if some_list:
     for item in some_list:
         do_something(item)
 ```
 
 If you use Nothing instead of None, you can write code like this:
 
 ```python
-some_list = Nothing
 for item in some_list:
     do_something(item)
 ```
 
 **Nothing** is a global variable of the class NothingClass.  **Nothing** has a len of 0, is False, returns an empty iterable,
 converts to an empty string, and responds to values(), keys() and items() like an empty dictionary.  **Nothing** equals
 other NothingClass instances, None and False.
```

