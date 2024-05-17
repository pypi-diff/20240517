# Comparing `tmp/puppetparser-0.2.7.tar.gz` & `tmp/puppetparser-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puppetparser-0.2.7.tar", max compression
+gzip compressed data, was "puppetparser-0.2.8.tar", max compression
```

## Comparing `puppetparser-0.2.7.tar` & `puppetparser-0.2.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.7/LICENSE
--rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.7/README.md
--rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.7/puppetparser/.gitignore
--rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.7/puppetparser/__init__.py
--rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.7/puppetparser/__main__.py
--rw-r--r--   0        0        0    11729 2024-05-16 16:47:43.476658 puppetparser-0.2.7/puppetparser/model.py
--rw-r--r--   0        0        0    64997 2024-05-07 14:12:37.072439 puppetparser-0.2.7/puppetparser/parser.py
--rw-r--r--   0        0        0     1001 2024-05-16 16:48:00.472422 puppetparser-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.8/LICENSE
+-rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.8/README.md
+-rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.8/puppetparser/.gitignore
+-rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.8/puppetparser/__init__.py
+-rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.8/puppetparser/__main__.py
+-rw-r--r--   0        0        0    12018 2024-05-17 17:03:35.701533 puppetparser-0.2.8/puppetparser/model.py
+-rw-r--r--   0        0        0    65624 2024-05-17 17:10:00.096096 puppetparser-0.2.8/puppetparser/parser.py
+-rw-r--r--   0        0        0     1001 2024-05-17 10:50:47.862136 puppetparser-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.8/PKG-INFO
```

### Comparing `puppetparser-0.2.7/LICENSE` & `puppetparser-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.7/README.md` & `puppetparser-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.7/puppetparser/model.py` & `puppetparser-0.2.8/puppetparser/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from types import NoneType
-from typing import Dict, List, Tuple, Optional, Generic, TypeVar
+from typing import Dict, Sequence, List, Tuple, Optional, Generic, TypeVar
 
 T = TypeVar(
     "T",
     str,
     int,
     float,
     bool,
@@ -37,14 +37,20 @@
         return self.value == __o.value
 
     def __hash__(self) -> int:
         if self.value is None:
             return 0
 
         return self.value.__hash__()  # type: ignore
+    
+class Id(Value[str]):
+    def __init__(
+        self, line: int, col: int, end_line: int, end_col: int, value: str
+    ) -> None:
+        super().__init__(line, col, end_line, end_col, value)
 
 
 class Hash(Value[Dict[CodeElement, CodeElement]]):
     def __init__(
         self,
         line: int,
         col: int,
@@ -78,20 +84,20 @@
     def __init__(
         self,
         line: int,
         col: int,
         end_line: int,
         end_col: int,
         type: Value[str],
-        title: Value[str] | None,
+        title: Value[str] | Array | None,
         attributes: List[Attribute],
     ) -> None:
         super().__init__(line, col, end_line, end_col)
         self.type = type
-        self.title: Value[str] | None = title
+        self.title: Value[str] | Array | None = title
         self.attributes: list[Attribute] = attributes
 
 
 class ResourceDeclaration(CodeElement):
     def __init__(
         self,
         line: int,
@@ -162,19 +168,19 @@
 class ClassAsResource(CodeElement):
     def __init__(
         self,
         line: int,
         col: int,
         end_line: int,
         end_col: int,
-        title: str,
+        title: Value[str] | Array | None,
         attributes: List[Attribute],
     ) -> None:
         super().__init__(line, col, end_line, end_col)
-        self.title: str = title
+        self.title: Value[str] | Array | None = title
         self.attributes: List[Attribute] = attributes
 
 
 class Node(CodeElement):
     def __init__(
         self,
         line: int,
@@ -443,15 +449,15 @@
     def __init__(
         self,
         line: int,
         col: int,
         end_line: int,
         end_col: int,
         default: Resource | None,
-        resources: List[Resource],
+        resources: Sequence[Resource | ClassAsResource],
     ) -> None:
         super().__init__(line, col, end_line, end_col)
         self.default = default
         self.resources = resources
 
 
 class Chaining(CodeElement):
```

### Comparing `puppetparser-0.2.7/puppetparser/parser.py` & `puppetparser-0.2.8/puppetparser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,17 +414,25 @@
                 find_column(script, p.lexpos(1)),
                 p.lineno(4),
                 find_column(script, p.lexpos(4)) + 1,
                 p[3][0][0],
                 p[3][0][1],
             )
         else:
-            p[0] = list(
+            resources = list(
                 map(lambda r: ClassAsResource(r[2], r[3], r[4], r[5], r[0], r[1]), p[3])
             )
+            p[0] = ResourceExpression(
+                p.lineno(1),
+                find_column(script, p.lexpos(1)),
+                p.lineno(4),
+                find_column(script, p.lexpos(4)) + 1,
+                None,
+                resources,
+            )
 
     def p_node(p: YaccProduction):
         r"node : NODE STRING LBRACKET block RBRACKET"
         p[0] = Node(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(5),
@@ -464,20 +472,27 @@
             find_column(script, p.lexpos(5)) + 1,
             p[2],
             p[4],
         )
 
     def p_assignment(p: YaccProduction):
         r"assignment : ID EQUAL expression"
+        id = Id(
+            p.lineno(1),
+            find_column(script, p.lexpos(1)),
+            p.lineno(1),
+            find_column(script, p.lexpos(1)) + len(p[1]),
+            p[1],
+        )
         p[0] = Assignment(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p[3].end_line,
             p[3].end_col,
-            p[1],
+            id,
             p[3],
         )
 
     def p_assignment_access(p: YaccProduction):
         r"assignment : access EQUAL expression"
         p[0] = Assignment(p[1].line, p[1].col, p[3].end_line, p[3].end_col, p[1], p[3])
 
@@ -519,20 +534,27 @@
             p[3].end_col,
             p[1],
             p[3],
         )
 
     def p_assignment_type_alias(p: YaccProduction):
         r"assignment : TYPE ID_TYPE EQUAL expression"
+        id = Id(
+            p.lineno(1),
+            find_column(script, p.lexpos(1)),
+            p.lineno(2),
+            find_column(script, p.lexpos(2)) + len(p[2]),
+            p[1] + " " + p[2],
+        )
         p[0] = Assignment(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p[4].end_line,
             p[4].end_col,
-            p[1] + " " + p[2],
+            id,
             p[4],
         )
 
     def p_block(p: YaccProduction):
         r"block : statement block"
         p[0] = [p[1]] + p[2]
 
@@ -542,15 +564,15 @@
 
     def p_block_empty(p: YaccProduction):
         r"block : empty"
         p[0] = []
 
     def p_resource_id(p: YaccProduction):
         r"resource : ID LBRACKET resource_list RBRACKET"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         if not re.match(r"([a-z][a-z0-9_]*)?(::[a-z][a-z0-9_]*)*", p[1]):
@@ -970,56 +992,56 @@
 
     def p_attributes_empty(p: YaccProduction):
         r"attributes : empty"
         p[0] = []
 
     def p_attribute(p: YaccProduction):
         r"attribute : ID HASH_ROCKET expression"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = Attribute(id, p[3])
 
     def p_attribute_key(p: YaccProduction):
         r"attribute : key HASH_ROCKET expression"
         p[0] = Attribute(p[1], p[3])
 
     def p_attribute_splat(p: YaccProduction):
         r"attribute : ARITH_MUL HASH_ROCKET expression"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = Attribute(id, p[3])
 
     def p_attribute_plussign(p: YaccProduction):
         r"attribute : ID PLUSIGNMENT expression"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = Attribute(id, p[3])
 
     def p_attribute_key_plussign(p: YaccProduction):
         r"attribute : key PLUSIGNMENT expression"
         p[0] = Attribute(p[1], p[3])
 
     def p_attribute_splat_plussign(p: YaccProduction):
         r"attribute : ARITH_MUL PLUSIGNMENT expression"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = Attribute(id, p[3])
@@ -1479,15 +1501,15 @@
     def p_access(p: YaccProduction):
         r"access : expression LPARENR expressionlist RPARENR"
         p[0] = Operation(
             p[1].line,
             p[1].col,
             p.lineno(4),
             find_column(script, p.lexpos(4)) + 1,
-            (p[1], p[3]),
+            (p[1],) + tuple(p[3]),
             p[2] + p[4],
         )
         p.set_lineno(0, p.lineno(1))
 
     ## Reference
     def p_expression_reference(p: YaccProduction):
         r"expression : reference"
@@ -1521,15 +1543,15 @@
         r"statement_function : key LPAREN expressionlist RPAREN"
         p[0] = globals()[statement_functions_class[p[1].value]](
             p[1].line, p[1].col, p.lineno(4), find_column(script, p.lexpos(4)) + 1, p[3]
         )
 
     def p_function_call_prefix(p: YaccProduction):
         r"function_call : ID LPAREN expressionlist RPAREN %prec NO_LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = FunctionCall(
@@ -1540,15 +1562,15 @@
             id,
             p[3],
             None,
         )
 
     def p_function_call_type(p: YaccProduction):
         r"function_call : TYPE LPAREN expressionlist RPAREN %prec NO_LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = FunctionCall(
@@ -1559,15 +1581,15 @@
             id,
             p[3],
             None,
         )
 
     def p_function_call_id_type(p: YaccProduction):
         r"function_call : ID_TYPE LPAREN expressionlist RPAREN %prec NO_LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = FunctionCall(
@@ -1578,15 +1600,15 @@
             id,
             p[3],
             None,
         )
 
     def p_function_call_prefix_lambda(p: YaccProduction):
         r"function_call : ID LPAREN expressionlist RPAREN lambda %prec LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
         p[0] = FunctionCall(
@@ -1597,15 +1619,15 @@
             id,
             p[3],
             p[5],
         )
 
     def p_function_call_chained(p: YaccProduction):
         r"function_call : expression DOT ID %prec NO_LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(3),
             find_column(script, p.lexpos(3)),
             p.lineno(3),
             find_column(script, p.lexpos(3)) + len(p[3]),
             p[3],
         )
         p[0] = FunctionCall(
@@ -1616,15 +1638,15 @@
             id,
             [p[1]],
             None,
         )
 
     def p_function_call_chained_args(p: YaccProduction):
         r"function_call : expression DOT ID LPAREN expressionlist RPAREN %prec NO_LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(3),
             find_column(script, p.lexpos(3)),
             p.lineno(3),
             find_column(script, p.lexpos(3)) + len(p[3]),
             p[3],
         )
         p[0] = FunctionCall(
@@ -1635,28 +1657,28 @@
             id,
             [p[1]] + p[5],
             None,
         )
 
     def p_function_call_chained_lambda(p: YaccProduction):
         r"function_call : expression DOT ID lambda %prec LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(3),
             find_column(script, p.lexpos(3)),
             p.lineno(3),
             find_column(script, p.lexpos(3)) + len(p[3]),
             p[3],
         )
         p[0] = FunctionCall(
             id.line, id.col, p[4].end_line, p[4].end_col, id, [p[1]], p[4]
         )
 
     def p_function_call_chained_lambda_args(p: YaccProduction):
         r"function_call : expression DOT ID LPAREN expressionlist RPAREN lambda %prec LAMBDA"
