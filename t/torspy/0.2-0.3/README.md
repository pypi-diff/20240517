# Comparing `tmp/torspy-0.2.tar.gz` & `tmp/torspy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torspy-0.2.tar", last modified: Thu May 16 15:44:22 2024, max compression
+gzip compressed data, was "torspy-0.3.tar", last modified: Thu May 16 18:46:52 2024, max compression
```

## Comparing `torspy-0.2.tar` & `torspy-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.093960 torspy-0.2/
--rw-rw-rw-   0        0        0     1065 2024-05-16 15:23:00.000000 torspy-0.2/LICENSE
--rw-rw-rw-   0        0        0     4266 2024-05-16 15:44:22.093960 torspy-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2024-05-16 15:23:00.000000 torspy-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 15:44:22.093960 torspy-0.2/setup.cfg
--rw-rw-rw-   0        0        0      827 2024-05-16 15:43:42.000000 torspy-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.062718 torspy-0.2/torspy/
--rw-rw-rw-   0        0        0       78 2024-05-16 15:22:59.000000 torspy-0.2/torspy/__init__.py
--rw-rw-rw-   0        0        0      914 2024-05-16 15:37:35.000000 torspy-0.2/torspy/cli.py
--rw-rw-rw-   0        0        0     2630 2024-05-16 15:22:59.000000 torspy-0.2/torspy/scraper.py
--rw-rw-rw-   0        0        0      102 2024-05-16 15:23:00.000000 torspy-0.2/torspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.093960 torspy-0.2/torspy.egg-info/
--rw-rw-rw-   0        0        0     4266 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 18:46:52.765569 torspy-0.3/
+-rw-rw-rw-   0        0        0     1065 2024-05-16 18:45:32.000000 torspy-0.3/LICENSE
+-rw-rw-rw-   0        0        0     5724 2024-05-16 18:46:52.765569 torspy-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5151 2024-05-16 18:45:32.000000 torspy-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:46:52.765569 torspy-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      827 2024-05-16 18:45:32.000000 torspy-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:46:52.703045 torspy-0.3/torspy/
+-rw-rw-rw-   0        0        0       78 2024-05-16 18:45:31.000000 torspy-0.3/torspy/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-05-16 18:45:31.000000 torspy-0.3/torspy/cli.py
+-rw-rw-rw-   0        0        0     2926 2024-05-16 18:45:32.000000 torspy-0.3/torspy/scraper.py
+-rw-rw-rw-   0        0        0      102 2024-05-16 18:45:32.000000 torspy-0.3/torspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:46:52.765569 torspy-0.3/torspy.egg-info/
+-rw-rw-rw-   0        0        0     5724 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 18:46:52.000000 torspy-0.3/torspy.egg-info/top_level.txt
```

### Comparing `torspy-0.2/LICENSE` & `torspy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torspy-0.2/PKG-INFO` & `torspy-0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,149 @@
-Metadata-Version: 2.1
-Name: torspy
-Version: 0.2
-Summary: Tor onion site scraping tool
-Home-page: https://github.com/mr-fidal/torspy
-Author: Fidal
-Author-email: mrfidal@proton.me
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# torspy
-
-torspy is a Python package for scraping .onion sites using Tor. It provides a simple interface for fetching HTML content from .onion URLs, searching for specific text within the content, and saving the results to a file.
-
-## Installation
-
-You can install torspy via pip:
-
-```
-pip install torspy
-```
-
-## Usage
-
-### Command-Line Interface
-
-torspy allows you to interact with .onion sites from the command line:
-
-- To display the content of a .onion site:
-```
-torspy http://example.onion
-```
-
-- To save the displayed content to a file:
-```
-torspy http://example.onion -s file.html
-```
-  - The `-s` flag indicates saving, and you can specify any file name.
-
-- To search for specific text within the content and save the results to a file:
-```
-torspy http://example.onion --find "search query" -s search_results.html
-```
-  - The `--find` flag followed by the search query indicates searching for specific text.
-  - The `-s` flag followed by the file name indicates saving the search results.
-
-- To save the content to a specified directory:
-```
-torspy http://example.onion -s file.html -d /path/to/directory
-```
-  - The `-d` flag followed by the directory path indicates where to save the file.
-
-- For more information on available options, you can use the `--help` flag:
-```
-torspy --help
-```
-
-### Additional Examples
-
-- Display the content of a .onion site and search for "important information", saving the results to a file named `results.html` in the specified directory:
-```
-torspy http://example.onion --find "important information" -s results.html -d /path/to/directory
-```
-
-- Save the entire HTML content of a .onion site to a file named `full_content.html` in the current directory:
-```
-torspy http://example.onion -s full_content.html
-```
-
-- Display the content of a .onion site and save it to a file named `output.txt` in the current directory:
-```
-torspy http://example.onion -s output.txt
-```
-
-### Using torspy in a Bash Script
-
-You can incorporate torspy into your Bash scripts for automated tasks. Here's an example script that fetches content from a list of .onion URLs and saves it to individual files:
-
-```bash
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
-
-### Contributing
-
-If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on GitHub.
-
-## How torspy Works
-
-torspy utilizes the following process to interact with .onion sites:
-
-1. **Checking Site Existence**: It verifies if the .onion site exists and is reachable through the Tor network.
-
-2. **Fetching HTML Content**: It retrieves the HTML content of the .onion site using Tor for anonymity.
-
-3. **Scraping and Searching**: If specified, torspy searches for specific text within the content and extracts matching results.
-
-4. **Saving Results**: Optionally, torspy allows you to save the retrieved content, either the entire HTML or the search results, to a file.
-
-## Code Overview
-
-torspy consists of the following components:
-
-- `check_onion_site(url)`: Checks if the .onion site exists and is reachable.
-
-- `scrape_onion_site(url, search_query, save_file, save_directory)`: Scrapes the .onion site, searches for specific text, and saves results if required.
-
-- `main()`: Handles command-line arguments and invokes the scraping functionality.
-
-## Contributing to torspy
-
-If you're interested in contributing to torspy, you can:
-
-- Report issues encountered while using torspy.
-- Suggest new features or enhancements.
-- Submit pull requests with improvements or fixes.
-- 
+# torspy
+
+torspy is a Python package for scraping .onion sites using Tor. It provides a simple interface for fetching HTML content from .onion URLs, searching for specific text within the content, and saving the results to a file.
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
+
+- To use a custom proxy for the requests:
+```sh
+torspy http://example.onion --proxy socks5h://127.0.0.1:9050
+```
+- The `--proxy` flag followed by the proxy URL specifies the proxy to use for the requests.
+
+- To use a custom User-Agent for the requests:
+```sh
+torspy http://example.onion --user-agent "CustomUserAgent/1.0"
+```
+- The `--user-agent` flag followed by the User-Agent string specifies the User-Agent to use for the requests.
+
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
+- Display the content of a .onion site using a custom proxy:
+```sh
+torspy http://example.onion --proxy socks5h://127.0.0.1:9050
+```
+- Display the content of a .onion site using a custom User-Agent:
+```sh
+torspy http://example.onion --user-agent "CustomUserAgent/1.0"
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

