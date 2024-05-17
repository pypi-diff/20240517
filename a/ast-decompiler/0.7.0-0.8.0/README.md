# Comparing `tmp/ast_decompiler-0.7.0.tar.gz` & `tmp/ast_decompiler-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_decompiler-0.7.0.tar", last modified: Tue Oct  4 00:13:09 2022, max compression
+gzip compressed data, was "ast_decompiler-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ast_decompiler-0.7.0.tar` & `ast_decompiler-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    10173 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/LICENSE
--rw-r--r--   0        0        0      303 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/README.rst
--rw-r--r--   0        0        0      115 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/ast_decompiler/__init__.py
--rw-r--r--   0        0        0      899 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/ast_decompiler/check.py
--rw-r--r--   0        0        0    38589 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/ast_decompiler/decompiler.py
--rw-r--r--   0        0        0        0 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/ast_decompiler/py.typed
--rw-r--r--   0        0        0     1753 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7845 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_basic.py
--rw-r--r--   0        0        0      350 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_indentation.py
--rw-r--r--   0        0        0     2878 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_line_length.py
--rw-r--r--   0        0        0     1479 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_literal.py
--rw-r--r--   0        0        0      785 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_patma.py
--rw-r--r--   0        0        0     2054 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_precedence.py
--rw-r--r--   0        0        0     5852 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/test_py3_syntax.py
--rw-r--r--   0        0        0     2387 2022-10-04 00:13:01.735651 ast_decompiler-0.7.0/tests/tests.py
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 ast_decompiler-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/LICENSE
+-rw-r--r--   0        0        0      525 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/README.rst
+-rw-r--r--   0        0        0      116 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/ast_decompiler/__init__.py
+-rw-r--r--   0        0        0      899 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/ast_decompiler/check.py
+-rw-r--r--   0        0        0    39920 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/ast_decompiler/decompiler.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/ast_decompiler/py.typed
+-rw-r--r--   0        0        0     1816 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7102 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/tests/test_basic.py
+-rw-r--r--   0        0        0      350 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/tests/test_indentation.py
+-rw-r--r--   0        0        0     2878 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/tests/test_line_length.py
+-rw-r--r--   0        0        0      992 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/tests/test_literal.py
+-rw-r--r--   0        0        0      785 2024-05-17 11:24:40.473753 ast_decompiler-0.8.0/tests/test_patma.py
+-rw-r--r--   0        0        0      456 2024-05-17 11:24:40.477753 ast_decompiler-0.8.0/tests/test_pep695.py
+-rw-r--r--   0        0        0     1823 2024-05-17 11:24:40.477753 ast_decompiler-0.8.0/tests/test_precedence.py
+-rw-r--r--   0        0        0     5031 2024-05-17 11:24:40.477753 ast_decompiler-0.8.0/tests/test_py3_syntax.py
+-rw-r--r--   0        0        0     2387 2024-05-17 11:24:40.477753 ast_decompiler-0.8.0/tests/tests.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 ast_decompiler-0.8.0/PKG-INFO
```

### Comparing `ast_decompiler-0.7.0/LICENSE` & `ast_decompiler-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_decompiler-0.7.0/ast_decompiler/check.py` & `ast_decompiler-0.8.0/ast_decompiler/check.py`

 * *Files identical despite different names*

### Comparing `ast_decompiler-0.7.0/ast_decompiler/decompiler.py` & `ast_decompiler-0.8.0/ast_decompiler/decompiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 
 Implementation of the decompiler class.
 
 """
+
 import ast
 import cmath
 from contextlib import contextmanager
 import math
 import sys
 from typing import Any, Dict, Generator, Iterable, Optional, Sequence, Type, Union
 
@@ -310,15 +311,20 @@
             self.write("@")
             self.visit(decorator)
             self.write_newline()
 
         self.write_indentation()
         if isinstance(node, ast.AsyncFunctionDef):
             self.write("async ")
-        self.write(f"def {node.name}(")
+        self.write(f"def {node.name}")
+        if sys.version_info >= (3, 12) and node.type_params:
+            self.write("[")
+            self.write_expression_list(node.type_params)
+            self.write("]")
+        self.write("(")
         self.visit(node.args)
         self.write(")")
         if node.returns is not None:
             self.write(" -> ")
             self.visit(node.returns)
         self.write(":")
         self.write_newline()
@@ -333,15 +339,20 @@
         for decorator in node.decorator_list:
             self.write_indentation()
             self.write("@")
             self.visit(decorator)
             self.write_newline()
 
         self.write_indentation()
-        self.write(f"class {node.name}(")
+        self.write(f"class {node.name}")
+        if sys.version_info >= (3, 12) and node.type_params:
+            self.write("[")
+            self.write_expression_list(node.type_params)
+            self.write("]")
+        self.write("(")
         exprs = node.bases + getattr(node, "keywords", [])
         self.write_expression_list(exprs, need_parens=False)
         self.write("):")
         self.write_newline()
         self.write_suite(node.body)
 
     def visit_For(self, node: Union[ast.For, ast.AsyncFor]) -> None:
@@ -460,14 +471,51 @@
         self.visit(node.target)
         self.write(" ")
         self.visit(node.op)
         self.write("= ")
         self.visit(node.value)
         self.write_newline()
 
+    if sys.version_info >= (3, 12):
+
+        def visit_TypeAlias(self, node: ast.TypeAlias) -> None:
+            self.write_indentation()
+            self.write("type ")
+            self.visit(node.name)
+            if node.type_params:
+                self.write("[")
+                self.write_expression_list(node.type_params)
+                self.write("]")
+            self.write(" = ")
+            self.visit(node.value)
+            self.write_newline()
+
+        def visit_TypeVar(self, node: ast.TypeVar) -> None:
+            self.write(node.name)
+            if node.bound:
+                self.write(": ")
+                self.visit(node.bound)
+            if sys.version_info >= (3, 13) and node.default_value:
+                self.write(" = ")
+                self.visit(node.default_value)
+
+        def visit_TypeVarTuple(self, node: ast.TypeVarTuple) -> None:
+            self.write("*")
+            self.write(node.name)
+            if sys.version_info >= (3, 13) and node.default_value:
+                self.write(" = ")
+                self.visit(node.default_value)
+
+        def visit_ParamSpec(self, node: ast.ParamSpec) -> None:
+            self.write("**")
+            self.write(node.name)
+            if sys.version_info >= (3, 13) and node.default_value:
+                self.write(" = ")
+                self.visit(node.default_value)
+
     def visit_AnnAssign(self, node: ast.AnnAssign) -> None:
         self.write_indentation()
         if not node.simple:
             self.write("(")
         self.visit(node.target)
         if not node.simple:
             self.write(")")
@@ -773,17 +821,14 @@
 
     def visit_KeywordArg(self, node: KeywordArg) -> None:
         self.visit(node.arg)
         if node.value is not None:
             self.write("=")
             self.visit(node.value)
 
-    def visit_Num(self, node: ast.Num) -> None:
-        self.write_number(node.n)
-
     def write_number(self, number: Union[int, float, complex]) -> None:
         should_parenthesize = (
             isinstance(number, int)
             and number >= 0
             and isinstance(self.get_parent_node(), ast.Attribute)
         )
         if not should_parenthesize:
@@ -802,22 +847,21 @@
             elif isinstance(number, (int, float)) and number < 0:
                 # needed for precedence to work correctly
                 me = self.node_stack.pop()
                 if isinstance(number, int):
                     val = str(-number)
                 else:
                     val = repr(type(number)(-number))  # - of long may be int
-                self.visit(ast.UnaryOp(op=ast.USub(), operand=ast.Name(id=val)))
+                self.visit(
+                    ast.UnaryOp(op=ast.USub(), operand=ast.Name(id=val, ctx=ast.Load()))
+                )
                 self.node_stack.append(me)
             else:
                 self.write(repr(number))
 
-    def visit_Str(self, node: ast.Str) -> None:
-        self.write_string(node.s, kind=None)
-
     def write_string(self, string_value: str, kind: Optional[str] = None) -> None:
         if kind is not None:
             self.write(kind)
         if isinstance(self.get_parent_node(), ast.Expr) and '"""' not in string_value:
             self.write('"""')
             s = string_value.encode("unicode-escape").decode("ascii")
             s = s.replace("\\n", "\n")
