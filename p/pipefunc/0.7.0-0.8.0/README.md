# Comparing `tmp/pipefunc-0.7.0.tar.gz` & `tmp/pipefunc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefunc-0.7.0.tar", last modified: Wed May 15 22:37:35 2024, max compression
+gzip compressed data, was "pipefunc-0.8.0.tar", last modified: Fri May 17 00:21:22 2024, max compression
```

## Comparing `pipefunc-0.7.0.tar` & `pipefunc-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:35.812435 pipefunc-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 22:37:29.000000 pipefunc-0.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 22:37:29.000000 pipefunc-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 22:37:29.000000 pipefunc-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-15 22:37:35.812435 pipefunc-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-15 22:37:29.000000 pipefunc-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:35.812435 pipefunc-0.7.0/pipefunc/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    47334 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    24881 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-15 22:37:35.812435 pipefunc-0.7.0/pipefunc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:35.808436 pipefunc-0.7.0/pipefunc/map/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/map/_filearray.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/map/_mapspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/map/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pipefunc/map/adaptive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:35.808436 pipefunc-0.7.0/pipefunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-15 22:37:35.000000 pipefunc-0.7.0/pipefunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-15 22:37:35.000000 pipefunc-0.7.0/pipefunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:37:35.000000 pipefunc-0.7.0/pipefunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 22:37:35.000000 pipefunc-0.7.0/pipefunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 22:37:35.000000 pipefunc-0.7.0/pipefunc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-15 22:37:29.000000 pipefunc-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:37:35.812435 pipefunc-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:35.808436 pipefunc-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17503 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-15 22:37:29.000000 pipefunc-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 00:21:09.000000 pipefunc-0.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-17 00:21:09.000000 pipefunc-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 00:21:09.000000 pipefunc-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-17 00:21:22.765198 pipefunc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-17 00:21:09.000000 pipefunc-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.769198 pipefunc-0.8.0/pipefunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47314 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 00:21:22.769198 pipefunc-0.8.0/pipefunc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.761198 pipefunc-0.8.0/pipefunc/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_filearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_mapspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/adaptive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/pipefunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:21:22.765198 pipefunc-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13132 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_utils.py
```

### Comparing `pipefunc-0.7.0/LICENSE` & `pipefunc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/PKG-INFO` & `pipefunc-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pipefunc-0.7.0/README.md` & `pipefunc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/__init__.py` & `pipefunc-0.8.0/pipefunc/__init__.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_cache.py` & `pipefunc-0.8.0/pipefunc/_cache.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_lazy.py` & `pipefunc-0.8.0/pipefunc/_lazy.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_perf.py` & `pipefunc-0.8.0/pipefunc/_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_pipefunc.py` & `pipefunc-0.8.0/pipefunc/_pipefunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,14 @@
     name: str,
     output_name: _OUTPUT_TYPE,
 ) -> Any:
     """Default output picker function for tuples."""
     return output[output_name.index(name)]
 
 
-def _update_wrapper(wrapper, wrapped) -> None:  # noqa: ANN001
-    functools.update_wrapper(wrapper, wrapped)
-    # Need to manually update __wrapped__ to keep functions picklable
-    del wrapper.__dict__["__wrapped__"]
-
-
 class PipeFunc(Generic[T]):
     """Function wrapper class for pipeline functions with additional attributes.
 
     Parameters
     ----------
     func
         The original function to be wrapped.
@@ -117,15 +111,14 @@
         profile: bool = False,
         debug: bool = False,
         cache: bool = False,
         save_function: Callable[[str | Path, dict[str, Any]], None] | None = None,
         mapspec: str | MapSpec | None = None,
     ) -> None:
         """Function wrapper class for pipeline functions with additional attributes."""
-        _update_wrapper(self, func)
         self.func: Callable[..., Any] = func
         self.output_name: _OUTPUT_TYPE = output_name
         self.debug = debug
         self.cache = cache
         self.save_function = save_function
         self.mapspec = MapSpec.from_string(mapspec) if isinstance(mapspec, str) else mapspec
         self.output_picker: Callable[[Any, str], Any] | None = output_picker
@@ -282,15 +275,15 @@
         self.__dict__.update(state)
         self.func = cloudpickle.loads(self.func)
 
     def _validate_mapspec(self) -> None:
         if self.mapspec is None:
             return
 
-        if not isinstance(self.mapspec, MapSpec):
+        if not isinstance(self.mapspec, MapSpec):  # pragma: no cover
             msg = (
                 "The 'mapspec' argument should be an instance of MapSpec,"
                 f" not {type(self.mapspec)}."
             )
             raise TypeError(msg)
 
         mapspec_input_names = {x.name for x in self.mapspec.inputs}
```

### Comparing `pipefunc-0.7.0/pipefunc/_pipeline.py` & `pipefunc-0.8.0/pipefunc/_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
         Returns
         -------
         Any
             The return value of the pipeline function.
 
         """
