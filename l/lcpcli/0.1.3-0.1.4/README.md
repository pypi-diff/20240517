# Comparing `tmp/lcpcli-0.1.3.tar.gz` & `tmp/lcpcli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcpcli-0.1.3.tar", last modified: Mon Apr 29 16:56:20 2024, max compression
+gzip compressed data, last modified: Fri May 17 15:31:23 2024, max compression
```

## Comparing `lcpcli-0.1.3.tar` & `lcpcli-0.1.4.tar`

### file list

```diff
@@ -1,71 +1,22 @@
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.000000 lcpcli-0.1.3/LICENSE.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)    11986 2024-04-29 16:56:20.530002 lcpcli-0.1.3/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    11021 2024-04-09 11:16:26.000000 lcpcli-0.1.3/README.md
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/bin/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       41 2023-12-05 17:05:43.000000 lcpcli-0.1.3/bin/lcpcli
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/_legacy_process_files/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16490 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/_legacy_process_files/process_opensubtitles.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    12104 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/_legacy_process_files/process_sparcling.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/corpert/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17713 2024-02-28 15:54:29.000000 lcpcli-0.1.3/corpert/build/lib/corpert/corpert.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3039 2024-02-28 15:58:27.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/_parser.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     7418 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/conllu.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/json.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/tei.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/vert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13067 2024-02-29 13:04:27.000000 lcpcli-0.1.3/corpert/build/lib/corpert/utils.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/corpert/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2024-04-24 13:45:22.000000 lcpcli-0.1.3/corpert/corpert/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16353 2024-04-24 13:52:37.000000 lcpcli-0.1.3/corpert/corpert/corpert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13554 2024-04-12 14:57:44.000000 lcpcli-0.1.3/corpert/corpert/lcp_corpus_template.json
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/corpert/parsers/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/parsers/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    30262 2024-04-29 16:47:45.000000 lcpcli-0.1.3/corpert/corpert/parsers/_parser.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    12612 2024-04-24 14:00:59.000000 lcpcli-0.1.3/corpert/corpert/parsers/conllu.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/parsers/json.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/corpert/parsers/tei.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/corpert/parsers/vert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17393 2024-04-29 16:35:07.000000 lcpcli-0.1.3/corpert/corpert/utils.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       71 2024-03-18 14:41:46.000000 lcpcli-0.1.3/corpert/requirements.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      809 2023-12-06 14:34:53.000000 lcpcli-0.1.3/corpert/setup.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/lib/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/lcp_upload.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/lcp_upload/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/lcp_upload.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       89 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/requirements.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      761 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/setup.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcpcli/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       50 2023-12-05 17:03:46.000000 lcpcli-0.1.3/lcpcli/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      199 2023-12-05 17:04:24.000000 lcpcli-0.1.3/lcpcli/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2843 2023-12-06 14:11:50.000000 lcpcli-0.1.3/lcpcli/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2371 2024-03-18 16:39:46.000000 lcpcli-0.1.3/lcpcli/lcpcli.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcpcli.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)    11986 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1614 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      162 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/requires.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       26 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2023-12-06 08:55:49.000000 lcpcli-0.1.3/lcpcli.egg-info/zip-safe
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1062 2024-04-29 16:56:13.000000 lcpcli-0.1.3/pyproject.toml
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-29 16:56:20.530002 lcpcli-0.1.3/setup.cfg
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      735 2024-02-28 10:19:59.000000 lcpcli-0.1.3/setup.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       64 2024-05-17 15:31:05.345346 lcpcli-0.1.4/lcpcli/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      161 2024-05-14 08:47:56.898196 lcpcli-0.1.4/lcpcli/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3204 2024-05-17 13:57:47.026392 lcpcli-0.1.4/lcpcli/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    18686 2024-05-17 08:35:50.371521 lcpcli-0.1.4/lcpcli/corpert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14826 2024-05-17 13:58:07.910331 lcpcli-0.1.4/lcpcli/lcp_upload.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2379 2024-05-14 08:47:56.898196 lcpcli-0.1.4/lcpcli/lcpcli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16619 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/utils.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13554 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/data/lcp_corpus_template.json
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2453 2024-05-02 11:39:20.926734 lcpcli-0.1.4/lcpcli/data/input/in.conllu
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      669 2024-05-02 11:39:20.926734 lcpcli-0.1.4/lcpcli/data/input/in.vert
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)   581704 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/data/input/in_tei_spoken.xml
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    32245 2024-05-17 08:20:09.846874 lcpcli-0.1.4/lcpcli/parsers/_parser.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14009 2024-05-17 08:20:14.054914 lcpcli-0.1.4/lcpcli/parsers/conllu.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/json.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/tei.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/vert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       81 2023-12-06 14:33:04.945962 lcpcli-0.1.4/.gitignore
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.083400 lcpcli-0.1.4/LICENSE.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14025 2024-05-17 15:26:55.848466 lcpcli-0.1.4/README.md
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2474 2024-05-02 11:39:20.930734 lcpcli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    15173 2024-05-17 15:31:23.000000 lcpcli-0.1.4/PKG-INFO
```

### Comparing `lcpcli-0.1.3/LICENSE.txt` & `lcpcli-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.3/PKG-INFO` & `lcpcli-0.1.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: lcpcli
-Version: 0.1.3
-Summary: Helper for converting CONLLU files and uploading the corpus to LCP
-Home-page: 
-Author: Jeremy Zehr and Jonathan Schaber
-Author-email: Jeremy Zehr <jeremy.zehr@uzh.ch>
-Project-URL: Homepage, https://gitlab.uzh.ch/LiRI/projects/lcpcli
-Project-URL: Issues, https://gitlab.uzh.ch/LiRI/projects/lcpcli/-/issues
-Keywords: corpus,linguistics,corpora,conll,tei,vert
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: lxml>=4.7.1
-Requires-Dist: lupa>=1.13
-Requires-Dist: xmltodict>=0.13
-Requires-Dist: jsonpickle>=3.0
-Requires-Dist: jsonschema>=4.21
-Requires-Dist: requests>=2.30.0
-Requires-Dist: py7zr>=0.20.5
-Requires-Dist: tqdm>=4.65.0
-Requires-Dist: types-tqdm>=4.65.0.1
-Requires-Dist: types-requests>=2.30.0.0
-
 # LCP CLI module
 
 > Command-line tool for converting CONLLU files and uploading the corpus to LCP
 
 ## Installation
 
 Make sure you have python 3.11+ with `pip` installed in your local environment, then run
@@ -133,14 +106,50 @@
         }
     }
 },
 ```
 
 Make sure to set the `abstract`, `layerType` and `contains` attributes as illustrated above. See the section [Convert and Upload](#convert-and-upload) for a full example of a template `.json` file.
 
+#### Other anchored entities
+
+Your corpus can include other entities besides tokens, sentences, documents and annotations that enter in a subset/superset relation with those. For example, a video corpus could include _gestures_ that are **time-anchored** but do not necessarily align with tokens or segments on the time axis (e.g. a gesture could start in the middle of a sentence and end some time after its end)
+
+In such a case, your template `.json` file should report that entity under `layer`, for example:
+
+```json
+"Gesture": {
+    "abstract": false,
+    "layerType": "unit",
+    "anchoring": {
+        "location": false,
+        "stream": false,
+        "time": true
+    },
+    "attributes": {
+        "name": {
+            "type": "categorical",
+            "values": [
+                "waving",
+                "thumbsup"
+            ]
+        }
+    }
+},
+```
+
+Much like in the case of named entities described above, you should also include a TSV file that lists the entities, named `<entity>.csv`. The first column should be named `<entity>_id` and list unique IDs; one column should be named `doc_id` and report the ID of the corresponding document (make sure to include corresponding `# newdoc id = <ID>` comments in your CoNLLU files); two columns named `start` and `end` should list the time points for temporal anchoring, measured in seconds from the start of the document's media file; with additional columns for the entity's attributes. For example, `gesture.csv`:
+
+```tsv
+gesture_id	doc_id	start	end	name
+1	video1	1.2	3.5	waving
+2	video1	2.3	4.7	thumbsup
+3	video2	3.2	4.5	thumbsup
+4	video2	8.3	9.7	waving
+```
 
 #### Global attributes
 
 In some cases, it makes sense for multiple entity types to share references: in those cases, they can define _global attributes_. An example of a global attribute is a speaker or an agent that can have a name, an age, etc. and be associated with both a segment (a sentence) and, say, a gesture. The corpus template would include definitions along these lines:
 
 ```json
 "globalAttributes": {
@@ -178,35 +187,58 @@
                 "ref": "agent"
             }
         }
     }
 }
 ```
 
-You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.tsv`. For example:
+You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.csv`. For example:
 
-*global_attribute_agent.tsv*:
+*global_attribute_agent.csv*:
 ```tsv
 agent_id	agent
 10	{"name": "Jane Doe", "age": 37}
 ```
 
 CoNLL-U file:
 ```conllu
+# newdoc id = video1
+
 # sent_id = 1
 # agent_id = 10
 The the _ _ _
 ```
 
-*gesture.tsv*:
+*gesture.csv*:
+```tsv
+gesture_id	agent_id	doc_id	start	end
+1	10	video1	1.25	2.6
+```
+
+#### Media files
+
+If your corpus include media files, your `.json` template should report it under a main `mediaSlots` key, e.g.:
+
+```json
+"mediaSlots": {
+    "interview": {
+        "type": "audio",
+        "isOptional": false
+    }
+}
+```
+
+Your CoNLL-U file(s) should accordingly report each document's media file's name in a comment, like so:
+
 ```tsv
-gesture_id	agent_id	frame_range
-1	10	[2345,5678]
+# newdoc interview = itvw1.mp3
 ```
 
+Finally, your **output** corpus folder should include a subfolder named `media` in which all the referenced media files have been placed
+
 
 ### Convert and Upload
 
 1. Create a directory in which you have all your properly-fromatted CONLLU files
 
 2. In the same directory, create a template `.json` file that describes your corpus structure (see above about the `attributes` key on `Document` and `Segment`), for example:
 
@@ -215,14 +247,20 @@
     "meta":{
         "name":"My corpus",
         "author":"Myself",
         "date":"2023",
         "version": 1,
         "corpusDescription":"This is my corpus"
     },
+    "mediaSlots": {
+        "interview": {
+            "type": "audio",
+            "isOptional": false
+        }
+    },
     "firstClass": {
         "document": "Document",
         "segment": "Segment",
         "token": "Token"
     },
     "layer": {
         "Token": {
@@ -268,18 +306,35 @@
                         "MISC",
                         "ORG"
                     ],
                     "nullable": true
                 }
             }
         },
+        "Gesture": {
+            "abstract": false,
+            "layerType": "unit",
+            "anchoring": {
+                "time": true
+            },
+            "attributes": {
+                "agent": {
+                    "ref": "agent"
+                }
+            }
+        },
         "Segment": {
             "abstract": false,
             "layerType": "span",
-            "contains": "Token"
+            "contains": "Token",
+            "attributes": {
+                "agent": {
+                    "ref": "agent"
+                }
+            }
         },
         "Document": {
             "abstract": false,
             "contains": "Segment",
             "layerType": "span",
             "attributes": {
                 "meta": {
@@ -298,14 +353,27 @@
                     "Titel": {
                         "type": "text",
                         "nullable": true
                     }
                 }
             }
         }
+    },
+    "globalAttributes": {
+        "agent": {
+            "type": "dict",
+            "keys": {
+                "name": {
+                    "type": "text"
+                },
+                "age": {
+                    "type": "number"
+                }
+            }
+        }
     }
 }
 ```
 
 3. If your corpus defines a character-anchored entity type such as named entities, make sure you also include a properly named and formatted TSV file for it in the directory (see [the Named Entities section](#named-entities))
 
 4. Visit an LCP instance (e.g. _catchphrase_) and create a new project if you don't already have one where your corpus should go
```

### Comparing `lcpcli-0.1.3/README.md` & `lcpcli-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.3
+Name: lcpcli
+Version: 0.1.4
+Summary: Helper for converting CONLLU files and uploading the corpus to LiRI Corpus Platform (LCP)
+Project-URL: Homepage, https://github.com/liri-uzh/lcpcli/issues
+Project-URL: Issues, https://github.com/liri-uzh/lcpcli/issues
+Author-email: Danny McDonald <daniel.mcdonald@uzh.ch>, Igor Mustač <igor.mustac@uzh.ch>, Jeremy Zehr <jeremy.zehr@uzh.ch>, Jonathan Schaber <jeremy.schaber@uzh.ch>
+License: MIT
+License-File: LICENSE.txt
+Keywords: CONLL,TEI,VERT,corpora,corpus,linguistics
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: jsonpickle>=3.0
+Requires-Dist: jsonschema>=4.21
+Requires-Dist: lupa>=1.13
+Requires-Dist: lxml>=4.7.1
+Requires-Dist: py7zr>=0.20.5
+Requires-Dist: requests>=2.30.0
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: types-requests>=2.30.0.0
+Requires-Dist: types-tqdm>=4.65.0.1
+Requires-Dist: xmltodict>=0.13
+Description-Content-Type: text/markdown
+
 # LCP CLI module
 
 > Command-line tool for converting CONLLU files and uploading the corpus to LCP
 
 ## Installation
 
 Make sure you have python 3.11+ with `pip` installed in your local environment, then run
@@ -106,14 +134,50 @@
         }
     }
 },
 ```
 
 Make sure to set the `abstract`, `layerType` and `contains` attributes as illustrated above. See the section [Convert and Upload](#convert-and-upload) for a full example of a template `.json` file.
 
+#### Other anchored entities
+
+Your corpus can include other entities besides tokens, sentences, documents and annotations that enter in a subset/superset relation with those. For example, a video corpus could include _gestures_ that are **time-anchored** but do not necessarily align with tokens or segments on the time axis (e.g. a gesture could start in the middle of a sentence and end some time after its end)
+
+In such a case, your template `.json` file should report that entity under `layer`, for example:
+
+```json
+"Gesture": {
+    "abstract": false,
+    "layerType": "unit",
+    "anchoring": {
+        "location": false,
+        "stream": false,
+        "time": true
+    },
+    "attributes": {
+        "name": {
+            "type": "categorical",
+            "values": [
+                "waving",
+                "thumbsup"
+            ]
+        }
+    }
+},
+```
+
+Much like in the case of named entities described above, you should also include a TSV file that lists the entities, named `<entity>.csv`. The first column should be named `<entity>_id` and list unique IDs; one column should be named `doc_id` and report the ID of the corresponding document (make sure to include corresponding `# newdoc id = <ID>` comments in your CoNLLU files); two columns named `start` and `end` should list the time points for temporal anchoring, measured in seconds from the start of the document's media file; with additional columns for the entity's attributes. For example, `gesture.csv`:
+
+```tsv
+gesture_id	doc_id	start	end	name
+1	video1	1.2	3.5	waving
+2	video1	2.3	4.7	thumbsup
+3	video2	3.2	4.5	thumbsup
+4	video2	8.3	9.7	waving
+```
 
 #### Global attributes
 
 In some cases, it makes sense for multiple entity types to share references: in those cases, they can define _global attributes_. An example of a global attribute is a speaker or an agent that can have a name, an age, etc. and be associated with both a segment (a sentence) and, say, a gesture. The corpus template would include definitions along these lines:
 
 ```json
 "globalAttributes": {
@@ -151,35 +215,58 @@
                 "ref": "agent"
             }
         }
     }
 }
 ```
 
-You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.tsv`. For example:
+You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.csv`. For example:
 
-*global_attribute_agent.tsv*:
+*global_attribute_agent.csv*:
 ```tsv
 agent_id	agent
 10	{"name": "Jane Doe", "age": 37}
 ```
 
 CoNLL-U file:
 ```conllu
+# newdoc id = video1
+
 # sent_id = 1
 # agent_id = 10
 The the _ _ _
 ```
 
-*gesture.tsv*:
+*gesture.csv*:
+```tsv
+gesture_id	agent_id	doc_id	start	end
+1	10	video1	1.25	2.6
+```
+
+#### Media files
+
+If your corpus include media files, your `.json` template should report it under a main `mediaSlots` key, e.g.:
+
+```json
+"mediaSlots": {
+    "interview": {
+        "type": "audio",
+        "isOptional": false
+    }
+}
+```
+
+Your CoNLL-U file(s) should accordingly report each document's media file's name in a comment, like so:
+
 ```tsv
-gesture_id	agent_id	frame_range
-1	10	[2345,5678]
+# newdoc interview = itvw1.mp3
 ```
 
