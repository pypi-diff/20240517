# Comparing `tmp/vutils-testing-2.0.0.tar.gz` & `tmp/vutils_testing-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-testing-2.0.0.tar", last modified: Tue Feb 20 21:23:55 2024, max compression
+gzip compressed data, was "vutils_testing-2.0.1.tar", last modified: Fri May 17 18:37:54 2024, max compression
```

## Comparing `vutils-testing-2.0.0.tar` & `vutils_testing-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.133078 vutils-testing-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-02-20 21:23:55.133078 vutils-testing-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-20 21:23:55.133078 vutils-testing-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.129078 vutils-testing-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.129078 vutils-testing-2.0.0/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.129078 vutils-testing-2.0.0/src/vutils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/src/vutils/testing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.133078 vutils-testing-2.0.0/src/vutils_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-02-20 21:23:55.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-20 21:23:55.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 21:23:55.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 21:23:54.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-20 21:23:55.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 21:23:55.000000 vutils-testing-2.0.0/src/vutils_testing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.129078 vutils-testing-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 21:23:55.133078 vutils-testing-2.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/test_testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tests/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-20 21:23:46.000000 vutils-testing-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.900024 vutils_testing-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-17 18:37:54.900024 vutils_testing-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 18:37:54.904024 vutils_testing-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.896024 vutils_testing-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.896024 vutils_testing-2.0.1/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.900024 vutils_testing-2.0.1/src/vutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/src/vutils/testing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.900024 vutils_testing-2.0.1/src/vutils_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 18:37:54.000000 vutils_testing-2.0.1/src/vutils_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.896024 vutils_testing-2.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:37:54.900024 vutils_testing-2.0.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/test_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-17 18:37:49.000000 vutils_testing-2.0.1/tox.ini
```

### Comparing `vutils-testing-2.0.0/ChangeLog.md` & `vutils_testing-2.0.1/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## 2.0.1
+
+* Minor code cleanup
+
 ## 2.0.0
 
 * Remove obsoleted classes/functions (`vutils.testing.utils`):
   * `TypingPatcher`
   * `ClassLikeSymbol`
   * `cover_typing`
```

### Comparing `vutils-testing-2.0.0/LICENSE` & `vutils_testing-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/PKG-INFO` & `vutils_testing-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 2.0.0
+Version: 2.0.1
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-2.0.0/README.md` & `vutils_testing-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/pyproject.toml` & `vutils_testing-2.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 79
 
+[tool.pylint.main]
+ignore-patterns = ["^\\.#", "^.*\\.pyi"]
+
 [tool.pylint.design]
 min-public-methods = 0
 
 [tool.pylint.format]
 max-line-length = 79
 
 [tool.pylint."messages control"]
```

### Comparing `vutils-testing-2.0.0/setup.cfg` & `vutils_testing-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/src/vutils/testing/__init__.pyi` & `vutils_testing-2.0.1/src/vutils/testing/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Date:    2021-09-17 14:14:50 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
 
 from collections.abc import Callable
+from typing import Protocol
 from unittest.mock import Mock, _patch
 
 from typing_extensions import TypeAlias
 
 ArgsType: TypeAlias = tuple[object, ...]
 KwArgsType: TypeAlias = dict[str, object]
 ExcType: TypeAlias = type[Exception]
@@ -20,16 +21,16 @@
 ReturnsType: TypeAlias = object | Callable[[object], object] | None
 SetupFuncType: TypeAlias = Callable[[MockableType], None] | None
 BasesType: TypeAlias = type | tuple[type, ...] | None
 MembersType: TypeAlias = KwArgsType | None
 ExcSpecType: TypeAlias = ExcType | tuple[ExcType, ...]
 PatchType: TypeAlias = _patch[MockableType]
 
-class TypeType:
+class TypeType(Protocol):
     def __call__(self, *args: object, **kwargs: object) -> object: ...
 
-class FuncType:
+class FuncType(Protocol):
     def __call__(self, *args: object, **kwargs: object) -> object: ...
 
 def make_patch(
     target: object, mock: MockableType, **kwargs: object
 ) -> PatchType: ...
