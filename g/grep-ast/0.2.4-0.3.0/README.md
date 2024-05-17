# Comparing `tmp/grep-ast-0.2.4.tar.gz` & `tmp/grep_ast-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grep-ast-0.2.4.tar", last modified: Tue Oct 31 23:48:07 2023, max compression
+gzip compressed data, was "grep_ast-0.3.0.tar", last modified: Fri May 17 21:41:13 2024, max compression
```

## Comparing `grep-ast-0.2.4.tar` & `grep_ast-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2023-10-31 23:48:07.822003 grep-ast-0.2.4/
--rw-r--r--   0 gauthier   (501) staff       (20)    11358 2023-07-28 21:17:34.000000 grep-ast-0.2.4/LICENSE.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       25 2023-10-19 17:15:21.000000 grep-ast-0.2.4/MANIFEST.in
--rw-r--r--   0 gauthier   (501) staff       (20)     2018 2023-10-31 23:48:07.821592 grep-ast-0.2.4/PKG-INFO
--rw-r--r--   0 gauthier   (501) staff       (20)     1721 2023-07-30 16:43:39.000000 grep-ast-0.2.4/README.md
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2023-10-31 23:48:07.817848 grep-ast-0.2.4/grep_ast/
--rw-r--r--   0 gauthier   (501) staff       (20)       86 2023-10-19 16:59:55.000000 grep-ast-0.2.4/grep_ast/__init__.py
--rw-r--r--   0 gauthier   (501) staff       (20)      653 2023-07-29 19:09:18.000000 grep-ast-0.2.4/grep_ast/dump.py
--rwxr-xr-x   0 gauthier   (501) staff       (20)     9040 2023-10-31 18:19:26.000000 grep-ast-0.2.4/grep_ast/grep_ast.py
--rwxr-xr-x   0 gauthier   (501) staff       (20)     3342 2023-10-31 18:19:26.000000 grep-ast-0.2.4/grep_ast/main.py
--rw-r--r--   0 gauthier   (501) staff       (20)     1284 2023-10-31 23:35:33.000000 grep-ast-0.2.4/grep_ast/parsers.py
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2023-10-31 23:48:07.820390 grep-ast-0.2.4/grep_ast.egg-info/
--rw-r--r--   0 gauthier   (501) staff       (20)     2018 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/PKG-INFO
--rw-r--r--   0 gauthier   (501) staff       (20)      371 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/SOURCES.txt
--rw-r--r--   0 gauthier   (501) staff       (20)        1 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/dependency_links.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       74 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/entry_points.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/requires.txt
--rw-r--r--   0 gauthier   (501) staff       (20)        9 2023-10-31 23:48:07.000000 grep-ast-0.2.4/grep_ast.egg-info/top_level.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-10-31 18:19:28.000000 grep-ast-0.2.4/requirements.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-10-31 23:48:07.822147 grep-ast-0.2.4/setup.cfg
--rw-r--r--   0 gauthier   (501) staff       (20)      765 2023-10-31 23:47:49.000000 grep-ast-0.2.4/setup.py
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2023-10-31 23:48:07.820727 grep-ast-0.2.4/tests/
--rw-r--r--   0 gauthier   (501) staff       (20)      247 2023-10-31 23:36:18.000000 grep-ast-0.2.4/tests/test_parsers.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.083300 grep_ast-0.3.0/
+-rw-r--r--   0 gauthier   (501) staff       (20)    11358 2023-07-28 21:17:34.000000 grep_ast-0.3.0/LICENSE.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       25 2023-10-19 17:15:21.000000 grep_ast-0.3.0/MANIFEST.in
+-rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-17 21:41:13.082416 grep_ast-0.3.0/PKG-INFO
+-rw-r--r--   0 gauthier   (501) staff       (20)     2255 2023-12-10 15:48:41.000000 grep_ast-0.3.0/README.md
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.076687 grep_ast-0.3.0/grep_ast/
+-rw-r--r--   0 gauthier   (501) staff       (20)       86 2023-10-19 16:59:55.000000 grep_ast-0.3.0/grep_ast/__init__.py
+-rw-r--r--   0 gauthier   (501) staff       (20)      653 2023-07-29 19:09:18.000000 grep_ast-0.3.0/grep_ast/dump.py
+-rwxr-xr-x   0 gauthier   (501) staff       (20)     9049 2024-05-17 21:18:06.000000 grep_ast-0.3.0/grep_ast/grep_ast.py
+-rwxr-xr-x   0 gauthier   (501) staff       (20)     3377 2024-01-25 20:59:41.000000 grep_ast-0.3.0/grep_ast/main.py
+-rw-r--r--   0 gauthier   (501) staff       (20)     1378 2024-05-17 21:40:39.000000 grep_ast-0.3.0/grep_ast/parsers.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.081726 grep_ast-0.3.0/grep_ast.egg-info/
+-rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/PKG-INFO
+-rw-r--r--   0 gauthier   (501) staff       (20)      371 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)        1 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       74 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/entry_points.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/requires.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)        9 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/top_level.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-12-10 15:44:50.000000 grep_ast-0.3.0/requirements.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-17 21:41:13.083438 grep_ast-0.3.0/setup.cfg
+-rw-r--r--   0 gauthier   (501) staff       (20)      765 2024-05-17 21:40:20.000000 grep_ast-0.3.0/setup.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.080761 grep_ast-0.3.0/tests/
+-rw-r--r--   0 gauthier   (501) staff       (20)      247 2023-12-10 15:44:50.000000 grep_ast-0.3.0/tests/test_parsers.py
```

### Comparing `grep-ast-0.2.4/LICENSE.txt` & `grep_ast-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grep-ast-0.2.4/PKG-INFO` & `grep_ast-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-Metadata-Version: 2.1
-Name: grep-ast
-Version: 0.2.4
-Summary: A tool to grep through the AST of a source file
-Home-page: https://github.com/paul-gauthier/grep-ast
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: tree-sitter-languages>=1.8.0
-Requires-Dist: pathspec
-
 # grep-ast
 
 Grep soure code files and see matching lines with
 useful context that show how they fit into the code.
 See the loops, functions, methods, classes, etc
 that contain all the matching lines.
 Get a sense of what's inside a matched class or function definition.
 You see relevant code from every layer of the
 abstract syntax tree, above and below the matches.
 