-        return self.pipeline._run_pipeline(output_name=self.output_name, kwargs=kwargs)
+        return self.pipeline.run(output_name=self.output_name, kwargs=kwargs)
 
     def call_full_output(self, **kwargs: Any) -> dict[str, Any]:
         """Call the pipeline function with the given arguments and return all outputs.
 
         Parameters
         ----------
         kwargs
@@ -122,15 +122,15 @@
 
         Returns
         -------
         Any
             The return value of the pipeline function.
 
         """
-        return self.pipeline._run_pipeline(self.output_name, full_output=True, kwargs=kwargs)
+        return self.pipeline.run(self.output_name, full_output=True, kwargs=kwargs)
 
     def call_with_dict(self, kwargs: dict[str, Any]) -> Any:
         """Call the pipeline function with the given arguments.
 
         Parameters
         ----------
         kwargs
@@ -251,15 +251,15 @@
         with contextlib.suppress(AttributeError):
             del self.all_arg_combinations
         with contextlib.suppress(AttributeError):
             del self.all_root_args
         with contextlib.suppress(AttributeError):
             del self.topological_generations
 
-    def get_cache(self) -> LRUCache | HybridCache | DiskCache | SimpleCache | None:
+    def _current_cache(self) -> LRUCache | HybridCache | DiskCache | SimpleCache | None:
         """Return the cache used by the pipeline."""
         if not isinstance(self.cache, SimpleCache) and (tg := task_graph()) is not None:
             return tg.cache
         return self.cache
 
     @property
     def profile(self) -> bool | None:
@@ -487,15 +487,15 @@
         all_results: dict[_OUTPUT_TYPE, Any],
         full_output: bool,
         used_parameters: set[str | None],
     ) -> Any:
         func = self.output_to_func[output_name]
         assert func.parameters is not None
 
-        cache = self.get_cache()
+        cache = self._current_cache()
         use_cache = (func.cache and cache is not None) or task_graph() is not None
 
         root_args = self.root_args(output_name)
         result_from_cache = False
         if use_cache:
             assert cache is not None
             cache_key = _compute_cache_key(func.output_name, kwargs, root_args)
@@ -529,15 +529,15 @@
         if use_cache and cache_key is not None:
             assert cache is not None
             _update_cache(cache, cache_key, r, start_time)
         _update_all_results(func, r, output_name, all_results, self.lazy)
         _save_results(func, r, output_name, all_results, root_args, self.lazy)
         return all_results[output_name]
 
-    def _run_pipeline(
+    def run(
         self,
         output_name: _OUTPUT_TYPE,
         *,
         full_output: bool = False,
         kwargs: dict[str, Any],
     ) -> Any:
         """Execute the pipeline for a specific return value.
```

### Comparing `pipefunc-0.7.0/pipefunc/_plotting.py` & `pipefunc-0.8.0/pipefunc/_plotting.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_simplify.py` & `pipefunc-0.8.0/pipefunc/_simplify.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/_sweep.py` & `pipefunc-0.8.0/pipefunc/_sweep.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
         self.items = items
         self.dims = dims
         self.exclude = exclude
         self.constants = constants
         self.derivers = derivers
 
     def generate(self) -> Generator[dict[str, Any], None, None]:  # noqa: PLR0912
+        if not self.items:
+            return  # If there are no items, return an empty generator
+
         if self.dims is None or set(self.dims) == self.items.keys():
             # Create the full Cartesian product if no dimensions are provided.
             names = self.items.keys()
             vals = self.items.values()
             for res in product(*vals):
                 combination = dict(zip(names, res))
                 if self.constants is not None:
@@ -164,14 +167,18 @@
                 for k, v in zip(keys, item):
                     new_items.setdefault(k, []).append(v)
             return Sweep(
                 items=new_items,  # type: ignore[arg-type]
                 dims=[tuple(keys)],
             )
 