```

### Comparing `vutils-testing-2.0.0/src/vutils/testing/mock.py` & `vutils_testing-2.0.1/src/vutils/testing/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,21 @@
     """
     if callable(returns):
         return unittest.mock.Mock(side_effect=returns)
     return unittest.mock.Mock(return_value=returns)
 
 
 class PatchSpec:
-    """
-    Holds the patch specification.
-
-    :ivar __target: The target to be patched
-    :ivar __setupfunc: The setup function for the patch
-    :ivar __kwargs: Key-value arguments passed to :func:`unittest.mock.patch`
-    """
+    """Holds the patch specification."""
 
+    #: The target to be patched
     __target: object
+    #: The setup function for the patch
     __setupfunc: "SetupFuncType"
+    #: Key-value arguments passed to :func:`unittest.mock.patch`
     __kwargs: "KwArgsType"
 
     __slots__ = ("__target", "__setupfunc", "__kwargs")
 
     def __init__(
         self, target: object, setupfunc: "SetupFuncType", **kwargs: object
     ) -> None:
@@ -107,20 +104,17 @@
         mock: "MockableType" = kwargs.pop("new", make_mock())
         if self.__setupfunc is not None:
             self.__setupfunc(mock)
         return make_patch(self.__target, mock, **kwargs)
 
 
 class PatchingContextManager:
-    """
-    Context manager that handles the patching.
-
-    :ivar __patchers: The list of patchers
-    """
+    """Context manager that handles the patching."""
 
+    #: The list of patchers
     __patchers: "list[PatchType]"
 
     __slots__ = ("__patchers",)
 
     def __init__(self, patchers: "Iterable[PatchType]") -> None:
         """
         Initialize the context manager.
@@ -149,16 +143,14 @@
             patcher.stop()
 
 
 class PatcherFactory:
     r"""
     Factory for creating patchers.
 
-    :ivar __specs: The list of patch specifications
-
     This factory allows to create and apply the set of patches simultaneously,
     omitting the nested ``with`` statements for every patch. In the following
     example, it is demonstrated how this class can be used to test the sending
     colored text to the standard output. First, define the factory that patch
     the :mod:`colorama` and :mod:`sys` modules::
 
         import colorama
@@ -198,14 +190,15 @@
 
             assert patcher.stream.getvalue() == f"<c:red>{message}</c>\n"
 
     The patches are applied in order as their specifications were added by
     :meth:`~.PatcherFactory.add_spec`.
     """
 
+    #: The list of patch specifications
     __specs: "list[PatchSpec]"
 
     __slots__ = ("__specs",)
 
     def __init__(self) -> None:
         """Initialize the factory."""
         self.__specs = []
```

### Comparing `vutils-testing-2.0.0/src/vutils/testing/testcase.py` & `vutils_testing-2.0.1/src/vutils/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/src/vutils/testing/utils.py` & `vutils_testing-2.0.1/src/vutils/testing/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,22 +71,19 @@
         bases = (bases,)
     if members is None:
         members = {}
     return type(name, bases, members, **kwargs)
 
 
 class LazyInstanceMethod:
-    """
-    Lazy instance method.
-
-    :ivar __owner: The lazy instance proxy
-    :ivar __name: The method name
-    """
+    """Lazy instance method."""
 
+    #: The lazy instance proxy
     __owner: "LazyInstanceProxy"
+    #: The method name
     __name: str
 
     __slots__ = ("__owner", "__name")
 
     def __init__(self, owner: "LazyInstanceProxy", name: str) -> None:
         """
         Initialize the method wrapper.
@@ -106,24 +103,21 @@
         :return: the value returned by the method
         """
         inst: object = self.__owner.get_instance()
         return cast("FuncType", getattr(inst, self.__name))(*args, **kwargs)
 
 
 class LazyInstanceProxy:
-    """
-    Lazy instance proxy.
-
-    :ivar __owner: The lazy instance
-    :ivar __args: Positional arguments passed to the instance constructor
-    :ivar __kwargs: Key-value arguments passed to the instance constructor
-    """
+    """Lazy instance proxy."""
 
