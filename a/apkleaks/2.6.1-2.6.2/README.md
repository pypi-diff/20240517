# Comparing `tmp/apkleaks-2.6.1.tar.gz` & `tmp/apkleaks-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkleaks-2.6.1.tar", last modified: Tue Nov  7 03:55:01 2023, max compression
+gzip compressed data, was "apkleaks-2.6.2.tar", last modified: Fri May 17 12:24:17 2024, max compression
```

## Comparing `apkleaks-2.6.1.tar` & `apkleaks-2.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2023-11-07 03:55:01.713478 apkleaks-2.6.1/
--rw-rw-r--   0 dw1       (1000) dw1       (1000)    11345 2023-02-09 08:55:11.000000 apkleaks-2.6.1/LICENSE
--rw-rw-r--   0 dw1       (1000) dw1       (1000)      108 2023-02-09 08:55:11.000000 apkleaks-2.6.1/MANIFEST.in
--rw-r--r--   0 dw1       (1000) dw1       (1000)     5480 2023-11-07 03:55:01.713478 apkleaks-2.6.1/PKG-INFO
--rw-rw-r--   0 dw1       (1000) dw1       (1000)     5002 2023-11-07 03:50:58.000000 apkleaks-2.6.1/README.md
--rw-rw-r--   0 dw1       (1000) dw1       (1000)        6 2023-02-09 08:55:11.000000 apkleaks-2.6.1/VERSION
-drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2023-11-07 03:55:01.713478 apkleaks-2.6.1/apkleaks/
--rw-rw-r--   0 dw1       (1000) dw1       (1000)        0 2023-02-09 08:55:11.000000 apkleaks-2.6.1/apkleaks/__init__.py
--rw-rw-r--   0 dw1       (1000) dw1       (1000)     5309 2023-11-07 03:50:58.000000 apkleaks-2.6.1/apkleaks/apkleaks.py
--rwxrwxr-x   0 dw1       (1000) dw1       (1000)     1579 2023-02-09 08:55:11.000000 apkleaks-2.6.1/apkleaks/cli.py
--rw-rw-r--   0 dw1       (1000) dw1       (1000)      201 2023-02-09 08:55:11.000000 apkleaks-2.6.1/apkleaks/colors.py
--rw-rw-r--   0 dw1       (1000) dw1       (1000)      704 2023-02-09 08:55:11.000000 apkleaks-2.6.1/apkleaks/utils.py
-drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2023-11-07 03:55:01.713478 apkleaks-2.6.1/apkleaks.egg-info/
--rw-r--r--   0 dw1       (1000) dw1       (1000)     5480 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/PKG-INFO
--rw-rw-r--   0 dw1       (1000) dw1       (1000)      396 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/SOURCES.txt
--rw-rw-r--   0 dw1       (1000) dw1       (1000)        1 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/dependency_links.txt
--rw-rw-r--   0 dw1       (1000) dw1       (1000)       47 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/entry_points.txt
--rw-rw-r--   0 dw1       (1000) dw1       (1000)       21 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/requires.txt
--rw-rw-r--   0 dw1       (1000) dw1       (1000)       16 2023-11-07 03:55:01.000000 apkleaks-2.6.1/apkleaks.egg-info/top_level.txt
-drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2023-11-07 03:55:01.713478 apkleaks-2.6.1/config/
--rw-rw-r--   0 dw1       (1000) dw1       (1000)      829 2023-02-09 08:55:11.000000 apkleaks-2.6.1/config/notkeyhacks.json
--rw-rw-r--   0 dw1       (1000) dw1       (1000)     4619 2023-02-09 08:55:11.000000 apkleaks-2.6.1/config/regexes.json
--rw-rw-r--   0 dw1       (1000) dw1       (1000)       21 2023-02-09 08:55:11.000000 apkleaks-2.6.1/requirements.txt
--rw-rw-r--   0 dw1       (1000) dw1       (1000)       38 2023-11-07 03:55:01.713478 apkleaks-2.6.1/setup.cfg
--rw-rw-r--   0 dw1       (1000) dw1       (1000)     1193 2023-02-09 08:55:11.000000 apkleaks-2.6.1/setup.py
+drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2024-05-17 12:24:17.830216 apkleaks-2.6.2/
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)    11345 2024-05-17 12:19:09.000000 apkleaks-2.6.2/LICENSE
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)      108 2023-11-17 14:27:15.000000 apkleaks-2.6.2/MANIFEST.in
+-rw-r--r--   0 dw1       (1000) dw1       (1000)     5629 2024-05-17 12:24:17.830216 apkleaks-2.6.2/PKG-INFO
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)     5151 2023-11-17 14:27:24.000000 apkleaks-2.6.2/README.md
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)        6 2024-05-17 12:10:46.000000 apkleaks-2.6.2/VERSION
+drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2024-05-17 12:24:17.826216 apkleaks-2.6.2/apkleaks/
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)        0 2023-11-17 14:27:15.000000 apkleaks-2.6.2/apkleaks/__init__.py
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)     5288 2024-05-17 12:04:33.000000 apkleaks-2.6.2/apkleaks/apkleaks.py
+-rwxrwxr-x   0 dw1       (1000) dw1       (1000)     1692 2024-05-17 12:19:00.000000 apkleaks-2.6.2/apkleaks/cli.py
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)      201 2023-11-17 14:27:15.000000 apkleaks-2.6.2/apkleaks/colors.py
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)      704 2023-11-17 14:27:15.000000 apkleaks-2.6.2/apkleaks/utils.py
+drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2024-05-17 12:24:17.826216 apkleaks-2.6.2/apkleaks.egg-info/
+-rw-r--r--   0 dw1       (1000) dw1       (1000)     5629 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/PKG-INFO
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)      396 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/SOURCES.txt
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)        1 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/dependency_links.txt
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)       47 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/entry_points.txt
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)       21 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/requires.txt
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)       16 2024-05-17 12:24:17.000000 apkleaks-2.6.2/apkleaks.egg-info/top_level.txt
+drwxrwxr-x   0 dw1       (1000) dw1       (1000)        0 2024-05-17 12:24:17.826216 apkleaks-2.6.2/config/
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)      829 2023-11-17 14:27:15.000000 apkleaks-2.6.2/config/notkeyhacks.json
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)     4619 2023-11-17 14:27:15.000000 apkleaks-2.6.2/config/regexes.json
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)       21 2023-11-17 14:27:15.000000 apkleaks-2.6.2/requirements.txt
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)       38 2024-05-17 12:24:17.830216 apkleaks-2.6.2/setup.cfg
+-rw-rw-r--   0 dw1       (1000) dw1       (1000)     1193 2023-11-17 14:27:15.000000 apkleaks-2.6.2/setup.py
```

### Comparing `apkleaks-2.6.1/LICENSE` & `apkleaks-2.6.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2020-2021 dwisiswant0
+   Copyright 2020-2024 dwisiswant0
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `apkleaks-2.6.1/PKG-INFO` & `apkleaks-2.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkleaks
-Version: 2.6.1
+Version: 2.6.2
 Summary: Scanning APK file for URIs, endpoints & secrets.
 Home-page: https://github.com/dwisiswant0/apkleaks/
 Author: dwisiswant0
 Author-email: me@dw1.io
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -26,16 +26,15 @@
   - [from Pypi](#from-pypi)
   - [from Source](#from-source)
   - [from Docker](#from-docker)
 - [Usage](#usage)
   - [Options](#options)
     - [Output](#output)
     - [Pattern](#pattern)
-    - [Pattern](#pattern)
-    - [Arguments (disassembler)](#arguments-disassembler)
+    - [Arguments (for disassembler)](#arguments-for-disassembler)
 - [License](#license)
 - [Acknowledments](#acknowledments)
 
 ---
 
 ## Installation
 
@@ -63,15 +62,15 @@
 
 ```bash
 $ docker pull dwisiswant0/apkleaks:latest
 ```
 
 ### Dependencies
 
-APKLeaks using [jadx](https://github.com/skylot/jadx) disassembler to decompile APK file. If it doesn't exist in your environment, it'll ask you to download.
+The APKLeaks utilizes the [jadx](https://github.com/skylot/jadx) disassembler to decompile APK files. If jadx is not present in your system, it will prompt you to download it.
 
 ## Usage
 
 Simply,
 
 ```bash
 $ apkleaks -f ~/path/to/file.apk
