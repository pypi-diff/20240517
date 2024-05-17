# Comparing `tmp/custom-tree-1.6.tar.gz` & `tmp/custom-tree-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-tree-1.6.tar", last modified: Tue Feb 27 01:11:09 2024, max compression
+gzip compressed data, was "custom-tree-1.7.tar", last modified: Fri May 17 20:13:40 2024, max compression
```

## Comparing `custom-tree-1.6.tar` & `custom-tree-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 01:11:09.488961 custom-tree-1.6/
--rw-rw-rw-   0        0        0     1089 2024-02-26 16:38:40.000000 custom-tree-1.6/LICENSE
--rw-rw-rw-   0        0        0     4890 2024-02-27 01:11:09.386903 custom-tree-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4240 2024-02-27 01:08:57.000000 custom-tree-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 01:11:09.366559 custom-tree-1.6/custom_tree/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:35:04.000000 custom-tree-1.6/custom_tree/__init__.py
--rw-rw-rw-   0        0        0     2565 2024-02-27 01:10:06.000000 custom-tree-1.6/custom_tree/main.py
-drwxrwxrwx   0        0        0        0 2024-02-27 01:11:09.383299 custom-tree-1.6/custom_tree.egg-info/
--rw-rw-rw-   0        0        0     4890 2024-02-27 01:11:09.000000 custom-tree-1.6/custom_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-02-27 01:11:09.000000 custom-tree-1.6/custom_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 01:11:09.000000 custom-tree-1.6/custom_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-02-27 01:11:09.000000 custom-tree-1.6/custom_tree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-02-27 01:11:09.000000 custom-tree-1.6/custom_tree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-27 01:11:09.488961 custom-tree-1.6/setup.cfg
--rw-rw-rw-   0        0        0      924 2024-02-27 01:11:05.000000 custom-tree-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:13:40.525608 custom-tree-1.7/
+-rw-rw-rw-   0        0        0     1089 2024-02-26 16:38:40.000000 custom-tree-1.7/LICENSE
+-rw-rw-rw-   0        0        0     4890 2024-05-17 20:13:40.524611 custom-tree-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4240 2024-02-27 01:08:57.000000 custom-tree-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 20:13:40.511645 custom-tree-1.7/custom_tree/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:35:04.000000 custom-tree-1.7/custom_tree/__init__.py
+-rw-rw-rw-   0        0        0     3152 2024-05-17 20:03:21.000000 custom-tree-1.7/custom_tree/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:13:40.523613 custom-tree-1.7/custom_tree.egg-info/
+-rw-rw-rw-   0        0        0     4890 2024-05-17 20:13:40.000000 custom-tree-1.7/custom_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-17 20:13:40.000000 custom-tree-1.7/custom_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:13:40.000000 custom-tree-1.7/custom_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-17 20:13:40.000000 custom-tree-1.7/custom_tree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 20:13:40.000000 custom-tree-1.7/custom_tree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:13:40.526605 custom-tree-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-05-17 20:11:58.000000 custom-tree-1.7/setup.py
```

### Comparing `custom-tree-1.6/LICENSE` & `custom-tree-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-tree-1.6/PKG-INFO` & `custom-tree-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-tree
-Version: 1.6
+Version: 1.7
 Summary: Creating a custom directory tree is an efficient method for visually organizing your project's directory structure, complete with detailed information. It provides a clear model of your project layout for easy reference and management.
 Home-page: https://github.com/dragon-devs/custom-tree
 Author: dragon-devs
 Author-email: dragonfourtyseven@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `custom-tree-1.6/README.md` & `custom-tree-1.7/README.md`

 * *Files identical despite different names*

### Comparing `custom-tree-1.6/custom_tree/main.py` & `custom-tree-1.7/custom_tree/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 import argparse
+from collections import defaultdict
 
 
-def generate_tree_str(folder_path, indent='', include_hidden=False):
+def generate_tree_str(folder_path, indent='', include_hidden=False, ext_counts=None):
+   if ext_counts is None:
+      ext_counts = defaultdict(int)
+
    tree_str = ''
    num_dirs = 0
    num_files = 0
 
    try:
       items = os.listdir(folder_path)
    except PermissionError:
       print(f"Permission denied: {folder_path}")
