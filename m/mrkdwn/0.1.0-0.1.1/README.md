# Comparing `tmp/mrkdwn-0.1.0.tar.gz` & `tmp/mrkdwn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrkdwn-0.1.0.tar", last modified: Fri May 17 14:28:37 2024, max compression
+gzip compressed data, was "mrkdwn-0.1.1.tar", last modified: Fri May 17 14:37:54 2024, max compression
```

## Comparing `mrkdwn-0.1.0.tar` & `mrkdwn-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:28:37.699353 mrkdwn-0.1.0/
--rw-r--r--   0 joel       (501) staff       (20)     1036 2024-05-17 14:24:34.000000 mrkdwn-0.1.0/LICENSE
--rw-r--r--   0 joel       (501) staff       (20)       58 2024-05-17 14:20:21.000000 mrkdwn-0.1.0/MANIFEST.in
--rw-r--r--   0 joel       (501) staff       (20)      445 2024-05-17 14:28:37.699169 mrkdwn-0.1.0/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)        0 2024-05-17 14:03:48.000000 mrkdwn-0.1.0/README.md
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:28:37.697612 mrkdwn-0.1.0/mrkdwn/
--rw-r--r--   0 joel       (501) staff       (20)        0 2024-05-17 14:03:12.000000 mrkdwn-0.1.0/mrkdwn/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     3011 2024-05-17 14:23:06.000000 mrkdwn-0.1.0/mrkdwn/main.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:28:37.698965 mrkdwn-0.1.0/mrkdwn.egg-info/
--rw-r--r--   0 joel       (501) staff       (20)      445 2024-05-17 14:28:37.000000 mrkdwn-0.1.0/mrkdwn.egg-info/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)      268 2024-05-17 14:28:37.000000 mrkdwn-0.1.0/mrkdwn.egg-info/SOURCES.txt
--rw-r--r--   0 joel       (501) staff       (20)        1 2024-05-17 14:28:37.000000 mrkdwn-0.1.0/mrkdwn.egg-info/dependency_links.txt
--rw-r--r--   0 joel       (501) staff       (20)       46 2024-05-17 14:28:37.000000 mrkdwn-0.1.0/mrkdwn.egg-info/entry_points.txt
--rw-r--r--   0 joel       (501) staff       (20)        7 2024-05-17 14:28:37.000000 mrkdwn-0.1.0/mrkdwn.egg-info/top_level.txt
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:28:37.698590 mrkdwn-0.1.0/scripts/
--rw-r--r--   0 joel       (501) staff       (20)     1310 2024-05-17 14:18:27.000000 mrkdwn-0.1.0/scripts/installer.bat
--rw-r--r--   0 joel       (501) staff       (20)      610 2024-05-17 14:16:30.000000 mrkdwn-0.1.0/scripts/installer.sh
--rw-r--r--   0 joel       (501) staff       (20)       38 2024-05-17 14:28:37.699392 mrkdwn-0.1.0/setup.cfg
--rw-r--r--   0 joel       (501) staff       (20)     1442 2024-05-17 14:28:26.000000 mrkdwn-0.1.0/setup.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:37:54.181844 mrkdwn-0.1.1/
+-rw-r--r--   0 joel       (501) staff       (20)     1036 2024-05-17 14:24:34.000000 mrkdwn-0.1.1/LICENSE
+-rw-r--r--   0 joel       (501) staff       (20)       58 2024-05-17 14:20:21.000000 mrkdwn-0.1.1/MANIFEST.in
+-rw-r--r--   0 joel       (501) staff       (20)      445 2024-05-17 14:37:54.181670 mrkdwn-0.1.1/PKG-INFO
+-rw-r--r--   0 joel       (501) staff       (20)        0 2024-05-17 14:03:48.000000 mrkdwn-0.1.1/README.md
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:37:54.180726 mrkdwn-0.1.1/mrkdwn/
+-rw-r--r--   0 joel       (501) staff       (20)        0 2024-05-17 14:03:12.000000 mrkdwn-0.1.1/mrkdwn/__init__.py
+-rw-r--r--   0 joel       (501) staff       (20)     3475 2024-05-17 14:36:37.000000 mrkdwn-0.1.1/mrkdwn/main.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:37:54.181530 mrkdwn-0.1.1/mrkdwn.egg-info/
+-rw-r--r--   0 joel       (501) staff       (20)      445 2024-05-17 14:37:54.000000 mrkdwn-0.1.1/mrkdwn.egg-info/PKG-INFO
+-rw-r--r--   0 joel       (501) staff       (20)      268 2024-05-17 14:37:54.000000 mrkdwn-0.1.1/mrkdwn.egg-info/SOURCES.txt
+-rw-r--r--   0 joel       (501) staff       (20)        1 2024-05-17 14:37:54.000000 mrkdwn-0.1.1/mrkdwn.egg-info/dependency_links.txt
+-rw-r--r--   0 joel       (501) staff       (20)       46 2024-05-17 14:37:54.000000 mrkdwn-0.1.1/mrkdwn.egg-info/entry_points.txt
+-rw-r--r--   0 joel       (501) staff       (20)        7 2024-05-17 14:37:54.000000 mrkdwn-0.1.1/mrkdwn.egg-info/top_level.txt
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2024-05-17 14:37:54.181398 mrkdwn-0.1.1/scripts/
+-rw-r--r--   0 joel       (501) staff       (20)     1310 2024-05-17 14:18:27.000000 mrkdwn-0.1.1/scripts/installer.bat
+-rw-r--r--   0 joel       (501) staff       (20)      610 2024-05-17 14:16:30.000000 mrkdwn-0.1.1/scripts/installer.sh
+-rw-r--r--   0 joel       (501) staff       (20)       38 2024-05-17 14:37:54.181881 mrkdwn-0.1.1/setup.cfg
+-rw-r--r--   0 joel       (501) staff       (20)     1442 2024-05-17 14:37:21.000000 mrkdwn-0.1.1/setup.py
```

### Comparing `mrkdwn-0.1.0/LICENSE` & `mrkdwn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrkdwn-0.1.0/mrkdwn/main.py` & `mrkdwn-0.1.1/mrkdwn/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,24 @@
                 "header": header,
                 "files": relevant_files
             }
             print(f"Adding {len(relevant_files)} files under: {root}")
 
     return file_dict
 
