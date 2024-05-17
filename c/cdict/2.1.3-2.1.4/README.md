# Comparing `tmp/cdict-2.1.3.tar.gz` & `tmp/cdict-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdict-2.1.3.tar", last modified: Sat Nov 11 01:37:23 2023, max compression
+gzip compressed data, was "cdict-2.1.4.tar", last modified: Fri May 17 03:34:46 2024, max compression
```

## Comparing `cdict-2.1.3.tar` & `cdict-2.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-11-11 01:37:23.220448 cdict-2.1.3/
--rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-2.1.3/LICENSE
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-11-11 01:37:23.219574 cdict-2.1.3/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)    10324 2023-09-11 00:08:14.000000 cdict-2.1.3/README.md
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-11-11 01:37:23.212603 cdict-2.1.3/cdict/
--rw-r--r--   0 jeffwu     (503) staff       (20)     1632 2023-11-11 01:36:51.000000 cdict-2.1.3/cdict/__init__.py
--rw-r--r--   0 jeffwu     (503) staff       (20)     6075 2023-10-26 20:11:45.000000 cdict-2.1.3/cdict/core.py
--rw-r--r--   0 jeffwu     (503) staff       (20)     1037 2023-10-26 20:12:18.000000 cdict-2.1.3/cdict/utils.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-11-11 01:37:23.215860 cdict-2.1.3/cdict.egg-info/
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-11-11 01:37:22.000000 cdict-2.1.3/cdict.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)      208 2023-11-11 01:37:23.000000 cdict-2.1.3/cdict.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-11-11 01:37:22.000000 cdict-2.1.3/cdict.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-11-11 01:37:22.000000 cdict-2.1.3/cdict.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-11-11 01:37:23.220526 cdict-2.1.3/setup.cfg
--rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-11-11 01:37:13.000000 cdict-2.1.3/setup.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-11-11 01:37:23.218860 cdict-2.1.3/tests/
--rw-r--r--   0 jeffwu     (503) staff       (20)    14848 2023-10-26 20:18:32.000000 cdict-2.1.3/tests/test_main.py
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-17 03:34:46.719746 cdict-2.1.4/
+-rw-r--r--   0 jeffwu     (502) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-2.1.4/LICENSE
+-rw-r--r--   0 jeffwu     (502) staff       (20)      199 2024-05-17 03:34:46.719372 cdict-2.1.4/PKG-INFO
+-rw-r--r--   0 jeffwu     (502) staff       (20)    11005 2024-03-06 21:20:47.000000 cdict-2.1.4/README.md
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-17 03:34:46.717236 cdict-2.1.4/cdict/
+-rw-r--r--   0 jeffwu     (502) staff       (20)     1638 2024-05-17 03:30:30.000000 cdict-2.1.4/cdict/__init__.py
+-rw-r--r--   0 jeffwu     (502) staff       (20)     7461 2024-05-17 03:30:30.000000 cdict-2.1.4/cdict/core.py
+-rw-r--r--   0 jeffwu     (502) staff       (20)     1176 2024-05-17 03:30:30.000000 cdict-2.1.4/cdict/utils.py
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-17 03:34:46.718398 cdict-2.1.4/cdict.egg-info/
+-rw-r--r--   0 jeffwu     (502) staff       (20)      199 2024-05-17 03:34:46.000000 cdict-2.1.4/cdict.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (502) staff       (20)      208 2024-05-17 03:34:46.000000 cdict-2.1.4/cdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)        1 2024-05-17 03:34:46.000000 cdict-2.1.4/cdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)        6 2024-05-17 03:34:46.000000 cdict-2.1.4/cdict.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)       38 2024-05-17 03:34:46.719813 cdict-2.1.4/setup.cfg
+-rw-r--r--   0 jeffwu     (502) staff       (20)      282 2024-05-17 03:34:32.000000 cdict-2.1.4/setup.py
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-17 03:34:46.718663 cdict-2.1.4/tests/
+-rw-r--r--   0 jeffwu     (502) staff       (20)    16653 2024-05-17 03:30:30.000000 cdict-2.1.4/tests/test_main.py
```

### Comparing `cdict-2.1.3/LICENSE` & `cdict-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdict-2.1.3/README.md` & `cdict-2.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,152 @@
 # cdict
 