@@ -845,53 +889,47 @@
             add_space = isinstance(
                 node.value, (ast.Set, ast.Dict, ast.SetComp, ast.DictComp)
             )
             if add_space:
                 self.write(" ")
             self.visit(node.value)
             if node.conversion != -1:
-                # https://github.com/python/typeshed/pull/7810
-                # static analysis: ignore[incompatible_argument]
                 self.write(f"!{chr(node.conversion)}")
             if node.format_spec is not None:
                 self.write(":")
                 if isinstance(node.format_spec, ast.JoinedStr):
                     self.visit(node.format_spec)
-                elif isinstance(node.format_spec, ast.Str):
-                    self.write(node.format_spec.s)
+                elif isinstance(node.format_spec, ast.Constant) and isinstance(
+                    node.format_spec.value, str
+                ):
+                    self.write(node.format_spec.value)
                 else:
                     raise TypeError(
                         f"format spec must be a string, not {node.format_spec}"
                     )
             if add_space:
                 self.write(" ")
             self.write("}")
 
     def visit_JoinedStr(self, node: ast.JoinedStr) -> None:
         has_parent = isinstance(self.get_parent_node(), ast.FormattedValue)
         with self.f_literalise_if(not has_parent):
             for value in node.values:
-                if isinstance(value, ast.Str):
+                if isinstance(value, ast.Constant) and isinstance(value.value, str):
                     # always escape '
                     self.write(
-                        value.s.encode("unicode-escape")
+                        value.value.encode("unicode-escape")
                         .decode("ascii")
                         .replace("'", r"\'")
                         .replace("{", "{{")
                         .replace("}", "}}")
                     )
                 else:
                     self.visit(value)
 