+Finally, your **output** corpus folder should include a subfolder named `media` in which all the referenced media files have been placed
+
 
 ### Convert and Upload
 
 1. Create a directory in which you have all your properly-fromatted CONLLU files
 
 2. In the same directory, create a template `.json` file that describes your corpus structure (see above about the `attributes` key on `Document` and `Segment`), for example:
 
@@ -188,14 +275,20 @@
     "meta":{
         "name":"My corpus",
         "author":"Myself",
         "date":"2023",
         "version": 1,
         "corpusDescription":"This is my corpus"
     },
+    "mediaSlots": {
+        "interview": {
+            "type": "audio",
+            "isOptional": false
+        }
+    },
     "firstClass": {
         "document": "Document",
         "segment": "Segment",
         "token": "Token"
     },
     "layer": {
         "Token": {
@@ -241,18 +334,35 @@
                         "MISC",
                         "ORG"
                     ],
                     "nullable": true
                 }
             }
         },
+        "Gesture": {
+            "abstract": false,
+            "layerType": "unit",
+            "anchoring": {
+                "time": true
+            },
+            "attributes": {
+                "agent": {
+                    "ref": "agent"
+                }
+            }
+        },
         "Segment": {
             "abstract": false,
             "layerType": "span",
-            "contains": "Token"
+            "contains": "Token",
+            "attributes": {
+                "agent": {
+                    "ref": "agent"
+                }
+            }
         },
         "Document": {
             "abstract": false,
             "contains": "Segment",
             "layerType": "span",
             "attributes": {
                 "meta": {
@@ -271,14 +381,27 @@
                     "Titel": {
                         "type": "text",
                         "nullable": true
                     }
                 }
             }
         }
+    },
+    "globalAttributes": {
+        "agent": {
+            "type": "dict",
+            "keys": {
+                "name": {
+                    "type": "text"
+                },
+                "age": {
+                    "type": "number"
+                }
+            }
+        }
     }
 }
 ```
 
 3. If your corpus defines a character-anchored entity type such as named entities, make sure you also include a properly named and formatted TSV file for it in the directory (see [the Named Entities section](#named-entities))
 
 4. Visit an LCP instance (e.g. _catchphrase_) and create a new project if you don't already have one where your corpus should go
```

### Comparing `lcpcli-0.1.3/corpert/_legacy_process_files/process_opensubtitles.py` & `lcpcli-0.1.4/lcpcli/corpert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,533 +1,474 @@
-import csv
-import uuid
-import lzma
-import re
+import codecs
+import json
+import os
+import shutil
+
+from .parsers.conllu import CONLLUParser
+from .parsers.vert import VERTParser
+from .parsers.tei import TEIParser
+from .parsers.json import JSONParser
+
+from .cli import _parse_cmd_line
+from .utils import default_json
+
+from jsonschema import validate
+from pathlib import Path
+
+# map between extensions and parsers
+PARSERS = {
+    "conllu": CONLLUParser,
+    "vert": VERTParser,
+    "xml": TEIParser,
+    "tei": TEIParser,
+    "json": JSONParser,
+}
+
+ERROR_MSG = """
+Unrecognized input format.
+Note: The converter currently supports the following formats:
+.conllu, .xml (TEI), .json and .vert.
+"""
 
-from datetime import timedelta
-from timeit import default_timer as timer
-
-
-green = "\033[92m"
-end = "\033[0m"
-
-
-### DATA & WRITE FILES
-
-PREFIX    = "/srv/data/jonathan/open_subtitles_en/"
-
-DEPREL_F1  = PREFIX + "deprel1.csv"
-DEPREL_F2  = PREFIX + "deprel2.csv"
-LINES_F1   = PREFIX + "lines1.csv"
-LINES_F2   = PREFIX + "lines2.csv"
-SEGMENT_F1 = PREFIX + "segment1.csv"
-SEGMENT_F2 = PREFIX + "segment2.csv"
-FTS_F1     = PREFIX + "fts_vector1.csv"
-FTS_F2     = PREFIX + "fts_vector2.csv"
-DOC_F      = PREFIX + "document.csv"
-WORD_F     = PREFIX + "word.csv"
-LEMMA_F    = PREFIX + "lemma.csv"
-UFEAT_F    = PREFIX + "ufeat.csv"
-XPOS_F     = PREFIX + "xpos.csv"
-
-DATA_F    = "/home/jonathan/TEMP_DIR/Projects/LCP/corpora/OpenSubtitles/OpenSubtitles_en.stanza.tsv.xz"
-
-
-
-def user_confirmation(message):
-    conf = input(message)
-
-    if conf.lower() != "y":
-        print("aborting.")
-        exit(1)
-
-
-class MyDict:
-    def __init__(self, is_ufeat=False):
-        self._dictionary = {}
-        self._max        = 1
-        self._is_ufeat   = is_ufeat
-
-    def __str__(self):
-        return str(self._dictionary)
-
-    def update(self, value):
-        if self._is_ufeat and value == '{"_"}':
-            return
-
-        if value and value not in self._dictionary:
-            self._dictionary[value] = self._max
-            self._max += 1
-
-    def get(self, value):
-        return self._dictionary.get(value, None)
-
-
-class GlobalState:
-    word      = MyDict()
-    lemma     = MyDict()
-    ufeats    = MyDict(is_ufeat=True)
-    xpos      = set()
-    docs      = {}
-    in_id_doc = False
-    no_id     = 0
-    cur_idx   = 1
-    cur_word  = 1
-    cur_seg   = uuid.uuid4()
-    left      = 1
-    right     = 2
-
-
-# TODO: not in use yet...
-# class TokenData:
-#     def __init__(self    , word_id, form_id,
-#                  lemma_id, upos   , xpos   , ufeats,
-#                  s_idx   , e_idx  , seg_id , deprel):
-#         self.word_id  = word_id
-#         self.form_id  = form_id
-#         self.lemma_id = lemma_id
-#         self.upos     = upos
-#         self.xpos     = xpos
-#         self.ufeats   = ufeats
-#         self.s_idx    = s_idx
-#         self.e_idx    = e_idx
-#         self.seg_id   = seg_id
-#         self.deprel   = deprel
-
-
-class Sentence:
-    _id_pat    = re.compile(r"^# id=(\d+)?")
-    _start_pat = re.compile(r"(?<=S=).+$")
-    _end_pat   = re.compile(r"(?<=E=).+$")
-
-    @staticmethod
-    def underscore2null(value):
-        if value == "_":
-            return None
-        else:
-            return value
 
+class Corpert:
     @staticmethod
-    def valid_lines(lines):
-        ret_lines = []
-        for line in lines:
-            if line.startswith("#"):
-                continue
-            split_l = line.split("\t")
-            if "-" in split_l[0]:
-                continue
-            ret_lines.append(split_l)
-
-        return ret_lines
-
-    @staticmethod
-    def jsonify_ufeats(string):
-        # change angular brackets to parens
-        string = string.replace("[", "(").replace("]", ")")
-        # put alternatves inside JSON-array
-        string = re.sub(r"(\w+,\s*\w+)", r"[\1]", string)
-        # convert pipes -separator to comma
-        string = string.replace("|", ",")
-        # converts equal to colon
-        string = string.replace("=", ":")
-        # surround literals with double quotes
-        string = re.sub(r"([\w()]+)", r'"\1"', string)
-
-        return "{" + string + "}"
+    def get_parsers():
+        return PARSERS
 
     @staticmethod
-    def _append(lst, elem):
-        """custom append function
-
-           in contrast to the built-in method, this function returns
-           the augmented list - useful for recursive calls
+    def mask(llist, n: int = 8):
         """
-        lst.append(elem)
+        computes a boolean mask to not write
+        columns that are always empty.
 
-        return lst
+        this is a simple heuristic which assumes that
+        attrobutes that are always empty are not specified
+        in the corpus template and therefore must not
+        be written to the files to upload
+
+        input is expected to be a list of
+        of Sentence.proc_lines instances
+        with a fixednumber of columns
+        (not more or less dims)
+        """
+        mask = []
+        for i in range(n):
+            mask.append(any([x[i] for y in llist for x in y]))
+
+        return mask
+
+    def __init__(
+        self,
+        content,
+        output=None,
+        extension=None,
+        filter=None,
+        lua_filter=None,
+        combine=True,
+        mode=None,
+        **kwargs,
+    ):
+        """
+        path (str): path or string of content
+        combine (bool): create single output file?
+        """
+        self.output = os.path.abspath(output) if output else None
+        self._output_format = None
+        self.mode = mode
+        if extension:
+            self._output_format = extension
+        elif self.output and self.output.endswith(
+            (".json", ".xml", ".conllu", ".vert", ".tei")
+        ):
+            self._output_format = os.path.splitext(self.output)[-1]
+        if self.output and not os.path.exists(self.output) and not combine:
+            os.makedirs(self.output)
+        self._filter = filter
+        self._lua_filter = lua_filter
+        self._lua = None
+        self._input_files = []
+        self._path = os.path.normpath(content)
+        self._combine = combine
+        self._on_disk = True
+        if os.path.isfile(content):
+            self._input_files.append(content)
+        elif os.path.isdir(content):
+            for root, dirs, files in os.walk(content):
+                for file in files:
+                    fullpath = os.path.join(root, file)
+                    self._input_files.append(fullpath)
+        elif isinstance(content, str):
+            self._input_files.append(content)
+            self._on_disk = False
+        else:
+            raise ValueError(ERROR_MSG)
 
-    @staticmethod
-    def _traverse(hierarchy, graph, ids):
-        """traverse flat list & build hierarchical structure
+    def __call__(self, *args, **kwargs):
+        """
+        Just allows us to do Corpert(**kwargs)()
+        """
+        return self.run(*args, **kwargs)
 
-           the flat structure is a parent: children dict
+    def _detect_format_from_string(self, content):
+        """
+        todo: this, but accurately!
         """
-        for id in ids:
-            hierarchy[id] = Sentence._traverse({}, graph, graph[id])
+        if "sent_id = " in content:
+            return "conllu"
+        elif "<xml" in content:
+            return "xml"
+        elif "<s sent_id" in content:
+            return "vert"
+        return "json"
 
-        return hierarchy
+    def _determine_format(self, filepath):
+        """
+        Deduce format from filepath, or from data string if need be
+        """
+        if os.path.isfile(filepath):
+            if filepath.endswith(".conllu"):
+                return "conllu"
+            elif filepath.endswith(".vert"):
+                return "vert"
+            elif filepath.endswith(".xml"):
+                return "xml"
+            elif filepath.endswith(".json"):
+                return "json"
+        elif isinstance(filepath, str):
+            return self._detect_format_from_string(filepath)
+        raise ValueError(ERROR_MSG)
 
