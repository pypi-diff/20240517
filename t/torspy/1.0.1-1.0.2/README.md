# Comparing `tmp/torspy-1.0.1.tar.gz` & `tmp/torspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torspy-1.0.1.tar", last modified: Fri May 17 10:16:10 2024, max compression
+gzip compressed data, was "torspy-1.0.2.tar", last modified: Fri May 17 15:14:29 2024, max compression
```

## Comparing `torspy-1.0.1.tar` & `torspy-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.956159 torspy-1.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-17 10:15:32.000000 torspy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5549 2024-05-17 10:16:10.956159 torspy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4846 2024-05-17 10:15:32.000000 torspy-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 10:16:10.956159 torspy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-17 10:15:32.000000 torspy-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.909307 torspy-1.0.1/torspy/
--rw-rw-rw-   0        0        0       78 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/__init__.py
--rw-rw-rw-   0        0        0     1145 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/cli.py
--rw-rw-rw-   0        0        0     4887 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/scraper.py
--rw-rw-rw-   0        0        0      102 2024-05-17 10:15:32.000000 torspy-1.0.1/torspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:16:10.956159 torspy-1.0.1/torspy.egg-info/
--rw-rw-rw-   0        0        0     5549 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 10:16:10.000000 torspy-1.0.1/torspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:14:29.001631 torspy-1.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-17 15:10:21.000000 torspy-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7052 2024-05-17 15:14:29.001631 torspy-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6066 2024-05-17 15:10:21.000000 torspy-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:14:29.001631 torspy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2024-05-17 15:14:12.000000 torspy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:14:28.954802 torspy-1.0.2/torspy/
+-rw-rw-rw-   0        0        0       78 2024-05-17 15:10:20.000000 torspy-1.0.2/torspy/__init__.py
+-rw-rw-rw-   0        0        0     1906 2024-05-17 15:10:21.000000 torspy-1.0.2/torspy/cli.py
+-rw-rw-rw-   0        0        0     8805 2024-05-17 15:10:21.000000 torspy-1.0.2/torspy/scraper.py
+-rw-rw-rw-   0        0        0      102 2024-05-17 15:10:21.000000 torspy-1.0.2/torspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:14:29.001631 torspy-1.0.2/torspy.egg-info/
+-rw-rw-rw-   0        0        0     7052 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 15:14:28.000000 torspy-1.0.2/torspy.egg-info/top_level.txt
```

### Comparing `torspy-1.0.1/LICENSE` & `torspy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torspy-1.0.1/PKG-INFO` & `torspy-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,152 @@
-Metadata-Version: 2.1
-Name: torspy
-Version: 1.0.1
-Summary: Tor onion site scraping tool
-Home-page: https://github.com/mr-fidal/torspy
-Author: Fidal
-Author-email: mrfidal@proton.me
-Keywords: mrfidal,tor,DarkWeb,onion,torspy,scraping,dark web,web scraping,hidden services,privacy,security,beautifulsoup4,requests,python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# torspy
-
-torspy is a Python package designed for scraping .onion sites using the Tor network. It offers a straightforward interface for retrieving HTML content from .onion URLs, searching for specific text within that content, and saving the results to a file. Additionally, torspy is capable of detecting hidden directories.
-
-## Installation
-
-You can install torspy via pip:
-
-```sh
-pip install torspy
-```
-## Usage
-### Command-Line Interface
-torspy allows you to interact with .onion sites from the command line:
-
-- To display the content of a .onion site:
-```sh
-torspy http://example.onion
-```
-- To save the displayed content to a file:
-```sh
-torspy http://example.onion -s file.html
-```
-- The `-s` flag indicates saving, and you can specify any file name.
-
-- To search for specific text within the content and save the results to a file:
-```sh
-torspy http://example.onion --find "search query" -s search_results.html
-```
-- The `--find` flag followed by the search query indicates searching for specific text.
-
-- The `-s` flag followed by the file name indicates saving the search results.
-
-- To save the content to a specified directory:
-```sh
-torspy http://example.onion -s file.html -d /path/to/directory
-```
-- The `-d` flag followed by the directory path indicates where to save the file.
-
-- To check for directories listed in a file:
-```sh
-torspy http://example.onion --dir directories.txt
-```
-- The `--dir` flag followed by the file name checks for directories listed in the specified file.
-- Move it all to another file
-```sh
-torspy http://example.onion --dir directories.txt -s output.txt
-```
-- For more information on available options, you can use the `--help` flag:
-```sh
-torspy --help
-```
-### Additional Examples
-- Display the content of a .onion site and search for "important information", saving the results to a file named `results.html` in the specified directory:
-```sh
-torspy http://example.onion --find "important information" -s results.html -d /path/to/directory
-```
-- Save the entire HTML content of a .onion site to a file named `full_content.html` in the current directory:
-```sh
-torspy http://example.onion -s full_content.html
-```
-- Display the content of a .onion site and save it to a file named `output.txt` in the current directory:
-```sh
-torspy http://example.onion -s output.txt
-```
-### Using torspy in a Bash Script
-- You can incorporate torspy into your Bash scripts for automated tasks. Here's an example script that fetches content from a list of .onion URLs and saves it to individual files:
-```sh
-#!/bin/bash
-
-# List of .onion URLs
-urls=("http://example1.onion" "http://example2.onion" "http://example3.onion")
-
-# Loop through each URL
-for url in "${urls[@]}"; do
-    # Fetch content and save to a file
-    torspy "$url" -s "${url##*/}.html"
-done
-```
-### Integrating torspy with Other Languages
-### Ruby
-- You can call the torspy command-line tool from Ruby using the system method:
-```ruby
-system("torspy http://example.onion -s output.html")
-```
-### Python
-- You can use the subprocess module to call torspy from a Python script:
-```sh
-import subprocess
-
-subprocess.run(["torspy", "http://example.onion", "-s", "output.html"])
-```
-### PHP
-- You can use the shell_exec function to call torspy from PHP:
-```php
-<?php
-shell_exec("torspy http://example.onion -s output.html");
-?>
-```
-### Node.js
-- You can use the `child_process` module to call torspy from Node.js:
-```js
-const { exec } = require('child_process');
-
-exec('torspy http://example.onion -s output.html', (error, stdout, stderr) => {
-    if (error) {
-        console.error(`Error: ${error.message}`);
-        return;
-    }
-    if (stderr) {
-        console.error(`Stderr: ${stderr}`);
-        return;
-    }
-    console.log(`Output: ${stdout}`);
-});
-```
-### How torspy Works
-torspy utilizes the following process to interact with .onion sites:
-
-<li><b>Checking Site Existence:</b> It verifies if the .onion site exists and is reachable through the Tor network.</li>
-
-<li><b></b>Fetching HTML Content: </b>It retrieves the HTML content of the .onion site using Tor for anonymity.</li>
-
-<li><b></b>Scraping and Searching:</b> If specified, torspy searches for specific text within the content and extracts matching results.</li>
-
-<li><b>Saving Results: </b>Optionally, torspy allows you to save the retrieved content, either the entire HTML or the search results, to a file.</li>
-
-### Contributing to torspy
-If you're interested in contributing to torspy, you can:
-
-- Report issues encountered while using torspy.
-- Suggest new features or enhancements.
-- Submit pull requests with improvements or fixes.
-
-### Disclaimer
-```
-This tool is intended for ethical use only. The author is not responsible for any misuse or damage caused by this tool. Users are responsible for ensuring their activities comply with all relevant laws and regulations.
-```
+# torspy
+
+<b>torspy</b> is a robust Python package fortified with powerful algorithms, designed for seamless exploration of .onion sites via the Tor network. Its arsenal includes adept scraping of HTML from .onion URLs, precise text localization within the acquired content, and proficient storage of findings. Moreover, torspy boasts formidable subdomain scanning capabilities, enabling thorough reconnaissance across diverse subdomains. Additionally, it excels at detecting hidden directories, further enhancing its efficacy in navigating and extracting valuable information from the depths of the dark web.
+
+## Installation
+
+You can install torspy via pip:
+
+```sh
+pip install torspy
+```
+## Usage
+### Command-Line Interface
+torspy allows you to interact with .onion sites from the command line:
+
+- To display the content of a .onion site:
+```sh
+torspy http://example.onion
+```
+- To save the displayed content to a file:
+```sh
+torspy http://example.onion -s file.html
+```
+- The `-s` flag indicates saving, and you can specify any file name.
+
+- To search for specific text within the content and save the results to a file:
+```sh
+torspy http://example.onion --find "search query" -s search_results.html
+```
+- The `--find` flag followed by the search query indicates searching for specific text.
+
+- The `-s` flag followed by the file name indicates saving the search results.
+
+- To save the content to a specified directory:
+```sh
+torspy http://example.onion -s file.html -d /path/to/directory
+```
+- The `-d` flag followed by the directory path indicates where to save the file.
+#### Message 
+- important <b>Remember that when trying to find subdomains, as well as trying to find directories, the success rate is only 20%.</b>
+- Finding directories and subdomains for onion sites is more challenging than for regular websites because onion sites are part of the dark web, which is intentionally designed to be less accessible and more private.
+#### Subdomain and Directories
+- To check for directories listed in a file:
+```sh
+torspy http://example.onion --dir directories.txt
+```
+- The `--dir` flag followed by the file name checks for directories listed in the specified file.
+- Move it all to another file
+```sh
+torspy http://example.onion --dir directories-list.txt -s output.txt
+```
+- This command performs directories scanning on the .onion site using the list of directories provided in the `directories-list.txt` file.
+- For subdomain scanning:
+```sh
+torspy http://example.onion --sub subdomain-list.txt
+```
+The `--sub` flag followed by the file name checks for subdomains listed in the specified file.
+
+```sh
+torspy http://example.onion --sub subdomain-list.txt -s output.txt
+```
+- This command performs subdomain scanning on the .onion site using the list of subdomains provided in the `subdomain-list.txt` file.
+- For more information on available options, you can use the `--help` flag:
+```sh
+torspy --help
+```
+### Additional Examples
+- Display the content of a .onion site and search for "important information", saving the results to a file named `results.html` in the specified directory:
+```sh
+torspy http://example.onion --find "important information" -s results.html -d /path/to/directory
+```
+- Save the entire HTML content of a .onion site to a file named `full_content.html` in the current directory:
+```sh
+torspy http://example.onion -s full_content.html
+```
+- Display the content of a .onion site and save it to a file named `output.txt` in the current directory:
+```sh
+torspy http://example.onion -s output.txt
+```
+### Using torspy in a Bash Script
+- You can incorporate torspy into your Bash scripts for automated tasks. Here's an example script that fetches content from a list of .onion URLs and saves it to individual files:
+```sh
+#!/bin/bash
+
+# List of .onion URLs
+urls=("http://example1.onion" "http://example2.onion" "http://example3.onion")
+
+# Loop through each URL
+for url in "${urls[@]}"; do
+    # Fetch content and save to a file
+    torspy "$url" -s "${url##*/}.html"
+done
+```
+### Integrating torspy with Other Languages
+### Ruby
+- You can call the torspy command-line tool from Ruby using the system method:
+```ruby
+system("torspy http://example.onion -s output.html")
+```
+### Python
+- You can use the subprocess module to call torspy from a Python script:
+```sh
+import subprocess
+
+subprocess.run(["torspy", "http://example.onion", "-s", "output.html"])
+```
+### PHP
+- You can use the shell_exec function to call torspy from PHP:
+```php
+<?php
+shell_exec("torspy http://example.onion -s output.html");
+?>
+```
+### Node.js
+- You can use the `child_process` module to call torspy from Node.js:
+```js
+const { exec } = require('child_process');
+
+exec('torspy http://example.onion -s output.html', (error, stdout, stderr) => {
+    if (error) {
+        console.error(`Error: ${error.message}`);
+        return;
+    }
+    if (stderr) {
+        console.error(`Stderr: ${stderr}`);
+        return;
+    }
+    console.log(`Output: ${stdout}`);
+});
+```
+### How torspy Works
+torspy utilizes the following process to interact with .onion sites:
+
+<li><b>Checking Site Existence:</b> It verifies if the .onion site exists and is reachable through the Tor network.</li>
+
+<li><b></b>Fetching HTML Content: </b>It retrieves the HTML content of the .onion site using Tor for anonymity.</li>
+
+<li><b></b>Scraping and Searching:</b> If specified, torspy searches for specific text within the content and extracts matching results.</li>
+
+<li><b>Saving Results: </b>Optionally, torspy allows you to save the retrieved content, either the entire HTML or the search results, to a file.</li>
+
+### Contributing to torspy
+If you're interested in contributing to torspy, you can:
+
+- Report issues encountered while using torspy.
+- Suggest new features or enhancements.
+- Submit pull requests with improvements or fixes.
+
+### Disclaimer
+```
+This tool is intended for ethical use only. The author is not responsible for any misuse or damage caused by this tool. Users are responsible for ensuring their activities comply with all relevant laws and regulations.
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torspy-1.0.1/torspy.egg-info/PKG-INFO` & `torspy-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 1.0.1
-Summary: Tor onion site scraping tool
+Version: 1.0.2
+Summary: torspy is a Python package for scraping .onion sites via the Tor network. It retrieves HTML content from .onion URLs, searches for specific text, and saves results to a file. It also detects hidden directories, making it a valuable tool for navigating and extracting information from the dark web.
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Keywords: mrfidal,tor,DarkWeb,onion,torspy,scraping,dark web,web scraping,hidden services,privacy,security,beautifulsoup4,requests,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # torspy
 
-torspy is a Python package designed for scraping .onion sites using the Tor network. It offers a straightforward interface for retrieving HTML content from .onion URLs, searching for specific text within that content, and saving the results to a file. Additionally, torspy is capable of detecting hidden directories.
+<b>torspy</b> is a robust Python package fortified with powerful algorithms, designed for seamless exploration of .onion sites via the Tor network. Its arsenal includes adept scraping of HTML from .onion URLs, precise text localization within the acquired content, and proficient storage of findings. Moreover, torspy boasts formidable subdomain scanning capabilities, enabling thorough reconnaissance across diverse subdomains. Additionally, it excels at detecting hidden directories, further enhancing its efficacy in navigating and extracting valuable information from the depths of the dark web.
 
 ## Installation
 
 You can install torspy via pip:
 
 ```sh
 pip install torspy