-This is a small library for creating lists of dictionaries combinatorially, for config/hyperparameter sweep management.
+This is a small library for creating iterators of dictionaries combinatorially, for config/hyperparameter sweep management.
 
 ## Installation
 
 `pip install cdict`
 
 ## Usage
 
 ### Basic features and primitives
 
-The basic unit in `cdict` is essentially a list of dictionaries.  We then have two main operations:
+The basic unit in `cdict` is essentially a stream of dictionaries (`Iterable[dict]`).  We then have two main operations:
+<ul>
+    <li>
 
-- `a + b` concatenates (includes items in list `a` and list `b`)
-- `a * b` does an outer product (includes items formed by combining all pairs of items from list `a` and list `b`)
+`x + y` concatenates (includes dictionaries in `x` and then dictionaries in `y`), much like list addition
 
-Other features include:
-- nesting of `cdict`s
-- customizable combining behavior, gives user control over conflict resolution
-- transforms of `cdict`s
-- `|` which does a zip/elementwise product of lists of equal length
-
-### Examples
-
-It can be easier to understand `cdict` by example!
-
-(Though shorter than the examples below, [the codebase](./cdict/core.py) is probably a more arduous read..)
+<details><summary>Example</summary>
 
 ```python
-import pytest
 import cdict as C
 
-###############################################################################
-# The basics
-###############################################################################
-
-# create very simple values
+# setup
 a1 = C.dict(a=1)
-# cdicts always represent a list of dictionaries
 assert list(a1) == [dict(a=1)]
 a2 = C.dict(a=2)
 assert list(a2) == [dict(a=2)]
 
 # "add" cdicts by union-ing the set of dicts
 sweep_a = a1 + a2
 assert list(sweep_a) == [dict(a=1), dict(a=2)]
 
 # equivalent way to add
-sweep_b = C.sum(C.dict(b=b) for b in [1,2])
+sweep_a = C.sum(C.dict(a=a) for a in [1,2])
+assert list(sweep_a) == [dict(a=1), dict(a=2)]
+
+# a convenience
+sweep_a = C.dict(a=C.list(1, 2))
+assert list(sweep_a) == [dict(a=1), dict(a=2)]
+```
+
+</details>
+</li>
+
+<li>
+
+`x * y` does an outer product (includes dictionaries formed by *combining* all pairs of dictionaries from `x` and `y`)
+
+<details><summary>Example</summary>
+
+```python
+import cdict as C
+
+# setup
+sweep_a = C.dict(a=C.list(1, 2))
+assert list(sweep_a) == [dict(a=1), dict(a=2)]
+sweep_b = C.dict(b=C.list(1,2))
 assert list(sweep_b) == [dict(b=1), dict(b=2)]
 
 # "multiply" cdicts by combinatorially combining all possibilities
 sweep_ab = sweep_a * sweep_b
 assert list(sweep_ab) == [
     dict(a=1, b=1), dict(a=1, b=2),
     dict(a=2, b=1), dict(a=2, b=2),
 ]
 
-###############################################################################
-# Composing building blocks
-###############################################################################
+# a convenience
+sweep_ab = C.dict(
+    a=C.list(1, 2),
+    b=C.list(1, 2),
+)
+assert list(sweep_ab) == [
+    dict(a=1, b=1), dict(a=1, b=2),
+    dict(a=2, b=1), dict(a=2, b=2),
+]
+```
+
+</details>
+</li>
+
+</ul>
+
+These two basic operations can be composed arbitrarily, and behave as you would expect!
+
+<details><summary>Example</summary>
+
+```python
+import cdict as C
+
+sweep_a = C.dict(a=C.list(1, 2))
+assert list(sweep_a) == [dict(a=1), dict(a=2)]
+sweep_b = C.dict(b=C.list(1,2))
+assert list(sweep_b) == [dict(b=1), dict(b=2)]
 
 # add and multiply all you want
-baseline = dict(a=0, b=0)
+baseline = C.dict(a=0, b=0)
 sweep_z = C.dict(z=1) + C.dict(z=2)
 sweep_complex = (sweep_a + sweep_z) * sweep_b + baseline
 assert list(sweep_complex) == [
     dict(a=1, b=1), dict(a=1, b=2),
     dict(a=2, b=1), dict(a=2, b=2),
     dict(z=1, b=1), dict(z=1, b=2),
     dict(z=2, b=1), dict(z=2, b=2),
     dict(a=0, b=0),
 ]
 
 # equivalent, thanks to left-distributive property
 sweep_complex_2 = sweep_a * sweep_b + sweep_z * sweep_b + baseline
 assert list(sweep_complex_2) == list(sweep_complex)
+```
 