-    @staticmethod
-    def _ord_keys(dic, key_list):
-        """traverse tree structure & build flat list
+    def _write_json(self, combined):
+        """
+        Create JSON file(s) depending on combine setting
+        """
+        if self._combine:
+            with open(self.output, "w") as fo:
+                json.dump(combined, fo, indent=4, sort_keys=False)
+        else:
+            for path, data in combined.items():
+                fixed_path = os.path.join(self.output, os.path.relpath(path))
+                if not os.path.isdir(os.path.dirname(fixed_path)):
+                    os.makedirs(os.path.dirname(fixed_path))
+                with open(fixed_path, "w") as fo:
+                    data = {path: data}
+                    json.dump(data, fo, indent=4, sort_keys=False)
 
+    def _write_to_file(self, filename, data):
+        """
+        Helper: write data to filename
         """
-        for el, vals in dic.items():
-            Sentence._ord_keys(vals, Sentence._append(key_list, el))
+        if not os.path.exists(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        with open(filename, "w") as fo:
+            fo.write(data)
 
-        return key_list
+    def _setup_filters(self):
+        """
+        If user wants to do lua/python filtering, we prepare things here
+        """
+        if self._lua_filter:
+            # import lupa
+            from lupa import LuaRuntime
+
+            self._lua = LuaRuntime(unpack_returned_tuples=True)
+        elif self._filter:
+            pass
 
-    @staticmethod
-    def _esc(string):
-        return string.replace("'", "''").replace("\\", "\\\\")
-        # return string
-
-    def __init__(self, lines, glob):
-        self._lines     = self.valid_lines(lines)
-        self._headers   = [x for x in lines if x.startswith("#")]
-        self._id        = None
-        self._start     = None
-        self._end       = None
-        self.glob       = glob
-        self.proc_lines = []
-        self.segment    = []
-        self.deprel     = []
-        self.fts_vector = []
-
-    def _scan_headers(self):
-        for line in self._headers:
-            id = re.search(self._id_pat, line)
-            if id:
-                if id[1]:
-                    self._id = id[1]
-                    if not self.glob.in_id_doc:
-                        self.glob.in_id_doc = True
-                else:
-                    if self.glob.in_id_doc:
-                        self.glob.no_id -= 1
-                        self.glob.in_id_doc = False
-                    self._id = str(self.glob.no_id)
-            start = re.search(self._start_pat, line)
-            if start:
-                self._start = start[0]
-            end = re.search(self._end_pat, line)
-            if end:
-                self._end = end[0]
-
-    def _tree_ins_order(self):
-        """ put list in hierarchical order for inserting
-
-            1. create dictionary structure (recursively)
-            2. flatten keys recursively into list
-            3. go over original list and append to
-               return list according to flattened keys
-        """
-        # index 2 = id, index 4 = head ATTENTION: adjust, if this changes!
-        id_par   = [(x[0], x[6]) for x in self._lines]
-        ret_list = []
-
-        # get root and check iff one
-        root = [id for (id, parent) in id_par if parent == "0"]
-        if len(root) != 1:
-            raise Exception("root error")
-
-        # flat parent:children mapping initialization
-        graph = {id: set() for (id, parent) in id_par}
-
-        # flat parent:children mapping building
-        for (id, parent) in id_par:
-            if parent != "0":
-                graph[parent].add(id)
-
-        # sorting in reverse, since inserting is done by shifting to the right
-        graph_sort = {k: sorted(v, key=lambda x: int(x), reverse=True) for k, v in graph.items()}
-
-        # build hierarchical structure
-        hier_ids = self._traverse({}, graph,  root)
-
-        # flatten keys into ordered list
-        flat_keys = self._ord_keys(hier_ids, [])
-
-        # re-order original rows for returning
-        for i in flat_keys:
-            for pair in id_par:
-                if pair[0] == i:
-                    ret_list.append(pair)
-                    continue
+    def _apply_lua_filter(self, content):
+        """
+        Run user's lua function on the JSON data for a file
+        """
+        with open(self._lua_filter, "r") as fo:
+            script = fo.read()
+        func = self._lua.eval(script)
+        return func(content)
 
-        return ret_list
+    def _apply_filter(self, content):
+        """
+        Run user's python function on the JSON data for a file
+        """
+        with open(self._filter, "r") as fo:
+            script = fo.read()
+        return exec(script, {}, {"content": content})
 
-    def _process_tree(self, ins, token_dict, tok_par_dict):
-        sent       = []
-        fts_str    = ""
-        root, rest = ins[0], ins[1:]
-        tree       = NestedSetTreeStructure(root[0], self.glob.left, self.glob.right)
-        for elem in rest:
-            tree.add_node(*elem)
-
-        # update globals
-        self.glob.left = max([x[1] for x in tree.nodes.values()]) + 1
-        self.glob.right = self.glob.left + 1
-
-        # look-up running indices and flatten into list
-        for k, v in tree.nodes.items():
-            token_id = token_dict[k][0]
-            deprel = token_dict[k][1]
-            head_id = token_dict[tok_par_dict[k]][0] if tok_par_dict[k] else None
-            sent.append((head_id, token_id, deprel, *v))
-
-        self.deprel += sent
-
-        # 4 = label_out (what am I?), 5 = labels_in (what do I encompass?)
-        tok_id2sent_idx = {v[0]: k for k, v in token_dict.items()}
-        for elem in sent:
-            fts_str += f" '4{elem[2]}':{tok_id2sent_idx[elem[1]]}"
-            fts_str += f" '5{elem[2]}':{tok_id2sent_idx[elem[1]]}"
-
-        return fts_str
-
-    def _process_lines(self):
-        # set up local variables
-        token_dict   = {}
-        tok_par_dict = {}
-        fts_str      = ""
-        start_char   = self.glob.cur_idx
-        end_char     = None
-
-        for line in self._lines:
-            w_id, word, lemma, upos, xpos, ufeats, p_id, deprel, _, _ = line
-
-            assert w_id
-            assert word
-
-            lemma, upos, xpos, ufeats, p_id, deprel = [self.underscore2null(x) for x in [lemma, upos, xpos, ufeats, p_id, deprel]]
-
-            l_word   = len(word)
-            end_char = self.glob.cur_idx + l_word
-            ufeats   = self.jsonify_ufeats(ufeats)
-
-            # update global dicts
-            self.glob.word.update(word)
-            self.glob.lemma.update(lemma)
-            self.glob.ufeats.update(ufeats)
-            self.glob.xpos.update(xpos)
-
-            # dictionary holding all info for 1 token
-            # TODO: this is not right 100% since w_id not always unique...
-            # word_id, form_fk, lemma_fk, upos, xpos, ufeat_fk, char_range, seg_fk
-            token_dict[w_id] = [
-                self.glob.cur_word,
-                self.glob.word.get(word),
-                self.glob.lemma.get(lemma),
-                upos,
-                xpos,
-                self.glob.ufeats.get(ufeats),
-                (self.glob.cur_idx, end_char),
-                self.glob.cur_seg,
-                deprel
-            ]
-
-            fts_str += f" '1{self._esc(word)}':{w_id} '2{self._esc(lemma)}':{w_id} '6{xpos}':{w_id} '3{upos}':{w_id}"
-
-            # update global word id and index
-            self.glob.cur_idx  += l_word
-            self.glob.cur_word += 1
-
-            tok_par_dict[w_id] = p_id if p_id != "0" else None
-
-        # create line entry for writing
-        self.proc_lines = [
-            line[:6]                         + \
-            [f"[{line[6][0]},{line[6][1]})"] + \
-            [line[7]] for line in token_dict.values()
-        ]
-
-        # build tree (if possible)
-        try:
-            ins = self._tree_ins_order()
-            fts = self._process_tree(ins, {k: (v[0], v[-1]) for k, v in token_dict.items()}, tok_par_dict)
-        except:
-            fts = ""
-
-        # create segment entry for writing
-        self.segment = [
-            self.glob.cur_seg,
-            f"[{start_char},{end_char})",
-            self._start,
-            self._end,
-            self._id
-        ]
-
-        self.fts_vector = [
-            self.glob.cur_seg,
-            f"{fts_str}{fts}"
-        ]
-
-
-        # set new segment id
-        self.glob.cur_seg = uuid.uuid4()
-
-
-        # create doc entry for writing
-        if self._id:
-            if self._id in self.glob.docs:
-                self.glob.docs[self._id][1] = end_char
+    def run(self):
+        """
+        The main routine: read in all input files and print/write them
+        """
+        combined = {}
+        self._setup_filters()
+        # sents = []
+        # docs = []
+
+        if self.mode == "upload":
+            ignore_files = set()
+            json_obj = None
+            json_file = next(
+                (
+                    os.path.join(self._path, f)
+                    for f in os.listdir(self._path)
+                    if f.endswith(".json")
+                ),
+                "",
+            )
+            if os.path.isfile(json_file):
+                ignore_files.add(json_file)
+                with open(json_file, "r") as jsf:
+                    json_obj = json.loads(jsf.read())
             else:
-                self.glob.docs[self._id] = [start_char, end_char]
+                json_obj = default_json(
+                    next(reversed(self._path.split(os.path.sep))) or "Anonymous Project"
+                )
+            parent_dir = os.path.dirname(__file__)
+            schema_path = os.path.join(parent_dir, "data", "lcp_corpus_template.json")
+            with open(schema_path) as schema_file:
+                validate(json_obj, json.loads(schema_file.read()))
+                print("validated json schema")
+
+            aligned_entities = {}
+            aligned_entities_segment = {}
+            firstClass = json_obj.get("firstClass", {})
+            # Detect the global attributes files and exclude them from the list of files to process
+            for glob_attr in json_obj.get("globalAttributes", {}):
+                filename = f"global_attribute_{glob_attr}.csv"
+                source = os.path.join(self._path, filename)
+                ignore_files.add(source)
+                if os.path.exists(source):
+                    shutil.copy(source, os.path.join(self.output or "./", filename))
+            # Parse the input files that are not at the token, segment or document level
+            for layer, properties in json_obj.get("layer", {}).items():
+                if layer in firstClass.values():
+                    continue
+                if (
+                    properties.get("abstract", False) == False
+                    and properties.get("layerType", "") == "span"
+                    and properties.get("contains", "")
+                    in (firstClass["token"], firstClass["segment"])
+                    and json_obj.get("layer", {})
+                    .get(firstClass["token"], {})
+                    .get("anchoring", {})
+                    .get("stream", False)
+                ):
+                    layerFile = next(
+                        (
+                            f
+                            for f in self._input_files
+                            if Path(f).stem.lower() == layer.lower()
+                        ),
+                        "",
+                    )
+                    assert layerFile, FileExistsError(
+                        f"Could not find a reference file for entity type '{layer}'"
+                    )
+                    ignore_files.add(layerFile)
+                    with open(layerFile, "r") as f:
+                        cols = [x.lower() for x in f.readline().split()]
+                        for a in properties.get("attributes", {}):
+                            assert a.lower() in cols, ReferenceError(
+                                f"No column found for attribute '{a}' in {layerFile}"
+                            )
+                    if properties["contains"] == firstClass["token"]:
+                        aligned_entities[layer.lower()] = {
+                            "fn": layerFile,
+                            "properties": properties,
+                        }
+                    else:
+                        aligned_entities_segment[layer.lower()] = {
+                            "fn": layerFile,
+                            "properties": properties,
+                        }
+            parser = None
+            # Parse the remaining input files
+            for filepath in self._input_files:
+                if filepath in ignore_files:
+                    continue
+                fn_before_ext = Path(filepath).stem
+                if fn_before_ext.lower() in {
+                    k.lower() for k in json_obj.get("layer", {})
+                }:
+                    continue
+                print("input file", filepath)
+                if not os.path.isfile(filepath):
+                    print(f"Not a file: ignoring '{filepath}'")
+                    continue
+                if os.path.basename(filepath) == "meta.json":
+                    continue
+                parser = parser or PARSERS[self._determine_format(filepath)](
+                    config=json_obj
+                )
+                print(filepath)
+                with open(filepath, "r") as f:
+                    parser.generate_upload_files_generator(
+                        f,
+                        path=self.output or "./",
+                        default_doc={"name": os.path.basename(filepath)},
+                        config=json_obj,
+                        aligned_entities=aligned_entities,
+                        aligned_entities_segment=aligned_entities_segment,
+                    )
+            parser.close_upload_files(
+                path=self.output or "./",
+            )
+            # Process time-anchored extra layers
+            for layer, properties in json_obj.get("layer", {}).items():
+                if (
+                    not properties.get("anchoring", {}).get("time", False)
+                    or layer in json_obj["firstClass"].values()
+                ):
+                    continue
+                fn = f"{layer.lower()}.csv"
+                assert os.path.exists(os.path.join(self._path, fn)), FileExistsError(
+                    f"Could not find a file named '{fn}' in {self._path} for time-anchored layer '{layer}'"
+                )
+                output_path = self.output or "./"
+                input_col_names = []
+                doc_id_idx = 0
+                start_idx = 0
+                end_idx = 0
+                with open(os.path.join(self._path, fn), "r") as input_file:
+                    with open(os.path.join(output_path, fn), "w") as output_file:
+                        while True:
+                            input_line = input_file.readline()
+                            if not input_line:
+                                break
+                            input_cols = input_line.split("\t")
+                            output_cols = []
+                            if not input_col_names:
+                                input_col_names = input_cols
+                                output_cols = [
+                                    c.strip()
+                                    for c in input_col_names
+                                    if c not in ("doc_id", "start", "end")
+                                ]
+                                assert "doc_id" in input_col_names, IndexError(
+                                    f"No column named 'doc_id' found in {fn}"
+                                )
+                                assert "start" in input_col_names, IndexError(
+                                    f"No column named 'start' found in {fn}"
+                                )
+                                assert "end" in input_col_names, IndexError(
+                                    f"No column named 'end' found in {fn}"
+                                )
+                                doc_id_idx = input_cols.index("doc_id")
+                                start_idx = input_cols.index("start")
+                                end_idx = input_cols.index("end")
+                                output_cols.append("frame_range")
+                            else:
+                                output_cols = [
+                                    c.strip()
+                                    for n, c in enumerate(input_cols)
+                                    if n not in (doc_id_idx, start_idx, end_idx)
+                                ]
+                                doc_frames = parser.doc_frames[
+                                    str(input_cols[doc_id_idx])
+                                ]
+                                times = [
+                                    float(input_cols[x]) for x in (start_idx, end_idx)
+                                ]
+                                start, end = [
+                                    str(int(times[n] * 25.0) + doc_frames[n])
+                                    for n in (0, 1)
+                                ]
+                                output_cols.append(f"[{start},{end})")
+                            output_file.write("\t".join(output_cols) + "\n")
+
+            print(f"outfiles written to '{self._path}'.")
+            json_str = json.dumps(json_obj, indent=4)
+            json_path = os.path.join(self.output or ".", "meta.json")
+            open(json_path, "w").write(json_str)
+            print(f"\n{json_str}\n")
+            print(
+                f"A default meta.json file with the structure above was automatically generated at '{json_path}' for the current corpus."
+            )
+            print(f"Please review it and make any changes as needed in a text editor.")
+            print(
+                f"Once the file contains the proper information, press any key to proceed."
+            )
+            input()
 
+        else:
+            format = (self._output_format or "").lstrip(".")
 
-    def process(self):
-        self._scan_headers()
-        self._process_lines()
+            for filepath in self._input_files:
+                print("input file", filepath)
+                if os.path.isfile(filepath):
+                    parser = PARSERS[self._determine_format(filepath)]()
+                else:
+                    parser = self._detect_format_from_string(filepath)
 
+                reader = parser.parse_generator(codecs.open(filepath, "r", "utf8"))
+                for sentence in parser.write_generator(reader):
+                    print("writing", sentence)
 
+                continue
+                if self._on_disk:
+                    with codecs.open(filepath, "r", "utf8") as fo:
+                        content = fo.read()
+                else:
+                    content = filepath
 
-class NestedSetTreeStructure:
-    """
-    Represents a tree structure with the nested set approach.
-    """
+                understood = parser.parse(content)
+                if self._filter:
+                    understood = self._apply_filter(understood)
+                if self._lua_filter:
+                    understood = self._apply_lua_filter(understood)
 
-    def __init__(self, key, left, right):
-        self.nodes = {}
-        if not right - left == 1:
-            raise Exception("invalid anchors for initialization")
-        self.nodes[key] = [left, right]
-
-    def __str__(self):
-        """
-        Returns a pretty-print version of the tree.
-        """
-        lines     = []
-        last_left = 0
-        indent    = -1
-        for key, node in sorted(self.nodes.items(), key=lambda item: item[1]):
-            if node[0] - last_left == 1:
-                indent += 1
-            elif node[0] - last_left > 2:
-                indent -= 1
-            lines.append("{}{}  [{},{}]".format(
-                (indent-1)*"│  " + ("" if node[0] == 1 else "├─╴"),
-                key,
-                node[0],
-                node[1]
-            ))
-            last_left = node[0]
-        return '\n'.join(lines)
-
-    def shift_anchors(self, parent_left):
-        """
-        Makes space in the tree by incrementing all nodes to the right by 2.
-        """
-        for key, node in self.nodes.items():
-            if node[0] > parent_left:
-                self.nodes[key][0] += 2
-            if node[1] > parent_left:
-                self.nodes[key][1] += 2
-
-    def add_node(self, key, parent):
-        """
-        Adds a node giving the id of the parent or None for the root node.
-        """
-        if parent is None:
-            if len(self.nodes):
-                raise Exception("there can only be one root node")
-            else:
-                self.nodes[key] = [1, 2]
-        else:
-            if parent in self.nodes:
-                parent_node = self.nodes[parent]
-            else:
-                raise Exception("key does not exist: {}".format(parent))
-            self.shift_anchors(parent_node[0])
-            self.nodes[key] = [parent_node[0]+1, parent_node[0]+2]
+                if len(understood) == 1:
+                    combined[filepath] = next(v for _, v in understood.items())
+                else:
+                    # if 'documents' in understood:
+                    for doc, v in understood.items():
+                        subfilepath = os.path.join(filepath, f"{doc}.{format}")
+                        combined[subfilepath] = v
+                # else:
+                #     combined[filepath] = understood
 
+            return
 
-def yield_block(xzf):
-    block = []
-    with lzma.open(xzf, "rt") as f:
-        for line in f:
-            if line != "\n":
-                block.append(line)
+            if not self.output:
+                print(json.dumps(combined, indent=4, sort_keys=False))
+                return combined
+            elif self._output_format.endswith("json"):
+                self._write_json(combined)
+                return
             else:
-                yield block
-                block = []
-
-        if block:
-            yield block
-
-
-def main():
-    globs = GlobalState()
-    t_start = timer()
-
-    with open(DEPREL_F1, "w")  as dep_f1, \
-         open(DEPREL_F2, "w")  as dep_f2, \
-         open(LINES_F1, "w")   as lin_f1, \
-         open(LINES_F2, "w")   as lin_f2, \
-         open(SEGMENT_F1, "w") as seg_f1, \
-         open(SEGMENT_F2, "w") as seg_f2, \
-         open(FTS_F1, "w")     as fts_f1, \
-         open(FTS_F2, "w")     as fts_f2, \
-         open(DOC_F, "w")      as doc_f:
-        dep_w1 = csv.writer(dep_f1, delimiter="\t", quotechar="\b")
-        dep_w2 = csv.writer(dep_f2, delimiter="\t", quotechar="\b")
-        lin_w1 = csv.writer(lin_f1, delimiter="\t", quotechar="\b")
-        lin_w2 = csv.writer(lin_f2, delimiter="\t", quotechar="\b")
-        seg_w1 = csv.writer(seg_f1, delimiter="\t", quotechar="\b")
-        seg_w2 = csv.writer(seg_f2, delimiter="\t", quotechar="\b")
-        fts_w1 = csv.writer(fts_f1, delimiter="\t", quotechar="\b")
-        fts_w2 = csv.writer(fts_f2, delimiter="\t", quotechar="\b")
-        doc_w = csv.writer(doc_f, delimiter="\t", quotechar="\b")
-        for i, block in enumerate(yield_block(DATA_F)):
-            dep_w = dep_w1 if i < 250_000_000 else dep_w2
-            lin_w = lin_w1 if i < 250_000_000 else lin_w2
-            seg_w = seg_w1 if i < 250_000_000 else seg_w2
-            fts_w = fts_w1 if i < 250_000_000 else fts_w2
-            sent = Sentence(block, globs)
-            sent.process()
-
-            # if not sent.deprel:
-            #     import pdb; pdb.set_trace()
-
-            for elem in sent.proc_lines:
-                lin_w.writerow(elem)
-            for elem in sent.deprel:
-                dep_w.writerow(elem)
-            seg_w.writerow(sent.segment)
-            fts_w.writerow(sent.fts_vector)
-
-            if i % 10_000_000 == 0 and i != 0:
-                t_count = timer()
-                t = timedelta(seconds=t_count-t_start)
-                print(f"Processed {i:,} segments. time elapsed: {t}")
-
-                if i == 250_000_000:
-                    print("closing files")
-                    dep_f1.close()
-                    lin_f1.close()
-                    seg_f1.close()
-                    fts_f1.close()
-                    input("push 1s to DB, then continue by pressing any key")
-
-        for k, v in sent.glob.docs.items():
-            doc_w.writerow([k, f"[{v[0]},{v[1]})"])
-
-    print("writing dictionaries...")
-    with open(WORD_F, "w") as wor_f,  \
-         open(LEMMA_F, "w") as lem_f, \
-         open(UFEAT_F, "w") as ufe_f:
-        wor_w = csv.writer(wor_f, delimiter="\t")
-        lem_w = csv.writer(lem_f, delimiter="\t")
-        ufe_w = csv.writer(ufe_f, delimiter="\t")
-
-        for k, v in globs.word._dictionary.items():
-            wor_w.writerow([v, k])
-        for k, v in globs.lemma._dictionary.items():
-            lem_w.writerow([v, k])
-        for k, v in globs.ufeats._dictionary.items():
-            ufe_w.writerow([v, k])
-
+                parser = PARSERS[format]()
+                if not self._combine:
+                    # print("combined", combined)
+                    for path, data in combined.items():
+                        # text_id = os.path.splitext(os.path.basename(path))[0]
+                        meta = {"id": path, **data.get("meta", {})}
+                        formatted = parser.write(
+                            data.get("sentences", {}), path, combine=False, meta=meta
+                        )
+                        # fixed_path = os.path.join(self.output, os.path.relpath(path))
+                        fixed_path = os.path.join(self.output, os.path.basename(path))
+                        # print(f"writing {len(formatted)} chars to {fixed_path}")
+                        self._write_to_file(fixed_path, formatted)
+                    return
+                else:
+                    if len(combined) == 1:
+                        path, data = combined.popitem()
+                        meta = {"id": path, **data.get("meta", {})}
+                        formatted = parser.write(
+                            data.get("sentences", {}), path, combine=False, meta=meta
+                        )
+                    else:
+                        formatted = parser.combine(combined)
+                    self._write_to_file(self.output, formatted)
+                    return
+
+            raise ValueError(ERROR_MSG.replace("input", "output"))
+
+
+def run() -> None:
+    kwargs = _parse_cmd_line()
+    Corpert(**kwargs).run()
 
 
 if __name__ == "__main__":
-    data_file_msg = f"processing file  '{green}{DATA_F}{end}'"
-    write_dir_msg = f"writing to dir   '{green}{PREFIX}{end}'"
-    print()
-    user_confirmation(
-        data_file_msg + \
-        "\n"          + \
-        write_dir_msg + \
-        "\n\ncontinue (y/Y)? "
-    )
-
-    main()
-
+    """
+    When the user calls the script directly in command line, this is what we do
+    """
+    run()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lcpcli-0.1.3/corpert/_legacy_process_files/process_sparcling.py` & `lcpcli-0.1.4/lcpcli/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,39 @@
-import csv
-import lzma
-import psycopg2
+import json
+import os
+import re
 import uuid
 
-from datetime import timedelta
-from timeit import default_timer as timer
+from datetime import date
 
 
-green = "\033[92m"
-end = "\033[0m"
-
-
-### DATA & WRITE FILES
-
-PREFIX    = "proc_files2/"
-
-DEPREL_F  = PREFIX + "deprel.csv"
-LINES_F   = PREFIX + "lines.csv"
-SEGMENT_F = PREFIX + "segment.csv"
-WORD_F    = PREFIX + "word.csv"
-LEMMA_F   = PREFIX + "lemma.csv"
-UFEAT_F   = PREFIX + "ufeat.csv"
-XPOS_F    = PREFIX + "xpos.csv"
-
-DATA_F    = [
-                # ("FEP9/token.de.tsv.xz", "german"),
-                # ("FEP9/token.en.tsv.xz", "english"),
-                ("FEP9/token.fr.tsv.xz", "french")
-            ]
-
-
-
-def user_confirmation(message):
-    conf = input(message)
-
-    if conf.lower() != "y":
-        print("aborting.")
-        exit()
-
-
-def yield_block(xzf):
-    block = []
-    with lzma.open(xzf, "rt") as f:
-        for line in f:
-            if line != "\n" and not line.startswith("#"):
-                block.append(line.strip())
-            else:
-                # only used for excluding first header line
-                if block:
-                    yield block
-                    block = []
-                else:
-                    continue
-
-        if block:
-            yield block
-
-
-# def get_meta_dicts(meta_text_file):
-#     """
-#     function that builds the dictionaries
-#     used as lookups for text IDs
-#     """
-#     line_doc, line_chp, line_trn,  = {}, {}, {}
-
-#     lines = [l.split("\t").strip() for l in [x for x in yield_line(meta_text_file)]]
-
-#     for line in lines:
-#         num_line, key_val = line[0], {x.split("=")[0]: x.split("=")[1] for x in line[1].split("|")}
-#         line_doc[num_line] = key_val.pop("Session")
-#         line_chp[num_line] = key_val.pop("Chapter")
-#         line_trn[num_line] = key_val
-
-#     return line_doc, line_chp, line_trn
+def get_ci(d: dict, p: str, default={}):
+    """
+    Case-insensitive get on an object
+    """
+    return next((v for n, v in d.items() if n.lower() == p.lower()), default)
 
 
-class MyDict:
+class CustomDict:
     def __init__(self, is_ufeat=False):
         self._dictionary = {}