+        if not any(k in self.items for k in keys):
+            # Return an empty sweep with no dimensions if no items match the filter keys
+            return Sweep({})
+
         dims: list[str | tuple[str, ...]]
         if self.dims is None or set(self.dims) == self.items.keys():
             dims = [k for k in self.items if k in keys]
         else:
             dims = []
             for dim_group in self.dims:
                 if isinstance(dim_group, str) and dim_group in keys:
@@ -207,22 +214,22 @@
             dims = at_least_tuple(dim_group)
             group_length = len(self.items[dims[0]])
             total_length *= group_length
         return total_length
 
     def __add__(self, other: Sweep) -> MultiSweep:
         """Combine this Sweep with another one, creating a MultiSweep."""
-        if not isinstance(other, Sweep):
-            msg = "Other object must be a Sweep or a MultiSweep instance."
+        if not isinstance(other, Sweep):  # pragma: no cover
+            msg = "Other object must be a `Sweep` or a `MultiSweep` instance."
             raise TypeError(msg)
         return MultiSweep(self, other)
 
     def combine(self, other: Sweep) -> MultiSweep:
         """Add another sweep to this MultiSweep."""
-        return other + self
+        return self + other
 
     def product(self, *others: Sweep) -> Sweep:
         """Create a Cartesian product of this Sweep with other Sweeps.
 
         Parameters
         ----------
         *others
@@ -245,15 +252,15 @@
          {'a': 2, 'b': 4, 'c': 5}, {'a': 2, 'b': 4, 'c': 6}]
 
         """
         items = self.items.copy()
         dims = self.dims.copy() if self.dims is not None else None
 
         for other in others:
-            if not isinstance(other, Sweep):
+            if not isinstance(other, Sweep):  # pragma: no cover
                 msg = "All arguments must be Sweep instances."
                 raise TypeError(msg)
             items.update(other.items)
             if dims is not None:
                 if other.dims is not None:
                     dims.extend(other.dims)
                 else:
@@ -343,21 +350,21 @@
     def filtered_sweep(self, keys: Iterable[str]) -> MultiSweep:
         """Return a new MultiSweep, but only include the specified keys in each dictionary, and remove duplicates."""
         filtered_sweeps = [sweep.filtered_sweep(keys) for sweep in self.sweeps]
         return MultiSweep(*filtered_sweeps)
 
     def __add__(self, other: Sweep) -> MultiSweep:
         """Add another sweep to this MultiSweep."""
-        if not isinstance(other, Sweep):
-            msg = "Other object must be a Sweep or a MultiSweep instance."
+        if not isinstance(other, Sweep):  # pragma: no cover
+            msg = "Other object must be a `Sweep` or a `MultiSweep` instance."
             raise TypeError(msg)
         return self.combine(other)
 
     def combine(self, other: Sweep) -> MultiSweep:
-        """Add another sweep to this MultiSweep."""
+        """Add another sweep to this `MultiSweep`."""
         if isinstance(other, MultiSweep):
             self.sweeps.extend(other.sweeps)
         else:
             self.sweeps.append(other)
         return self
```

### Comparing `pipefunc-0.7.0/pipefunc/map/_filearray.py` & `pipefunc-0.8.0/pipefunc/map/_filearray.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,22 @@
         return self.folder / self.filename_template.format(index)
 
     def _key_to_file(self, key: tuple[int, ...]) -> Path:
         """Return the filename associated with the given key."""
         index = sum(k * s for k, s in zip(key, self.strides))
         return self._index_to_file(index)
 
