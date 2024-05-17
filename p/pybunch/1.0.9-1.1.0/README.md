# Comparing `tmp/pybunch-1.0.9.tar.gz` & `tmp/pybunch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.9.tar", last modified: Tue Apr 23 14:28:45 2024, max compression
+gzip compressed data, was "pybunch-1.1.0.tar", last modified: Fri May 17 15:28:36 2024, max compression
```

## Comparing `pybunch-1.0.9.tar` & `pybunch-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.588784 pybunch-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.580783 pybunch-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 14:28:40.000000 pybunch-1.0.9/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 14:28:40.000000 pybunch-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 14:28:40.000000 pybunch-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 14:28:45.584784 pybunch-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 14:28:40.000000 pybunch-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 14:28:40.000000 pybunch-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:28:45.588784 pybunch-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.580783 pybunch-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/packed_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.283361 pybunch-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.279361 pybunch-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.279361 pybunch-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-17 15:28:32.000000 pybunch-1.1.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 15:28:32.000000 pybunch-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 15:28:32.000000 pybunch-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 15:28:36.283361 pybunch-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 15:28:32.000000 pybunch-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.279361 pybunch-1.1.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 15:28:32.000000 pybunch-1.1.0/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-17 15:28:32.000000 pybunch-1.1.0/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.283361 pybunch-1.1.0/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 15:28:32.000000 pybunch-1.1.0/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-17 15:28:32.000000 pybunch-1.1.0/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:32.000000 pybunch-1.1.0/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-17 15:28:32.000000 pybunch-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:28:36.283361 pybunch-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.279361 pybunch-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.283361 pybunch-1.1.0/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:32.000000 pybunch-1.1.0/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 15:28:32.000000 pybunch-1.1.0/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-17 15:28:32.000000 pybunch-1.1.0/src/pybunch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-17 15:28:32.000000 pybunch-1.1.0/src/pybunch/packed_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-17 15:28:32.000000 pybunch-1.1.0/src/pybunch/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:28:36.283361 pybunch-1.1.0/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 15:28:36.000000 pybunch-1.1.0/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.9/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.1.0/.github/workflows/publish-to-pypi.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -50,50 +50,41 @@
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
     name: >-
-      Sign the Python 🐍 distribution 📦 with Sigstore
-      and upload them to GitHub Release
+      Upload the Python 🐍 distribution 📦 as GitHub Release
     needs:
     - publish-to-pypi
     runs-on: ubuntu-latest
 
     permissions:
       contents: write  # IMPORTANT: mandatory for making GitHub Releases