### Comparing `torspy-0.2/setup.py` & `torspy-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='torspy',
-    version='0.2',
+    version='0.3',
     author='Fidal',
     author_email='mrfidal@proton.me',
     description='Tor onion site scraping tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mr-fidal/torspy',
     packages=find_packages(),
```

### Comparing `torspy-0.2/torspy/cli.py` & `torspy-0.3/torspy/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # copyright ©️ 2024 author Fidal
 
 import argparse
 from .scraper import scrape_onion_site
 
 def main():
     epilog_text = '''
-Copyright (©️) 2024 author: Fidal
+Copyright (c) 2024 author: Fidal
 Issue: https://GitHub.com/mr-fidal/torspy
 '''
     parser = argparse.ArgumentParser(description='Scrape a .onion site.', epilog=epilog_text,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('url', type=str, help='The .onion site URL to scrape')
     parser.add_argument('--find', type=str, help='The text to search for within the site')
     parser.add_argument('-s', '--save', type=str, help='The file name to save the content')
     parser.add_argument('-d', '--directory', type=str, help='The directory to save the file')
+    parser.add_argument('--proxy', type=str, help='The proxy server to use')
+    parser.add_argument('--user-agent', type=str, help='The User-Agent string to use')
     args = parser.parse_args()
-    scrape_onion_site(args.url, args.find, args.save, args.directory)
+    scrape_onion_site(args.url, args.find, args.save, args.directory, args.proxy, args.user_agent)
 
 if __name__ == "__main__":
     main()
-   
+
```

### Comparing `torspy-0.2/torspy.egg-info/PKG-INFO` & `torspy-0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 0.2
+Version: 0.3
 Summary: Tor onion site scraping tool
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,114 +16,148 @@
 
 torspy is a Python package for scraping .onion sites using Tor. It provides a simple interface for fetching HTML content from .onion URLs, searching for specific text within the content, and saving the results to a file.
 
 ## Installation
 
 You can install torspy via pip:
 
-```
+```sh
 pip install torspy
 ```
-
 ## Usage
-
 ### Command-Line Interface
-
 torspy allows you to interact with .onion sites from the command line:
 
 - To display the content of a .onion site:
-```
+```sh
 torspy http://example.onion
 ```
-
 - To save the displayed content to a file:
-```
+```sh
 torspy http://example.onion -s file.html
 ```
-  - The `-s` flag indicates saving, and you can specify any file name.
+- The `-s` flag indicates saving, and you can specify any file name.
 
 - To search for specific text within the content and save the results to a file:
-```
+```sh
 torspy http://example.onion --find "search query" -s search_results.html
 ```
-  - The `--find` flag followed by the search query indicates searching for specific text.
-  - The `-s` flag followed by the file name indicates saving the search results.
+- The `--find` flag followed by the search query indicates searching for specific text.
+
+- The `-s` flag followed by the file name indicates saving the search results.
 
 - To save the content to a specified directory:
-```
+```sh
 torspy http://example.onion -s file.html -d /path/to/directory
 ```
-  - The `-d` flag followed by the directory path indicates where to save the file.
+- The `-d` flag followed by the directory path indicates where to save the file.
 
-- For more information on available options, you can use the `--help` flag:
+- To use a custom proxy for the requests:
+```sh
+torspy http://example.onion --proxy socks5h://127.0.0.1:9050
 ```
-torspy --help
+- The `--proxy` flag followed by the proxy URL specifies the proxy to use for the requests.
+
+- To use a custom User-Agent for the requests:
+```sh
+torspy http://example.onion --user-agent "CustomUserAgent/1.0"
 ```
+- The `--user-agent` flag followed by the User-Agent string specifies the User-Agent to use for the requests.
 
+- For more information on available options, you can use the `--help` flag:
+```sh
+torspy --help
+```
 ### Additional Examples
-
 - Display the content of a .onion site and search for "important information", saving the results to a file named `results.html` in the specified directory:
-```
+```sh
 torspy http://example.onion --find "important information" -s results.html -d /path/to/directory
 ```
-
 - Save the entire HTML content of a .onion site to a file named `full_content.html` in the current directory:
-```
+```sh
 torspy http://example.onion -s full_content.html
 ```
-
 - Display the content of a .onion site and save it to a file named `output.txt` in the current directory:
-```
+```sh
 torspy http://example.onion -s output.txt
 ```
-
+- Display the content of a .onion site using a custom proxy:
+```sh
+torspy http://example.onion --proxy socks5h://127.0.0.1:9050
+```
+- Display the content of a .onion site using a custom User-Agent:
+```sh
+torspy http://example.onion --user-agent "CustomUserAgent/1.0"
+```
 ### Using torspy in a Bash Script
-
-You can incorporate torspy into your Bash scripts for automated tasks. Here's an example script that fetches content from a list of .onion URLs and saves it to individual files:
-
-```bash
+- You can incorporate torspy into your Bash scripts for automated tasks. Here's an example script that fetches content from a list of .onion URLs and saves it to individual files:
+```sh
 #!/bin/bash
 
 # List of .onion URLs
 urls=("http://example1.onion" "http://example2.onion" "http://example3.onion")
 
 # Loop through each URL
 for url in "${urls[@]}"; do
     # Fetch content and save to a file
     torspy "$url" -s "${url##*/}.html"
 done
 ```
-
-### Contributing
-
-If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on GitHub.
-
-## How torspy Works
-
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
 torspy utilizes the following process to interact with .onion sites:
 
-1. **Checking Site Existence**: It verifies if the .onion site exists and is reachable through the Tor network.
-
-2. **Fetching HTML Content**: It retrieves the HTML content of the .onion site using Tor for anonymity.
-
-3. **Scraping and Searching**: If specified, torspy searches for specific text within the content and extracts matching results.
-
-4. **Saving Results**: Optionally, torspy allows you to save the retrieved content, either the entire HTML or the search results, to a file.
-
-## Code Overview
+<li><b>Checking Site Existence:</b> It verifies if the .onion site exists and is reachable through the Tor network.</li>
 
-torspy consists of the following components:
+<li><b></b>Fetching HTML Content: </b>It retrieves the HTML content of the .onion site using Tor for anonymity.</li>
 
-- `check_onion_site(url)`: Checks if the .onion site exists and is reachable.
+<li><b></b>Scraping and Searching:</b> If specified, torspy searches for specific text within the content and extracts matching results.</li>
 
-- `scrape_onion_site(url, search_query, save_file, save_directory)`: Scrapes the .onion site, searches for specific text, and saves results if required.
-
-- `main()`: Handles command-line arguments and invokes the scraping functionality.
-
-## Contributing to torspy
+<li><b>Saving Results: </b>Optionally, torspy allows you to save the retrieved content, either the entire HTML or the search results, to a file.</li>
 
+### Contributing to torspy
 If you're interested in contributing to torspy, you can:
 
 - Report issues encountered while using torspy.
 - Suggest new features or enhancements.
 - Submit pull requests with improvements or fixes.
-- 
+
+### Disclaimer
+```
+This tool is intended for ethical use only. The author is not responsible for any misuse or damage caused by this tool. Users are responsible for ensuring their activities comply with all relevant laws and regulations.
+```
```