+    def get_from_index(self, index: int) -> Any:
+        """Return the data associated with the given linear index."""
+        return load(self._index_to_file(index))
+
+    def has_index(self, index: int) -> bool:
+        """Return whether the given linear index exists."""
+        return self._index_to_file(index).is_file()
+
     def _files(self) -> Iterator[Path]:
         """Yield all the filenames that constitute the data in this array."""
         return (self._key_to_file(x) for x in itertools.product(*map(range, self.shape)))
 
     def _slice_indices(self, key: tuple[int | slice, ...]) -> list[range]:
         return [
             range(*k.indices(self.shape[i])) if isinstance(k, slice) else range(k, k + 1)
```

### Comparing `pipefunc-0.7.0/pipefunc/map/_mapspec.py` & `pipefunc-0.8.0/pipefunc/map/_mapspec.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pipefunc/map/_run.py` & `pipefunc-0.8.0/pipefunc/map/_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, NamedTuple, Tuple, Union
 
 import numpy as np
 
-from pipefunc._utils import at_least_tuple, dump, handle_error, load, prod
+from pipefunc._utils import at_least_tuple, dump, equal_dicts, handle_error, load, prod
 from pipefunc.map._filearray import FileArray
 from pipefunc.map._mapspec import MapSpec, array_shape
 
 if TYPE_CHECKING:
     import sys
 
     from pipefunc import PipeFunc, Pipeline
@@ -68,44 +68,77 @@
 
 
 def _load_input(name: str, input_paths: dict[str, Path]) -> Any:
     path = input_paths[name]
     return load(path, cache=True)
 
 
-def _output_path(output_name: str, folder: Path) -> Path:
-    return folder / f"{output_name}.cloudpickle"
+def _output_path(output_name: str, run_folder: Path) -> Path:
+    return run_folder / "outputs" / f"{output_name}.cloudpickle"
 
 
 def _dump_output(func: PipeFunc, output: Any, run_folder: Path) -> Any:
     folder = run_folder / "outputs"
     folder.mkdir(parents=True, exist_ok=True)
 
     if isinstance(func.output_name, tuple):
         new_output = []  # output in same order as func.output_name
         for output_name in func.output_name:
             assert func.output_picker is not None
             _output = func.output_picker(output, output_name)
             new_output.append(_output)
-            path = _output_path(output_name, folder)
+            path = _output_path(output_name, run_folder)
             dump(output, path)
         output = new_output
     else:
-        path = _output_path(func.output_name, folder)
+        path = _output_path(func.output_name, run_folder)
         dump(output, path)
 
     return output
 
 
 def _load_output(output_name: str, run_folder: Path) -> Any:
-    folder = run_folder / "outputs"
-    path = _output_path(output_name, folder)
+    path = _output_path(output_name, run_folder)
     return load(path)
 
 
+def cleanup_run_folder(run_folder: str | Path) -> None:
+    """Remove the run folder and its contents."""
+    run_folder = Path(run_folder)
+    shutil.rmtree(run_folder, ignore_errors=True)
+
+
+def _compare_to_previous_run_info(
+    pipeline: Pipeline,
+    run_folder: Path,
+    inputs: dict[str, Any],
+    manual_shapes: dict[str, int | tuple[int, ...]],
+) -> None:
+    if not RunInfo.path(run_folder).is_file():
+        return
+    old = RunInfo.load(run_folder, cache=False)
+    if manual_shapes != old.manual_shapes:
+        msg = "Manual shapes do not match previous run, cannot use `cleanup=False`."
+        raise ValueError(msg)
+    if map_shapes(pipeline, inputs, manual_shapes) != old.shapes:
+        msg = "Shapes do not match previous run, cannot use `cleanup=False`."
+        raise ValueError(msg)
+    old_inputs = {k: _load_input(k, old.input_paths) for k in inputs}
+    equal_inputs = equal_dicts(inputs, old_inputs, verbose=True)
+    if equal_inputs is None:
+        print(
+            "Could not compare new `inputs` to `inputs` from previous run."
+            " Proceeding without `cleanup`, hoping for the best.",
+        )
+        return
+    if not equal_inputs:
+        msg = "Inputs do not match previous run, cannot use `cleanup=False`."
+        raise ValueError(msg)
+
+
 class RunInfo(NamedTuple):
     input_paths: dict[str, Path]
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]]
     manual_shapes: dict[str, int | tuple[int, ...]]
     run_folder: Path
 
     @classmethod
@@ -117,39 +150,45 @@
         manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
         *,
         cleanup: bool = True,
     ) -> RunInfo:
         run_folder = Path(run_folder)
         manual_shapes = manual_shapes or {}
         if cleanup:
-            shutil.rmtree(run_folder, ignore_errors=True)
+            cleanup_run_folder(run_folder)
+        else:
+            _compare_to_previous_run_info(pipeline, run_folder, inputs, manual_shapes)
         input_paths = _dump_inputs(inputs, pipeline.defaults, run_folder)
         shapes = map_shapes(pipeline, inputs, manual_shapes)
         return cls(
             input_paths=input_paths,
             shapes=shapes,
             manual_shapes=manual_shapes,
             run_folder=run_folder,
         )
 
     def dump(self, run_folder: str | Path) -> None:
-        path = Path(run_folder) / "run_info.cloudpickle"
+        path = self.path(run_folder)
         dump(self._asdict(), path)
 
     @classmethod
     def load(
         cls: type[RunInfo],
         run_folder: str | Path,
         *,
         cache: bool = True,
     ) -> RunInfo:
-        path = Path(run_folder) / "run_info.cloudpickle"
+        path = cls.path(run_folder)
         dct = load(path, cache=cache)
         return cls(**dct)
 
+    @staticmethod
+    def path(run_folder: str | Path) -> Path:
+        return Path(run_folder) / "run_info.cloudpickle"
+
 
 def _file_array_path(output_name: str, run_folder: Path) -> Path:
     assert isinstance(output_name, str)
     return run_folder / "outputs" / output_name
 
 
 def _load_parameter(
@@ -263,42 +302,86 @@
     index: int,
     output: list[Any],
 ) -> None:
     for result_array, _output in zip(result_arrays, output):
         result_array[index] = _output
 
 
+def _existing_and_missing_indices(file_arrays: list[FileArray]) -> tuple[list[int], list[int]]:
+    masks = (arr._mask_list() for arr in file_arrays)
+    existing_indices = []
+    missing_indices = []
+    for i, mask_values in enumerate(zip(*masks)):
+        if any(mask_values):  # rerun if any of the outputs are missing
+            missing_indices.append(i)
+        else:
+            existing_indices.append(i)
+    return existing_indices, missing_indices
+
+
 def _execute_map_spec(
     func: PipeFunc,
     kwargs: dict[str, Any],
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]],
     run_folder: Path,
     parallel: bool,  # noqa: FBT001
 ) -> np.ndarray | list[np.ndarray]:
     assert isinstance(func.mapspec, MapSpec)
     shape = shapes[func.output_name]
-    n = prod(shape)
     file_arrays = _init_file_arrays(func.output_name, shape, run_folder)
     result_arrays = _init_result_arrays(func.output_name, shape)
     process_index = partial(_run_iteration_and_pick_output, func=func, kwargs=kwargs, shape=shape)
+    existing, missing = _existing_and_missing_indices(file_arrays)
+    n = len(missing)
     if parallel and n > 1:
         with ProcessPoolExecutor() as ex:
-            outputs_list = list(ex.map(process_index, range(n)))
+            outputs_list = list(ex.map(process_index, missing))
     else:
-        outputs_list = [process_index(index) for index in range(n)]
+        outputs_list = [process_index(index) for index in missing]
 
-    for index, outputs in enumerate(outputs_list):
+    for index, outputs in zip(missing, outputs_list):
         _update_file_array(func, file_arrays, shape, index, outputs)
         _update_result_array(result_arrays, index, outputs)
 
+    for index in existing:
+        outputs = [file_array.get_from_index(index) for file_array in file_arrays]
+        _update_result_array(result_arrays, index, outputs)
+
     result_arrays = [x.reshape(shape) for x in result_arrays]
     return result_arrays if isinstance(func.output_name, tuple) else result_arrays[0]
 
 
+def _maybe_load_single_output(
+    func: PipeFunc,
+    run_folder: Path,
+    *,
+    return_output: bool = True,
+) -> tuple[Any, bool]:
+    """Load the output if it exists.
+
+    Returns the output and a boolean indicating whether the output exists.
+    """
+    output_paths = [_output_path(p, run_folder) for p in at_least_tuple(func.output_name)]
+    if all(p.is_file() for p in output_paths):
+        if not return_output:
+            return None, True
+        outputs = [load(p) for p in output_paths]
+        if isinstance(func.output_name, tuple):
+            return outputs, True
+        return outputs[0], True
+    return None, False
+
+
 def _execute_single(func: PipeFunc, kwargs: dict[str, Any], run_folder: Path) -> Any:
+    # Load the output if it exists
+    output, exists = _maybe_load_single_output(func, run_folder)
+    if exists:
+        return output
+
+    # Otherwise, run the function
     _load_file_array(kwargs)
     try:
         output = func(**kwargs)
     except Exception as e:
         handle_error(e, func, kwargs)
         raise  # handle_error raises but mypy doesn't know that
     return _dump_output(func, output, run_folder)
@@ -394,16 +477,16 @@
 
 def run(
     pipeline: Pipeline,
     inputs: dict[str, Any],
     run_folder: str | Path,
     manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
     *,
-    cleanup: bool = True,
     parallel: bool = True,
+    cleanup: bool = True,
 ) -> list[Result]:
     run_folder = Path(run_folder)
     run_info = RunInfo.create(run_folder, pipeline, inputs, manual_shapes, cleanup=cleanup)
     run_info.dump(run_folder)
     outputs = []
     for gen in pipeline.topological_generations[1]:
         # These evaluations *can* happen in parallel