-    def visit_Bytes(self, node: ast.Bytes) -> None:
-        self.write(repr(node.s))
-
-    def visit_NameConstant(self, node: ast.NameConstant) -> None:
-        self.write(repr(node.value))
-
     def visit_Constant(self, node: ast.Constant) -> None:
         if isinstance(node.value, str):
             kind = node.kind
         else:
             kind = None
         self.write_constant(node.value, kind)
 
@@ -965,17 +1003,14 @@
                 else:
                     self.write_expression_list(
                         node.elts, need_parens=allow_parens and not should_parenthesize
                     )
 
     # slice
 
-    def visit_Ellipsis(self, node: ast.Ellipsis) -> None:
-        self.write("...")
-
     def visit_Slice(self, node: ast.Slice) -> None:
         if node.lower:
             self.visit(node.lower)
         self.write(":")
         if node.upper:
             self.visit(node.upper)
         if node.step:
@@ -996,19 +1031,17 @@
 
     # operators
     for op, string in _OP_TO_STR.items():
         exec(f"def visit_{op.__name__}(self, node): self.write({string!r})")
 
     # Other types
 
-    visit_Load = (
-        visit_Store
-    ) = (
-        visit_Del
-    ) = visit_AugLoad = visit_AugStore = visit_Param = lambda self, node: None
+    visit_Load = visit_Store = visit_Del = visit_AugLoad = visit_AugStore = (
+        visit_Param
+    ) = lambda self, node: None
 
     def visit_comprehension(self, node: ast.comprehension) -> None:
         if node.is_async:
             self.write("async ")
         self.write("for ")
         self.visit(node.target)
         self.write(" in ")
@@ -1032,17 +1065,17 @@
                 self.write(node.name)
         self.write(":")
         self.write_newline()
         self.write_suite(node.body)
 
     def visit_arguments(self, node: ast.arguments) -> None:
         args = []
-        if sys.version_info >= (3, 8) and node.posonlyargs:
+        if node.posonlyargs:
             args += node.posonlyargs
-            args.append(ast.Name(id="/"))
+            args.append(ast.Name(id="/", ctx=ast.Load()))
 
         num_defaults = len(node.defaults)
         if num_defaults:
             args += node.args[:-num_defaults]
             default_args = zip(node.args[-num_defaults:], node.defaults)
         else:
             args += list(node.args)
```

### Comparing `ast_decompiler-0.7.0/pyproject.toml` & `ast_decompiler-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "ast_decompiler"
-version = "0.7.0"
+version = "0.8.0"
 description = "Python module to decompile AST to Python code"
 readme = "README.rst"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 urls.Home = "https://github.com/JelleZijlstra/ast_decompiler"
 license.file = "LICENSE"
 keywords = ["ast", "decompiler"]
 # Classifiers list: https://pypi.org/classifiers/
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Python Software Foundation License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Topic :: Software Development",
 ]
 
 # Project metadata -- authors. Flit stores this as a list of dicts, so it can't
 # be inline above.
 [[project.authors]]
 name = "Jelle Zijlstra"