-        self._max        = 1
-        self._is_ufeat   = is_ufeat
+        self._max = 1
 
     def __str__(self):
-        return str(self._dictionary)
+        return str(dict(sorted(self._dictionary)))
 
     def update(self, value):
-        if self._is_ufeat and value == '{"_"}':
-            return
-
-        if not value in self._dictionary:
+        if value and value not in self._dictionary:
             self._dictionary[value] = self._max
             self._max += 1
 
     def get(self, value):
         return self._dictionary.get(value, None)
 
 
-class GlobalState:
-    word      = MyDict()
-    lemma     = MyDict()
-    docs      = {}
-    cur_idx   = 1
-    cur_seg   = uuid.uuid4()
-    left      = 1
-    right     = 2
-
-
 class NestedSetTreeStructure:
     """
     Represents a tree structure with the nested set approach.
     """
 
     def __init__(self, key, left, right):
         self.nodes = {}
@@ -117,30 +41,32 @@
             raise Exception("invalid anchors for initialization")
         self.nodes[key] = [left, right]
 
     def __str__(self):
         """
         Returns a pretty-print version of the tree.
         """
-        lines     = []
+        lines = []
         last_left = 0
-        indent    = -1
+        indent = -1
         for key, node in sorted(self.nodes.items(), key=lambda item: item[1]):
             if node[0] - last_left == 1:
                 indent += 1
             elif node[0] - last_left > 2:
                 indent -= 1
-            lines.append("{}{}  [{},{}]".format(
-                (indent-1)*"│  " + ("" if node[0] == 1 else "├─╴"),
-                key,
-                node[0],
-                node[1]
-            ))
+            lines.append(
+                "{}{}  [{},{}]".format(
+                    (indent - 1) * "│  " + ("" if node[0] == 1 else "├─╴"),
+                    key,
+                    node[0],
+                    node[1],
+                )
+            )
             last_left = node[0]
-        return '\n'.join(lines)
+        return "\n".join(lines)
 
     def shift_anchors(self, parent_left):
         """
         Makes space in the tree by incrementing all nodes to the right by 2.
         """
         for key, node in self.nodes.items():
             if node[0] > parent_left:
@@ -159,257 +85,474 @@
                 self.nodes[key] = [1, 2]
         else:
             if parent in self.nodes:
                 parent_node = self.nodes[parent]
             else:
                 raise Exception("key does not exist: {}".format(parent))
             self.shift_anchors(parent_node[0])
-            self.nodes[key] = [parent_node[0]+1, parent_node[0]+2]
+            self.nodes[key] = [parent_node[0] + 1, parent_node[0] + 2]
 
 
 class Sentence:
+    _space_after = re.compile(r"(?<=SpaceAfter=)(Yes|No)")
+    _frame_range = re.compile(r"(?<=start=)(\d+(.\d+)?\|end=\d+(.\d+)?)")
+
     @staticmethod
-    def split_lines(lines):
+    def valid_lines(lines):
         ret_lines = []
+
         for line in lines:
-            split_l = line.split("\t")
-            ret_lines.append(split_l)
+            if line.startswith("#"):
+                continue
+            toks = [x if x != "_" else None for x in line.split("\t")]
+            # valid CoNNL-U?
+            assert len(toks) == 10
+            # make sure ID and form present
+            assert [x for x in toks[:2]]
+            # skip contracted tokens and ellpsis
+            if "-" in toks[0] or "." in toks[0]:
+                continue
+
+            ret_lines.append(toks)
 
         return ret_lines
 
     @staticmethod
+    def jsonify_ufeats(string):
+        if string:
+            # change angular brackets to parens
+            string = string.replace("[", "(").replace("]", ")")
+            # put alternatves inside JSON-array
+            string = re.sub(r"(\w+,\s*\w+)", r"[\1]", string)
+            # convert pipes -separator to comma
+            string = string.replace("|", ",")
+            # converts equal to colon
+            string = string.replace("=", ":")
+            # surround literals with double quotes
+            string = re.sub(r"([\w()]+)", r'"\1"', string)
+
+            return "{" + string + "}"
+        else:
+            return None
+
+    @staticmethod
     def _append(lst, elem):
         """custom append function
 
-           in contrast to the built-in method, this function returns
-           the augmented list - useful for recursive calls
+        in contrast to the built-in method, this function returns
+        the augmented list - useful for recursive calls
         """
         lst.append(elem)
 
         return lst
 
     @staticmethod
     def _traverse(hierarchy, graph, ids):
         """traverse flat list & build hierarchical structure
 
-           the flat structure is a parent: children dict
+        the flat structure is a parent: children dict
         """
         for id in ids:
             hierarchy[id] = Sentence._traverse({}, graph, graph[id])
 
         return hierarchy
 
     @staticmethod
     def _ord_keys(dic, key_list):
-        """traverse tree structure & build flat list
-
-        """
+        """traverse tree structure & build flat list"""
         for el, vals in dic.items():
             Sentence._ord_keys(vals, Sentence._append(key_list, el))
 
         return key_list
 
-    def __init__(self, lines, glob, lang):
-        self._lines     = self.split_lines(lines)
-        self.glob       = glob
+    @staticmethod
+    def _esc(string):
+        return string.replace("'", "''").replace("\\", "\\\\")
+
+    def __init__(self, lines, parser):
+        self._comments = [l for l in lines if l.startswith("# ")]
+        self._lines = self.valid_lines(lines)
+        self.parser = parser
         self.proc_lines = []
-        self.segment    = []
-        self.deprel     = []
-        self.lang       = lang
+        self.segment = []
+        self.deprel = []
+        self.fts_vector = []
+        self.docs = []
+        self.meta = {}
 
     def _tree_ins_order(self):
-        """ put list in hierarchical order for inserting
+        """put list in hierarchical order for inserting
 