+By default, grep-AST recurses the current directory to search all source code files.
+It respects `.gitignore`, so it will usually "do the right thing" in most repos
+if you just do `grep-ast <regex>` without specifying any filenames.
+
+You can also invoke `grep-ast` as `gast` for convenience.
+
 Grep-AST is built with [tree-sitter](https://tree-sitter.github.io/tree-sitter/) and
 [tree-sitter-languages](https://github.com/grantjenks/py-tree-sitter-languages).
 So it supports a lot of popular [code languages](https://github.com/paul-gauthier/grep-ast/blob/main/grep_ast/parsers.py).
 
 ## Install
 
 ```bash
@@ -54,14 +50,19 @@
   --encoding ENCODING  file encoding
   --languages          print the parsers table
   --verbose            enable verbose output
 ```
 
 ## Examples
 
-Here we search for **"encoding"** in the source to this tool:
+Here we search for **"encoding"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+shows you how the matches fit into the code base.
 
 <img src="assets/screenshot-encoding.svg" alt="aider screencast">
 
-Here we search for **"TreeContext"** in the source to this tool:
+Here we search for **"TreeContext"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+helps you understand the *contents* of a matching
+named code block (class, function, method, etc).
 
 <img src="assets/screenshot-TreeContext.svg" alt="aider screencast">
```

### Comparing `grep-ast-0.2.4/README.md` & `grep_ast-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,33 @@
+Metadata-Version: 2.1
+Name: grep-ast
+Version: 0.3.0
+Summary: A tool to grep through the AST of a source file
+Home-page: https://github.com/paul-gauthier/grep-ast
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: tree-sitter-languages>=1.8.0
+Requires-Dist: pathspec
+
 # grep-ast
 
 Grep soure code files and see matching lines with
 useful context that show how they fit into the code.
 See the loops, functions, methods, classes, etc
 that contain all the matching lines.
 Get a sense of what's inside a matched class or function definition.
 You see relevant code from every layer of the
 abstract syntax tree, above and below the matches.
 
+By default, grep-AST recurses the current directory to search all source code files.
+It respects `.gitignore`, so it will usually "do the right thing" in most repos
+if you just do `grep-ast <regex>` without specifying any filenames.
+
+You can also invoke `grep-ast` as `gast` for convenience.
+
 Grep-AST is built with [tree-sitter](https://tree-sitter.github.io/tree-sitter/) and
 [tree-sitter-languages](https://github.com/grantjenks/py-tree-sitter-languages).
 So it supports a lot of popular [code languages](https://github.com/paul-gauthier/grep-ast/blob/main/grep_ast/parsers.py).
 
 ## Install
 
 ```bash
@@ -44,14 +60,19 @@
   --encoding ENCODING  file encoding
   --languages          print the parsers table
   --verbose            enable verbose output
 ```
 
 ## Examples
 
-Here we search for **"encoding"** in the source to this tool:
+Here we search for **"encoding"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+shows you how the matches fit into the code base.
 
 <img src="assets/screenshot-encoding.svg" alt="aider screencast">
 
-Here we search for **"TreeContext"** in the source to this tool:
+Here we search for **"TreeContext"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+helps you understand the *contents* of a matching
+named code block (class, function, method, etc).
 
 <img src="assets/screenshot-TreeContext.svg" alt="aider screencast">
```

### Comparing `grep-ast-0.2.4/grep_ast/dump.py` & `grep_ast-0.3.0/grep_ast/dump.py`

 * *Files identical despite different names*

### Comparing `grep-ast-0.2.4/grep_ast/grep_ast.py` & `grep_ast-0.3.0/grep_ast/grep_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         self.done_parent_scopes = set()
 
         self.show_lines = set(self.lines_of_interest)
 
         if self.loi_pad:
             for line in list(self.show_lines):
-                for new_line in [line - self.loi_pad, line + self.loi_pad]:
+                for new_line in range(line - self.loi_pad, line + self.loi_pad + 1):
                     if self.scopes[line].intersection(self.scopes[new_line]):
                         self.show_lines.add(new_line)
 
         if self.last_line:
             # add the bottom line (plus parent context)
             bottom_line = self.num_lines - 2
             self.show_lines.add(bottom_line)
```

### Comparing `grep-ast-0.2.4/grep_ast/main.py` & `grep_ast-0.3.0/grep_ast/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,28 +56,28 @@
     else:
         spec = pathspec.PathSpec.from_lines("gitwildmatch", [])
 
     for fname in enumerate_files(args.filenames, spec):
         process_filename(fname, args)
 
 
-def enumerate_files(fnames, spec):
+def enumerate_files(fnames, spec, use_spec=False):
     for fname in fnames:
         fname = Path(fname)
 
         # oddly, Path('.').name == "" so we will recurse it
-        if fname.name.startswith(".") or spec.match_file(fname):
+        if fname.name.startswith(".") or use_spec and spec.match_file(fname):
             continue
 
         if fname.is_file():
             yield str(fname)
             continue
 
         if fname.is_dir():
-            for sub_fnames in enumerate_files(fname.iterdir(), spec):
+            for sub_fnames in enumerate_files(fname.iterdir(), spec, True):
                 yield sub_fnames
 
 
 def process_filename(filename, args):
     try:
         with open(filename, "r", encoding=args.encoding) as file:
             code = file.read()
```

### Comparing `grep-ast-0.2.4/grep_ast/parsers.py` & `grep_ast-0.3.0/grep_ast/parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 # Updated mapping of file extensions to parsers
 PARSERS = {
     ".py": "python",
     ".js": "javascript",
+    ".mjs": "javascript", # mjs file extension stands for "module JavaScript."
     ".go": "go",
     ".bash": "bash",
     ".c": "c",
     ".cc": "cpp",
     ".cs": "c_sharp",
     ".cl": "commonlisp",
     ".cpp": "cpp",
@@ -34,14 +35,15 @@
     # ".md": "markdown", # https://github.com/ikatyang/tree-sitter-markdown/issues/59
     ".m": "objc",
     ".ml": "ocaml",
     ".pl": "perl",
     ".php": "php",
     ".ql": "ql",
     ".r": "r",
+    ".R": "r",
     ".regex": "regex",
     ".rst": "rst",
     ".rb": "ruby",
     ".rs": "rust",
     ".scala": "scala",
     ".sql": "sql",
     ".sqlite": "sqlite",
```

### Comparing `grep-ast-0.2.4/grep_ast.egg-info/PKG-INFO` & `grep_ast-0.3.0/grep_ast.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grep-ast
-Version: 0.2.4
+Version: 0.3.0
 Summary: A tool to grep through the AST of a source file
 Home-page: https://github.com/paul-gauthier/grep-ast
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: tree-sitter-languages>=1.8.0
 Requires-Dist: pathspec
 
@@ -14,14 +14,20 @@
 useful context that show how they fit into the code.
 See the loops, functions, methods, classes, etc
 that contain all the matching lines.
 Get a sense of what's inside a matched class or function definition.
 You see relevant code from every layer of the
 abstract syntax tree, above and below the matches.
 
+By default, grep-AST recurses the current directory to search all source code files.
+It respects `.gitignore`, so it will usually "do the right thing" in most repos
+if you just do `grep-ast <regex>` without specifying any filenames.
+
+You can also invoke `grep-ast` as `gast` for convenience.
+
 Grep-AST is built with [tree-sitter](https://tree-sitter.github.io/tree-sitter/) and
 [tree-sitter-languages](https://github.com/grantjenks/py-tree-sitter-languages).
 So it supports a lot of popular [code languages](https://github.com/paul-gauthier/grep-ast/blob/main/grep_ast/parsers.py).
 
 ## Install
 
 ```bash
@@ -54,14 +60,19 @@
   --encoding ENCODING  file encoding
   --languages          print the parsers table
   --verbose            enable verbose output
 ```
 
 ## Examples
 
-Here we search for **"encoding"** in the source to this tool:
+Here we search for **"encoding"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+shows you how the matches fit into the code base.
 
 <img src="assets/screenshot-encoding.svg" alt="aider screencast">
 
-Here we search for **"TreeContext"** in the source to this tool:
+Here we search for **"TreeContext"** in the source to this tool.
+These results mainly highlight how `grep-ast`
+helps you understand the *contents* of a matching
+named code block (class, function, method, etc).
 
 <img src="assets/screenshot-TreeContext.svg" alt="aider screencast">
```

### Comparing `grep-ast-0.2.4/setup.py` & `grep_ast-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     long_description = re.sub(r"\n!\[.*\]\(.*\)", "", long_description)
 
 setup(
     name="grep-ast",
-    version="0.2.4",
+    version="0.3.0",
     description="A tool to grep through the AST of a source file",
     url="https://github.com/paul-gauthier/grep-ast",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
```