-###############################################################################
-# Overridable and combinable values
-###############################################################################
+</details>
+
+Note that `cdict`s are lazy.
+
+<details><summary>Example</summary>
+
+```python
+import cdict as C
+
+# avoid lists if needed, for memory efficiency
+sweep_lazy = C.dict(a=C.iter(range(1, 3)), b=C.iter(range(1, 3)))
+it = iter(sweep_lazy)
+assert next(it) == dict(a=1, b=1)
+assert next(it) == dict(a=1, b=2)
+assert next(it) == dict(a=2, b=1)
+assert next(it) == dict(a=2, b=2)
+```
+
+</details>
+
+
+Other features include:
+
+<ul>
+    <li>
+
+customizable combining behavior, gives user control over conflict resolution (allowing vs disallow override)
+
+<details><summary>Example</summary>
+
+```python
+import pytest
+import cdict as C
 
 # conflicting keys errors by default
 a1 = C.dict(a=1)
 a2 = C.dict(a=2)
 with pytest.raises(ValueError):
     list(a1 * a2)
 
@@ -140,44 +203,67 @@
 with pytest.raises(ValueError):
     # defaults don't override
     list(a2 * defaults)
 
 with pytest.raises(ValueError):
     # can't override twice
     list(defaults * a2 * a2)
+```
+
+</details>
+</li>
+
+<li>
+
+nesting of `cdict`s
+
+<details><summary>Example</summary>
+
+```python
+import pytest
+import cdict as C
 
 ###############################################################################
 # Nesting, basics
 ###############################################################################
 
 # You can nest cdicts, to get lists of nested dicts.
 # This is useful if you have nested configuration
-sweep_nested = C.dict(nested_a=sweep_a, nested_b=sweep_b)
+sweep_nested = C.dict(
+    nested_a=C.dict(a=1) + C.dict(a=2),
+    nested_b=C.dict(b=1) + C.dict(b=2),
+)
 assert list(sweep_nested) == [
     dict(nested_a=dict(a=1), nested_b=dict(b=1)),
     dict(nested_a=dict(a=1), nested_b=dict(b=2)),
     dict(nested_a=dict(a=2), nested_b=dict(b=1)),
     dict(nested_a=dict(a=2), nested_b=dict(b=2)),
 ]
 
 # Multiplying nested cdicts acts as expected
-sweep_nested_2 = C.dict(nested_a=sweep_a) * C.dict(nested_b=sweep_b)
+sweep_nested_2 = C.dict(
+    nested_a=C.dict(a=1) + C.dict(a=2),
+) * C.dict(
+    nested_b=C.dict(b=1) + C.dict(b=2),
+)
 assert list(sweep_nested_2) == list(sweep_nested)
 
 ###############################################################################
 # Nesting convenience syntax
 ###############################################################################
 
-# "nested" way to add
+# "nested" syntax for adding
 sweep_a = C.dict(a=C.list(1,2))
 assert list(sweep_a) == [dict(a=1), dict(a=2)]
+sweep_b = C.dict(b=C.list(1,2))
+assert list(sweep_b) == [dict(b=1), dict(b=2)]
 
 # "nested" multiply
-sweep_concise = C.dict(a=C.list(1, 2), b=C.list(1, 2))
-assert list(sweep_concise) == [
+sweep_ab = C.dict(a=C.list(1, 2), b=C.list(1, 2))
+assert list(sweep_ab) == [
     dict(a=1, b=1), dict(a=1, b=2),
     dict(a=2, b=1), dict(a=2, b=2),
 ]
 
 ###############################################################################
 # Nesting and conflicts
 ###############################################################################
@@ -217,31 +303,33 @@
 # since the outer dict isn't final, separate keys is fine even with final values
 nested_sweep_nonconflict = (
     C.dict(nested_a=C.finaldict(a=C.list(1, 2))) *
     C.dict(nested_b=C.finaldict(b=C.list(1, 2)))
 )
 assert list(nested_sweep_nonconflict) == list(sweep_nested)
 
-###############################################################################
-# Everything can be lazy
-###############################################################################
+```
 