+def read_file_with_fallback(file_path):
+    encodings = ['utf-8', 'latin-1', 'iso-8859-1']
+    for encoding in encodings:
+        try:
+            with open(file_path, 'r', encoding=encoding) as file:
+                return file.read()
+        except UnicodeDecodeError:
+            continue
+    raise UnicodeDecodeError(f"Unable to decode {file_path} with any known encodings")
+
 def write_markdown(file_dict, output_file, base_path):
     base_dir_name = os.path.basename(base_path.rstrip('/'))
     with open(output_file, 'w', encoding='utf-8') as md_file:
         print(f"Writing to {output_file}")
         for path, data in sorted(file_dict.items(), key=lambda x: x[0]):
             relative_path = os.path.relpath(path, base_path)
             if relative_path == '.':
@@ -44,17 +54,19 @@
             md_file.write(f"{data['header']} {relative_path}\n")
             for filename in data['files']:
                 file_ext = Path(filename).suffix.lstrip('.')
                 if not file_ext:
                     file_ext = 'text'
                 md_file.write(f"{data['header']}# {filename}\n")
                 file_path = os.path.join(path, filename)
-                with open(file_path, 'r', encoding='utf-8') as file:
-                    content = file.read()
+                try:
+                    content = read_file_with_fallback(file_path)
                     md_file.write(f"```{file_ext}\n{content}\n```\n")
+                except UnicodeDecodeError as e:
+                    print(f"Error reading {file_path}: {e}")
 
 def main():
     parser = argparse.ArgumentParser(description="Generate a Markdown file from directory contents.")
     parser.add_argument("path", help="Path to the directory")
     parser.add_argument("-r", "--recurse", action='store_true', help="Recurse into subdirectories")
     parser.add_argument("-n", "--name", help="Filter files by name, separated by ' | '", type=str)
     parser.add_argument("-t", "--type", help="Filter files by file type")
```

### Comparing `mrkdwn-0.1.0/scripts/installer.bat` & `mrkdwn-0.1.1/scripts/installer.bat`

 * *Files identical despite different names*

### Comparing `mrkdwn-0.1.0/scripts/installer.sh` & `mrkdwn-0.1.1/scripts/installer.sh`

 * *Files identical despite different names*

### Comparing `mrkdwn-0.1.0/setup.py` & `mrkdwn-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             subprocess.run(['cmd', '/c', script])
         else:
             script = os.path.join(os.path.dirname(__file__), 'scripts', 'installer.sh')
             subprocess.run(['sh', script])
 
 setup(
     name='mrkdwn',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'markdown=mrkdwn.main:main',
         ],
     },
     install_requires=[],
```