-      return tree_str, num_dirs, num_files
+      return tree_str, num_dirs, num_files, ext_counts
 
    for i, item in enumerate(items):
       if not include_hidden and item.startswith('.'):
          continue
 
       if i == len(items) - 1:
          branch = '└── '
@@ -27,49 +31,61 @@
 
       if os.path.isdir(item_path):
          item_display = f"📂 {item}"
          num_dirs += 1
       else:
          item_display = f"📄 {item}"  # File icon
          num_files += 1
+         ext = os.path.splitext(item)[1]
+         if ext:
+            ext_counts[ext] += 1
+         else:
+            ext_counts['no_ext'] += 1
       tree_str += f"{indent}{branch}{item_display}\n"
 
       if os.path.isdir(item_path):
-         subtree, dirs, files = generate_tree_str(item_path, new_indent, include_hidden)
+         subtree, dirs, files, ext_counts = generate_tree_str(item_path, new_indent, include_hidden, ext_counts)
          tree_str += subtree
          num_dirs += dirs
          num_files += files
 
-   return tree_str, num_dirs, num_files
+   return tree_str, num_dirs, num_files, ext_counts
 
 
 def save_project_structure_to_file(file_path, include_hidden=False):
    current_directory = os.getcwd()
-   tree, num_dirs, num_files = generate_tree_str(current_directory, include_hidden=include_hidden)
+   tree, num_dirs, num_files, ext_counts = generate_tree_str(current_directory, include_hidden=include_hidden)
 
    with open(file_path, 'w', encoding='utf-8') as file:
       file.write(f"Project structure for directory: {current_directory}\n\n")
       file.write(tree)
       file.write(f"\n\nTotal directories 📂: {num_dirs}\n")
       file.write(f"Total files 📄: {num_files}\n")
+      file.write("File extensions count:\n")
+      for ext, count in ext_counts.items():
+         file.write(f"{ext} : {count}\n")
 
    print(f"Project structure saved to {file_path}")
 
+
 def main():
    parser = argparse.ArgumentParser(description='Display directory tree structure')
    parser.add_argument('--output', '-o', metavar='FILE', help='Output file path')
    parser.add_argument('--hidden', action='store_true', help='Include hidden directories')
    args = parser.parse_args()
 
    if args.output:
       save_project_structure_to_file(args.output, include_hidden=args.hidden)
    else:
       current_directory = os.getcwd()
-      tree, num_dirs, num_files = generate_tree_str(current_directory, include_hidden=args.hidden)
+      tree, num_dirs, num_files, ext_counts = generate_tree_str(current_directory, include_hidden=args.hidden)
       print(tree)
       print(f"Total directories 📂: {num_dirs}")
       print(f"Total files 📄: {num_files}")
-      print(f"\nIf you liked it give us a star & follow for more :) ... https://github.com/dragon-devs/custom-tree")
+      print("\nFile extensions count:")
+      for ext, count in ext_counts.items():
+         print(f"{ext} : {count}")
+      print(f"\nIf you liked it give us a star & follow for more :) ... https://github.com/dragon-devs")
 
 
 if __name__ == "__main__":
    main()
```

### Comparing `custom-tree-1.6/custom_tree.egg-info/PKG-INFO` & `custom-tree-1.7/custom_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-tree
-Version: 1.6
+Version: 1.7
 Summary: Creating a custom directory tree is an efficient method for visually organizing your project's directory structure, complete with detailed information. It provides a clear model of your project layout for easy reference and management.
 Home-page: https://github.com/dragon-devs/custom-tree
 Author: dragon-devs
 Author-email: dragonfourtyseven@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `custom-tree-1.6/setup.py` & `custom-tree-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='custom-tree',
-   version='1.6',
+   version='1.7',
    packages=find_packages(),
    description="Creating a custom directory tree is an efficient method for visually organizing your project's directory structure, complete with detailed information. It provides a clear model of your project layout for easy reference and management.",
    long_description=open('README.md', encoding='utf-8').read(),
    long_description_content_type='text/markdown',
    author='dragon-devs',
    author_email='dragonfourtyseven@email.com',
    url='https://github.com/dragon-devs/custom-tree',
```