-# avoid lists if needed, for memory efficiency
-sweep_lazy = C.dict(a=C.iter(range(1, 3)), b=C.iter(range(1, 3)))
-it = iter(sweep_lazy)
-assert next(it) == dict(a=1, b=1)
-assert next(it) == dict(a=1, b=2)
-assert next(it) == dict(a=2, b=1)
-assert next(it) == dict(a=2, b=2)
+</details>
+</li>
 
-###############################################################################
-# Everything can be transformed (mapped/filtered/etc)
-###############################################################################
+<li>
+
+transforms
+
+<details><summary>Example</summary>
+
+```python
+import cdict as C
+
+sweep_ab = C.dict(
+    a=C.list(1, 2), b=C.list(1, 2),
+)
 
-# and transform with map
+# transform with map
 def square_a(x):
     x['aa'] = x['a']**2
     return x
 
 sweep_squares = sweep_ab.map(square_a)
 assert list(sweep_squares) == [
     dict(a=1, aa=1, b=1),
@@ -265,46 +353,72 @@
 
 sweep_squares_filtered_seeded = sweep_squares_filtered.apply(add_seeds)
 assert list(sweep_squares_filtered_seeded) == [
     dict(aab=2, seed=120), dict(aab=2, seed=121),
     dict(aab=4, seed=210), dict(aab=4, seed=211),
     dict(aab=8, seed=220), dict(aab=8, seed=221),
 ]
+```
 
-###############################################################################
-# Zipping
-###############################################################################
+</details>
+</li>
+
+<li>
+
+a "zip" operation `|` which does an elementwise product of `cdict`s of equal length
+
+
+<details><summary>Example</summary>
+
+```python
+import pytest
+import cdict as C
+
+sweep_a = C.dict(a=C.list(1, 2))
+assert list(sweep_a) == [dict(a=1), dict(a=2)]
+sweep_b = C.dict(b=C.list(1,2))
+assert list(sweep_b) == [dict(b=1), dict(b=2)]
 
 # zipping of equal length things
 diag_sweep = sweep_a | sweep_b
 assert list(diag_sweep) == [
     dict(a=1, b=1), dict(a=2, b=2),
 ]
-
 ```
 
+</details>
+</li>
+
+</ul>
+
+
 ### Properties
 
-`cdict` combinators have some nice properties:
+`cdict` combinators have some nice properties, including essentially everything you would expect given the `+` and `*` syntax.
+
+To be precise:
 
 - `+` is associative
 - `*` is associative if 1
 - `+` is commutative if 2
 - `*` is commutative if 1 and 2
 - `*` is left-distributive over `+`, and right-distributive if 2
-- `|` is associative if 1
-- `|` is commutative if 1
-- `(a + b) | (c + d) = (a | c) + (b | d)` if `len(a) == len(c)`
-- `(a * b) | (c * d) = (a | c) * (b | d)` if `len(a) == len(c)` and `len(b) == len(d)` and `cdict_combine` is associative and commutative 
 
-Where
+Where:
 1. *if values implement `cdict_combine` satisfying the same property, at any/all conflicting keys*
 2. *if ignoring order of the resulting yielded items*
 
-We get essentially every property one would expect given the `+` and `*` syntax.  In fact, they form a commutative semiring with `0 = C.list()` and `1 = C.dict()`!
+For math nerds: assuming these two things, they form a commutative semiring with `0 = C.list()` and `1 = C.dict()`!
+
+We also have properties of `|`:
+
+- `|` is associative if 1
+- `|` is commutative if 1
+- `(a + b) | (c + d) = (a | c) + (b | d)` if `len(a) == len(c)`
+- `(a * b) | (c * d) = (a | c) * (b | d)` if `len(a) == len(c)` and `len(b) == len(d)` and `cdict_combine` is associative and commutative 
 
 ## Tests
 
 `pytest tests`
 
 ## Acknowledgements
```

### Comparing `cdict-2.1.3/cdict/__init__.py` & `cdict-2.1.4/cdict/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from builtins import sum as builtin_sum
 from typing import Any, Iterable
 from .core import cdict_base, cdict_dict, cdict_iter
-from .utils import overridable, override, combinable, combiner
+from .utils import overridable, override, combinable, combiner, lazy
 
 class C():
     @staticmethod
     def dict(**kwargs: Any) -> cdict_base:
         return cdict_dict(kwargs)
 
     @staticmethod
