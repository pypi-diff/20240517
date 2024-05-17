# Comparing `tmp/deps_rocker-0.1.5.tar.gz` & `tmp/deps_rocker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.5.tar` & `deps_rocker-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     1288 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/__init__.py
--rw-r--r--   0        0        0      128 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/dep_rocker_cli.py
--rw-r--r--   0        0        0     8012 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      127 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/deps.yaml
--rw-r--r--   0        0        0      226 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0     1422 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/dependencies_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0      152 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/toposort.py
--rw-r--r--   0        0        0     2292 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 deps_rocker-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7090 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/__init__.py
+-rw-r--r--   0        0        0     1097 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/command_layer.py
+-rw-r--r--   0        0        0      128 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/dep_rocker_cli.py
+-rw-r--r--   0        0        0     6772 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      226 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-17 15:16:31.637214 deps_rocker-0.1.6/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0     2292 2024-05-17 15:16:31.641214 deps_rocker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 deps_rocker-0.1.6/PKG-INFO
```

### Comparing `deps_rocker-0.1.5/deps_rocker/dependencies.py` & `deps_rocker-0.1.6/deps_rocker/dependencies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,13 @@
-import em
-import pkgutil
-from rocker.extensions import RockerExtension
 from pathlib import Path
+from collections import defaultdict
 import yaml
 import toml
-from collections import defaultdict
-from dataclasses import dataclass, field
-from typing import List
-
-
-@dataclass
-class CommandLayer:
-    layer: str = None
-    command: str = None
-    data: set = field(default_factory=set)
-
-    def get_filename(self):
-        return f"{self.command}_{self.layer}"
-
-    def update(self, key: str, value: List):
-        split = key.split("_")
-        self.command = split[0]
-        if len(split) > 1:
-            self.layer = split[1]
-        else:
-            self.layer = "default"
-        if isinstance(value, list):
-            for v in value:
-                self.data.add(v)
-        else:
-            self.data.add(value)
-
-    def to_snippet(self):
-        snippet = pkgutil.get_data(
-            "deps_rocker", f"templates/{self.command}_snippet.Dockerfile"
-        ).decode("utf-8")
-
-        empy_data = dict(
-            data_list=list(sorted(self.data)),
-            filename=self.get_filename(),
-            layer_name=self.layer,
-        )
-        print("empy_snippet", snippet)
-        print("empy_data", empy_data)
-
-        return em.expand(snippet, empy_data)
+from rocker.extensions import RockerExtension
+from .command_layer import CommandLayer
 
 
 class Dependencies(RockerExtension):
     name = "deps_dependencies"
 
     def __init__(self, pattern: str = "*deps.yaml", path: Path = None) -> None:
         if path is None:
@@ -73,17 +32,15 @@
         for p in path.rglob(pattern):
             print(f"found {p}")
             self.deps_files.append(p)
             with open(p, "r", encoding="utf-8") as file:
                 vals = yaml.safe_load(file)
                 print(vals)
                 if vals is not None:
-                    # prev_k = "PRIMAL_DEPENDENCY"
                     prev_k = None
-
                     for k in vals:
                         for v in vals[k]:
                             if "script" in k:
                                 if v is not None:
                                     v = (p.parent / Path(v)).absolute().as_posix()
                             print(f"key:{k} val:{v}")
 
@@ -95,18 +52,14 @@
                                 self.layers[k].update(k, v)
 
                             self.dependencies[k].add(v)
                         if prev_k is not None:
                             self.dep_group_order[k].append(prev_k)
                         prev_k = k
 
-        # self.dep_group_order["PRIMAL_DEPENDENCY"] = sorted(
-        #     self.dep_group_order["PRIMAL_DEPENDENCY"]
-        # )
-
         for k, v in self.dep_group_order.items():
             self.dep_group_order[k] = list(dict.fromkeys(v))
 
     def get_deps(self, key: str, as_list: bool = False) -> str:
         """Given a dependency key return a space delimited string of dependencies
 
         Args:
```

### Comparing `deps_rocker-0.1.5/pyproject.toml` & `deps_rocker-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deps_rocker"
-version = "0.1.5"
+version = "0.1.6"
 license = { text = "MIT" }
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A rocker plugin to help installing apt and pip dependencies"
 readme = "README.md"
 
 requires-python = ">=3.10"
```