+    #: The lazy instance
     __owner: "LazyInstance"
+    #: Positional arguments passed to the instance constructor
     __args: "ArgsType"
+    #: Key-value arguments passed to the instance constructor
     __kwargs: "KwArgsType"
 
     __slots__ = ("__owner", "__args", "__kwargs")
 
     def __init__(
         self,
         owner: "LazyInstance",
@@ -167,20 +161,14 @@
         return cast(object, getattr(inst, name))
 
 
 class LazyInstance:
     r"""
     Support lazy initialization.
 
-    :ivar __cache: The lazy instance proxy to the instance mapping
-    :ivar __klass: The class of the instance
-    :ivar __initialize_once: When :obj:`False`,
-        :meth:`~.LazyInstance.get_instance` creates a new instance every time
-        when called
-
     Object is constructed/initialized at time when its member function is
     called. Example::
 
         foo_factory = LazyInstance(Foo, initialize_once=False)
         foo = foo_factory.create(1, bar=2)
         test(foo.quux)
 
@@ -220,16 +208,20 @@
         foo_factory = LazyInstance(Foo)
         foo = foo_factory.create()
         test(foo.greet, mystream)
 
     now, ``Hello!\n`` is written to ``mystream`` as expected.
     """
 
+    #: The lazy instance proxy to the instance mapping
     __cache: "dict[LazyInstanceProxy, object]"
+    #: The class of the instance
     __klass: "TypeType"
+    #: When :obj:`False`, :meth:`~.LazyInstance.get_instance` creates a new
+    #: instance every time when called
     __initialize_once: bool
 
     __slots__ = ("__cache", "__klass", "__initialize_once")
 
     def __init__(
         self, klass: "TypeType", initialize_once: bool = False
     ) -> None:
@@ -290,19 +282,14 @@
         return LazyInstanceProxy(self, args, kwargs)
 
 
 class AssertRaises:
     """
     Wrapper that asserts that callable raises.
 
-    :ivar __testcase: The test case
-    :ivar __func: The callable object to be tested
-    :ivar __raises: Expected exceptions
-    :ivar __exception: The caught exception
-
     Consider there are two functions ``func1`` and ``func2`` that are very
     similar to each other except ``func2`` raises an exception. Since their
     similarity, the test case defines a function ``run_and_verify(func)`` which
     runs them and test their results and side-effects. However, since ``func2``
     raises an exception, ``run_and_verify(func2)`` fails. To deal with such a
     situation, :class:`.AssertRaises` can be used::
 
@@ -315,17 +302,21 @@
                 self.run_and_verify(func1)
                 # Does not fail, exception is caught and stored for later use
                 self.run_and_verify(wfunc2)
                 # Analyze caught exception
                 self.assertEqual(wfunc2.get_exception().detail, "foo")
     """
 
+    #: The test case
     __testcase: "TestCase"
+    #: The callable object to be tested
     __func: "FuncType"
+    #: Expected exceptions
     __raises: "ExcSpecType"
+    #: The caught exception
     __exception: "Exception | None"
 
     __slots__ = ("__testcase", "__func", "__raises", "__exception")
 
     def __init__(
         self, testcase: "TestCase", func: "FuncType", raises: "ExcSpecType"
     ) -> None:
```

### Comparing `vutils-testing-2.0.0/src/vutils_testing.egg-info/PKG-INFO` & `vutils_testing-2.0.1/src/vutils_testing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 2.0.0
+Version: 2.0.1
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-2.0.0/src/vutils_testing.egg-info/SOURCES.txt` & `vutils_testing-2.0.1/src/vutils_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/tests/unit/test_mock.py` & `vutils_testing-2.0.1/tests/unit/test_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,35 +100,32 @@
         """
         func = make_callable(lambda x: x + 1)
 
         self.assertEqual(func(3), 4)
 
 
 class PatchXTestCaseBase(TestCase):
-    """
-    Base class for |PatchSpecTestCase| and |PatcherFactoryTestCase|.
-
-    :ivar mock: The :class:`unittest.mock.Mock` object used as an argument
-    :ivar patch: The mocked :func:`unittest.mock.patch`
-    :ivar patcher: The patcher
-    :ivar target: The target to be patched
-    """
+    """Base class for |PatchSpecTestCase| and |PatcherFactoryTestCase|."""
 
     __slots__ = ("mock", "patch", "patcher", "target")
 
     def setUp(self):
         """Set up the test."""
+        #: The :class:`unittest.mock.Mock` object used as an argument
         self.mock = make_mock()
         mock_mock = make_callable(lambda *x: self.mock)
+        #: The mocked :func:`unittest.mock.patch`
         self.patch = make_callable(lambda *x, **y: make_mock())
+        #: The patcher
         self.patcher = (
             PatcherFactory()
             .add_spec("vutils.testing.mock.make_patch", new=self.patch)
             .add_spec("unittest.mock.Mock", new=mock_mock)
         )
+        #: The target to be patched
         self.target = "__main__.print"
 
 
 class PatchSpecTestCase(PatchXTestCaseBase):
     """Test case for |PatchSpec|."""
 
     __slots__ = ()
```

### Comparing `vutils-testing-2.0.0/tests/unit/test_testcase.py` & `vutils_testing-2.0.1/tests/unit/test_testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/tests/unit/test_utils.py` & `vutils_testing-2.0.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/tests/unit/test_version.py` & `vutils_testing-2.0.1/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-2.0.0/tests/unit/utils.py` & `vutils_testing-2.0.1/tests/unit/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,82 +2,70 @@
 # File:    ./tests/unit/utils.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2021-09-22 23:46:47 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
-"""
-Unit tests utilities.
-
-:const FOO_CONSTANT: The auxiliary constant used in tests
-"""
+"""Unit tests utilities."""
 
 import io
 import sys
 
 from vutils.testing.mock import PatcherFactory
 
+#: The auxiliary constant used in tests
 FOO_CONSTANT = 42
 
 
 class FooError(Exception):
-    """
-    Dummy exception.
-
-    :ivar detail: The error detail
-    """
+    """Dummy exception."""
 
     __slots__ = ("detail",)
 
     def __init__(self, detail):
         """
         Initialize the exception object.
 
         :param detail: The error detail
         """
         Exception.__init__(self, detail)
+        #: The error detail
         self.detail = detail
 
 
 class StderrPatcher(PatcherFactory):
-    """
-    :mod:`sys.stderr` patcher.
-
-    :ivar stream: The new error stream
-    """
+    """:mod:`sys.stderr` patcher."""
 
     __slots__ = ("stream",)
 
     def setup(self):
         """Set up the patcher."""
+        #: The new error stream
         self.stream = io.StringIO()
         self.add_spec("sys.stderr", new=self.stream)
 
 
 class StderrWriter:
-    """
-    Dummy standard error output writer.
-
-    :ivar stream: The error stream to write
-    :ivar code: The error code
-    :ivar label: The label of an error message
-    """
+    """Dummy standard error output writer."""
 
     __slots__ = ("stream", "code", "label")
 
     def __init__(self, code, label=""):
         """
         Initialize the writer.
 
         :param code: The code
         :param label: The label
         """
+        #: The error stream to write
         self.stream = sys.stderr
+        #: The error code
         self.code = code
+        #: The label of an error message
         self.label = label
 
     @staticmethod
     def format(code, label, text):
         """
         Format the message.
```

### Comparing `vutils-testing-2.0.0/tox.ini` & `vutils_testing-2.0.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
+    idna >=3.7
     pip-audit
     pytest
     pytest-cov
     coveralls
 allowlist_externals =
     bash
     rm
@@ -53,14 +54,15 @@
 basepython = {[linters]basepython}
 skipsdist = {[linters]skipsdist}
 skip_install = {[linters]skip_install}
 setenv = {[linters]setenv}
 description =
     {envname}: Run general checks
 deps =
+    idna >=3.7
     pip-audit
     check-manifest
     twine
 commands =
     python -m pip_audit --progress-spinner off
     bash -c 'python -m pip_audit --progress-spinner off -r <(pip freeze --all)'
     check-manifest .
```