@@ -87,49 +86,53 @@
 
 | **Argument**  	| **Description**                             	| **Example**                                                   |
 |---------------	|---------------------------------------------	|-------------------------------------------------------------  |
 | -f, --file    	| APK file to scanning                        	| `apkleaks -f file.apk`                                        |
 | -o, --output  	| Write to file results _(random if not set)_ 	| `apkleaks -f file.apk -o results.txt`                         |
 | -p, --pattern 	| Path to custom patterns JSON                	| `apkleaks -f file.apk -p custom-rules.json`                   |
 | -a, --args    	| Disassembler arguments                      	| `apkleaks -f file.apk --args="--deobf --log-level DEBUG"`     |
-| --json        	| Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
+|     --json      | Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
 
 ### Output
 
 In general, if you don't provide `-o` argument, then it will generate results file automatically.
 
-**NOTE:** By default it will also save the results in text format, use `--json` argument if you want JSON output format.
+> [!TIP]
+> By default it will also save the results in text format, use `--json` argument if you want JSON output format.
 
 ### Pattern
 
-Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If not set, it'll use default patterns from [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
+Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If no file is set, the tool will use the default patterns found in [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
 
-Example patterns file:
+Here's an example of what a custom pattern file could look like:
 
 ```json
 // custom-rules.json
 {
   "Amazon AWS Access Key ID": "AKIA[0-9A-Z]{16}",
-  ...
+  // ...
 }
 ```
 
-```
+To run the tool using these custom rules, use the following command:
+
+```bash
 $ apkleaks -f /path/to/file.apk -p rules.json -o ~/Documents/apkleaks-results.txt
 ```
 
 ### Arguments (disassembler)
 
 We give user complete discretion to pass the disassembler arguments. For example, if you want to activate threads in `jadx` decompilation process, you can add it with `-a/--args` argument, example: `--args="--threads-count 5"`.
 
 ```
 $ apkleaks -f /path/to/file.apk -a "--deobf --log-level DEBUG"
 ```
 
-**NOTE:** Please pay attention to the default disassembler arguments we use to prevent collisions.
+> [!WARNING]
+> Please pay attention to the default disassembler arguments we use to prevent collisions.
 
 ## License
 
 `apkleaks` is distributed under Apache 2.
 
 ## Acknowledments
```

### Comparing `apkleaks-2.6.1/README.md` & `apkleaks-2.6.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,15 @@
   - [from Pypi](#from-pypi)
   - [from Source](#from-source)
   - [from Docker](#from-docker)
 - [Usage](#usage)
   - [Options](#options)
     - [Output](#output)
     - [Pattern](#pattern)
-    - [Pattern](#pattern)
-    - [Arguments (disassembler)](#arguments-disassembler)
+    - [Arguments (for disassembler)](#arguments-for-disassembler)
 - [License](#license)
 - [Acknowledments](#acknowledments)
 
 ---
 
 ## Installation
 
@@ -47,15 +46,15 @@
 
 ```bash
 $ docker pull dwisiswant0/apkleaks:latest
 ```
 
 ### Dependencies
 
-APKLeaks using [jadx](https://github.com/skylot/jadx) disassembler to decompile APK file. If it doesn't exist in your environment, it'll ask you to download.
+The APKLeaks utilizes the [jadx](https://github.com/skylot/jadx) disassembler to decompile APK files. If jadx is not present in your system, it will prompt you to download it.
 
 ## Usage
 
 Simply,
 
 ```bash
 $ apkleaks -f ~/path/to/file.apk
@@ -71,49 +70,53 @@
 
 | **Argument**  	| **Description**                             	| **Example**                                                   |
 |---------------	|---------------------------------------------	|-------------------------------------------------------------  |
 | -f, --file    	| APK file to scanning                        	| `apkleaks -f file.apk`                                        |
 | -o, --output  	| Write to file results _(random if not set)_ 	| `apkleaks -f file.apk -o results.txt`                         |
 | -p, --pattern 	| Path to custom patterns JSON                	| `apkleaks -f file.apk -p custom-rules.json`                   |
 | -a, --args    	| Disassembler arguments                      	| `apkleaks -f file.apk --args="--deobf --log-level DEBUG"`     |
-| --json        	| Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
+|     --json      | Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
 
 ### Output
 
 In general, if you don't provide `-o` argument, then it will generate results file automatically.
 
-**NOTE:** By default it will also save the results in text format, use `--json` argument if you want JSON output format.
+> [!TIP]
+> By default it will also save the results in text format, use `--json` argument if you want JSON output format.
 
 ### Pattern
 
-Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If not set, it'll use default patterns from [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
+Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If no file is set, the tool will use the default patterns found in [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
 
-Example patterns file:
+Here's an example of what a custom pattern file could look like:
 
 ```json
 // custom-rules.json
 {
   "Amazon AWS Access Key ID": "AKIA[0-9A-Z]{16}",
-  ...
+  // ...
 }
 ```
 
-```
+To run the tool using these custom rules, use the following command:
+
+```bash
 $ apkleaks -f /path/to/file.apk -p rules.json -o ~/Documents/apkleaks-results.txt
 ```
 
 ### Arguments (disassembler)
 
 We give user complete discretion to pass the disassembler arguments. For example, if you want to activate threads in `jadx` decompilation process, you can add it with `-a/--args` argument, example: `--args="--threads-count 5"`.
 
 ```
 $ apkleaks -f /path/to/file.apk -a "--deobf --log-level DEBUG"
 ```
 
-**NOTE:** Please pay attention to the default disassembler arguments we use to prevent collisions.
+> [!WARNING]
+> Please pay attention to the default disassembler arguments we use to prevent collisions.
 
 ## License
 
 `apkleaks` is distributed under Apache 2.
 
 ## Acknowledments
```

### Comparing `apkleaks-2.6.1/apkleaks/apkleaks.py` & `apkleaks-2.6.2/apkleaks/apkleaks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 import re
 import shutil
 import sys
 import tempfile
 import threading
 
 from contextlib import closing
-from distutils.spawn import find_executable
+from shutil import which
 from pathlib import Path
 from pipes import quote
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 from pyaxmlparser import APK
 
 from apkleaks.colors import color as col
 from apkleaks.utils import util
 
 class APKLeaks:
 	def __init__(self, args):
 		self.apk = None
-		self.file = args.file
+		self.file = os.path.realpath(args.file)
 		self.json = args.json
 		self.disarg = args.args
 		self.prefix = "apkleaks-"
 		self.tempdir = tempfile.mkdtemp(prefix=self.prefix)
 		self.main_dir = os.path.dirname(os.path.realpath(__file__))
 		self.output = tempfile.mkstemp(suffix=".%s" % ("json" if self.json else "txt"), prefix=self.prefix)[1] if args.output is None else args.output
 		self.fileout = open(self.output, "%s" % ("w" if self.json else "a"))
 		self.pattern = os.path.join(str(Path(self.main_dir).parent), "config", "regexes.json") if args.pattern is None else args.pattern
-		self.jadx = find_executable("jadx") if find_executable("jadx") is not None else os.path.join(str(Path(self.main_dir).parent), "jadx", "bin", "jadx%s" % (".bat" if os.name == "nt" else "")).replace("\\","/")
+		self.jadx = which("jadx") if which("jadx") is not None else os.path.join(str(Path(self.main_dir).parent), "jadx", "bin", "jadx%s" % (".bat" if os.name == "nt" else "")).replace("\\","/")
 		self.out_json = {}
 		self.scanned = False
 		logging.config.dictConfig({"version": 1, "disable_existing_loggers": True})
 
 	def apk_info(self):
 		return APK(self.file)
```

### Comparing `apkleaks-2.6.1/apkleaks/cli.py` & `apkleaks-2.6.2/apkleaks/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 import argparse
 import os
 import sys
 from pathlib import Path
 
-import pkg_resources
-
 from apkleaks.apkleaks import APKLeaks
 from apkleaks.colors import color as col
 
 def header():
 	try:
-		VERSION = "v" + pkg_resources.require("apkleaks")[0].version
-	except Exception:
-		VERSION = open(os.path.join(str(Path(__file__).parent.parent), "VERSION"), "r").read().strip()
-	print(col.HEADER + "     _    ____  _  ___               _        \n    / \\  |  _ \\| |/ / |    ___  __ _| | _____ \n   / _ \\ | |_) | ' /| |   / _ \\/ _` | |/ / __|\n  / ___ \\|  __/| . \\| |__|  __/ (_| |   <\\__ \\\n /_/   \\_\\_|   |_|\\_\\_____\\___|\\__,_|_|\\_\\___/\n {}\n --\n Scanning APK file for URIs, endpoints & secrets\n (c) 2020-2021, dwisiswant0\n".format(VERSION) + col.ENDC, file=sys.stderr)
+		from importlib import metadata
+		VERSION = "v" + metadata.version("apkleaks")
+	except ImportError:
+		try:
+			import pkg_resources
+			VERSION = "v" + pkg_resources.require("apkleaks")[0].version
+		except Exception:
+			VERSION = open(os.path.join(str(Path(__file__).parent.parent), "VERSION"), "r").read().strip()
+	print(col.HEADER + "     _    ____  _  ___               _        \n    / \\  |  _ \\| |/ / |    ___  __ _| | _____ \n   / _ \\ | |_) | ' /| |   / _ \\/ _` | |/ / __|\n  / ___ \\|  __/| . \\| |__|  __/ (_| |   <\\__ \\\n /_/   \\_\\_|   |_|\\_\\_____\\___|\\__,_|_|\\_\\___/\n {}\n --\n Scanning APK file for URIs, endpoints & secrets\n (c) 2020-2024, dwisiswant0\n".format(VERSION) + col.ENDC, file=sys.stderr)
 
 def argument():
 	parser = argparse.ArgumentParser()
 	parser.add_argument("-f", "--file", help="APK file to scanning", type=str, required=True)
 	parser.add_argument("-o", "--output", help="Write to file results (random if not set)", type=str, required=False)
 	parser.add_argument("-p", "--pattern", help="Path to custom patterns JSON", type=str, required=False)
 	parser.add_argument("-a", "--args", help="Disassembler arguments (e.g. --threads-count 5 --deobf)", type=str, required=False)
```

### Comparing `apkleaks-2.6.1/apkleaks/utils.py` & `apkleaks-2.6.2/apkleaks/utils.py`

 * *Files identical despite different names*

### Comparing `apkleaks-2.6.1/apkleaks.egg-info/PKG-INFO` & `apkleaks-2.6.2/apkleaks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkleaks
-Version: 2.6.1
+Version: 2.6.2
 Summary: Scanning APK file for URIs, endpoints & secrets.
 Home-page: https://github.com/dwisiswant0/apkleaks/
 Author: dwisiswant0
 Author-email: me@dw1.io
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -26,16 +26,15 @@
   - [from Pypi](#from-pypi)
   - [from Source](#from-source)
   - [from Docker](#from-docker)
 - [Usage](#usage)
   - [Options](#options)
     - [Output](#output)
     - [Pattern](#pattern)
-    - [Pattern](#pattern)
-    - [Arguments (disassembler)](#arguments-disassembler)
+    - [Arguments (for disassembler)](#arguments-for-disassembler)
 - [License](#license)
 - [Acknowledments](#acknowledments)
 
 ---
 
 ## Installation
 
@@ -63,15 +62,15 @@
 
 ```bash
 $ docker pull dwisiswant0/apkleaks:latest
 ```
 
 ### Dependencies
 
-APKLeaks using [jadx](https://github.com/skylot/jadx) disassembler to decompile APK file. If it doesn't exist in your environment, it'll ask you to download.
+The APKLeaks utilizes the [jadx](https://github.com/skylot/jadx) disassembler to decompile APK files. If jadx is not present in your system, it will prompt you to download it.
 
 ## Usage
 
 Simply,
 
 ```bash
 $ apkleaks -f ~/path/to/file.apk
@@ -87,49 +86,53 @@
 
 | **Argument**  	| **Description**                             	| **Example**                                                   |
 |---------------	|---------------------------------------------	|-------------------------------------------------------------  |
 | -f, --file    	| APK file to scanning                        	| `apkleaks -f file.apk`                                        |
 | -o, --output  	| Write to file results _(random if not set)_ 	| `apkleaks -f file.apk -o results.txt`                         |
 | -p, --pattern 	| Path to custom patterns JSON                	| `apkleaks -f file.apk -p custom-rules.json`                   |
 | -a, --args    	| Disassembler arguments                      	| `apkleaks -f file.apk --args="--deobf --log-level DEBUG"`     |
-| --json        	| Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
+|     --json      | Save as JSON format                         	| `apkleaks -f file.apk -o results.json --json`                 |
 
 ### Output
 
 In general, if you don't provide `-o` argument, then it will generate results file automatically.
 
-**NOTE:** By default it will also save the results in text format, use `--json` argument if you want JSON output format.
+> [!TIP]
+> By default it will also save the results in text format, use `--json` argument if you want JSON output format.
 
 ### Pattern
 
-Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If not set, it'll use default patterns from [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
+Custom patterns can be added with the following argument to provide sensitive _search rules_ in the JSON file format: `--pattern /path/to/custom-rules.json`. If no file is set, the tool will use the default patterns found in [regexes.json](https://github.com/dwisiswant0/apkleaks/blob/master/config/regexes.json) file.
 
-Example patterns file:
+Here's an example of what a custom pattern file could look like:
 
 ```json
 // custom-rules.json
 {
   "Amazon AWS Access Key ID": "AKIA[0-9A-Z]{16}",
-  ...
+  // ...
 }
 ```
 
-```
+To run the tool using these custom rules, use the following command:
+
+```bash
 $ apkleaks -f /path/to/file.apk -p rules.json -o ~/Documents/apkleaks-results.txt
 ```
 
 ### Arguments (disassembler)
 
 We give user complete discretion to pass the disassembler arguments. For example, if you want to activate threads in `jadx` decompilation process, you can add it with `-a/--args` argument, example: `--args="--threads-count 5"`.
 
 ```
 $ apkleaks -f /path/to/file.apk -a "--deobf --log-level DEBUG"
 ```
 
-**NOTE:** Please pay attention to the default disassembler arguments we use to prevent collisions.
+> [!WARNING]
+> Please pay attention to the default disassembler arguments we use to prevent collisions.
 
 ## License
 
 `apkleaks` is distributed under Apache 2.
 
 ## Acknowledments
```

### Comparing `apkleaks-2.6.1/config/notkeyhacks.json` & `apkleaks-2.6.2/config/notkeyhacks.json`

 * *Files identical despite different names*

### Comparing `apkleaks-2.6.1/config/regexes.json` & `apkleaks-2.6.2/config/regexes.json`

 * *Files identical despite different names*

### Comparing `apkleaks-2.6.1/setup.py` & `apkleaks-2.6.2/setup.py`

 * *Files identical despite different names*