-      id-token: write  # IMPORTANT: mandatory for sigstore
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
-    - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
-      with:
-        inputs: >-
-          ./dist/*.tar.gz
-          ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         --repo '${{ github.repository }}'
         --notes ""
-    - name: Upload artifact signatures to GitHub Release
+    - name: Upload artifacts to GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
       # Upload to GitHub Release using the `gh` CLI.
-      # `dist/` contains the built packages, and the
-      # sigstore-produced signatures and certificates.
+      # `dist/` contains the built packages
       run: >-
         gh release upload
         '${{ github.ref_name }}' dist/**
         --repo '${{ github.repository }}'
 
   publish-to-testpypi:
     name: Publish Python 🐍 distribution 📦 to TestPyPI
```

### Comparing `pybunch-1.0.9/LICENSE` & `pybunch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.9/PKG-INFO` & `pybunch-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.9
+Version: 1.1.0
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.9/pyproject.toml` & `pybunch-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -23,7 +23,10 @@
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "no-local-version"
 
 [project.urls]
 Homepage = "https://github.com/ykaridi/pybunch"
 Issues = "https://github.com/ykaridi/pybunch/issues"
+
+[project.scripts]
+pybunch = "pybunch.cli:main"
```

### Comparing `pybunch-1.0.9/src/pybunch/packed_base.py` & `pybunch-1.1.0/src/pybunch/packed_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         self.path = ModulePath(*name.split('.'))
         self.parent_name = '.'.join(self.path.parts[:-1])
         self.package = None  # type: str
         self.source_code = code
         self._compiled = None  # type: 'code'
         self._module = None  # type: _module_type | None
 
-
     @property
     def compiled(self):
+        # type: () -> 'code'
         if self._compiled is None:
             self._compiled = compile(self.source_code, self.file_name, 'exec')
         return self._compiled
 
     def is_package(self, name):
         # type: (str) -> bool
         return self.path.parts[-1] == '__init__'
@@ -98,28 +98,36 @@
     def load_module(self, name):
         # type: (str) -> _module_type
         if self._module is None:
             if self.is_package(None):
                 module = _module_type(self.parent_name)
                 self.package = '.'.join(self.path.parts[:-2])
                 self.name = self.parent_name
-                module.__path__ = []
+                module.__path__ = [self.name]
             else:
                 module = _module_type(self.name)
                 self.package = self.parent_name
 
+            sys.modules[self.name] = module
+
             module.__package__ = self.package
             module.__file__ = self.file_name
-            self.run_module(_globals=module.__dict__)
+
+            try:
+                self.run_module(_globals=module.__dict__)
+            except:  # noqa
+                del sys.modules[self.name]
+                raise
+
             self._module = module
 
         return sys.modules.setdefault(name, self._module)
 
     def run_module(self, _globals=None, name=None):
-        # type: (str) -> None
+        # type: (dict[str, object], str) -> dict[str, object]
         if _globals is None:
             _globals = {}
 
         _globals.update(__name__=name if name is not None else self.name,
                         __file__=self.file_name,
                         __loader__=self,
                         __package__=self.parent_name)
@@ -127,15 +135,15 @@
         restore_name = '__name__' in _globals
         old_filename = _globals.get('__name__', None)
         if name is not None:
             _globals['__name__'] = name
 
         exec(self.compiled, _globals)
         if restore_name:
-            _globals[''] = old_filename
+            _globals['__name__'] = old_filename
         else:
             del _globals['__name__']
 
         return _globals
 
     def get_code(self, name):
         # type: (str) -> 'code'
@@ -202,14 +210,15 @@
         sys.meta_path = [self] + sys.meta_path
         yield
         sys.meta_path = old_meta_path
 
     @property
     @contextmanager
     def with_custom_stacktrace(self):
+        # type: () -> 'Generator[None, None, None]'
         old_except_hook = sys.excepthook
         print_exception = traceback.print_exception
 
         def except_hook(ex_type, ex, tb):
             print_exception(ex_type, ex, tb)
 
         sys.excepthook = except_hook
@@ -225,14 +234,17 @@
         # type: (str) -> _module_type
         with self.add_to_meta_path, self.with_custom_stacktrace:
             try:
                 new_globals = runpy.run_module(module, run_name='__main__')
             except ImportError:
                 # Fallback for jython
                 imported_module = importlib.import_module(module)
+                loader = imported_module.__loader__
+                if not isinstance(loader, ModuleDescription):
+                    raise
                 new_globals = imported_module.__loader__.run_module(name='__main__')
 
         current_globals = globals()
         keys_to_delete = set(current_globals.keys()).difference(new_globals)
         current_globals.update(new_globals)
         for key in keys_to_delete:
             del current_globals[key]
```

### Comparing `pybunch-1.0.9/src/pybunch/project.py` & `pybunch-1.1.0/src/pybunch/project.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,118 @@
 import importlib.resources
-from functools import cached_property
+import ast
+from functools import cached_property, reduce
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
 
-from . import packed_base
+import pybunch
 from .packed_base import DynamicLocalImporter, ModulePath, ModuleDescription
 
 
 class Project:
-    def __init__(self, package_mapping: Dict[ModulePath, Path], package: str):
-        if package is not None:
-            package_mapping = {ModulePath(package) / relative_path: absolute_path
-                               for relative_path, absolute_path in package_mapping.items()}
+    def __init__(self, package_mapping: Dict[ModulePath, Path]):
         self._package_mapping = package_mapping
-        self._package = package
 
     @property
     def dynamic_local_importer(self) -> DynamicLocalImporter:
         module_descriptions = {}
         for relative_path, absolute_path in self._package_mapping.items():
             name = '.'.join(relative_path.parts)
             module_descriptions[name] = ModuleDescription(name, code=absolute_path.read_text())
 
         return DynamicLocalImporter(module_descriptions)
 
     @cached_property
     def packed_code_base(self) -> str:
-        packed_base_file = importlib.resources.files(packed_base) / 'packed_base.py'
+        packed_base_file = importlib.resources.files(pybunch) / 'packed_base.py'
         with packed_base_file.open("rt") as f:
             return f.read()
 
+    def translate_module(self, name: str) -> Optional[ModulePath]:
+        path = ModulePath.from_name(name)
+        if path in self._package_mapping:
+            return path
+        elif (path / '__main__') in self._package_mapping:
+            return path / '__main__'
+        else:
+            return None
+
+    def static_find_imports(self, entrypoint: ModulePath):
+        visited = set()
+        queue = {entrypoint}
+        while queue:
+            path = queue.pop()
+            visited.add(path)
+
+            tree = ast.parse(self._package_mapping[path].read_text())
+            for node in ast.walk(tree):
+                if isinstance(node, ast.ImportFrom):
+                    level = node.level
+                    if level == 0:
+                        base = ModulePath()
+                    else:
+                        base = reduce(lambda p, _: p.parent, range(level), path)
+
+                    base = base / ModulePath.from_name(node.module)
+                    modules = [base]
+                    for name in node.names:
+                        modules.append(base / ModulePath.from_name(name.name))
+
+                elif isinstance(node, ast.Import):
+                    modules = [ModulePath.from_name(name.name) for name in node.names]
+                else:
+                    continue
+
+                for module in modules:
+                    if module in self._package_mapping:
+                        if module not in visited and module not in queue:
+                            queue.add(module)
+
+                    while len(module.parts) > 0:
+                        init = module / '__init__'
+                        if init in self._package_mapping:
+                            if init not in visited and module not in queue:
+                                queue.add(init)
+                        module = module.parent
+
+        return visited
+
     def pack(self, entrypoint: str, statically_optimize: bool = False) -> str:
-        entrypoint_path = ModulePath.from_name(entrypoint)
-        if self._package is not None and entrypoint_path.parts[0] != self._package:
-            entrypoint_path = ModulePath(self._package) / entrypoint_path
-        if entrypoint_path not in self._package_mapping:
+        entrypoint_path = self.translate_module(entrypoint)
+        if entrypoint_path is None:
             raise ValueError("Nonexistent entrypoint")
-        entrypoint = str(entrypoint_path)
+        entrypoint = '.'.join(entrypoint_path.parts)
 
         included_packages = set(self._package_mapping.keys())
         if statically_optimize:
-            dli = self.dynamic_local_importer
-            dli.import_module(entrypoint)
-
-            loaded_modules = {ModulePath.from_name(name) for name in dli.loaded_modules}
-            included_packages = {relative_path for relative_path in self._package_mapping
-                                 if (relative_path in loaded_modules) or
-                                 (relative_path.name == '__init__' and relative_path.parent in loaded_modules)}
+            included_packages = self.static_find_imports(entrypoint_path)
 
         code_entries = []
         package_entries = []
         for pth in included_packages:
             name = '.'.join(pth.parts)
             escaped_name = 'PYBUNCH_%s' % '_'.join(pth.parts).upper()
             code = self._package_mapping[pth].read_text()
-            escaped_code = code.replace('"', '\\"')
 
-            code_entries.append(f'# Code for module <{name}>\n{escaped_name} = """\n{escaped_code}\n"""[1:]')
+            # Escape code
+            _escaped_code = repr(code)
+            open_quote, escaped_code, close_quote = _escaped_code[0], _escaped_code[1:-1], _escaped_code[-1]
+            assert open_quote == close_quote
+            quote = open_quote * 3
+            escaped_code = escaped_code.replace("\\n", "\n")
+            escaped_code = f"{quote}\n{escaped_code}\n{quote}"
+
+            code_entries.append(f'# Code for module <{name}>\n{escaped_name} = {escaped_code}')
             package_entries.append(f"'{name}': ModuleDescription('{name}', code={escaped_name})")
 
         header = ''.join(entry + "\n\n\n" for entry in code_entries)
-        footer = f"""\n\n
+        NEWLINE = '\n'
+        footer = f"""{NEWLINE * 2}
 dli = DynamicLocalImporter({{
-{',\n'.join("    %s" % entry for entry in package_entries)}
+{(',' + NEWLINE).join("    %s" % entry for entry in package_entries)}
 }})
 dli.execute_module('{entrypoint}')
 """
 
         packed_code_base_lines = self.packed_code_base.splitlines()
         last_import_line = max(lineno for lineno, line in enumerate(packed_code_base_lines)
                                if line.startswith("import ") or line.startswith("from "))
```

### Comparing `pybunch-1.0.9/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.1.0/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.9
+Version: 1.1.0
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

