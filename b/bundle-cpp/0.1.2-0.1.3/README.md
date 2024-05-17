# Comparing `tmp/bundle_cpp-0.1.2.tar.gz` & `tmp/bundle_cpp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundle_cpp-0.1.2.tar", max compression
+gzip compressed data, was "bundle_cpp-0.1.3.tar", max compression
```

## Comparing `bundle_cpp-0.1.2.tar` & `bundle_cpp-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      418 2024-05-12 09:32:09.611817 bundle_cpp-0.1.2/README.md
--rw-r--r--   0        0        0     2785 2024-05-12 11:18:14.371601 bundle_cpp-0.1.2/bundle_cpp/__init__.py
--rw-r--r--   0        0        0     1783 2024-05-12 11:10:06.231835 bundle_cpp-0.1.2/bundle_cpp/__main__.py
--rw-r--r--   0        0        0     1168 2024-05-12 11:20:31.045388 bundle_cpp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 bundle_cpp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      418 2024-05-17 04:27:24.699708 bundle_cpp-0.1.3/README.md
+-rw-r--r--   0        0        0     3258 2024-05-17 09:45:53.033998 bundle_cpp-0.1.3/bundle_cpp/__init__.py
+-rw-r--r--   0        0        0     1783 2024-05-17 04:27:24.699972 bundle_cpp-0.1.3/bundle_cpp/__main__.py
+-rw-r--r--   0        0        0     1232 2024-05-17 10:02:56.227075 bundle_cpp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 bundle_cpp-0.1.3/PKG-INFO
```

### Comparing `bundle_cpp-0.1.2/bundle_cpp/__init__.py` & `bundle_cpp-0.1.3/bundle_cpp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import List
+import os
+import re
 from pathlib import Path
+from typing import List
 from typing import Optional as Opt
-import re
-import os
 
 WD = Path(os.getcwd())
 
 
 def _read(p: Path) -> List[str]:
     with p.open() as f:
         return f.readlines()
@@ -21,27 +21,30 @@
     if include_paths is None:
         include_paths = []
 
     is_once = set()
     edges = set()
 
     def expand(file: Path) -> str:
+        file = file.resolve()  # ./main.cpp
         dir = file.parent
 
         # angle: #include <header>
         def find_file(
             header: str,
             angle: bool = False,
         ) -> Opt[Path]:
             if not angle:
                 file = dir / header
+                file = file.resolve()  # ../lib.hpp
                 if file.exists():
                     return file
             for d in include_paths:
                 file = d / header
+                file = file.resolve()
                 if file.exists():
                     return file
             return None
 
         def included_file(
             line: str,
         ) -> Opt[str]:
@@ -75,16 +78,20 @@
                 if al and add_line:
                     f = file
                     # if relpath:
                     #     f.relative_to(WD, walk_up=True)
                     result_lines.append(
                         f'#line {i + 1} "{f}"\n'
                     )
+                    # result_lines.append(
+                    #     f'#line {i + 1} "{f}"'
+                    # )
                     al = False
                 result_lines.append(l)
+                # result_lines.append(l.rstrip())
                 continue
             if dep in is_once:
                 al = True
                 continue
             e = (file, dep)
             if e in edges:
                 raise "circular includes"
@@ -95,10 +102,17 @@
 
         # result_lines.reverse()
         # while result_lines:
         #     if result_lines[-1] != "\n":
         #         break
         #     result_lines.pop()
         # result_lines.reverse()
-        return "".join(result_lines)
+
+        # res = '\n'.join(result_lines).rstrip()
+        # return res
+        res = "".join(result_lines)
+        if res == "\n":
+            res = ""
+        return res
+        # return "".join(result_lines)
 
     return expand(src)
```

### Comparing `bundle_cpp-0.1.2/bundle_cpp/__main__.py` & `bundle_cpp-0.1.3/bundle_cpp/__main__.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
-from typing import List
 import argparse
-from pathlib import Path
-from dataclasses import dataclass
 import dataclasses
+import os
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List
 from typing import Optional as Opt
-from . import bundle
 
+from . import bundle
 
 WD = Path(os.getcwd())
 
 
 @dataclass
 class CLIParam:
     src: Path
```

### Comparing `bundle_cpp-0.1.2/pyproject.toml` & `bundle_cpp-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bundle-cpp"
-version = "0.1.2"
+version = "0.1.3"
 description = "expand includes and create a single file"
 authors = ["kagemeka <kagemeka1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bundle_cpp" }]
 # exclude = ["tests"]
 
@@ -30,14 +30,18 @@
 python_files = ["*.py"]
 # by default only test_*.py supported.
 
 python_functions = ["_test*", "test*"]
 # global _test*, and _Tests.test*
 # plz use test* only in private-to-user modules.
 
-python_classes = ["_Tests", "Tests"]
+# python_classes = ["_Tests", "Tests"]
 # classes inheriting unittest.TestCase are also tested by default
 # but if use unittest.TestCase, python_functions are neglected.
 # that is, only 'test*' methods are tested by default
 # plz use Tests only in private-to-user modules.
 
+python_classes = ["_Tests*", "Tests*"]
+# e.g. _Tests_a_func
+
+
 addopts = "--doctest-modules -v"
```

### Comparing `bundle_cpp-0.1.2/PKG-INFO` & `bundle_cpp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bundle-cpp
-Version: 0.1.2
+Version: 0.1.3
 Summary: expand includes and create a single file
 License: MIT
 Author: kagemeka
 Author-email: kagemeka1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