```

### Comparing `cdict-2.1.3/cdict/core.py` & `cdict-2.1.4/cdict/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from __future__ import annotations
 import functools
-from typing import Any, Union, Iterable, Optional, Generator, Tuple, Callable, ItemsView
+from typing import Any, Union, Iterable, Optional, Generator, Tuple, Callable, ItemsView, cast
 import itertools
 
+
+AnyDict = dict[Any, Any]
+
+
 def recursive_map_dict(x: Any, f: Callable[[Any], Any]) -> Any:
     if isinstance(x, dict):
         return {k: recursive_map_dict(v, f) for k, v in x.items()}
     else:
         return f(x)
 
 
@@ -15,51 +19,72 @@
 
 
 class _cdict_value():
     def __init__(self, d: AnyDict, final: bool = False):
         self.d = d
         self.final = final
 
-    def cdict_combine(self, other: AnyDict) -> _cdict_value:
+    def cdict_combine(self, other: _cdict_value) -> _cdict_value:
         if not isinstance(other, _cdict_value):
             raise ValueError(f"Cannot combine with {other}, must be cdict")
         if self.final:
             raise ValueError("Value already finalized")
         return _cdict_value(_combine_dicts([self.d, other.d]), final=other.final)
 
+    def __or__(self, other: _cdict_value | AnyDict) -> _cdict_value:
+        if isinstance(other, dict):
+            return self.cdict_combine(_cdict_value(other))
+        return self.cdict_combine(other)
+
+    def __ror__(self, other: _cdict_value | AnyDict) -> _cdict_value:
+        assert not isinstance(other, _cdict_value), f"Unexpected call to __ror__, should use __or__"
+        if isinstance(other, dict):
+            return _cdict_value(other) | self
+        raise TypeError(f"Cannot combine with {other}, must be dict")
+
+    def __mul__(self, other: Iterable[_cdict_value]) -> Generator[_cdict_value, None, None]:
+        for x in other:
+            yield self | x
+
+    def __rmul__(self, other: Iterable[_cdict_value]) -> Generator[_cdict_value, None, None]:
+        for x in other:
+            yield x | self
+
+    def __getitem__(self, k: Any) -> Any:
+        return self.d[k]
+
     def cdict_item(self) -> AnyDict:
         return recursive_cdict_item(self.d) # type: ignore
 
     def items(self) -> ItemsView[Any, Any]:
         return self.d.items()
 
 
-AnyDict = dict[Any, Any]
-
-
 class cdict_base():
-    def apply(self, fn: Callable[[Any], Any]) -> cdict_base:
-        return _cdict_apply(fn, self)
+    def apply(self, fn: Callable[[Any], Any], raw: bool = False) -> cdict_base:
+        return _cdict_apply(fn, self, raw=raw)
 
-    def map(self, fn: Callable[[Any], Any]) -> cdict_base:
+    def map(self, fn: Callable[[Any], Any], raw: bool = False) -> cdict_base:
         @functools.wraps(fn)
         def apply_fn(x: Any) -> Any:
             yield fn(x)
-        return _cdict_apply(apply_fn, self)
+        return _cdict_apply(apply_fn, self, raw=raw)
 
-    def filter(self, fn: Callable[[Any], bool]) -> cdict_base:
+    def filter(self, fn: Callable[[Any], bool], raw: bool = False) -> cdict_base:
         @functools.wraps(fn)
         def apply_fn(x: Any) -> Any:
             if fn(x): yield x
-        return _cdict_apply(apply_fn, self)
+        return _cdict_apply(apply_fn, self, raw=raw)
 
     def __add__(self, other: cdict_base) -> cdict_base:
         return cdict_iter([self, other])
 
     def __mul__(self, other: cdict_base) -> cdict_base:
+        if not isinstance(other, cdict_base):
+            return NotImplemented
         return _cdict_product(self, other)
 
     def __or__(self, other: cdict_base) -> cdict_base:
         return _cdict_zip([self, other])
 
     def cdict_iter(self) -> Generator[_cdict_value, None, None]:
         raise NotImplementedError("Please override this method")
@@ -67,14 +92,17 @@
     def __iter__(self) -> Generator[AnyDict, None, None]:
         for x in self.cdict_iter():
             yield recursive_cdict_item(x)
 
     def __len__(self) -> int:
         return len(list(iter(self)))
 