@@ -54,7 +54,12 @@
 suggested_return_type = true
 incompatible_override = true
 
 [tool.black]
 target_version = ['py36']
 skip-magic-trailing-comma = true
 preview = true
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
```

### Comparing `ast_decompiler-0.7.0/tests/test_basic.py` & `ast_decompiler-0.8.0/tests/test_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ast
 from ast_decompiler import decompile
-from .tests import assert_decompiles, check, only_on_version
+from .tests import assert_decompiles, check
 
 
 def test_non_module() -> None:
-    assert "3" == decompile(ast.Num(n=3))
+    assert "3" == decompile(ast.Constant(value=3))
     assert "1 + 1" == decompile(
-        ast.BinOp(op=ast.Add(), left=ast.Num(n=1), right=ast.Num(n=1))
+        ast.BinOp(op=ast.Add(), left=ast.Constant(value=1), right=ast.Constant(value=1))
     )
 
 
 def test_FunctionDef() -> None:
     check(
         """
 @foo
@@ -57,24 +57,14 @@
 
 
 def test_AugAssign() -> None:
     check("x += 3")
     check("y *= 5")
 
 
-@only_on_version(2)
-def test_Print() -> None:
-    check("print")
-    check("print >>sys.stderr")
-    check("print a, b")
-    check("print a, b,")
-    check("print a,")
-    check("print >>sys.stderr, a, b,")
-
-
 def test_For() -> None:
     check("for x in y: pass")
     check(
         """
 for x in y:
     pass
 else:
@@ -133,20 +123,14 @@
 
 
 def test_Raise() -> None:
     check("raise")
     check("raise e")
 
 
-@only_on_version(2)
-def test_Raise_old_syntax() -> None:
-    check("raise TypeError, e")
-    check("raise TypeError, e, tb")
-
-
 def test_TryExcept() -> None:
     check(
         """
 try:
     1/0
 except:
     pass
@@ -214,21 +198,14 @@
 def test_ImportFrom() -> None:
     check("from . import foo")
     check("from .foo import bar")
     check("from foo import bar")
     check("from ....... import bar as foo")
 
 
-@only_on_version(2)
-def test_Exec() -> None:
-    check('exec "hello"')
-    check('exec "hello" in {}')
-    check('exec "hello" in {}, {}')
-
-
 def test_Global() -> None:
     check("global a")
     check("global a, b")
 
 
 def test_Expr() -> None:
     check("call()")
@@ -322,38 +299,28 @@
 
 def test_Yield() -> None:
     check("def f(): yield")
     check("def f(): yield 3")
     check("def f(): x = yield 3")
 
 
-@only_on_version(2)
-def test_Yield_in_print() -> None:
-    check("def f(): print (yield 4)")
-
-
 def test_Compare() -> None:
     check("x < y")
     check("x > y < z")
     check("x == y > z")
 
 
 def test_Call() -> None:
     check("f()")
     check("f(1)")
     check("f(1, x=2)")
     check("f(*args, **kwargs)")
     check("f(foo, *args, **kwargs)")
 
 
-@only_on_version(2)
-def test_Repr() -> None:
-    check("`foo`")
-
-
 def test_Num() -> None:
     check("1")
     check("1.0")
     check("1.0e10")
     check("1+2j")
     check("-2147483648")  # previously had a bug that made us add L
     check("2147483648")
@@ -367,21 +334,14 @@
     assert_decompiles("3j", "3j\n")
     assert_decompiles("-3j", "-3j\n")
     assert_decompiles("1 + 3j", "1 + 3j\n")
     assert_decompiles("-1-42j", "-1 - 42j\n")
     assert_decompiles("-(1-42j)", "-(1 - 42j)\n")
 
 
-@only_on_version(2)
-def test_longs() -> None:
-    check("-2147483648L")
-    check("2147483648L")
-    check("1L")
-
-
 def test_Str() -> None:
     check('"foo"')
     check('u"foo"')
     check('"foo\\"bar"')
     check(
         """from __future__ import unicode_literals
 b'foo'
```

### Comparing `ast_decompiler-0.7.0/tests/test_line_length.py` & `ast_decompiler-0.8.0/tests/test_line_length.py`

 * *Files identical despite different names*

### Comparing `ast_decompiler-0.7.0/tests/test_literal.py` & `ast_decompiler-0.8.0/tests/test_literal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,19 @@
-from .tests import assert_decompiles, only_on_version
+from .tests import assert_decompiles
 
 
 def test_With() -> None:
     assert_decompiles(
         "with x as y, a as b: pass",
         """with x as y, a as b:
     pass
 """,
     )
 
 
-@only_on_version(2)
-def test_With_collapsed() -> None:
-    assert_decompiles(
-        """
-with x as y:
-    with a as b:
-        pass
-""",
-        """with x as y, a as b:
-    pass
-""",
-    )
-
-
 def test_TryFinally() -> None:
     assert_decompiles(
         """
 try:
     1 / 0
 except Exception as e:
     pass
@@ -44,36 +30,14 @@
     z = 3
 finally:
     z = 4
 """,
     )
 
 
-@only_on_version(2)
-def test_TryFinally_collapsed() -> None:
-    assert_decompiles(
-        """
-try:
-    try:
-        1 / 0
-    except Exception as e:
-        pass
-finally:
-    z = 4
-""",
-        """try:
-    1 / 0
-except Exception as e:
-    pass
-finally:
-    z = 4
-""",
-    )
-
-
 def test_If() -> None:
     assert_decompiles(
         """
 if x: pass
 else:
     if y: pass
     else: pass
```

### Comparing `ast_decompiler-0.7.0/tests/test_patma.py` & `ast_decompiler-0.8.0/tests/test_patma.py`

 * *Files identical despite different names*

### Comparing `ast_decompiler-0.7.0/tests/test_py3_syntax.py` & `ast_decompiler-0.8.0/tests/test_py3_syntax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from .tests import check, skip_before, skip_after
+from .tests import check
 
 
-@skip_before((3, 5))
 def test_MatMult() -> None:
     check("a @ b")
     check("(a * b) @ c")
     check("a * (b @ c)")
     check("a + (b @ c)")
 
 
-@skip_before((3, 5))
 def test_AsyncFunctionDef() -> None:
     check(
         """
 async def f(a, b):
     pass
 """
     )
 
 
-@skip_before((3, 6))
 def test_async_gen() -> None:
     check(
         """
 async def f():
     yield
 """
     )
 
 
-@skip_before((3, 6))
 def test_async_comprehensions() -> None:
     check(
         """
 async def f(lst):
     return [await x for x in lst]
 """
     )
@@ -44,26 +40,23 @@
     b = {x async for x in lst}
     c = {x: x async for x in lst}
     d = (x async for x in lst)
 """
     )
 
 
-@skip_before((3, 0))
-def test_annotations() -> None:
-    # TODO test precedence
+def test_function_annotations() -> None:
     check(
         """
 def f(a: int, b: str) -> float:
     pass
 """
     )
 
 
-@skip_before((3, 0))
 def test_class_keywords() -> None:
     check(
         """
 class Foo(a=3):
     pass
 """
     )
@@ -71,31 +64,28 @@
         """
 class WithMeta(metaclass=type):
     pass
 """
     )
 
 
-@skip_before((3, 0))
 def test_annotations() -> None:
     check("def f(a: int, b: int = 0, *args: int, c: int, **kwargs: int): pass")
 
 
-@skip_before((3, 5))
 def test_AsyncFor() -> None:
     check(
         """
 async def f(y):
     async for x in y:
         pass
 """
     )
 
 
-@skip_before((3, 0))
 def test_py3_with() -> None:
     check(
         """
 with a as b:
     pass
 """
     )
@@ -110,35 +100,32 @@
 with a as b:
     with c as d:
         pass
 """
     )
 
 
-@skip_before((3, 5))
 def test_async_with() -> None:
     check(
         """
 async def f(a):
     async with a as b:
         pass
 """
     )
 
 
-@skip_before((3, 0))
 def test_raise_with_cause() -> None:
     check(
         """
 raise e from ee
 """
     )
 
 
-@skip_before((3, 0))
 def test_Nonlocal() -> None:
     check(
         """
 def f(x):
     nonlocal y
 """
     )
@@ -146,15 +133,14 @@
         """
 def f(x):
     nonlocal y, z
 """
     )
 
 
-@skip_before((3, 5))
 def test_Await() -> None:
     check(
         """
 async def f(x):
     await x
 """
     )
@@ -180,24 +166,22 @@
         """
 async def f(x):
     return 3, (await x)
 """
     )
 
 
-@skip_before((3, 0))
 def test_YieldFrom() -> None:
     check("yield from x")
     check("1 + (yield from x)")
     check("x = yield from x")
     check("x += yield from x")
     check("return 3, (yield from x)")
 
 
-@skip_before((3, 6))
 def test_FormattedValue() -> None:
     check('f"a"')
     check('f"{b}"')
     check('f"{b}a"')
     check('f"{b!r}"')
     check('f"{b:a}"')
     check('f"{b!r:a}"')
@@ -215,40 +199,35 @@
     check(r"f'{a}\t'")
     check("f'{a}é'")
     check('f"{{"')
     check('f"}}"')
     check('f"{{{a}"')
 
 
-@skip_before((3, 0))
 def test_Bytes() -> None:
     check('b"a"')
 
 
-@skip_before((3, 0))
 def test_NameConstant() -> None:
     check("True")
 
 
-@skip_before((3, 0))
 def test_Starred() -> None:
     check("a, *b = 3")
     check("[a, *b]")
 
 
-@skip_before((3, 0))
 def test_kwonlyargs() -> None:
     check("def f(a, *, b): pass")
     check("def f(a, *args, b): pass")
     check("def f(a, *, b=3): pass")
     check("def f(a, *args, b=3): pass")
     check("def f(a, *args, b=3, **kwargs): pass")
 
 
-@skip_before((3, 6))
 def test_annassign() -> None:
     check("a: int")
     check("a: int = 3")
     check("(a): int")
     check(
         """
 class A:
@@ -259,15 +238,14 @@
         """
 def f():
     a: int
 """
     )
 
 
