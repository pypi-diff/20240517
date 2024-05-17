# Comparing `tmp/pynimbar-1.0.1.tar.gz` & `tmp/pynimbar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynimbar-1.0.1.tar", last modified: Wed Mar  1 22:28:35 2023, max compression
+gzip compressed data, was "pynimbar-1.1.0.tar", last modified: Fri May 17 01:13:33 2024, max compression
```

## Comparing `pynimbar-1.0.1.tar` & `pynimbar-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 22:28:35.636126 pynimbar-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-01 21:53:22.000000 pynimbar-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2058 2023-03-01 22:28:35.636126 pynimbar-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1652 2023-03-01 22:23:20.000000 pynimbar-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 22:28:35.624127 pynimbar-1.0.1/pynimbar/
-drwxrwxrwx   0        0        0        0 2023-03-01 22:28:35.634127 pynimbar-1.0.1/pynimbar/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 22:28:35.634127 pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/
--rw-rw-rw-   0        0        0     2058 2023-03-01 22:28:35.000000 pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-03-01 22:28:35.000000 pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 22:28:35.000000 pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 22:28:35.000000 pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2135 2023-03-01 22:24:25.000000 pynimbar-1.0.1/pynimbar/src/pynimbar.py
--rw-rw-rw-   0        0        0       42 2023-03-01 22:28:35.636126 pynimbar-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-03-01 22:28:17.000000 pynimbar-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:13:33.723431 pynimbar-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-03-01 21:53:22.000000 pynimbar-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2329 2024-05-17 01:13:33.722431 pynimbar-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1923 2024-05-17 00:41:56.000000 pynimbar-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 01:13:33.710431 pynimbar-1.1.0/pynimbar/
+-rw-rw-rw-   0        0        0        0 2023-03-09 22:18:19.000000 pynimbar-1.1.0/pynimbar/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:13:33.720431 pynimbar-1.1.0/pynimbar/src/
+-rw-rw-rw-   0        0        0       39 2023-03-09 22:18:42.000000 pynimbar-1.1.0/pynimbar/src/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-05-17 01:12:13.000000 pynimbar-1.1.0/pynimbar/src/pynimbar.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:13:33.721430 pynimbar-1.1.0/pynimbar.egg-info/
+-rw-rw-rw-   0        0        0     2329 2024-05-17 01:13:33.000000 pynimbar-1.1.0/pynimbar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-17 01:13:33.000000 pynimbar-1.1.0/pynimbar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 01:13:33.000000 pynimbar-1.1.0/pynimbar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 01:13:33.000000 pynimbar-1.1.0/pynimbar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 01:13:33.724431 pynimbar-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      760 2024-05-17 01:11:23.000000 pynimbar-1.1.0/setup.py
```

### Comparing `pynimbar-1.0.1/LICENSE` & `pynimbar-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynimbar-1.0.1/PKG-INFO` & `pynimbar-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynimbar
-Version: 1.0.1
+Version: 1.1.0
 Summary: Make your Python scripts more user friendly with loading animations
 Author: Gabriel Mitelman Tkacz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -32,13 +32,18 @@
 ```
 
 ## Customization
 You can customize the appearance and behavior of the loading animation using the following parameters:
 - `text` (str): The text to display during the animation.
 - `success_msg` (str, optional): The text to display when the animation is done. Defaults to `'ok'`.
 - `animation_frequency` (float, optional): The frequency of the animation. Defaults to `0.1`.
-- `break_on_error` (bool, optional): Whether to break on error. Defaults to `False`.
+- `break_on_error` (bool, optional): Whether to break on error. Defaults to `True`.
 - `verbose_errors` (bool, optional): Whether to print the error traceback. Defaults to `False`.
 - `frames` (str, optional): The frames of the animation. Defaults to `'|/-\\'`.
+- `time_it` (bool, optional): Whether to time the execution of the code block. Defaults to False.
+- `time_it_live` (bool, optional): Whether to print the live execution time of the code block. Defaults to False.
 
 ## Contributing
 If you have any suggestions or improvements for pynimbar, feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/gtkacz/pynimbar). We appreciate any feedback or contributions!
+
+## Example
+![Example functionality](/img/example.gif)
```

### Comparing `pynimbar-1.0.1/README.md` & `pynimbar-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,13 +20,18 @@
 ```
 
 ## Customization
 You can customize the appearance and behavior of the loading animation using the following parameters:
 - `text` (str): The text to display during the animation.
 - `success_msg` (str, optional): The text to display when the animation is done. Defaults to `'ok'`.
 - `animation_frequency` (float, optional): The frequency of the animation. Defaults to `0.1`.
-- `break_on_error` (bool, optional): Whether to break on error. Defaults to `False`.
+- `break_on_error` (bool, optional): Whether to break on error. Defaults to `True`.
 - `verbose_errors` (bool, optional): Whether to print the error traceback. Defaults to `False`.
 - `frames` (str, optional): The frames of the animation. Defaults to `'|/-\\'`.
+- `time_it` (bool, optional): Whether to time the execution of the code block. Defaults to False.
+- `time_it_live` (bool, optional): Whether to print the live execution time of the code block. Defaults to False.
 
 ## Contributing
-If you have any suggestions or improvements for pynimbar, feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/gtkacz/pynimbar). We appreciate any feedback or contributions!
+If you have any suggestions or improvements for pynimbar, feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/gtkacz/pynimbar). We appreciate any feedback or contributions!
+
+## Example
+![Example functionality](/img/example.gif)
```

### Comparing `pynimbar-1.0.1/pynimbar/src/pynimbar.egg-info/PKG-INFO` & `pynimbar-1.1.0/pynimbar.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynimbar
-Version: 1.0.1
+Version: 1.1.0
 Summary: Make your Python scripts more user friendly with loading animations
 Author: Gabriel Mitelman Tkacz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -32,13 +32,18 @@
 ```
 
 ## Customization
 You can customize the appearance and behavior of the loading animation using the following parameters:
 - `text` (str): The text to display during the animation.
 - `success_msg` (str, optional): The text to display when the animation is done. Defaults to `'ok'`.
 - `animation_frequency` (float, optional): The frequency of the animation. Defaults to `0.1`.
-- `break_on_error` (bool, optional): Whether to break on error. Defaults to `False`.
+- `break_on_error` (bool, optional): Whether to break on error. Defaults to `True`.
 - `verbose_errors` (bool, optional): Whether to print the error traceback. Defaults to `False`.
 - `frames` (str, optional): The frames of the animation. Defaults to `'|/-\\'`.
+- `time_it` (bool, optional): Whether to time the execution of the code block. Defaults to False.
+- `time_it_live` (bool, optional): Whether to print the live execution time of the code block. Defaults to False.
 
 ## Contributing
 If you have any suggestions or improvements for pynimbar, feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/gtkacz/pynimbar). We appreciate any feedback or contributions!
+
+## Example
+![Example functionality](/img/example.gif)
```

### Comparing `pynimbar-1.0.1/setup.py` & `pynimbar-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
+from pathlib import Path
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pynimbar',
-    version='1.0.1',
+    version='1.1.0',
     author='Gabriel Mitelman Tkacz',
     description='Make your Python scripts more user friendly with loading animations',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     py_modules=['pynimbar'],
-    package_dir={'': 'pynimbar/src'},
+    # package_dir={'': Path('pynimbar/src').__str__()},
     install_requires=[]
 )
```