```

### Comparing `pipefunc-0.7.0/pipefunc/map/adaptive.py` & `pipefunc-0.8.0/pipefunc/map/adaptive.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Provides functions to create adaptive learners for a pipeline."""
 
 from __future__ import annotations
 
 import functools
+from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Tuple, Union
+from typing import TYPE_CHECKING, Any, Tuple, Union
 
 import adaptive
 
 from pipefunc._utils import prod
 from pipefunc.map._mapspec import MapSpec
 from pipefunc.map._run import (
     RunInfo,
     _execute_single,
     _func_kwargs,
     _init_file_arrays,
+    _maybe_load_single_output,
     _MockPipeline,
     _run_iteration_and_pick_output,
     _update_file_array,
     run,
 )
 
 if TYPE_CHECKING:
@@ -38,14 +40,15 @@
 def create_learners(
     pipeline: Pipeline,
     inputs: dict[str, Any],
     run_folder: str | Path,
     manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
     *,
     return_output: bool = False,
+    cleanup: bool = True,
 ) -> list[dict[_OUTPUT_TYPE, adaptive.SequenceLearner]]:
     """Create adaptive learners for a single `Pipeline.map` call.
 
     Creates a learner for each function node in the graph. Which means that
     the returned lists of learners have to be executed in order.
     If a single list contains multiple learners, they can be executed in
     parallel.
@@ -58,24 +61,26 @@
         The inputs to the pipeline, the same as passed to `pipeline.map`.
     run_folder
         The folder to store the run information.
     manual_shapes
         The manual shapes to use for the run.
     return_output
         Whether to return the output of the function in the learner.
+    cleanup
+        Whether to clean up the `run_folder`.
 
     Returns
     -------
     A list of dictionaries where the keys are the output names of the
     functions and the values are the corresponding adaptive learners. As noted
     above, the learners have to be executed in order.
 
     """
     run_folder = Path(run_folder)
-    run_info = RunInfo.create(run_folder, pipeline, inputs, manual_shapes)
+    run_info = RunInfo.create(run_folder, pipeline, inputs, manual_shapes, cleanup=cleanup)
     run_info.dump(run_folder)
     learners = []
     for gen in pipeline.topological_generations[1]:
         _learners = {}
         for func in gen:
             if func.mapspec:
                 f = functools.partial(
@@ -97,26 +102,36 @@
                 sequence = [None]  # type: ignore[list-item]
             learner = adaptive.SequenceLearner(f, sequence)
             _learners[func.output_name] = learner
         learners.append(_learners)
     return learners
 
 
+def flatten_learners(
+    learners_dicts: list[dict[_OUTPUT_TYPE, adaptive.SequenceLearner]],
+) -> dict[_OUTPUT_TYPE, adaptive.SequenceLearner]:
+    """Flatten the list of dictionaries of learners into a single dictionary."""
+    return {k: v for learner_dict in learners_dicts for k, v in learner_dict.items()}
+
+
 def _execute_iteration_in_single(
     _: Any,
     func: PipeFunc,
     run_info: RunInfo,
     run_folder: Path,
     *,
     return_output: bool = False,
 ) -> Any | None:
     """Execute a single iteration of a single function.
 
     Meets the requirements of `adaptive.SequenceLearner`.
     """
+    output, exists = _maybe_load_single_output(func, run_folder, return_output=return_output)
+    if exists:
+        return output
     kwargs = _func_kwargs(
         func,
         run_info.input_paths,
         run_info.shapes,
         run_info.manual_shapes,
         run_folder,
     )
@@ -127,61 +142,79 @@
 def _execute_iteration_in_map_spec(
     index: int,
     func: PipeFunc,
     run_info: RunInfo,
     run_folder: Path,
     *,
     return_output: bool = False,
-) -> Any | None:
+) -> list[Any] | None:
     """Execute a single iteration of a map spec.
 
     Performs a single iteration of the code in `_execute_map_spec`, however,
     it does not keep and return the output. This is meant to be used in the
     parallel execution of the map spec.
 
     Meets the requirements of `adaptive.SequenceLearner`.
     """
+    shape = run_info.shapes[func.output_name]
+    file_arrays = _init_file_arrays(func.output_name, shape, run_folder)
+    # Load the data if it exists
+    if all(arr.has_index(index) for arr in file_arrays):
+        if not return_output:
+            return None
+        return [arr.get_from_index(index) for arr in file_arrays]
+    # Otherwise, run the function
     assert isinstance(func.mapspec, MapSpec)
     kwargs = _func_kwargs(
         func,
         run_info.input_paths,
         run_info.shapes,
         run_info.manual_shapes,
         run_folder,
     )
-    shape = run_info.shapes[func.output_name]
-    file_arrays = _init_file_arrays(func.output_name, shape, run_folder)
     outputs = _run_iteration_and_pick_output(index, func, kwargs, shape)
     _update_file_array(func, file_arrays, shape, index, outputs)
     return outputs if return_output else None
 
 
-def _map_wrapper(
-    pipeline: _MockPipeline,
-    inputs: dict[str, Any],
-    run_folder: Path,
-    manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
-) -> Callable[[Any], None]:
+@dataclass
+class _MapWrapper:
     """Wraps the `pipefunc.map.run` function and makes it a callable with a single unused argument.
 
     Uses a `_MockPipeline` that contains all the required information to run the pipeline but is
     cheaper to serialize and pass around.
     """
 
-    def wrapped(_: Any) -> None:
-        run(pipeline, inputs, run_folder=run_folder, manual_shapes=manual_shapes)  # type: ignore[arg-type]
-
-    return wrapped
+    mock_pipeline: _MockPipeline
+    inputs: dict[str, Any]
+    run_folder: Path
+    manual_shapes: dict[str, int | tuple[int, ...]] | None
+    parallel: bool
+    cleanup: bool
+
+    def __call__(self, _: Any) -> None:
+        """Run the pipeline."""
+        run(
+            self.mock_pipeline,  # type: ignore[arg-type]
+            self.inputs,
+            self.run_folder,
+            self.manual_shapes,
+            parallel=self.parallel,
+            cleanup=self.cleanup,
+        )
 
 
 def create_learners_from_sweep(
     pipeline: Pipeline,
     sweep: Sweep,
     run_folder: str | Path,
     manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+    *,
+    parallel: bool = True,
+    cleanup: bool = True,
 ) -> tuple[list[adaptive.SequenceLearner], list[Path]]:
     """Create adaptive learners for a sweep.
 
     Creates an `adaptive.SequenceLearner` for each sweep run. These learners
     have a single iteration that executes the map in parallel. This means
     that here we rely on the internal parallelization of the pipeline. Each
     learner is fully independent of the others, and they can be executed in