-@skip_before((3, 7))
 def test_future_annotations() -> None:
     # This doesn't really affect ast_decompiler because the __future__
     # import doesn't change the AST.
     check(
         """
 from __future__ import annotations
 
@@ -275,33 +253,19 @@
     pass
 
 y: float
 """
     )
 
 
-@skip_after((3, 6))
-def test_async_varname() -> None:
-    check("import async")
-    check("await = 3")
-    check(
-        """
-def async(async, await=3):
-    return async + await
-"""
-    )
-
-
-@skip_before((3, 7))
 def test_async_await_in_fstring() -> None:
     check("f'{await x}'")
     check("f'{[x async for x in y]}'")
 
 
-@skip_before((3, 7))
 def test_too_many_args() -> None:
     args = ", ".join(f"x{i}" for i in range(300))
     check(
         """
 def f({}):
     pass
 
@@ -321,58 +285,53 @@
             whatever
         finally:
             continue
 """
     )
 
 
-@skip_before((3, 4))
 def test_unpacking() -> None:
     check(
         """
 def parse(family):
     lastname, *members = family.split()
     return (lastname.upper(), *members)
 """
     )
 
 
-@skip_before((3, 8))
 def test_unparenthesized_unpacking() -> None:
     check(
         """
 def parse(family):
     lastname, *members = family.split()
     return lastname.upper(), *members
 """
     )
 
 