@@ -47,24 +47,38 @@
 - The `-s` flag followed by the file name indicates saving the search results.
 
 - To save the content to a specified directory:
 ```sh
 torspy http://example.onion -s file.html -d /path/to/directory
 ```
 - The `-d` flag followed by the directory path indicates where to save the file.
-
+#### Message 
+- important <b>Remember that when trying to find subdomains, as well as trying to find directories, the success rate is only 20%.</b>
+- Finding directories and subdomains for onion sites is more challenging than for regular websites because onion sites are part of the dark web, which is intentionally designed to be less accessible and more private.
+#### Subdomain and Directories
 - To check for directories listed in a file:
 ```sh
 torspy http://example.onion --dir directories.txt
 ```
 - The `--dir` flag followed by the file name checks for directories listed in the specified file.
 - Move it all to another file
 ```sh
-torspy http://example.onion --dir directories.txt -s output.txt
+torspy http://example.onion --dir directories-list.txt -s output.txt
+```
+- This command performs directories scanning on the .onion site using the list of directories provided in the `directories-list.txt` file.
+- For subdomain scanning:
+```sh
+torspy http://example.onion --sub subdomain-list.txt
+```
+The `--sub` flag followed by the file name checks for subdomains listed in the specified file.
+
+```sh
+torspy http://example.onion --sub subdomain-list.txt -s output.txt
 ```
+- This command performs subdomain scanning on the .onion site using the list of subdomains provided in the `subdomain-list.txt` file.
 - For more information on available options, you can use the `--help` flag:
 ```sh
 torspy --help
 ```
 ### Additional Examples
 - Display the content of a .onion site and search for "important information", saving the results to a file named `results.html` in the specified directory:
 ```sh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