@@ -199,26 +232,30 @@
         The sweep to create learners for, must generate `input` dictionaries as
         expected by `pipeline.map`.
     run_folder
         The folder to store the run information. Each sweep run will be stored in
         a subfolder of this folder.
     manual_shapes
         The manual shapes to use for the run, as expected by `pipeline.map`.
+    parallel
+        Whether to run the map in parallel.
+    cleanup
+        Whether to clean up the `run_folder`.
 
     Returns
     -------
     A tuple of lists where the first list contains the learners and the second
     list contains the run folders for each sweep run.
 
     """
     run_folder = Path(run_folder)
     learners = []
     folders = []
     max_digits = len(str(len(sweep) - 1))
     for i, inputs in enumerate(sweep):
         sweep_run = run_folder / f"sweep_{str(i).zfill(max_digits)}"
         mock_pipeline = _MockPipeline.from_pipeline(pipeline)
-        f = _map_wrapper(mock_pipeline, inputs, sweep_run, manual_shapes)
+        f = _MapWrapper(mock_pipeline, inputs, sweep_run, manual_shapes, parallel, cleanup)
         learner = adaptive.SequenceLearner(f, sequence=[None])
         learners.append(learner)
         folders.append(sweep_run)
     return learners, folders
```

### Comparing `pipefunc-0.7.0/pipefunc.egg-info/PKG-INFO` & `pipefunc-0.8.0/pipefunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pipefunc-0.7.0/pipefunc.egg-info/SOURCES.txt` & `pipefunc-0.8.0/pipefunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/pyproject.toml` & `pipefunc-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/tests/test_cache.py` & `pipefunc-0.8.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/tests/test_dag.py` & `pipefunc-0.8.0/tests/test_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 
     @pipefunc.pipefunc(output_name="e")
     def f3(c, d, x=1):
         return c * d * x
 
     pipeline = pipefunc.Pipeline([f1, f2, f3], lazy=True)
     f = pipeline.func("e")
-    assert not isinstance(pipeline.get_cache(), pipefunc._cache.SimpleCache)
+    assert not isinstance(pipeline._current_cache(), pipefunc._cache.SimpleCache)
     with construct_dag() as dag:
-        cache = pipeline.get_cache()
+        cache = pipeline._current_cache()
         assert isinstance(cache, pipefunc._cache.SimpleCache)
         assert not cache.cache
         f(a=1, b=2)
         f(a=1, b=2)
         assert cache.cache
         assert cache is dag.cache
```

### Comparing `pipefunc-0.7.0/tests/test_perf.py` & `pipefunc-0.8.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/tests/test_pipefunc.py` & `pipefunc-0.8.0/tests/test_pipefunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for pipefunc.py."""
 
 from __future__ import annotations
 
 import inspect
 import pickle