-@skip_before((3, 8))
 def test_assignment_expression() -> None:
     # Some of these can be used unparenthesized in 3.10+ but we don't bother.
     check(
         """
 if (x := 3):
     pass
 {(y := 4)}
 {(z := 5) for a in b}
 lst[(alpha := 3)]
 lst[(beta := 4):(gamma := 5)]
 """
     )
 
 
-@skip_before((3, 8))
 def test_positional_only() -> None:
     check(
         """
 def f(x, /):
     pass
 """
     )
 
 
-@skip_before((3, 8))
 def test_fstring_debug_specifier() -> None:
     check("f'{user=} {member_since=}'")
     check("f'{user=!s}  {delta.days=:,d}'")
```

### Comparing `ast_decompiler-0.7.0/tests/tests.py` & `ast_decompiler-0.8.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `ast_decompiler-0.7.0/PKG-INFO` & `ast_decompiler-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ast_decompiler
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python module to decompile AST to Python code
 Keywords: ast,decompiler
 Author-email: Jelle Zijlstra <jelle.zijlstra@gmail.com>
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development
 Project-URL: Home, https://github.com/JelleZijlstra/ast_decompiler
 
 **************
 ast_decompiler
 **************
 
@@ -31,9 +31,18 @@
 
     >> import ast
     >> from ast_decompiler import decompile
 
     >> decompile(ast.parse('(a + b) * c'))
     (a + b) * c
 
-This module supports Python 3.6 through 3.11.
+This module supports Python 3.8 through 3.13.
+
+====================
+Tests and formatting
+====================
+
+To run the tests, install ``pytest`` in a virtual environment. Then, either use
+``tox``, or simply run ``pytest tests/``.
+
+The code is formatted with Black.
```

