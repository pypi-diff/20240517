# Comparing `tmp/pgs3-0.0.2.tar.gz` & `tmp/pgs3-0.0.3.tar.gz`

## Comparing `pgs3-0.0.2.tar` & `pgs3-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/pg-utils.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pgs3-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pgs3-0.0.2/src/pgs3/__init__.py
--rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 pgs3-0.0.2/src/pgs3/cli.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pgs3-0.0.2/.gitignore
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pgs3-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pgs3-0.0.2/readme.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pgs3-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/pg-utils.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pgs3-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pgs3-0.0.3/src/pgs3/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pgs3-0.0.3/src/pgs3/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 pgs3-0.0.3/src/pgs3/cli.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pgs3-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pgs3-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 pgs3-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pgs3-0.0.3/readme.md
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pgs3-0.0.3/PKG-INFO
```

### Comparing `pgs3-0.0.2/.idea/pg-utils.iml` & `pgs3-0.0.3/.idea/pg-utils.iml`

 * *Files identical despite different names*

### Comparing `pgs3-0.0.2/.idea/workspace.xml` & `pgs3-0.0.3/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `pgs3-0.0.2/.idea/workspace.xml` & `pgs3-0.0.3/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="0e73f781-6b46-4562-8d98-e4dbeea57c4a" name="Changes" comment="">
+      <change afterPath="$PROJECT_DIR$/LICENSE.txt" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/src/pgs3/__about__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/pgs3/cli.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/pgs3/cli.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
@@ -22,36 +24,43 @@
         <entry key="$USER_HOME$/code/dev/hooray-gradle" value="PREVIEW"/>
       </map>
     </option>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
-  <component name="ProjectColorInfo"><![CDATA[{
-  "associatedIndex": 3
-}]]></component>
+  <component name="ProjectColorInfo">{
+  &quot;associatedIndex&quot;: 3
+}</component>
   <component name="ProjectId" id="2g2ri54Ft02SNXj85CoNvXV5qVo"/>
   <component name="ProjectViewState">
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
     "git-widget-placeholder": "main",
+    "last_opened_file_path": "/Users/haowu4/code-new/pg-utils/src/pgs3",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
+  <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$/src/pgs3"/>
+      <recent name="$PROJECT_DIR$"/>
+    </key>
+  </component>
   <component name="RunManager">
     <configuration default="true" type="Application" factoryName="Application">
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <method v="2">
         <option name="Make" enabled="true"/>
       </method>
     </configuration>
@@ -76,15 +85,17 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="0e73f781-6b46-4562-8d98-e4dbeea57c4a" name="Changes" comment=""/>
       <created>1714906637309</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714906637309</updated>
-      <workItem from="1714906638368" duration="2014000"/>
+      <workItem from="1714906638368" duration="3368000"/>
+      <workItem from="1715929694228" duration="2192000"/>
+      <workItem from="1715953369581" duration="798000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `pgs3-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `pgs3-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pgs3-0.0.2/src/pgs3/cli.py` & `pgs3-0.0.3/src/pgs3/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,17 @@
 
 
 # Fetch backups from S3
 def list_backups(config: Config) -> list[str]:
     """
     Return a list of versions from the provided config.
     For example if the following path exists:
-        ${config.s3.path}/20200101_120000/db_dump.sql
-        ${config.s3.path}/20200101_120000/schema_dump.sql
-        ${config.s3.path}/20190202_110000/schema_dump.sql
+        ${config.s3.path}/20200101_120000/db_dump.pgdump
+        ${config.s3.path}/20200101_120000/schema_dump.pgdump
+        ${config.s3.path}/20190202_110000/schema_dump.pgdump
 
     This function should return ['20200101_120000', '20200202_110000']
 
     """
     client = s3_client(config)
     bucket_path = config.s3.path
     paginator = client.get_paginator('list_objects_v2')
@@ -247,15 +247,15 @@
 @cli.command(name='init')
 @click.option('-p', '--profile', default=DEFAULT_PROFILE, help='Path to the JSON profile configuration file')
 def cmd_init(profile):
     create_config(profile)
 
 
 @cli.command(name='backup')
-@click.option('--schema-only', '-s', is_flag=True, help='Backup only the schema without data')
+@click.option('--schema-only', '-s', is_flag=True, default=False, help='Backup only the schema without data')
 @click.option('-p', '--profile', default=DEFAULT_PROFILE, help='Path to the JSON profile configuration file')
 @click.option('--upload', '-u', is_flag=True, show_default=True, default=False, help='Upload back to s3.')
 def cmd_backup(schema_only, profile, upload):
     config = get_profile(profile)
     backup(config, schema_only, upload)
```

### Comparing `pgs3-0.0.2/.gitignore` & `pgs3-0.0.3/.gitignore`

 * *Files identical despite different names*