-            1. create dictionary structure (recursively)
-            2. flatten keys recursively into list
-            3. go over original list and append to
-               return list according to flattened keys
+        1. create dictionary structure (recursively)
+        2. flatten keys recursively into list
+        3. go over original list and append to
+           return list according to flattened keys
         """
         # index 2 = id, index 4 = head ATTENTION: adjust, if this changes!
-        id_par   = [(x[0], x[6]) for x in self._lines]
+        id_par = [(x[0], x[6]) for x in self._lines]
         ret_list = []
 
         # get root and check iff one
         root = [id for (id, parent) in id_par if parent == "0"]
         if len(root) != 1:
             raise Exception("root error")
 
         # flat parent:children mapping initialization
         graph = {id: set() for (id, parent) in id_par}
 
         # flat parent:children mapping building
-        for (id, parent) in id_par:
+        for id, parent in id_par:
             if parent != "0":
                 graph[parent].add(id)
 
         # sorting in reverse, since inserting is done by shifting to the right
-        graph_sort = {k: sorted(v, key=lambda x: int(x), reverse=True) for k, v in graph.items()}
+        graph_sort = {
+            k: sorted(v, key=lambda x: int(x), reverse=True) for k, v in graph.items()
+        }
 
         # build hierarchical structure
-        hier_ids = self._traverse({}, graph_sort,  root)
+        hier_ids = self._traverse({}, graph, root)
 
         # flatten keys into ordered list
         flat_keys = self._ord_keys(hier_ids, [])
 
         # re-order original rows for returning
         for i in flat_keys:
             for pair in id_par:
                 if pair[0] == i:
                     ret_list.append(pair)
                     continue
 
         return ret_list
 
     def _process_tree(self, ins, token_dict, tok_par_dict):
+        sent = []
+        fts_str = ""
         root, rest = ins[0], ins[1:]
-        tree       = NestedSetTreeStructure(root[0], self.glob.left, self.glob.right)
+        tree = NestedSetTreeStructure(root[0], self.parser.left, self.parser.right)
         for elem in rest:
             tree.add_node(*elem)
 
         # update globals
-        self.glob.left = max([x[1] for x in tree.nodes.values()]) + 1
-        self.glob.right = self.glob.left + 1
+        self.parser.left = max([x[1] for x in tree.nodes.values()]) + 1
 
         # look-up running indices and flatten into list
         for k, v in tree.nodes.items():
             token_id = token_dict[k][0]
-            deprel   = token_dict[k][1]
-            head_id  = token_dict[tok_par_dict[k]][0] if tok_par_dict[k] else None
-            self.deprel.append((head_id, token_id, deprel, *v))
+            deprel = token_dict[k][1]
+            head_id = token_dict[tok_par_dict[k]][0] if tok_par_dict[k] else None
+            sent.append((head_id, token_id, deprel, *v))
+
+        self.deprel += sent
+
+        # 4 = label_out (what am I?), 5 = labels_in (what do I encompass?)
+        # enumerate tokens that are not multi-word units
+        tok_id2sent_idx = {
+            v[0]: n
+            for n, (k, v) in enumerate(token_dict.items(), start=1)
+            if "-" not in k
+        }
+        for elem in sent:
+            fts_str += f" '4{elem[2]}':{tok_id2sent_idx[elem[1]]}"
+            fts_str += f" '5{elem[2]}':{tok_id2sent_idx[elem[1]]}"
+
+        return fts_str
 
     def _process_lines(self):
         # set up local variables
-        token_dict   = {}
+        token_dict = {}
         tok_par_dict = {}
-        start_char   = self.glob.cur_idx
-        end_char     = None
+        fts_str = ""
+        start_char = self.parser.cur_idx
+        end_char = None
 
+        n_fts = 1
         for line in self._lines:
-            w_id,         \
-            word,         \
-            lemma,        \
-            upos,         \
-            xpos,         \
-            _,            \
-            p_id,         \
-            deprel,       \
-            _,            \
-            space_after,  \
-            pacoco_tokid, \
-            pacoco_senid, \
-            pacoco_txtid = line
+            w_id, word, lemma, upos, xpos, ufeats, p_id, deprel, _, misc = line
 
-            l_word   = len(word)
-            end_char = self.glob.cur_idx + l_word
+            try:
+                assert w_id
+                assert word
+            except:
+                continue
+
+            l_word = len(word)
+            end_char = self.parser.cur_idx + l_word
+            ufeats = self.jsonify_ufeats(ufeats)
 
             # update global dicts
-            self.glob.word.update(word)
-            self.glob.lemma.update(lemma)
+            self.parser.word.update(word)
+            self.parser.lemma.update(lemma)
+            self.parser.ufeats.update(ufeats)
+            xpos and self.parser.xpos.update(xpos)
 
             # dictionary holding all info for 1 token
             # TODO: this is not right 100% since w_id not always unique...
             # word_id, form_fk, lemma_fk, upos, xpos, ufeat_fk, char_range, seg_fk
             token_dict[w_id] = [
-                pacoco_tokid,
-                self.glob.word.get(word),
-                self.glob.lemma.get(lemma),
-                upos,
-                xpos,
-                (self.glob.cur_idx, end_char),
-                self.glob.cur_seg,
-                deprel
+                self.parser.cur_word,  # 0
+                self.parser.word.get(word),  # 1
+                self.parser.lemma.get(lemma),  # 2
+                upos,  # 3
+                xpos,  # 4
+                self.parser.ufeats.get(ufeats),  # 5
+                (self.parser.cur_idx, end_char),  # 6
+                self.parser.cur_seg,  # 7
+                deprel,  # 8
             ]
 
+            fts_str += f" '1{self._esc(word)}':{n_fts}"
+            if lemma:
+                fts_str += f" '2{self._esc(lemma)}':{n_fts}"
+            if upos:
+                # escaping UPOS not needed
+                fts_str += f" '3{upos}':{n_fts}"
+            if xpos:
+                fts_str += f" '6{self._esc(xpos)}':{n_fts}"
+            n_fts += 1
+
             # update global word id and index
-            if space_after != "_":
-                self.glob.cur_idx += l_word
-            else:
-                self.glob.cur_idx += l_word + 1
+            self.parser.cur_idx += l_word + 1
+
+            if misc:
+                if parse_misc := re.search(Sentence._space_after, misc):
+                    if parse_misc[1] == "No":
+                        self.parser.cur_idx -= 1
+                if frame_range := re.search(Sentence._frame_range, misc):
+                    start, end = frame_range[1].split("|")
+                    start = round(25.0 * float(start))
+                    end = round(25.0 * float(end.lstrip("end=")))
+                    token_dict[w_id].append([start, end])
+                jsonbMisc = {}
+                for bit in misc.split("|"):
+                    if "=" not in bit:
+                        continue
+                    key, value = bit.split("=")
+                    if key in ("SpaceAfter", "start", "end"):
+                        continue
+                    jsonbMisc[key] = value
+                if jsonbMisc:
+                    jsonbMisc = {x: jsonbMisc[x] for x in sorted(jsonbMisc)}
+                    jd = json.dumps(jsonbMisc)
+                    self.parser.jsonbMisc.update(jd)
+                    token_dict[w_id].append(self.parser.jsonbMisc.get(jd))
+
+            self.parser.cur_word += 1
 
             tok_par_dict[w_id] = p_id if p_id != "0" else None
 
         # create line entry for writing
         self.proc_lines = [
-            line[:5]                         + \
-            [f"[{line[5][0]},{line[5][1]})"] + \
-            [line[6]] for line in token_dict.values()
+            line[:6]
+            + [f"[{line[6][0]},{line[6][1]})"]
+            + [line[7]]
+            + [(f"[{x[0]},{x[1]})" if isinstance(x, list) else x) for x in line[9:]]
+            for line in token_dict.values()
         ]
 
         # build tree (if possible)
-        try:
-            ins = self._tree_ins_order()
-            self._process_tree(ins, {k: (v[0], v[-1]) for k, v in token_dict.items()}, tok_par_dict)
-        except:
-            pass
+        # smth like "id IS_PARSED:"
+        if True:
+            try:
+                ins = self._tree_ins_order()
+                fts = self._process_tree(
+                    ins, {k: (v[0], v[-1]) for k, v in token_dict.items()}, tok_par_dict
+                )
+            except:
+                fts = ""
 
         # create segment entry for writing
-        self.segment = [
-            self.glob.cur_seg,
-            pacoco_senid,
-            pacoco_txtid,
-            f"[{start_char},{end_char})"
-        ]
+        self.segment = [self.parser.cur_seg, f"[{start_char},{end_char})"]
+
+        self.fts_vector = [self.parser.cur_seg, f"{fts_str}{fts}"]
+
         # set new segment id
-        self.glob.cur_seg = uuid.uuid4()
+        self.parser.cur_seg = uuid.uuid4()
 
+        for l in self._comments:
+            if " = " not in l:
+                continue
+            k, v = l.split(" = ")
+            if k.startswith("# newdoc"):
+                continue
+            k = k[2:].strip()
+            v = v.strip()
+            if not k or not v:
+                continue
+            self.meta[k] = v
+
+        # TODO
+        # create doc entry for writing
+        # For simple CoNLL-U, we assume hole corpus one doc...
+        # if self._id:
+        #     if self._id in self.glob.docs:
+        #         self.glob.docs[self._id][1] = end_char
+        #     else:
+        #         self.glob.docs[self._id] = [start_char, end_char]
 
     def process(self):
         self._process_lines()
 
 
-def main():
-    globs = GlobalState()
-    t_start = timer()
-
-    with open(DEPREL_F, "w") as dep_f,  \
-         open(LINES_F, "w") as lin_f,   \
-         open(SEGMENT_F, "w") as seg_f:
-        dep_w = csv.writer(dep_f, delimiter="\t")
-        lin_w = csv.writer(lin_f, delimiter="\t")
-        seg_w = csv.writer(seg_f, delimiter="\t")
-        for f, lang in DATA_F:
-            for i, block in enumerate(yield_block(f)):
-                sent = Sentence(block, globs, lang)
-                sent.process()
-
-                # if not sent.deprel:
-                #     import pdb; pdb.set_trace()
-
-                for elem in sent.proc_lines:
-                    lin_w.writerow(elem)
-                for elem in sent.deprel:
-                    dep_w.writerow(elem)
-                seg_w.writerow(sent.segment)
-
-                if i % 100_000 == 0 and i != 0:
-                    t_count = timer()
-                    t = timedelta(seconds=t_count-t_start)
-                    print(f"Processed {i:,} segments. time elapsed: {t}")
-
-                # if i == 1_000_000:
-                #     break
-
-
-    print("writing dictionaries...")
-    with open(WORD_F, "w") as wor_f,  \
-         open(LEMMA_F, "w") as lem_f:
-        wor_w = csv.writer(wor_f, delimiter="\t")
-        lem_w = csv.writer(lem_f, delimiter="\t")
-
-        for k, v in globs.word._dictionary.items():
-            wor_w.writerow([v, k])
-        for k, v in globs.lemma._dictionary.items():
-            lem_w.writerow([v, k])
-
-
-if __name__ == "__main__":
-    data_file_msg = f"processing file  '{green}{DATA_F}{end}'"
-    write_dir_msg = f"writing to dir   '{green}{PREFIX}{end}'"
-    print()
-    user_confirmation(
-        data_file_msg + \
-        "\n"          + \
-        write_dir_msg + \
-        "\n\ncontinue (y/Y)?"
-    )
+class Table:
+    def __init__(self, name, path, config={}):
+        self.name = name
+        self.path = os.path.join(path, f"{name}.csv")
+        self.file = open(self.path, "a")
+        self.config = config
+        self.cursor = 1
+        self.currentEntity = dict()
+        self.previousEntity = None
+        self.colNames = ([],)
+        self.labels = dict()
+        self.texts = dict()
+        self.deps = dict()
+        self.anchor_right = 0
+        self.non_null_attributes = {}
+        self.sep = "\t"
+
+    def write(self, row: list):
+        self.file.write(self.sep.join([str(x) for x in row]) + "\n")
+
+
+class Attribute:
+    def __init__(self, name, value):
+        self.name = name
+        self._value = value
+
+    @property
+    def value(self):
+        if not self._value:
+            return ""
+        else:
+            return str(self._value)
+
+
+class Meta(Attribute):
+    def __init__(self, name, value):
+        super().__init__(name, value)
+
+    @property
+    def value(self):
+        if not self._value:
+            return ""
+        else:
+            return json.dumps(self._value)
+
+
+class Text(Attribute):
+    def __init__(self, name, value):
+        super().__init__(name, value)
+
+
+class Categorical(Attribute):
+    def __init__(self, name, value):
+        super().__init__(name, value)
+
+
+class Dependency(Attribute):
+    def __init__(self, name, value):
+        super().__init__(name, value)
+        self.label = ""
+
+
+# class Jsonb(Attribute):
+#     def __init__(self,name,value):
+# super().__init__(name,value)
+
+
+class EntityType:
+    def __init__(self):
+        self.id: int | str = ""
+        self.attributes: dict[str, Attribute] = {}
+
+
+token_id = 0
+
+
+class Token(EntityType):
+    def __init__(self):
+        super().__init__()
+        global token_id
+        token_id += 1
+        self.id = token_id
+        self.attributes["form"] = Text("form", "")
+        self.spaceAfter = True
+        self.frame_range = None
+
+
+class Segment(EntityType):
+    def __init__(self):
+        super().__init__()
+        self.id = uuid.uuid4()
+        self.tokens: list[Token] = []
+
+
+doc_id = 0
+
+
+class Document(EntityType):
+    def __init__(self):
+        super().__init__()
+        global doc_id
+        doc_id += 1
+        self.id = doc_id
+        self.char_range_start: int = 0
+        self.frame_range: list[int] = [0, 0]
+        self.left = 1
+        self.right = 2
+
+
+# Compute left/right from parent only once
+class NestedSet:
+    def __init__(self, id, label, cursor):
+        self.id = id
+        self.children = []
+        self.parent = None
+        self.label = label
+        self.cursor_id = cursor
+
+    def compute_anchors(self, left=1):
+        self.left = left
+        for c in self.children:
+            left = c.compute_anchors(left=left + 1)
+        self.right = left + 1
+        return self.right
+
+    @property
+    def all_ids(self):
+        ids = [self.id]
+        for c in self.children:
+            ids += c.all_ids
+        return ids
+
+    def add(self, child):
+        if child in self.children:
+            return
+        self.children.append(child)
+        child.parent = self
+
 
-    main()
+def default_json(name):
+    return {
+        "meta": {
+            "name": name,
+            "author": "Anonymous",
+            "date": date.today().strftime("%Y-%m-%d"),
+            "version": 1,
+            "corpusDescription": "",
+        },
+        "firstClass": {"document": "Document", "segment": "Segment", "token": "Token"},
+        "layer": {
+            "Token": {
+                "abstract": False,
+                "layerType": "unit",
+                "anchoring": {"location": False, "stream": True, "time": False},
+            },
+            "Segment": {"abstract": False, "layerType": "span", "contains": "Token"},
+            "Document": {
+                "abstract": False,
+                "contains": "Segment",
+                "layerType": "span",
+            },
+        },
+    }
```

### Comparing `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/tei.py` & `lcpcli-0.1.4/lcpcli/parsers/tei.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/vert.py` & `lcpcli-0.1.4/lcpcli/parsers/vert.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.3/corpert/build/lib/corpert/utils.py` & `lcpcli-0.1.4/lcpcli/parsers/conllu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,402 +1,378 @@
-import json
+"""
+Parser and writer for CONLLU-style data
+
+
+ID: Word index, integer starting at 1 for each new sentence; may be a range for multiword tokens; may be a decimal number for empty nodes (decimal numbers can be lower than 1 but must be greater than 0).
+FORM: Word form or punctuation symbol.
+LEMMA: Lemma or stem of word form.
+UPOS: Universal part-of-speech tag.
+XPOS: Language-specific part-of-speech tag; underscore if not available.
+FEATS: List of morphological features from the universal feature inventory or from a defined language-specific extension; underscore if not available.
+HEAD: Head of the current word, which is either a value of ID or zero (0).
+DEPREL: Universal dependency relation to the HEAD (root iff HEAD = 0) or a defined language-specific subtype of one.
+DEPS: Enhanced dependency graph in the form of a list of head-deprel pairs.
+MISC: Any other annotation.
+
+"""
+
 import re
 import uuid
 
-class CustomDict:
-    def __init__(self, is_ufeat=False):
-        self._dictionary = {}
-        self._max        = 1
-
-    def __str__(self):
-        return str(dict(sorted(self._dictionary)))
-
-    def update(self, value):
-        if value and value not in self._dictionary:
-            self._dictionary[value] = self._max
-            self._max += 1
-
-    def get(self, value):
-        return self._dictionary.get(value, None)
-
-
-class NestedSetTreeStructure:
-    """
-    Represents a tree structure with the nested set approach.
-    """
-
-    def __init__(self, key, left, right):
-        self.nodes = {}
-        if not right - left == 1:
-            raise Exception("invalid anchors for initialization")
-        self.nodes[key] = [left, right]
+from inspect import isgenerator
+from typing import cast
 
-    def __str__(self):
+from ._parser import Parser
+from ..utils import (
+    Attribute,
+    Categorical,
+    CustomDict,
+    Dependency,
+    Document,
+    Meta,
+    Segment,
+    Text,
+    Token,
+)
+
+
+FEATURES = [
+    "id",
+    "form",
+    "lemma",
+    "upos",
+    "xpos",
+    "feats",
+    "head",
+    "deprel",
+    "deps",
+    "misc",
+]
+
+
+class CONLLUParser(Parser):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.word = CustomDict()
+        self.lemma = CustomDict()
+        self.ufeats = CustomDict()
+        self.jsonbMisc = CustomDict()
+        self.xpos = set()
+        self.cur_idx = 1
+        self.cur_word = 1
+        self.cur_seg = uuid.uuid4()
+        self.left = 1
+
+        self.start_idx = re.compile(r"^\[\d+")
+        self.end_idx = re.compile(r"\d+\)$")
+        self.text_id = -1
+
+        self.n_doc = 0
+
+        self._features = FEATURES
+
+    @property
+    def right(self):
+        return self.left + 1
+
+    def parse_sentence(
+        self, sentence_lines, config={}
+    ) -> tuple[Segment | None, Document | None]:
         """
-        Returns a pretty-print version of the tree.
+        Take a list of ConLLU lines (comments + tokens) and output (sentence, new_doc | None)
         """
-        lines     = []
-        last_left = 0
-        indent    = -1
-        for key, node in sorted(self.nodes.items(), key=lambda item: item[1]):
-            if node[0] - last_left == 1:
-                indent += 1
-            elif node[0] - last_left > 2:
-                indent -= 1
-            lines.append("{}{}  [{},{}]".format(
-                (indent-1)*"│  " + ("" if node[0] == 1 else "├─╴"),
-                key,
-                node[0],
-                node[1]
-            ))
-            last_left = node[0]
-        return '\n'.join(lines)
+        new_doc = None
+        current_sentence: dict = {"meta": {}, "text": []}
+        mediaSlots = self.config.get("meta", {}).get("mediaSlots", {})
+        for line in sentence_lines:
+            if re.match(r"# newdoc", line):
+                if not new_doc:
+                    self.n_doc += 1
+                    new_doc = {"meta": {}, "sentences": {}, "id": self.n_doc}
+                if match := re.match(r"# newdoc id = (.+)", line):
+                    new_doc["id"] = match[1]
+                elif match := re.match(r"# newdoc ([^=]+) = (.+)", line):
+                    key = match[1].strip()
+                    value = match[2].strip()
+                    if mediaSlots and key in mediaSlots:
+                        new_doc["media"] = new_doc.get("media", {})
+                        new_doc["media"][key] = value
+                    else:
+                        new_doc["meta"][key] = value
+            elif match := re.match(r"# sent_id = (.+)", line):
+                current_sentence["id"] = match[1]
+            elif match := re.match(r"#\s+([^=]+)\s+= (.+)", line):
+                current_sentence["meta"][match[1]] = match[2]
+            elif re.match(r"\d+[\t\s]", line):
+                line = line.split("\t")
+                line = {k: v for k, v in zip(self._features, line)}
+                current_sentence["text"].append(line)
+
+        if new_doc:
+            for media_name, attribs in mediaSlots.items():
+                assert (
+                    media_name in new_doc.get("media", {})
+                    or attribs.get("isOptional", False) is not False
+                ), KeyError(
+                    f"Filename missing for required media '{media_name}' in current document"
+                )
+
+        sentence = None
+        if current_sentence["text"]:
+            sentence = Segment()
+            for t in current_sentence["text"]:
+                token = Token()
+                sentence.tokens.append(token)
+                for k, v in t.items():
+                    if v == "_":
+                        v = None
+                    if k == "id":
+                        token.id = v
+                    elif k in ("form", "lemma"):
+                        token.attributes[k] = Text(k, v)
+                    elif k in ("upos", "xpos"):
+                        token.attributes[k] = Categorical(k, v)
+                    elif k == "feats":
+                        v = v or ""
+                        d = {}
+                        for pkpv in v.split("|"):
+                            if "=" not in pkpv:
+                                continue
+                            pk, pv = pkpv.split("=")
+                            d[pk.strip()] = pv.strip()
+                        token.attributes["ufeat"] = Meta("ufeat", d)
+                    elif k == "head":
+                        if v == "0":
+                            v = None
+                        token.attributes["deprel"] = Dependency("deprel", v)
+                    elif k == "deprel":
+                        dep: Dependency = cast(
+                            Dependency,
+                            token.attributes.get("deprel", Dependency("deprel", None)),
+                        )
+                        dep.label = v
+                        token.attributes["head"] = dep
+                    elif k == "misc":
+                        if not v or "=" not in v:
+                            continue
+                        misc = {}
+                        for pkpv in v.split("|"):
+                            if "=" not in pkpv:
+                                continue
+                            pk, pv = pkpv.split("=")
+                            pk = pk.strip()
+                            pv = pv.strip()
+                            if pk in ("start", "end"):
+                                token.frame_range = token.frame_range or [0, 0]
+                                token.frame_range[0 if pk == "start" else 1] = int(
+                                    25.0 * float(pv)
+                                )
+                                has_frame_range = True
+                            else:
+                                misc[pk] = str(pv)
+                        token.attributes["misc"] = Meta("misc", misc)
+                    else:
+                        token.attributes[k] = Text(k, v)
+
+            # if has_frame_range:
+            #     assert all(t.frame_range is not None for t in sentence.tokens), AttributeError("Some tokens miss start-end time information")
+
+            # sentence.tokens = current_sentence["text"]
+            meta = current_sentence["meta"]
+            if config:
+                # If a config was provided, pop any entry from meta that's listed as a main attribute
+                seg_layer = config.get("firstClass", {}).get("segment", "")
+                seg_config = (
+                    config.get("layer", {}).get(seg_layer, {}).get("attributes", {})
+                )
+                segment_containers = [
+                    layer.lower()
+                    for layer, props in config.get("layer", {}).items()
+                    if props.get("layerType", "") == "span"
+                    and props.get("contains", "") == seg_layer
+                ]
+                for attr_name in seg_config:
+                    name = attr_name
+                    if name + "_id" in meta:
+                        name = name + "_id"
+                    elif name not in meta:
+                        continue
+                    a = meta.pop(name)
+                    sentence.attributes[name] = Attribute(name, a)
+                for seg_container in segment_containers:
+                    attr_name = next(
+                        (k for k in meta.keys() if k.lower() == seg_container), None
+                    )
+                    if attr_name is None:
+                        continue
+                    sentence.attributes[attr_name] = Text(
+                        attr_name, meta.pop(attr_name)
+                    )
+            if meta:
+                # if name.lower() in segment_containers:
+                #     sentence.attributes[name] = Text(name, meta.pop(name))
+                sentence.attributes["meta"] = Meta("meta", meta)
+
+        ret_doc: Document | None = None
+        if new_doc:
+            ret_doc = Document()
+            if id := new_doc.get("id"):
+                new_doc["meta"]["name"] = id
+            ret_doc.attributes["meta"] = Meta("meta", new_doc["meta"])
+            if new_doc.get("media"):
+                ret_doc.attributes["media"] = Meta("media", new_doc["media"])
+            # doc.first_sentence = sentence
+
+        return (sentence, ret_doc)
+        # return (current_sentence, new_doc)
+
+    def parse_generator(self, reader, config={}):
+        checked_first_line_for_conllu_plus = False
+        sentence_lines = []
+        while line := reader.readline():
+            l = line.strip()
+            if l:
+                if not checked_first_line_for_conllu_plus and l.startswith(
+                    "# global.columns = "
+                ):
+                    self._features = [f.lower() for f in l[19:].split()]
+                else:
+                    sentence_lines.append(line)
+            else:
+                # empty line: new sentence
+                if sentence_lines:
+                    yield self.parse_sentence(sentence_lines, config=config)
+                sentence_lines = []
+            checked_first_line_for_conllu_plus = True
 
-    def shift_anchors(self, parent_left):
-        """
-        Makes space in the tree by incrementing all nodes to the right by 2.
-        """
-        for key, node in self.nodes.items():
-            if node[0] > parent_left:
-                self.nodes[key][0] += 2
-            if node[1] > parent_left:
-                self.nodes[key][1] += 2
+        if sentence_lines:
+            yield self.parse_sentence(sentence_lines, config=config)
 
-    def add_node(self, key, parent):
+    def parse(self, content):
         """