+from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import pytest
 
 from pipefunc import (
     PipeFunc,
     Pipeline,
@@ -655,7 +656,28 @@
 def test_output_picker_single_output():
     @pipefunc(output_name=("y",), output_picker=dict.__getitem__)
     def f(a, b):
         return {"y": a + b, "_throw": 1}
 
     pipeline = Pipeline([f])
     assert pipeline("y", a=1, b=2) == 3
+
+
+def f(a, b):
+    return a + b
+
+
+@dataclass
+class DataClass:
+    a: int
+
+
+def test_pickle_pipefunc():
+    func = PipeFunc(f, output_name="c")
+    p = pickle.dumps(func)
+    func2 = pickle.loads(p)  # noqa: S301
+    assert func(1, 2) == func2(1, 2)
+
+    func = PipeFunc(DataClass, output_name="c")
+    p = pickle.dumps(func)
+    func2 = pickle.loads(p)  # noqa: S301
+    assert func(a=1) == func2(a=1)
```

### Comparing `pipefunc-0.7.0/tests/test_simplify.py` & `pipefunc-0.8.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.7.0/tests/test_sweep.py` & `pipefunc-0.8.0/tests/test_sweep.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,17 +150,20 @@
 
 
 def test_multi_sweep():
     sweep1 = Sweep({"a": [1, 2], "b": [3, 4]})
     sweep2 = Sweep({"x": [5, 6], "y": [7, 8]})
     multi_sweep = MultiSweep(sweep1, sweep2)
     multi_sweep2 = sweep1 + sweep2
+    multi_sweep3 = sweep1.combine(sweep2)
     expected_result = sweep1.list() + sweep2.list()
     assert multi_sweep.list() == multi_sweep2.list() == expected_result
+    assert multi_sweep.list() == multi_sweep3.list() == expected_result
     assert len(multi_sweep) == len(multi_sweep2) == 8
+    assert len(multi_sweep) == len(multi_sweep3) == 8
 
 
 def test_sweep_add():
     sweep1 = Sweep({"a": [1, 2], "b": [3, 4]})
     sweep2 = Sweep({"x": [5, 6], "y": [7, 8]})
     multi_sweep = sweep1 + sweep2
     assert isinstance(multi_sweep, MultiSweep)
@@ -270,14 +273,18 @@
         dims=[("a", "b"), ("c",)],
         derivers=derivers,
     )
     filtered_sweep = sweep.filtered_sweep(("b", "d"))
 
     assert filtered_sweep.list() == [{"b": 3, "d": 3}, {"b": 4, "d": 8}]
 
+    multi = sweep.filtered_sweep(("b",)) + sweep.filtered_sweep(("d",))
+    assert multi.list() == [{"b": 3}, {"b": 4}, {"d": 3}, {"d": 8}]
+    assert multi.filtered_sweep(("b",)).list() == [{"b": 3}, {"b": 4}]
+
     # Test with unhashable items
     sweep = Sweep(
         items={"a": [[1], [2]], "b": [[3], [4]]},  # type: ignore[arg-type]
         derivers={"c": lambda combo: combo["a"][0] * 2},
     )
     assert sweep.list() == [  # check normal sweep
         {"a": [1], "b": [3], "c": 2},
@@ -416,7 +423,15 @@
 
     assert sweep3.list() == [
         {"a": 1, "b": 3, "x": 10, "y": 20},
         {"a": 1, "b": 4, "x": 10, "y": 20},
         {"a": 2, "b": 3, "x": 10, "y": 20},
         {"a": 2, "b": 4, "x": 10, "y": 20},
     ]
+
+
+def test_empty_filtered_sweep() -> None:
+    assert Sweep({}).list() == []
+
+    sweep = Sweep({"a": [1, 2], "b": [3, 4]})
+    filtered_sweep = sweep.filtered_sweep(("x",))
+    assert filtered_sweep.list() == []
```

