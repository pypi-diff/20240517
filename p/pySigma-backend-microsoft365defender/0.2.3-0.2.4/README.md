# Comparing `tmp/pysigma_backend_microsoft365defender-0.2.3.tar.gz` & `tmp/pysigma_backend_microsoft365defender-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_microsoft365defender-0.2.3.tar", max compression
+gzip compressed data, was "pysigma_backend_microsoft365defender-0.2.4.tar", max compression
```

## Comparing `pysigma_backend_microsoft365defender-0.2.3.tar` & `pysigma_backend_microsoft365defender-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7653 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/LICENSE
--rw-r--r--   0        0        0      652 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      407 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/sigma/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    13077 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/sigma/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      315 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/sigma/pipelines/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    33264 2024-01-23 18:07:44.420580 pysigma_backend_microsoft365defender-0.2.3/sigma/pipelines/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     7653 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/LICENSE
+-rw-r--r--   0        0        0      652 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      407 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/sigma/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    14140 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/sigma/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      315 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/sigma/pipelines/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    33264 2024-02-18 23:55:08.352193 pysigma_backend_microsoft365defender-0.2.4/sigma/pipelines/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.2.4/PKG-INFO
```

### Comparing `pysigma_backend_microsoft365defender-0.2.3/LICENSE` & `pysigma_backend_microsoft365defender-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.2.3/pyproject.toml` & `pysigma_backend_microsoft365defender-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-microsoft365defender"
-version = "0.2.3"
+version = "0.2.4"
 description = "pySigma Microsoft 365 Defender backend"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/AttackIQ/pySigma-backend-microsoft365defender"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_microsoft365defender-0.2.3/sigma/backends/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.2.4/sigma/backends/microsoft365defender/microsoft365defender.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import re
+from typing import ClassVar, Dict, Tuple, Pattern, Any, Union, Optional
+
+from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT, ConditionFieldEqualsValueExpression
+from sigma.conversion.base import TextQueryBackend
+from sigma.conversion.deferred import DeferredQueryExpression
 from sigma.conversion.state import ConversionState
 from sigma.processing.pipeline import ProcessingPipeline
 from sigma.rule import SigmaRule
-from sigma.conversion.base import TextQueryBackend
-from sigma.conversion.deferred import DeferredQueryExpression
-from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT, ConditionFieldEqualsValueExpression
-from sigma.types import SigmaCompareExpression, SigmaString
+from sigma.types import SigmaCompareExpression, SigmaString, SpecialChars
+
 from sigma.pipelines.microsoft365defender import microsoft_365_defender_pipeline
-import sigma
-import re
-from typing import ClassVar, Dict, Tuple, Pattern, Any, Union, Optional
 
 
 class Microsoft365DefenderBackend(TextQueryBackend):
     """Microsoft 365 Defender KQL Backend. Automatically applied the microsoft_365_defender_pipeline from
     sigma.pipelines.microsoft365defender."""
 
     # The backend generates grouping if required
@@ -63,16 +64,15 @@
         False: "false",
     }
 
     # String matching operators. if none is appropriate eq_token is used.
     startswith_expression: ClassVar[str] = "{field} startswith {value}"
     endswith_expression: ClassVar[str] = "{field} endswith {value}"
     contains_expression: ClassVar[str] = "{field} contains {value}"
-    wildcard_match_expression: ClassVar[
-        str] = "match"  # Special expression if wildcards can't be matched with the eq_token operator
+    wildcard_match_expression: ClassVar[str] = None  # Special expression if wildcards can't be matched with the eq_token operator
 
     # Regular expressions
     re_expression: ClassVar[
         str] = "{field} matches regex \"{regex}\""  # Regular expression query as format string with placeholders {field} and {regex}
     re_escape_char: ClassVar[str] = "\\"  # Character used for escaping in regular expressions
     re_escape: ClassVar[Tuple[str]] = ()  # List of strings that are escaped
     re_escape_escape_char: bool = True  # If True, the escape character is also escaped
@@ -182,15 +182,26 @@
                 op=op1,
                 list=list_nonwildcard
             )
         wildcard_exprs_list = []
         if list_wildcards:
             for arg in list_wildcards:
                 new_cond = ConditionFieldEqualsValueExpression(field=field, value=arg)
-                expr = self.convert_condition_field_eq_val_str(new_cond, state)
+                if arg[1:-1].contains_special():  # Wildcard in string, not at start or end.
+                    # We need to get rid of all wildcards, and create a 'and contains' for each element in the list
+                    expr = f'{self.token_separator}{self.and_token}{self.token_separator}'.join(
+                        [self.contains_expression.format(
+                            field=field,
+                            value=self.convert_value_str(
+                                SigmaString(x), state)) for x in arg.s if not isinstance(x, SpecialChars)
+                        ]
+                    )
+                    expr = self.group_expression.format(expr=expr)
+                else:
+                    expr = self.convert_condition_field_eq_val_str(new_cond, state)
                 wildcard_exprs_list.append(expr)
         wildcard_exprs = f'{self.token_separator}{op2}{self.token_separator}'.join(wildcard_exprs_list)
         if as_in_expr and wildcard_exprs:
             return as_in_expr + self.token_separator + op2 + self.token_separator + wildcard_exprs
         return as_in_expr + wildcard_exprs
 
     def convert_condition_not(self, cond: ConditionNOT, state: ConversionState) -> Union[str, DeferredQueryExpression]:
@@ -217,7 +228,14 @@
         This is taken from the ProcessingPipeline state, which is why we automatically run the
         pipeline as part of the backend.
         """
         query_table = state.processing_state.get('query_table', None)
         query_table = query_table + "\n| where " if query_table else "search "
 
         return query_table + query
+
+    def convert_value_str(self, s: SigmaString, state: ConversionState) -> str:
+        """Convert a SigmaString into a plain string which can be used in query."""
+        converted = super().convert_value_str(s, state)
+        # If we have a wildcard in a string, we need to un-escape it
+        # See issue #13
+        return re.sub(r"\\\*", r"*", converted)
```

### Comparing `pysigma_backend_microsoft365defender-0.2.3/sigma/pipelines/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.2.4/sigma/pipelines/microsoft365defender/microsoft365defender.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.2.3/PKG-INFO` & `pysigma_backend_microsoft365defender-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySigma-backend-microsoft365defender
-Version: 0.2.3
+Version: 0.2.4
 Summary: pySigma Microsoft 365 Defender backend
 Home-page: https://github.com/AttackIQ/pySigma-backend-microsoft365defender
 License: LGPL-3.0-only
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