-        Adds a node giving the id of the parent or None for the root node.
+        When iterator is True, yield ({id,meta,text},None|{id,meta}) -- content should have a readline method and
+        When iterator is False, return a writable string
         """
-        if parent is None:
-            if len(self.nodes):
-                raise Exception("there can only be one root node")
-            else:
-                self.nodes[key] = [1, 2]
-        else:
-            if parent in self.nodes:
-                parent_node = self.nodes[parent]
-            else:
-                raise Exception("key does not exist: {}".format(parent))
-            self.shift_anchors(parent_node[0])
-            self.nodes[key] = [parent_node[0]+1, parent_node[0]+2]
 
+        conllu_parsed = {}
+        current_document = {"meta": {}, "sentences": {}}
+        current_sentences = {}
 
-# class GlobalState:
-#     def __new__(cls):
-#         if not hasattr(cls, "instance"):
-#             cls.instance = super(GlobalState, cls).__new__(cls)
-#         return cls.instance
+        self.n_doc = 0
+        n_sent = 0
 
-#     word      = CustomDict()
-#     lemma     = CustomDict()
-#     ufeats    = CustomDict()
-#     xpos      = set()
-#     # docs      = {}
-#     cur_idx   = 1
-#     cur_word  = 1
-#     cur_seg   = uuid.uuid4()
-#     left      = 1
+        sentences = [sent for sent in content.split("\n\n") if sent]
 
-#     @property
-#     def right(self):
-#         return self.left + 1
+        for sent in sentences:
 
+            sent_list = [line for line in sent.split("\n") if line]
+            sentence, new_doc = self.parse_sentence(sent_list)
 
+            if new_doc:
+                if current_sentences:
+                    current_document["sentences"] = current_sentences
+                    self.n_doc += 1
+                    conllu_parsed[current_document.pop("id", self.n_doc)] = (
+                        current_document
+                    )
+                current_document = new_doc
+                current_sentences = {}
 
+            current_sentences[sentence.pop("id", n_sent := n_sent + 1)] = sentence
 
+        if current_sentences:
+            current_document["sentences"] = current_sentences
+            self.n_doc += 1
+            conllu_parsed[current_document.pop("id", self.n_doc)] = current_document
 
-class Sentence:
-    _space_after = re.compile("(?<=SpaceAfter=)(Yes|No)")
-    _frame_range = re.compile("(?<=start=)(\d+(.\d+)?\|end=\d+(.\d+)?)")
+        return conllu_parsed
 
-    @staticmethod
-    def valid_lines(lines):
-        ret_lines = []
-
-        for line in lines:
-            if line.startswith("#"):
-                continue
-            toks = [x if x != "_" else None for x in line.split("\t")]
-            # valid CoNNL-U?
-            assert len(toks) == 10
-            # make sure ID and form present
-            assert [x for x in toks[:2]]
-            # skip contracted tokens and ellpsis
-            if "-" in toks[0] or "." in toks[0]:
+    def doc_meta(self, id, meta):
+        """
+        content is a dict {id,meta}
+        """
+        lines = []
+        lines.append(f"# newdoc id = {id}")
+        for key, value in meta.items():
+            text = value.lstrip(" ").rstrip(" ") if value else None
+            if not key or not text:
                 continue
+            lines.append(f"# newdoc {key} = {text}")
+        return f"\n".join(lines)
 
-            ret_lines.append(toks)
-
-        return ret_lines
-
-    @staticmethod
-    def jsonify_ufeats(string):
-        if string:
-            # change angular brackets to parens
-            string = string.replace("[", "(").replace("]", ")")
-            # put alternatves inside JSON-array
-            string = re.sub(r"(\w+,\s*\w+)", r"[\1]", string)
-            # convert pipes -separator to comma
-            string = string.replace("|", ",")
-            # converts equal to colon
-            string = string.replace("=", ":")
-            # surround literals with double quotes
-            string = re.sub(r"([\w()]+)", r'"\1"', string)
-
-            return "{" + string + "}"
-        else:
-            return None
-
-    @staticmethod
-    def _append(lst, elem):
-        """custom append function
-
-           in contrast to the built-in method, this function returns
-           the augmented list - useful for recursive calls
+    def combine(self, content):
         """
-        lst.append(elem)
+        content is a dict of filepaths and conllu data strings. combine them into one corpus and return as string?
 
-        return lst
-
-    @staticmethod
-    def _traverse(hierarchy, graph, ids):
-        """traverse flat list & build hierarchical structure
-
-           the flat structure is a parent: children dict
+        probably we have to add the filepaths to each sentence's sent-metadata
         """
-        for id in ids:
-            hierarchy[id] = Sentence._traverse({}, graph, graph[id])
 
-        return hierarchy
+        conllu_lines = []
 
-    @staticmethod
-    def _ord_keys(dic, key_list):
-        """traverse tree structure & build flat list
+        for doc_id, doc_content in content.items():
+            conllu_lines.append(self.doc_meta(doc_id, doc_content.get("meta", {})))
+            conllu_lines.append(self.write(doc_content.get("sentences", {})))
+
+        return f"\n".join(conllu_lines)
+
+    def write_sentence(self, sentence):
+        lines = []
+        sent_meta, sent_text = {}, []
+
+        for item in sentence:
+            if "meta" in item:
+                sent_meta = sentence[item]
+            elif "text" in item:
+                sent_text = sentence[item]
+
+        for k, v in sent_meta.items():
+            lines.append("# {} = {}\n".format(k, v))
+
+        if not sent_text:
+            return lines
+
+        lines.append(
+            f"# text = {' '.join([token.get('form',' ') for token in sent_text])}\n"
+        )
+
+        for n, item in enumerate(sent_text):
+            # cols = [n+1, *item[1:]]
+            # cols = [(str(i) if i else '_') for i in cols]
+            # lines.append(f"\t".join(cols))
+            lines.append(f"\t".join([item.get(f, "_") for f in self._features]))
+
+        return lines
+
+    def write_generator(self, generator):
+        self.n_doc = 0
+        n_sent = 0
+
+        for sentence, doc in generator:
+            lines = []
+            # For now we don't support combine=False: yield new docs
+            if doc:
+                self.n_doc += 1
+                lines.append("# newdoc id = {}".format(doc.pop("id", self.n_doc)))
+                for k, v in doc.get("meta", {}).items():
+                    lines.append("# newdoc {} = {}".format(k, v))
+            lines.append(
+                "# sent_id = {}\n".format(sentence.pop("id", n_sent := n_sent + 1))
+            )
+            lines += self.write_sentence(sentence)
+            yield "".join(lines)
 
+    def write(self, content, filename=None, combine=True, meta={}):
+        """
+        content is a dict of sentences: key is the id, value is {meta,text}
         """
-        for el, vals in dic.items():
-            Sentence._ord_keys(vals, Sentence._append(key_list, el))
 
-        return key_list
+        conllu_lines = []
 
-    @staticmethod
-    def _esc(string):
-        return string.replace("'", "''").replace("\\", "\\\\")
-
-    def __init__(self, lines, parser):
-        self._comments  = [l for l in lines if l.startswith("# ")]
-        self._lines     = self.valid_lines(lines)
-        self.parser     = parser
-        self.proc_lines = []
-        self.segment    = []
-        self.deprel     = []
-        self.fts_vector = []
-        self.docs       = []
-        self.meta       = {}
-
-    def _tree_ins_order(self):
-        """ put list in hierarchical order for inserting
-
-            1. create dictionary structure (recursively)
-            2. flatten keys recursively into list
-            3. go over original list and append to
-               return list according to flattened keys
-        """
-        # index 2 = id, index 4 = head ATTENTION: adjust, if this changes!
-        id_par   = [(x[0], x[6]) for x in self._lines]
-        ret_list = []
-
-        # get root and check iff one
-        root = [id for (id, parent) in id_par if parent == "0"]
-        if len(root) != 1:
-            raise Exception("root error")
-
-        # flat parent:children mapping initialization
-        graph = {id: set() for (id, parent) in id_par}
-
-        # flat parent:children mapping building
-        for (id, parent) in id_par:
-            if parent != "0":
-                graph[parent].add(id)
-
-        # sorting in reverse, since inserting is done by shifting to the right
-        graph_sort = {k: sorted(v, key=lambda x: int(x), reverse=True) for k, v in graph.items()}
-
-        # build hierarchical structure
-        hier_ids = self._traverse({}, graph,  root)
-
-        # flatten keys into ordered list
-        flat_keys = self._ord_keys(hier_ids, [])
-
-        # re-order original rows for returning
-        for i in flat_keys:
-            for pair in id_par:
-                if pair[0] == i:
-                    ret_list.append(pair)
-                    continue
-
-        return ret_list
-
-    def _process_tree(self, ins, token_dict, tok_par_dict):
-        sent       = []
-        fts_str    = ""
-        root, rest = ins[0], ins[1:]
-        tree       = NestedSetTreeStructure(root[0], self.parser.left, self.parser.right)
-        for elem in rest:
-            tree.add_node(*elem)
-
-        # update globals
-        self.parser.left = max([x[1] for x in tree.nodes.values()]) + 1
-
-        # look-up running indices and flatten into list
-        for k, v in tree.nodes.items():
-            token_id = token_dict[k][0]
-            deprel = token_dict[k][1]
-            head_id = token_dict[tok_par_dict[k]][0] if tok_par_dict[k] else None
-            sent.append((head_id, token_id, deprel, *v))
-
-        self.deprel += sent
-
-        # 4 = label_out (what am I?), 5 = labels_in (what do I encompass?)
-        # enumerate tokens that are not multi-word units
-        tok_id2sent_idx = {v[0]: n for n, (k, v) in enumerate(token_dict.items(), start=1) if '-' not in k}
-        for elem in sent:
-            fts_str += f" '4{elem[2]}':{tok_id2sent_idx[elem[1]]}"
-            fts_str += f" '5{elem[2]}':{tok_id2sent_idx[elem[1]]}"
-
-        return fts_str
-
-    def _process_lines(self):
-        # set up local variables
-        token_dict   = {}
-        tok_par_dict = {}
-        fts_str      = ""
-        start_char   = self.parser.cur_idx
-        end_char     = None
-        
-        n_fts = 1
-        for line in self._lines:
-            w_id, word, lemma, upos, xpos, ufeats, p_id, deprel, _, misc = line
-
-            try:
-                assert w_id
-                assert word
-            except:
-                continue
+        for sent_id, sent_data in content.items():
 
-            l_word   = len(word)
-            end_char = self.parser.cur_idx + l_word
-            ufeats   = self.jsonify_ufeats(ufeats)
-
-            # update global dicts
-            self.parser.word.update(word)
-            self.parser.lemma.update(lemma)
-            self.parser.ufeats.update(ufeats)
-            xpos and self.parser.xpos.update(xpos)
-
-            # dictionary holding all info for 1 token
-            # TODO: this is not right 100% since w_id not always unique...
-            # word_id, form_fk, lemma_fk, upos, xpos, ufeat_fk, char_range, seg_fk
-            token_dict[w_id] = [
-                self.parser.cur_word,            # 0
-                self.parser.word.get(word),      # 1
-                self.parser.lemma.get(lemma),    # 2
-                upos,                            # 3
-                xpos,                            # 4
-                self.parser.ufeats.get(ufeats),  # 5
-                (self.parser.cur_idx, end_char), # 6
-                self.parser.cur_seg,             # 7
-                deprel                           # 8
-            ]
-
-            fts_str += f" '1{self._esc(word)}':{n_fts}"
-            if lemma:
-                fts_str += f" '2{self._esc(lemma)}':{n_fts}"
-            if upos:
-                # escaping UPOS not needed
-                fts_str += f" '3{upos}':{n_fts}"
-            if xpos:
-                fts_str += f" '6{self._esc(xpos)}':{n_fts}"
-            n_fts += 1
-
-            # update global word id and index
-            self.parser.cur_idx += l_word + 1
-
-            if misc:
-                if parse_misc := re.search(Sentence._space_after, misc):
-                    if parse_misc[1] == "No":
-                        self.parser.cur_idx -= 1
-                if frame_range := re.search(Sentence._frame_range, misc):
-                    start, end = frame_range[1].split("|")
-                    start = round(25.0 * float(start))
-                    end = round(25.0 * float(end.lstrip("end=")))
-                    token_dict[w_id].append( [start, end] )
-                jsonbMisc = {}
-                for bit in misc.split("|"):
-                    if "=" not in bit:
-                        continue
-                    key, value = bit.split("=")
-                    if key in ("SpaceAfter", "start", "end"):
-                        continue
-                    jsonbMisc[key] = value
-                if jsonbMisc:
-                    jsonbMisc = {x:jsonbMisc[x] for x in sorted(jsonbMisc)}
-                    jd = json.dumps(jsonbMisc)
-                    self.parser.jsonbMisc.update(jd)
-                    token_dict[w_id].append( self.parser.jsonbMisc.get(jd) )
-
-            self.parser.cur_word += 1
-
-            tok_par_dict[w_id] = p_id if p_id != "0" else None
-
-        # create line entry for writing
-        self.proc_lines = [
-            line[:6] + [f"[{line[6][0]},{line[6][1]})"] + [line[7]] + [
-                (f"[{x[0]},{x[1]})" if isinstance(x,list) else x)
-                for x in line[9:]
-            ]
-            for line in token_dict.values()
-        ]
-
-        # build tree (if possible)
-        # smth like "id IS_PARSED:"
-        if True:
-            try:
-                ins = self._tree_ins_order()
-                fts = self._process_tree(ins, {k: (v[0], v[-1]) for k, v in token_dict.items()}, tok_par_dict)
-            except:
-                fts = ""
-
-        # create segment entry for writing
-        self.segment = [
-            self.parser.cur_seg,
-            f"[{start_char},{end_char})"
-        ]
-
-        self.fts_vector = [
-            self.parser.cur_seg,
-            f"{fts_str}{fts}"
-        ]
-
-        # set new segment id
-        self.parser.cur_seg = uuid.uuid4()
-
-        for l in self._comments:
-            k, v = l.split(" = ")
-            if k.startswith("# newdoc"):
-                continue
-            k = k[2:].strip()
-            v = v.strip()
-            if not k or not v:
-                continue
-            self.meta[k] = v
+            if conllu_lines:
+                conllu_lines.append(f"")  # Add an empty line
 