+    def __pos__(self) -> cdict_base:
+        return self
+
 
 def _combine_dicts(ds: Iterable[AnyDict]) -> AnyDict:
     res: AnyDict = {}
     for d in ds:
         for k, v in d.items():
             if k in res:
                 if hasattr(res[k], "cdict_combine"):
@@ -124,36 +152,42 @@
             yield _cdict_value(d, final=self._final)
 
     def __repr__(self) -> str:
         return "cdict(" + ", ".join([f"{k}={v}" for k, v in self._item.items()]) + ")"
 
 
 class _cdict_apply(cdict_base):
-    def __init__(self, fn: Callable[[Any], Any], _inner: cdict_base) -> None:
+    def __init__(self, fn: Callable[[Any], Any], _inner: cdict_base, raw: bool = False) -> None:
         self._inner = _inner
         self._fn = fn
+        self.raw = raw
 
     def cdict_iter(self) -> Generator[_cdict_value, None, None]:
         for x in self._inner.cdict_iter():
-            # NOTE: currently this has a few oddities
-            # could expose a "raw" version of cdict apply
-            # TODO don't allow apply for finalized items?
-            # also, give user control over what to finalize?
-            # TODO preserve nesting properly?
-            for v in self._fn(recursive_cdict_item(x)):
-                yield _cdict_value(v)
+            if self.raw:
+                # this version respects finalize, gives user control over that
+                # also lets user use cdict_combine on the values
+                for v in self._fn(x):
+                    if not isinstance(v, _cdict_value):
+                        raise ValueError(f"Raw apply function must return cdict values, got {v}")
+                    yield v
+            else:
+                # TODO preserve nesting properly?
+                for v in self._fn(recursive_cdict_item(x)):
+                    yield _cdict_value(v)
 
     def __repr__(self) -> str:
         return f"{self._inner}.apply({self._fn})"
 
 
 class _cdict_product(cdict_base):
     def __init__(self, _item1: Any, _item2: Any) -> None:
         for c in [_item1, _item2]:
-            assert isinstance(c, cdict_base), f"Cannot multiply non-cdicts: {c}"
+            if not isinstance(c, cdict_base):
+                raise TypeError(f"Cannot multiply non-cdicts: {c}")
         self._item1 = _item1
         self._item2 = _item2
 
     def cdict_iter(self) -> Generator[_cdict_value, None, None]:
         for (d1, d2) in itertools.product(self._item1.cdict_iter(), self._item2.cdict_iter()):
             yield d1.cdict_combine(d2)
```

### Comparing `cdict-2.1.3/cdict/utils.py` & `cdict-2.1.4/cdict/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,7 +37,15 @@
 
     def cdict_item(self) -> Any:
         return self.x
 
 
 def combiner(f: Callable[[Any, Any], Any], multi: bool = True) -> Callable[[Any], combinable]:
     return lambda x: combinable(x, f, multi)
+
+
+class lazy():
+    def __init__(self, f: Callable[[], Any]):
+        self.f = f
+
+    def cdict_item(self) -> Any:
+        return self.f()
```

### Comparing `cdict-2.1.3/tests/test_main.py` & `cdict-2.1.4/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -218,14 +218,60 @@
         dict(a=6, b=3, seed=2, sum=9),
         dict(a=7, b=4, seed=1, sum=11),
         dict(a=7, b=4, seed=2, sum=11),
     ])
     c1 = (cbase.map(increment_a).map(aplusb)) * seeds
     assert_equivalent(c0, c1)
 