-        id = Value(
+        id = Id(
             p.lineno(3),
             find_column(script, p.lexpos(3)),
             p.lineno(3),
             find_column(script, p.lexpos(3)) + len(p[3]),
             p[3],
         )
         p[0] = FunctionCall(
@@ -2105,40 +2127,40 @@
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(str(p[1])),
             float(p[1]),
         )
 
     def p_value_id(p: YaccProduction):
         r"value : ID"
-        p[0] = Value(
+        p[0] = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
 
     def p_value_type_id(p: YaccProduction):
         r"value : ID_TYPE"
-        p[0] = Value(
+        p[0] = Id(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
             p[1],
         )
 
     def p_value_undef(p: YaccProduction):
         r"value : UNDEF"
         p[0] = Value(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(1),
             find_column(script, p.lexpos(1)) + len(p[1]),
-            p[1],
+            None,
         )
 
     def p_value_stat_func(p: YaccProduction):
         r"value : key"
         p[0] = p[1]
 
     def p_value_regex(p: YaccProduction):
```

### Comparing `puppetparser-0.2.7/pyproject.toml` & `puppetparser-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "puppetparser"
-version = "0.2.7"
+version = "0.2.8"
 description = "A parser from Puppet to an object model"
 authors = ["Nuno Saavedra <nuno.saavedra@tecnico.ulisboa.pt>"]
 license = "GPL-3.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `puppetparser-0.2.7/PKG-INFO` & `puppetparser-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puppetparser
-Version: 0.2.7
+Version: 0.2.8
 Summary: A parser from Puppet to an object model
 License: GPL-3.0
 Keywords: puppet,parser,object model
 Author: Nuno Saavedra
 Author-email: nuno.saavedra@tecnico.ulisboa.pt
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