-        # TODO
-        # create doc entry for writing
-        # For simple CoNLL-U, we assume hole corpus one doc...
-        # if self._id:
-        #     if self._id in self.glob.docs:
-        #         self.glob.docs[self._id][1] = end_char
-        #     else:
-        #         self.glob.docs[self._id] = [start_char, end_char]
+            conllu_lines.append(f"# sent_id = {sent_id}\n")
+            conllu_lines += self.write_sentence(sent_data)
 
-    def process(self):
-        self._process_lines()
+        return f"\n".join(conllu_lines)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lcpcli-0.1.3/corpert/corpert/lcp_corpus_template.json` & `lcpcli-0.1.4/lcpcli/data/lcp_corpus_template.json`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.3/corpert/corpert/parsers/_parser.py` & `lcpcli-0.1.4/lcpcli/parsers/_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,33 @@
 
 Note that .write() doesn't write to file, but returns a string that can be written to file!
 
 TODO: create a class for the entries in self._tables
 TODO: it needs to be easy to make lookup files like *_form for that class too
 TODO: update meta.json when new attributes are discovered
 """
+
 import abc
 import json
 import os
 import re
 
-from ..utils import get_ci, Table, EntityType, Document, Categorical, Dependency, Meta, Text, Sentence, NestedSet
+from ..utils import (
+    get_ci,
+    Table,
+    EntityType,
+    Document,
+    Categorical,
+    Dependency,
+    Meta,
+    Text,
+    Sentence,
+    NestedSet,
+)
+
 
 class Parser(abc.ABC):
     def __init__(self, *args, **kwargs):
         super().__init__()
         self.char_range_cur = 1
         self.frame_range_cur = 0
         self._tables = {}
@@ -58,26 +71,27 @@
     @abc.abstractmethod
     def combine(self, content):
         """
         Combine a dictionary of {original_filepath: json_representation}
         """
         pass
 
-
     def compute_doc(self, content, first_sentence, last_sentence):
         """
         Return (doc_id,char_range,meta) for a given pair of first and last sentences
         """
         meta_obj = {}
         start_idx = re.search(self.start_idx, first_sentence)[0]
-        end_idx   = re.search(self.end_idx, last_sentence)[0]
+        end_idx = re.search(self.end_idx, last_sentence)[0]
         char_range = f"{start_idx},{end_idx}"
 
         # meta_lines = [line for line in content.split("\n\n") if line.startswith("# text")]
-        meta_lines = [line for line in content.split("\n") if line.startswith("# newdoc ")]
+        meta_lines = [
+            line for line in content.split("\n") if line.startswith("# newdoc ")
+        ]
         for line in meta_lines:
             if " = " not in line:
                 continue
             k, v = line.split(" = ")
             meta_obj[k[9:].strip()] = v.strip()
 
         # if "text_id" in meta_obj:
@@ -85,197 +99,214 @@
             doc_id = meta_obj.pop("id")
         else:
             self.text_id += 1
             doc_id = self.text_id
 
         return doc_id, char_range, json.dumps(meta_obj)
 
-
     def upload_new_doc(self, doc, table, docName="document"):
         """
         Take a document instance, a character_range cursor and a file handle, and write a line to the file
         """
         meta = doc.attributes.get("meta")
-        col_names = [f"{docName}_id", 'char_range']
+        col_names = [f"{docName}_id", "char_range"]
         cols = [
             str(table.cursor),
-            f"[{str(doc.char_range_start)},{str(self.char_range_cur-1)})"
+            f"[{str(doc.char_range_start)},{str(self.char_range_cur-1)})",
         ]
         if doc.frame_range[1] != 0:
             col_names.append("frame_range")
             cols.append(f"[{str(doc.frame_range[0])},{str(doc.frame_range[1])})")
             doc_frame_id = str(meta._value.get("name", doc.id) if meta else doc.id)
             self.doc_frames[doc_frame_id] = [*doc.frame_range]
         if meta:
-            if 'name' in meta._value:
+            if "name" in meta._value:
                 # dll_gen would require a lookup table to have a column of type text
                 # cols.append( str(meta._value.pop('name')) )
                 # col_names.append("name")
                 pass
             if meta._value:
-                col_names.append( 'meta' )
-                cols.append( str(meta.value) )
+                col_names.append("meta")
+                cols.append(str(meta.value))
+        mediaSlots = self.config.get("meta", {}).get("mediaSlots", {})
+        if mediaSlots:
+            col_names.append("media")
+            media = doc.attributes.get("media", Meta("dymmy", {})).value
+            for name, attribs in mediaSlots.items():
+                assert (
+                    attribs.get("isOptional") is not False or name in media
+                ), KeyError(
+                    f"Filename missing for required media '{name}' from document {doc.id}"
+                )
+            cols.append(media)
         if table.cursor == 1:
-            table.write( col_names )
-        table.write( cols )
+            table.write(col_names)
+        table.write(cols)
         table.cursor += 1
 
-
-    def write_token_deps(self, table, working_on=''):
+    def write_token_deps(self, table, working_on=""):
         """
         Take a file handle with a 'deps' key that contains NestedSet's to be linked and write to file, then clear memory
         """
         # head_id is None: this is a new head, process the previous one
         empty_segments = []
         nested_set_of_previous_head = None
         for segment_id, tokens in table.deps.items():
             if segment_id == working_on:
                 continue
             for token_id, attrs in tokens.items():
                 # Link the nested sets from the dependencies in memory
-                hid = attrs['head_id']
+                hid = attrs["head_id"]
                 if hid == "":
-                    nested_set_of_previous_head = attrs['nested_set']
+                    nested_set_of_previous_head = attrs["nested_set"]
                 if hid not in tokens:
                     continue
-                tokens[hid]['nested_set'].add(tokens[token_id]['nested_set'])
+                tokens[hid]["nested_set"].add(tokens[token_id]["nested_set"])
             anchor_right = table.anchor_right
             nested_set_of_previous_head.compute_anchors()
             for id in nested_set_of_previous_head.all_ids:
-                nested_set = tokens[id]['nested_set']
-                parent_id = ('' if nested_set.parent is None else str(nested_set.parent.cursor_id))
-                table.write([
-                    str(parent_id),                       # head
-                    str(str(nested_set.cursor_id)),       # dependent (self)
-                    nested_set.label,                     # label
-                    str(anchor_right + nested_set.left),  # left_anchor
-                    str(anchor_right + nested_set.right), # right_anchor
-                ])
+                nested_set = tokens[id]["nested_set"]
+                parent_id = (
+                    ""
+                    if nested_set.parent is None
+                    else str(nested_set.parent.cursor_id)
+                )
+                table.write(
+                    [
+                        str(parent_id),  # head
+                        str(str(nested_set.cursor_id)),  # dependent (self)
+                        nested_set.label,  # label
+                        str(anchor_right + nested_set.left),  # left_anchor
+                        str(anchor_right + nested_set.right),  # right_anchor
+                    ]
+                )
             table.anchor_right = anchor_right + nested_set_of_previous_head.right
             # Now clear the processed tokens
             for id in nested_set_of_previous_head.all_ids:
                 tokens.pop(id)
             if not tokens:
                 empty_segments.append(segment_id)
         # Clear the segments with no tokens left
         for s_id in empty_segments:
             table.deps.pop(s_id)
 
-
-    def aligned_entity(
-        self,
-        entity,
-        path,
-        attribute,
-        aligned_entities={}
-    ):
+    def aligned_entity(self, entity, path, attribute, aligned_entities={}):
         aname_low = attribute.name.lower()
-        assert isinstance(attribute, Text), TypeError(f"Foreign key '{attribute.name}' should be a simple text")
-        layer_name = next( (x for x in self.config.get("layer",{}).keys() if x.lower() == aname_low) , None )
-        layer_attributes = self.config["layer"].get(layer_name,{}).get("attributes",{}) if layer_name else {}
+        assert isinstance(attribute, Text), TypeError(
+            f"Foreign key '{attribute.name}' should be a simple text"
+        )
+        layer_name = next(
+            (x for x in self.config.get("layer", {}).keys() if x.lower() == aname_low),
+            None,
+        )
+        layer_attributes = (
+            self.config["layer"].get(layer_name, {}).get("attributes", {})
+            if layer_name
+            else {}
+        )
         if aname_low not in self._tables:
-            self._tables[aname_low] = Table(aname_low, path, config=get_ci(self.config['layer'], layer_name))
+            self._tables[aname_low] = Table(
+                aname_low, path, config=get_ci(self.config["layer"], layer_name)
+            )
             table = self._tables[aname_low]
-            with open(aligned_entities[aname_low]['fn'], "r") as aligned_file:
+            with open(aligned_entities[aname_low]["fn"], "r") as aligned_file:
                 entity_col_names = [f"{aname_low}_id"]
                 entity_col_names += aligned_file.readline().rstrip().split("\t")[1:]
                 table.colNames = [*entity_col_names]
                 # TODO: form will need a lookup table here too
                 # if 'form' not in entity_col_names:
                 #     entity_col_names.append('form')
                 entity_col_names.append("char_range")
-                table.write( entity_col_names )
+                table.write(entity_col_names)
         table = self._tables[aname_low]
         fk = attribute.value.strip()
         ce = table.currentEntity
         if fk == ce.get("id", ""):
             # TODO: form will need a lookup table here too
             # if 'form' in ce and 'form' not in self._tables[aname_low]['col_names']:
             #     ce['form'] += token.attributes['form'].value + (' ' if token.spaceAfter else '')
             table.previousEntity = entity
             pass
         else:
             if ce:
                 entity_cols = [table.cursor]
                 table.cursor += 1
-                entity_cols += ce['cols']
+                entity_cols += ce["cols"]
                 # Process labels
                 lbls = table.labels
                 for n, col_name in enumerate(table.colNames):
-                    ctype = layer_attributes.get(col_name,{}).get("type","")
+                    ctype = layer_attributes.get(col_name, {}).get("type", "")
                     if ctype != "labels":
                         continue
-                    bits = int('0',2)
+                    bits = int("0", 2)
                     for label in entity_cols[n].split(","):
                         l = label.strip()
                         idx = lbls.get(l, len(lbls))
                         lbls[l] = idx
-                        bs = "1" + ''.join(['0' for _ in range(idx-1)])
-                        bits = bits | int(bs,2)
+                        bs = "1" + "".join(["0" for _ in range(idx - 1)])
+                        bits = bits | int(bs, 2)
                     entity_cols[n] = bin(bits)[2:]
                 # TODO: form will need a lookup table here too
                 # if 'form' in ce and 'form' not in self._tables[aname_low]['col_names']:
                 #     if ce['form'].endswith(' '):
                 #         ce['form'] = ce['form'][:-1]
                 #     entity_cols.append( ce['form'] )
-                range_up = self.char_range_cur - 1 # Stop just before this entity
-                entity_cols.append( f"[{str(ce['range_low'])},{str(range_up)})" )
-                table.write( entity_cols )
+                range_up = self.char_range_cur - 1  # Stop just before this entity
+                entity_cols.append(f"[{str(ce['range_low'])},{str(range_up)})")
+                table.write(entity_cols)
             if not fk or fk.strip() == "_":
                 ce = {}
             else:
-                ce = {'id': fk}
-                with open(aligned_entities[aname_low]['fn'], "r") as aligned_file:
+                ce = {"id": fk}
+                with open(aligned_entities[aname_low]["fn"], "r") as aligned_file:
                     while True:
                         line = aligned_file.readline()
                         if not line:
                             break
                         line = line.rstrip().split("\t")
                         if line[0].strip() == fk:
-                            ce['cols'] = line[1:]
+                            ce["cols"] = line[1:]
                             # TODO: form will need a lookup table here too
                             # if 'form' not in self._tables[aname_low]['col_names']:
                             #     ce['form'] = token.attributes['form'].value + (' ' if token.spaceAfter else '')
-                            ce['range_low'] = str(self.char_range_cur)
+                            ce["range_low"] = str(self.char_range_cur)
                             break
             table.currentEntity = ce
 
-
     def close_aligned_entity(self, name, path, aligned_entities={}):
         dummy_entity = EntityType()
         dummy_attribute = Text(name, "dummy")
         self.aligned_entity(dummy_entity, path, dummy_attribute, aligned_entities)
         if name in self._tables:
             self._tables[name].currentEntity = {}
 
-
     def close_upload_files(self, path="./"):
         if self._tables is None:
             return
         # Write label files
         for n, tab in self._tables.items():
             tab.file.close()
             if not tab.labels:
                 continue
             nlabels = len(tab.labels)
-            with open(os.path.join(path,f"{n}_labels.csv"), "w") as f:
-                f.write( "\t".join(["bit","label"]) + "\n" )
+            with open(os.path.join(path, f"{n}_labels.csv"), "w") as f:
+                f.write("\t".join(["bit", "label"]) + "\n")
                 for l, i in tab.labels.items():
-                    f.write( "\t".join([str(i),str(l)]) + "\n" )
-            tab.config['nlabels'] = nlabels
+                    f.write("\t".join([str(i), str(l)]) + "\n")
+            tab.config["nlabels"] = nlabels
             # Pad 0s to match the bit length
             label_attributes = {}
-            for n, v in tab.config.get("attributes",{}).items():
+            for n, v in tab.config.get("attributes", {}).items():
                 # List all the attributes of type "labels"
                 if v.get("type") != "labels":
                     continue
                 label_attributes[n] = -1
             if not label_attributes:
                 continue
-            with open(tab.path, "r") as input, open(tab.path+".tmp", "w") as output:
+            with open(tab.path, "r") as input, open(tab.path + ".tmp", "w") as output:
                 while True:
                     il = input.readline()
                     if not il:
                         break
                     il = il.rstrip()
                     cols = il.split("\t")
                     if next(x for x in label_attributes.values()) == -1:
@@ -287,94 +318,108 @@
                                 # Report the index of the column corresponding to the attribute
                                 label_attributes[la] = n
                     else:
                         # Not first line = row
                         for n in label_attributes.values():
                             bits = cols[n]
                             if len(bits) < nlabels:
-                                bits = ''.join(['0' for _ in range(nlabels-len(bits))]) + bits
+                                bits = (
+                                    "".join(["0" for _ in range(nlabels - len(bits))])
+                                    + bits
+                                )
                             cols[n] = bits
-                    output.write( "\t".join(cols) + "\n" )
-            os.rename(tab.path+".tmp", tab.path)
+                    output.write("\t".join(cols) + "\n")
+            os.rename(tab.path + ".tmp", tab.path)
 
     def generate_upload_files_generator(
         self,
         reader,
         path="./",
         default_doc={},
         config={},
         aligned_entities={},
-        aligned_entities_segment={}
+        aligned_entities_segment={},
     ):
         """
         Take a reader object and outputs verticalized LCP self._tables
         """
         docName = "document"
         segName = "segment"
         tokName = "token"
         if "firstClass" in config:
-            docName = config['firstClass'].get("document", docName).lower()
-            segName = config['firstClass'].get("segment", segName).lower()
-            tokName = config['firstClass'].get("token", tokName).lower()
+            docName = config["firstClass"].get("document", docName).lower()
+            segName = config["firstClass"].get("segment", segName).lower()
+            tokName = config["firstClass"].get("token", tokName).lower()
 
         self._tables = self._tables or {
-            'document': Table(docName, path, config=get_ci(self.config['layer'], docName)),
-            'segment': Table(segName, path, config=get_ci(self.config['layer'], docName)),
-            'token': Table(tokName, path, config=get_ci(self.config['layer'], docName))
+            "document": Table(
+                docName, path, config=get_ci(self.config["layer"], docName)
+            ),
+            "segment": Table(
+                segName, path, config=get_ci(self.config["layer"], docName)
+            ),
+            "token": Table(tokName, path, config=get_ci(self.config["layer"], docName)),
         }
-        token_table = self._tables['token']
+        token_table = self._tables["token"]
         char_range_start = self.char_range_cur
         has_frame_range = False
         offset_frame_range = self.frame_range_cur
         token_have_dependencies = False
         current_document = None
-        for (segment, doc) in self.parse_generator(reader, config=config):
+        for segment, doc in self.parse_generator(reader, config=config):
 
             char_range_segment_start = self.char_range_cur
             frame_range_segment_start = None
 
             if doc:
                 if current_document is not doc:
                     if current_document:
                         self.upload_new_doc(
-                            current_document,
-                            self._tables['document'],
-                            docName=docName
+                            current_document, self._tables["document"], docName=docName
                         )
                     current_document = doc
                     current_document.char_range_start = char_range_segment_start
 
             if not segment:
                 continue
 
             non_null_attributes = token_table.non_null_attributes
             if not non_null_attributes and token_table.cursor == 1:
-                col_names = {f"{tokName}_id":None}
+                col_names = {f"{tokName}_id": None}
                 for token in segment.tokens:
                     if token.frame_range:
                         has_frame_range = True
                     for attr_name, attr_value in token.attributes.items():
                         if not attr_value.value:
                             continue
                         non_null_attributes[attr_name] = True
-                        if isinstance(attr_value,Dependency) or attr_name.lower() in aligned_entities:
+                        if (
+                            isinstance(attr_value, Dependency)
+                            or attr_name.lower() in aligned_entities
+                        ):
                             continue
-                        if any(isinstance(attr_value,klass) for klass in (Text,Meta)):
+                        if any(isinstance(attr_value, klass) for klass in (Text, Meta)):
                             col_names[attr_name + "_id"] = None
                         else:
                             col_names[attr_name] = None
                 token_table.non_null_attributes = non_null_attributes
-                col_names['char_range'] = None
+                col_names["char_range"] = None
                 if has_frame_range:
-                    col_names['frame_range'] = None
+                    col_names["frame_range"] = None
                 col_names[f"{segName}_id"] = None
-                token_table.write( [c for c in col_names] )
+                token_table.write([c for c in col_names])
 
+            print(
+                "segment",
+                segment.id,
+                "meta",
+                segment.attributes.get("meta", Meta("dummy", "dummy")).value,
+            )
             for token in segment.tokens:
-                cols = [ str(token_table.cursor) ]
+                cols = [str(token_table.cursor)]
                 for attr_name in non_null_attributes:
                     attribute = token.attributes.get(attr_name, None)
                     aname_low = attr_name.lower()
 
                     if attribute is None:
                         cols.append("")
                         continue
@@ -438,143 +483,172 @@
                         #                     # if 'form' not in self._tables[aname_low]['col_names']:
                         #                     #     ce['form'] = token.attributes['form'].value + (' ' if token.spaceAfter else '')
                         #                     ce['range_low'] = str(self.char_range_cur)
                         #                     break
                         #     self._tables[aname_low]['currentEntity'] = ce
 
                     elif isinstance(attribute, Categorical):
-                        cols.append( str(attribute.value) )
+                        cols.append(str(attribute.value))
 
                     # if isinstance(attribute, Meta):
                     #     cols.append( json.dumps(attribute.value) )
 
                     # We create dicts for text attributes to keep track of their IDs
                     # One idea to optimize memory:
                     # - only using a dict (form -> id) and no verticalized file at all to start with
                     # - once the dict's length passes a certain threshold (e.g. 10k diff entries)
                     #   then start writing entries to self._tables whose name start with the text's first letter
                     # - if a text is not found in the dict, look up the file, and if not found in the file, write to it
-                    elif any(isinstance(attribute, klass) for klass in (Text,Meta)):
+                    elif any(isinstance(attribute, klass) for klass in (Text, Meta)):
                         name = f"{tokName}_{attribute.name}"
                         if name not in self._tables:
                             self._tables[name] = Table(name, path)
                         table = self._tables[name]
                         text = str(attribute.value)
-                        id = table.texts.get(text,0)
+                        id = table.texts.get(text, 0)
                         if id < 1:
                             id = table.cursor
                             table.texts[text] = id
                             if table.cursor == 1:
-                                table.write( [f"{attribute.name}_id", attribute.name] )
+                                table.write([f"{attribute.name}_id", attribute.name])
                             table.cursor += 1
-                            table.write( [str(id),text] )
-                        cols.append( str(id) )
+                            table.write([str(id), text])
+                        cols.append(str(id))
 
                     elif isinstance(attribute, Dependency):
                         # token_have_dependencies = True
                         name = attribute.name
                         if name not in self._tables:
                             self._tables[name] = Table(name, path)
-                            self._tables[name].write( ['head','dependent','label','left_anchor','right_anchor'] )
+                            self._tables[name].write(
+                                [
+                                    "head",
+                                    "dependent",
+                                    "label",
+                                    "left_anchor",
+                                    "right_anchor",
+                                ]
+                            )
                         table = self._tables[name]
                         if str(segment.id) not in table.deps:
                             table.deps[str(segment.id)] = {}
                         deps = table.deps[str(segment.id)]
                         head_id = attribute.value
                         # We assume a new head necessarily means all of the previous head's dependencies have been parsed
                         if head_id == "" and deps:
                             # head_id is None: this is a new head, process the previous one
-                            self.write_token_deps(self._tables[name], working_on=str(segment.id))
+                            self.write_token_deps(
+                                self._tables[name], working_on=str(segment.id)
+                            )
                         deps[token.id] = {
-                            'head_id': head_id,
-                            'nested_set': NestedSet(token.id, attribute.label, token_table.cursor)
+                            "head_id": head_id,
+                            "nested_set": NestedSet(
+                                token.id, attribute.label, token_table.cursor
+                            ),
                         }
                         self._tables[name].cursor += 1
 
                 # If this token doesn't have an attribute for an aligned entity, close any pending one
                 for aligned_entity in aligned_entities:
                     if aligned_entity in [a.lower() for a in non_null_attributes]:
                         continue
                     self.close_aligned_entity(aligned_entity, path, aligned_entities)
 
                 left_char_range = self.char_range_cur
-                self.char_range_cur += len(token.attributes['form'].value) - (0 if token.spaceAfter else 1)
-                cols.append( f"[{str(left_char_range)},{str(self.char_range_cur)})" )
+                self.char_range_cur += len(token.attributes["form"].value) - (
+                    0 if token.spaceAfter else 1
+                )
+                cols.append(f"[{str(left_char_range)},{str(self.char_range_cur)})")
                 self.char_range_cur += 1
                 if token.frame_range:
-                    has_frame_range = True # Keep it here too for iterations where non_null_attributes is already set
+                    has_frame_range = True  # Keep it here too for iterations where non_null_attributes is already set
                     left_frame_range, right_frame_range = token.frame_range
                     left_frame_range += offset_frame_range
                     right_frame_range += offset_frame_range
-                    cols.append( f"[{str(left_frame_range)},{str(right_frame_range)})" )
+                    cols.append(f"[{str(left_frame_range)},{str(right_frame_range)})")
                     if current_document:
                         if current_document.frame_range[0] == 0:
-                            current_document.frame_range[0] = offset_frame_range + token.frame_range[0]
-                        current_document.frame_range[1] = offset_frame_range + token.frame_range[1]
+                            current_document.frame_range[0] = (
+                                offset_frame_range + token.frame_range[0]
+                            )
+                        current_document.frame_range[1] = (
+                            offset_frame_range + token.frame_range[1]
+                        )
                     if frame_range_segment_start is None:
-                        frame_range_segment_start = offset_frame_range + token.frame_range[0]
+                        frame_range_segment_start = (
+                            offset_frame_range + token.frame_range[0]
+                        )
                     self.frame_range_cur = right_frame_range
-                cols.append( str(segment.id) )
-                token_table.write( cols )
+                cols.append(str(segment.id))
+                token_table.write(cols)
                 token_table.cursor += 1
 
-            segment_table = self._tables['segment']
+            segment_table = self._tables["segment"]
             if segment_table.cursor == 1:
-                col_names = [f"{segName}_id",'char_range']
+                col_names = [f"{segName}_id", "char_range"]
                 if has_frame_range:
                     col_names.append("frame_range")
                 # Add the names of all segment attributes
                 for a in segment.attributes:
                     if a in aligned_entities_segment:
                         continue
                     col_names.append(a)
-                segment_table.write( col_names )
-            cols = [ str(segment.id) ]
-            cols.append( f"[{char_range_segment_start},{self.char_range_cur-1})" )
+                segment_table.write(col_names)
+            cols = [str(segment.id)]
+            cols.append(f"[{char_range_segment_start},{self.char_range_cur-1})")
             if has_frame_range:
-                cols.append( f"[{str(frame_range_segment_start)},{str(self.frame_range_cur)})" )
+                cols.append(
+                    f"[{str(frame_range_segment_start)},{str(self.frame_range_cur)})"
+                )
             # Add all segment attributes
             for a in segment.attributes.values():
                 aname_low = a.name.lower()
                 if aname_low in aligned_entities_segment:
                     self.aligned_entity(segment, path, a, aligned_entities_segment)
                 else:
-                    cols.append( a.value )
+                    cols.append(a.value)
             # If this segment doesn't have an attribute for one the aligned entities, close it
             for aligned_entity in aligned_entities_segment:
                 if aligned_entity in [a.lower() for a in segment.attributes.keys()]:
                     continue
-                self.close_aligned_entity(aligned_entity, path, aligned_entities_segment)
+                self.close_aligned_entity(
+                    aligned_entity, path, aligned_entities_segment
+                )
             # Now write to the file and update cursor
-            segment_table.write( cols )
+            segment_table.write(cols)
             segment_table.cursor += 1
 
             # FTS VECTOR if no dependencies
             # Always run for now, since we don't use the same value for "LABEL_IN" and "LABELS_OUT"
             if not token_have_dependencies:
                 name = "fts_vector"
                 if name not in self._tables:
                     self._tables[name] = Table(name, path)
                 fts_table = self._tables[name]
                 vector = []
                 for n, token in enumerate(segment.tokens, start=1):
                     attributes_to_fts = []
                     for an in non_null_attributes:
                         a = token.attributes[an]
-                        if any(isinstance(a,k) for k in (Categorical,Text)) and an.lower() not in aligned_entities:
+                        if (
+                            any(isinstance(a, k) for k in (Categorical, Text))
+                            and an.lower() not in aligned_entities
+                        ):
                             attributes_to_fts.append(a)
-                        elif isinstance(a,Dependency): # same value for LABEL_IN and LABELS_OUT
+                        elif isinstance(
+                            a, Dependency
+                        ):  # same value for LABEL_IN and LABELS_OUT
                             attributes_to_fts.append(a)
                             attributes_to_fts.append(a)
                     for i, a in enumerate(attributes_to_fts, start=1):
                         vector.append(f"'{i}{str(a.value)}':{n}")
-                cols[1:] = [ " ".join(vector) ]
+                cols[1:] = [" ".join(vector)]
                 if fts_table.cursor == 1:
-                    fts_table.write( [f"{segName}_id", 'vector'] )
-                fts_table.write( cols )
+                    fts_table.write([f"{segName}_id", "vector"])
+                fts_table.write(cols)
                 fts_table.cursor += 1
 
         if token_have_dependencies:
             # Write any pending dependencies
             for _, tab in self._tables.items():
                 if not tab.deps:
                     continue
@@ -586,23 +660,19 @@
         for ename in aligned_entities_segment:
             self.close_aligned_entity(ename, path, aligned_entities_segment)
 
         if current_document is None:
             # No new document marker found when parsing: create an all-encompassing one
             current_document = Document()
             if default_doc:
-                current_document.attributes['meta'] = Meta("meta", default_doc)
+                current_document.attributes["meta"] = Meta("meta", default_doc)
             current_document.char_range_start = char_range_start
 
         # Write the last document
-        self.upload_new_doc(
-            current_document,
-            self._tables['document'],
-            docName=docName
-        )
+        self.upload_new_doc(current_document, self._tables["document"], docName=docName)
 
         # for _, v in self._tables.items():
         #     v['file'].close()
 
     def generate_upload_files(self, content):
         """
         Return ([sentences], (doc_id,char_range,meta)) for a given document file
@@ -624,12 +694,16 @@
 
         for s in proc_sentences:
             for l in s.proc_lines:
                 for _ in range(ncols - len(l)):
                     l.append("")
 
         if proc_sentences:
-            doc = self.compute_doc(content, proc_sentences[0].proc_lines[0][6], proc_sentences[-1].proc_lines[-1][6])
+            doc = self.compute_doc(
+                content,
+                proc_sentences[0].proc_lines[0][6],
+                proc_sentences[-1].proc_lines[-1][6],
+            )
             # self.compute_doc()
             return proc_sentences, doc
         else:
-            return None, None
+            return None, None
```