+    c2 = c1.filter(lambda x: x['sum'] > 10)
+    assert_dicts(c2, [
+        dict(a=7, b=4, seed=1, sum=11),
+        dict(a=7, b=4, seed=2, sum=11),
+    ])
+
+
+def test_apply():
+    cbase = C.dict(a=5, b=3) + C.dict(a=6, b=4)
+    seeds = C.dict(seed=C.list(1, 2))
+
+    c0 = cbase.apply(lambda x: [x | dict(seed=1), x | dict(seed=2)])
+    assert_dicts(c0, cbase * seeds)
+
+    c0_raw = cbase.apply(lambda x: [x | dict(seed=1), x | dict(seed=2)], raw=True)
+    assert_dicts(c0_raw, cbase * seeds)
+
+    c1 = cbase.apply(lambda x: [dict(**x, seed=1), dict(**x, seed=2)])
+    assert_dicts(c1, cbase * seeds)
+
+    c2 = cbase.apply(lambda x: [dict(seed=1) | x, dict(seed=2) | x])
+    assert_dicts(c2, cbase * seeds)
+
+    with pytest.raises(TypeError):
+        c1_bad = cbase.apply(lambda x: [dict(**x, seed=1), dict(**x, seed=2)], raw=True)
+        assert_dicts(c1_bad, cbase * seeds)
+
+    with pytest.raises(TypeError):
+        c2_bad = cbase.apply(lambda x: [dict(seed=1) | x, dict(seed=2 | x)], raw=True)
+        assert_dicts(c2_bad, cbase * seeds)
+
+    with pytest.raises(TypeError):
+        cmul = cbase.apply(
+            lambda x: x * seeds,
+        )
+        assert_dicts(cmul, cbase * seeds)
+
+    cmul = cbase.apply(
+        lambda x: x * seeds, raw=True
+    )
+    assert_dicts(cmul, cbase * seeds)
+
+    cmul = cbase.apply(
+        lambda x: seeds * x, raw=True
+    )
+    assert_dicts(cmul, cbase * seeds)
 
 def test_mut():
     mut = C.dict(
             inner=C.dict(a=1)
     ) * (
         C.dict() + C.dict(inner=C.dict(b=1))
     )
@@ -453,32 +499,47 @@
         dict(a=1, b=1, c=0, d=1, job=dict(label="a1/b1/c0/d1")),
         dict(a=1, b=1, c=1, d=0, job=dict(label="a1/b1/c1/d0")),
         dict(a=1, b=1, c=1, d=1, job=dict(label="a1/b1/c1/d1")),
     ])
 
 
 
+def test_lazy():
+    called = False
+    def f():
+        nonlocal called
+        called = True
+        return 5
+
+    x = C.dict(a=C.lazy(f))
+    assert not called
+    z = x * C.dict(b=3)
+    assert not called
+    assert_dicts(z, [dict(a=5, b=3)])
+    assert called
+
 
 def test_readme_code():
     readme_file = os.path.join(os.path.dirname(__file__), '..', 'README.md')
     with open(readme_file) as f:
         text = f.read()
-    m = re.search('```(.+?)```', text, flags=re.DOTALL)
-    assert m
-    code = m.group(1)
-    assert code.startswith('python')
-    code = code[6:].strip()
-    try:
-        exec(code, globals(), globals())
-    except Exception as err:
-        error_class = err.__class__.__name__
-        detail = err.args[0] if len(err.args) else ""
-        cl, exc, tb = sys.exc_info()
-        line_number = traceback.extract_tb(tb)[-1][1]
-        raise Exception(f'Error in README.md line {line_number}: {error_class} {detail}')
+    blocks = re.findall('```(.+?)```', text, flags=re.DOTALL)
+    assert len(blocks) > 0
+    for code in blocks:
+        assert code.startswith('python')
+        code = code[6:].strip()
+        env = globals().copy()
+        try:
+            exec(code, env, env)
+        except Exception as err:
+            error_class = err.__class__.__name__
+            detail = err.args[0] if len(err.args) else ""
+            cl, exc, tb = sys.exc_info()
+            line_number = traceback.extract_tb(tb)[-1][1]
+            raise Exception(f'Error in README.md line {line_number}: {error_class} {detail}\n\n{code}') from None
 
 
 def test_types():
     files = []
     for dirpath, dirnames, filenames in os.walk(
         os.path.join(os.path.dirname(__file__), '..', 'cdict'),
     ):
@@ -488,24 +549,28 @@
     stdout, stderr, _ = mypy.api.run(['--strict'] + files)
     if 'Success: no issues found' not in stdout:
         print("MyPy stdout:\n", stdout)
         print("MyPy stderr:\n", stderr)
         raise AssertionError("MyPy found type errors")
 
 
+
+
 if __name__ == "__main__":
     test_multilist()
     test_simple()
     test_list_of_dicts()
     test_dotkeys()
     test_overwriting()
     test_defaultdict()
     test_map()
+    test_apply()
     test_mut()
     test_nested_times()
     test_nested_fail()
     test_or()
     test_semiring_properties()
     test_or_distribution_property()
     test_combiners()
+    test_lazy()
     test_readme_code()
     test_types()
```