### Comparing `lcpcli-0.1.3/lcpcli/cli.py` & `lcpcli-0.1.4/lcpcli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 
 
 def _parse_cmd_line():
     """
     Helper for parsing CLI call and displaying help message
     """
     parser = argparse.ArgumentParser(description="Convert and upload corpus to LCP")
-    
+
     # CORPERT
     parser.add_argument(
         "-i", "--input", type=str, required=False, help="Input file path"
     )
     parser.add_argument("-o", "--output", type=str, help="Output file path")
     parser.add_argument(
         "-m",
         "--mode",
         type=str,
         nargs="?",
         choices=["normal", "upload"],
         default="normal",
-        help="LCP upload ('upload') or not ('normal', default)")
+        help="LCP upload ('upload') or not ('normal', default)",
+    )
     parser.add_argument(
         "-e", "--extension", type=str, help="Output format when output is a directory"
     )
     parser.add_argument(
         "-f", "--filter", required=False, type=str, help="Path to a Python filter file"
     )
     parser.add_argument(
@@ -43,15 +44,15 @@
         "--combine",
         required=False,
         type=bool,
         default=False,
         help="Combine into single file?",
         # action=argparse.BooleanOptionalAction,
     )
-    
+
     # LCPUPLOAD
     parser.add_argument(
         "-c",
         "--corpus",
         type=str,
         required=False,
         help="Corpus path (either a directory or a zip/7z/tar/tar.gz/tar.xz archive)",
@@ -86,22 +87,37 @@
     )
     parser.add_argument(
         "-l",
         "--live",
         required=False,
         default=False,
         help="Use live system? If false, use test system.",
-        **BOOL_KWARGS
+        **BOOL_KWARGS,
     )
     parser.add_argument(
         "-v",
         "--vian",
         required=False,
         default=False,
         help="Upload to VIAN instead of LCP?",
-        **BOOL_KWARGS
+        **BOOL_KWARGS,
+    )
+    parser.add_argument(
+        "-t",
+        "--to",
+        type=str,
+        required=False,
+        help="URL of the LCP instance receiving the corpus.",
     )
-    
+    parser.add_argument(
+        "-ch",
+        "--check-only",
+        required=False,
+        default=False,
+        help="Use live system? If false, use test system.",
+        **BOOL_KWARGS,
+    )
+
     kwargs = vars(parser.parse_args())
     kwargs["content"] = kwargs.pop("input", "")
     kwargs["template"] = kwargs.pop("json", False)
     return kwargs
```

