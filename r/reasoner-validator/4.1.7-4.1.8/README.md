# Comparing `tmp/reasoner_validator-4.1.7.tar.gz` & `tmp/reasoner_validator-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.7.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.8.tar", max compression
```

## Comparing `reasoner_validator-4.1.7.tar` & `reasoner_validator-4.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/README.md
--rw-r--r--   0        0        0      131 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43219 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    95193 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    47100 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/message.py
--rw-r--r--   0        0        0    47007 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38176 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/tests/conftest.py
--rw-r--r--   0        0        0   150844 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    49059 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_semver.py
--rw-r--r--   0        0        0     2351 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36764 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_validate.py
--rw-r--r--   0        0        0    30423 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/README.md
+-rw-r--r--   0        0        0      131 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43520 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2341 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    96715 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    47438 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3995 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/message.py
+-rw-r--r--   0        0        0    47007 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38176 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/conftest.py
+-rw-r--r--   0        0        0   151994 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    49059 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_semver.py
+-rw-r--r--   0        0        0     2351 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36764 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_validate.py
+-rw-r--r--   0        0        0    30423 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.8/PKG-INFO
```

### Comparing `reasoner_validator-4.1.7/LICENSE` & `reasoner_validator-4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/README.md` & `reasoner_validator-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/docs/Makefile` & `reasoner_validator-4.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/docs/conf.py` & `reasoner_validator-4.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/docs/index.rst` & `reasoner_validator-4.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/docs/make.bat` & `reasoner_validator-4.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.8/docs/validation_codes_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -1110,15 +1110,15 @@
 
 **Context:** edge_id, identifier
 
 **Description:** Non-Biolink CURIEs are tolerated, but not preferred, as term value for the attribute_type_id properties of edge attributes.
 
 ### warning.knowledge_graph.edge.attribute.type_id.deprecated
 
-**Message:** Edge has a deprecated attribute_type_id
+**Message:** Edge has a deprecated 'attribute_type_id'
 
 **Context:** identifier
 
 **Description:** Edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement.
 
 ### warning.knowledge_graph.edge.provenance.multiple_primary
 
@@ -1142,28 +1142,36 @@
 
 **Context:** edge_id, identifier, kp_source_type
 
 **Description:** Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP.
 
 ### warning.knowledge_graph.edge.knowledge_level.missing
 
-**Message:** Edge is missing its required 'knowledge_level' property!
+**Message:** Edge is missing its required 'knowledge_level' property
 
 **Context:** edge_id
 
 **Description:** The 'knowledge_level' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!
 
 ### warning.knowledge_graph.edge.agent_type.missing
 
-**Message:** Edge is missing its required 'agent_type' property!
+**Message:** Edge is missing its required 'agent_type' property
 
 **Context:** identifier
 
 **Description:** The 'agent_type' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified Biolink Model release!
 
+### warning.knowledge_graph.edge.treats.support_graph.missing
+
+**Message:** Edge with a treats-related predicate is missing its required 'support_graph' attribute
+
+**Context:** identifier
+
+**Description:** A 'support_graph' may be required as an explanation for a given 'treats' statement assertion.
+
 ## Information
 
 ### info.excluded
 
 **Message:** All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples
 
 **Context:** identifier
```

### Comparing `reasoner_validator-4.1.7/pyproject.toml` & `reasoner_validator-4.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.7"
+version = "4.1.8"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -37,20 +37,21 @@
 include = [
     { path = "tests" },
     { path = "docs" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-bmt = "^1.4.0"
+bmt = "^1.4.1"
 bioregistry = "^0.11.1"
 
 # jsonschema needs to be pinned to <= 4.18.0 for now,
 # since 4.18.0 appeared to break something for the
-# access and processing of JSON schemata
+# access and processing of JSON schemata;
+# maybe now try a later version 4.22.0(?)
 jsonschema = "~4.17.3"
 dictdiffer = "^0.9.0"
 PyYAML = "^6.0"
 requests = "^2.28.1"
 pydantic = "^2"
 urllib3 = "^1.26.15"
```

### Comparing `reasoner_validator-4.1.7/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.8/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         :param name: name of the element
         :return: True if element is a symmetric (predicate) slot.
         """
         # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
         if not name:
             return False
         element: Optional[Element] = self.bmt.get_element(name)
-        if element['symmetric']:
+        if element is not None and element['symmetric']:
             return True
         else:
             return False
 
     def get_inverse_predicate(self, predicate: Optional[str]) -> Optional[str]:
         """
         Utility wrapper of logic to robustly test if a predicate exists and has an inverse.
@@ -781,14 +781,17 @@
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
 
             # Track presence of 'knowledge_level' and 'agent_type' attributes
             found_knowledge_level = False
             found_agent_type = False
 
+            # Track presence of 'support_graph' for some predicates (e.g. 'treats')
+            found_support_graph = False
+
             for attribute in attributes:
 
                 # Validate attribute_type_id
                 if 'attribute_type_id' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.missing",
                         identifier=edge_id,
@@ -877,18 +880,18 @@
                                                     identifier=attribute_type_id,
                                                     edge_id=edge_id,
                                                     source_trail=source_trail
                                                 )
                                             else:
                                                 # attribute_type_id is a Biolink 'association_slot': validate further...
 
-                                                # TODO: only check knowledge_source provenance here for now.
-                                                #       Are there other association_slots to be validated here too?
-                                                #       For example, once new terms with defined value ranges are published
-                                                #       in the Biolink Model, then perhaps 'value' validation will be feasible.
+                                                # TODO: only check knowledge_source provenance here for now. Are there
+                                                #       other association_slots to be validated here too? For example,
+                                                #       once new terms with defined value ranges are published in the
+                                                #       Biolink Model, then perhaps 'value' validation will be feasible.
 
                                                 # Edge provenance tags only recorded in
                                                 # Edge attributes prior to TRAPI 1.4.0-beta
                                                 if not self.minimum_required_trapi_version("1.4.0-beta"):
 
                                                     if attribute_type_id in \
                                                             [
@@ -919,21 +922,25 @@
                                                                         and infores == ara_source:
                                                                     found_ara_knowledge_source = True
                                                                 elif kp_source and \
                                                                         attribute_type_id == kp_source_type and \
                                                                         infores == kp_source:
                                                                     found_kp_knowledge_source = True
 
-                                                # We won't likely care if these shows up in
-                                                # graphs compliant with Biolink earlier than 4.2.0.
-                                                # But we validate their values anyhow...
+                                                # Check for 'support_graph'
+                                                if attribute_type_id == "biolink:support_graph":
+                                                    found_support_graph = False
 
-                                                # We expect at this point that the value should be a single scalar
+                                                # We expect at this point that, if 'attribute_type_id' is a
+                                                # 'knowledge_level' or 'agent_type', then the value is a scalar
                                                 value = value[0]
 
+                                                # We won't likely care if 'knowledge_level' or 'agent_type'
+                                                # show up in graphs compliant with Biolink earlier than 4.2.0,
+                                                # but we validate their values anyhow...
                                                 if attribute_type_id == "biolink:knowledge_level":
                                                     found_knowledge_level = \
                                                         self.validate_knowledge_level(
                                                             edge_id=edge_id,
                                                             found=found_knowledge_level,
                                                             value=value
                                                         )
@@ -983,27 +990,36 @@
                             identifier=edge_id
                         )
                     else:
                         self.report(
                             code="warning.knowledge_graph.edge.knowledge_level.missing",
                             identifier=edge_id
                         )
+
                 if not found_agent_type:
                     # Currently projected to be mandatory only in TRAPI 1.6.0
                     if self.minimum_required_trapi_version("1.6.0"):
                         self.report(
                             code="error.knowledge_graph.edge.agent_type.missing",
                             identifier=edge_id
                         )
                     else:
                         self.report(
                             code="warning.knowledge_graph.edge.agent_type.missing",
                             identifier=edge_id
                         )
 
+                #
+                predicate = edge['predicate'] if 'predicate' in edge else None
+                if self.is_treats(predicate) and not found_support_graph:
+                    self.report(
+                        code="warning.knowledge_graph.edge.treats.support_graph.missing",
+                        identifier=edge_id
+                    )
+
         return source_trail  # may be 'None' if the required attributes are missing
 
     def validate_attribute_constraints(self, edge_id: str, edge: Dict):
         """
         Validate Query Edge Attributes.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
@@ -1508,14 +1524,19 @@
                         break
 
             # "infores:chebi -> infores:biothings-explorer -> infores:molepro -> infores:arax"
             return source_trail
         else:
             return None
 
+    def is_treats(self, predicate: Optional[str]) -> bool:
+        if not predicate:
+            return False
+        return predicate in self.bmt.get_descendants("treats", formatted=True)
+
     def validate_graph_edge(self, edge: Dict, graph_type: TRAPIGraphType):
         """
         Validate slot properties of a relationship ('biolink:Association') edge.
 
         :param edge: Dict[str, str], dictionary of slot properties of the edge.
         :param graph_type: TRAPIGraphType, type of TRAPI component being validated
         """
@@ -1559,15 +1580,20 @@
             # as an Edge property, from TRAPI 1.4.0-beta onwards
             if self.minimum_required_trapi_version("1.4.0-beta"):
                 # For TRAPI 1.4.0, the 'source_trail' is parsed in by 'validate_sources'...
                 source_trail = self.validate_sources(edge_id=edge_id, edge=edge)
 
                 # ...then the 'validate_sources' computed 'source_trail' is communicated
                 #    to 'validate_attributes' for use in attribute validation reporting
-                self.validate_attributes(graph_type=graph_type, edge_id=edge_id, edge=edge, source_trail=source_trail)
+                self.validate_attributes(
+                    graph_type=graph_type,
+                    edge_id=edge_id,
+                    edge=edge,
+                    source_trail=source_trail
+                )
             else:
                 # For TRAPI 1.3.0, the 'sources' are discovered internally by 'validate_attributes'
                 # and the resulting source_trail returned, for further external reporting purposes
                 source_trail = self.validate_attributes(graph_type=graph_type, edge_id=edge_id, edge=edge)
 
             associations: Optional[List[str]] = None
             if self.validate_biolink():
@@ -1600,14 +1626,17 @@
             # Edge property, from TRAPI 1.3.0-beta onwards
             # We don't care about 'source_trail' here, for the Query Graph edges
             if self.minimum_required_trapi_version("1.3.0-beta"):
                 self.validate_qualifier_constraints(edge_id=edge_id, edge=edge)
 
         # Validate Subject node
         if not subject_id:
+            # This message may no longer be triggered
+            # for TRAPI release >= 1.4-beta since the
+            # schema deems the Edge.subject 'nullable: false'
             self.report(
                 code=f"error.{context}.edge.subject.missing",
                 source_trail=source_trail,
                 identifier=edge_id
             )
 
         elif subject_id not in self.get_node_identifiers():
@@ -1664,14 +1693,17 @@
                         predicate=predicate,
                         graph_type=graph_type,
                         source_trail=source_trail
                     )
 
         # Validate Object Node
         if not object_id:
+            # This message may no longer be triggered
+            # for TRAPI release >= 1.4-beta since the
+            # schema deems the Edge.object 'nullable: false'
             self.report(
                 code=f"error.{context}.edge.object.missing",
                 source_trail=source_trail,
                 identifier=edge_id
             )
         elif object_id not in self.get_node_identifiers():
             self.report(
```

### Comparing `reasoner_validator-4.1.7/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.8/reasoner_validator/codes.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
           non_biolink_prefix:
             $message: "Edge has an attribute_type_id that has a non-Biolink CURIE prefix mapped to Biolink"
             $context:
               - edge_id
               - identifier
             $description: "Non-Biolink CURIEs are tolerated, but not preferred, as term value for the attribute_type_id properties of edge attributes."
           deprecated:
-            $message: "Edge has a deprecated attribute_type_id"
+            $message: "Edge has a deprecated 'attribute_type_id'"
             $context:
               - identifier
             $description: "Edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement."
       provenance:
         multiple_primary:
           $message: "Edge has recorded multiple 'primary' knowledge sources"
           $context:
@@ -905,24 +905,31 @@
             $context:
               - edge_id
               - identifier
               - kp_source_type
             $description: "Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP."
       knowledge_level:
         missing:
-          $message: "Edge is missing its required 'knowledge_level' property!"
+          $message: "Edge is missing its required 'knowledge_level' property"
           $context:
             - edge_id
           $description: "The 'knowledge_level' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!"
       agent_type:
         missing:
-          $message: "Edge is missing its required 'agent_type' property!"
+          $message: "Edge is missing its required 'agent_type' property"
           $context:
             - identifier
           $description: "The 'agent_type' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified Biolink Model release!"
+      treats:
+        support_graph:
+          missing:
+            $message: "Edge with a treats-related predicate is missing its required 'support_graph' attribute"
+            $context:
+              - identifier
+            $description: "A 'support_graph' may be required as an explanation for a given 'treats' statement assertion."
 info:
   excluded:
     $message: "All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples"
     $context:
       - identifier
     $description: "Check the JSON KP test edge data file for specific 'exclude_tests' directives, either global to the file, or on specific edges."
   compliant:
```

### Comparing `reasoner_validator-4.1.7/reasoner_validator/github.py` & `reasoner_validator-4.1.8/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/message.py` & `reasoner_validator-4.1.8/reasoner_validator/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module provides standalone global reasoner-validator validation Message types
 to avoid load order conflicts for other modules using these data types.
 """
 from enum import Enum
 from typing import Optional, List, Dict
+
 #
 # The MESSAGE_CATALOG data structure is something like the following:
 #
 #  {
 #    # message 'type'
 #     "information": {
 #
@@ -89,18 +90,18 @@
     warning = "warnings"
     error = "errors"
     critical = "critical errors"
 
 
 # A individual MESSAGE_CATALOG contains
 # the validation messages from
-# all four major categories of validation:
-# critical/errors/warnings/information
+# all five major categories of validation:
+# critical errors/errors/warnings/skipped tests/information
 MESSAGE_CATALOG = Dict[
-    str,  # message type (info/skipped/warning/error/critical)
+    str,  # message type (critical/error/warning/skipped/info)
     MESSAGE_PARTITION
 ]
 
 # MESSAGES_BY_TEST contains MESSAGE_CATALOG
 # entries indexed by individual tests
 MESSAGES_BY_TEST = Dict[
     str,  # unique identifiers for each test
```

### Comparing `reasoner_validator-4.1.7/reasoner_validator/report.py` & `reasoner_validator-4.1.8/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.8/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.8/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.8/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.8/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/validator.py` & `reasoner_validator-4.1.8/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/versioning.py` & `reasoner_validator-4.1.8/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.8/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/__init__.py` & `reasoner_validator-4.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.8/tests/test_biolink_compliance_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,15 @@
                 'subject_category': 'biolink:Drug',
                 'object_category': 'biolink:BiologicalProcess',
                 'predicate': 'biolink:treats',
                 'subject_id': 'NDC:50090‑0766',  # Metformin
                 'object_id': 'GO:0006094'  # Gluconeogenesis
             },
             # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
-            # "info.input_edge.predicate.mixin"
-            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:treats
+            "info.input_edge.predicate.mixin"
         ),
         (   # Query 11 - Unknown predicate element
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:not_a_predicate',
@@ -850,16 +849,15 @@
                     "treats": {
                         "subject": "drug",
                         "predicates": ["biolink:treats"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            # "info.query_graph.edge.predicate.mixin"
-            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:treats
+            "info.query_graph.edge.predicate.mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 19: 'Subject' id used in edge is mandatory
             {
                 "nodes": {
                     "drug": {
@@ -1036,15 +1034,15 @@
                     "gene": {
                         "categories": ["biolink:Gene"]
                     },
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:increases amount or activity of"],
+                        "predicates": ["biolink:treats"],
                         "object": "disease"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
             "info.query_graph.edge.predicate.mixin"
         ),
@@ -1066,14 +1064,15 @@
                     "treats": {
                         "subject": "drug",
                         "predicates": ["biolink:treats"],
                         "object": "disease"
                     }
                 }
             },
+            # 'treats' mixin predicate ignored prior to release of Biolink 4.2.1
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
             # Query 29: ... but if present, predicates must be valid
             #           for the specified Biolink Model version, but...
             {
@@ -3177,21 +3176,22 @@
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
-            ""  # predicate "biolink:interacts_with" is now on
-                # the PREDICATE_INCLUSIONS list so 'mixin' validation is skipped
+            # Since 'interacts_with' mixin predicate is in PREDICATE_INCLUSIONS,
+            # it is ignored prior to the 4.2.1 release of the Biolink Model
+            ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: predicate is a mixin - not allowed in Knowledge Graphs,
-            #           but only in QueryGraphs from Biolink Model 4.2.0 onwards
+            # Query 21: predicate is a mixin allowed in both Knowledge and
+            #           Query Graphs from Biolink Model 4.2.1 onwards
             {
                 "nodes": {
                     "HGNC:3059": {
                         "name": "Heparin binding EGF like growth factor",
                         "categories": [
                            "biolink:Gene"
                         ],
@@ -3221,20 +3221,47 @@
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
-            # "error.knowledge_graph.edge.predicate.mixin"
-            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:interacts_with
+            # The 'interacts_with' mixin predicate is in the 'related_to' predicate hierarchy
+            # from the 4.2.1 release, onwards, of the Biolink Model, hence, properly validated
+            # with an INFO message about its status as a mixin
+            "info.knowledge_graph.edge.predicate.mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: predicate is abstract - not allowed in Knowledge Graphs
+            # Query 22: 'biolink:treats' is a beast with special behaviours to be vetted
+            {
+                "nodes": {
+                    "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                    "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "ncats.drug:9100L32L2N",
+                        "predicate": "biolink:treats",
+                        "object": "MONDO:0005148",
+                        "attributes": DEFAULT_KL_AND_AT_ATTRIBUTES,
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            "info.knowledge_graph.edge.predicate.mixin"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 23: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
                         "name": "article title",
                         "categories": [
                            "biolink:InformationContentEntity"
                         ],
@@ -3268,15 +3295,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.predicate.abstract"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: predicate is non-canonical
+            # Query 24: predicate is non-canonical
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:affected_by",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3295,15 +3322,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: 'object' id is missing from the nodes catalog
+            # Query 25: 'object' id is missing from the nodes catalog
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:678",
@@ -3322,15 +3349,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: attribute 'attribute_type_id' is missing
+            # Query 26: attribute 'attribute_type_id' is missing
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3348,15 +3375,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.type_id.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 26: attribute 'value' is missing?
+            # Query 27: attribute 'value' is missing?
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3375,15 +3402,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 27: 'attribute_type_id' is not a CURIE
+            # Query 28: 'attribute_type_id' is not a CURIE
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3402,15 +3429,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 28: 'attribute_type_id' is a Biolink (node) category - not sure yet
+            # Query 29: 'attribute_type_id' is a Biolink (node) category - not sure yet
             #           whether this reflects "best practices" so issue a warning for now
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3430,15 +3457,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.is_category"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 29: 'attribute_type_id' is a Biolink (edge) predicate - not sure yet
+            # Query 30: 'attribute_type_id' is a Biolink (edge) predicate - not sure yet
             #           whether this reflects "best practices" so issue a warning for now
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3458,15 +3485,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.is_predicate"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 30: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
+            # Query 31: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3485,15 +3512,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.not_association_slot"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 31: 'attribute_type_id' has a 'biolink' CURIE prefix and
+            # Query 32: 'attribute_type_id' has a 'biolink' CURIE prefix and
             #           is an association_slot, so it should pass
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3517,15 +3544,15 @@
                     }
                 }
             },
             ""  # this should recognize the 'attribute_type_id' as a Biolink CURIE
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 32: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
+            # Query 33: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3542,15 +3569,15 @@
                             }
                         ]
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix"
         ),
-        (   # Query 33:  # An earlier Biolink Model won't recognize a category not found in its specified release
+        (   # Query 34:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
                         "categories": [
                             "biolink:Gene"
@@ -3571,15 +3598,15 @@
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                     }
                 }
             },
             "error.knowledge_graph.node.category.unknown"
         ),
-        (   # Query 34:  # 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
+        (   # Query 35:  # 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3601,15 +3628,15 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 35: 'attribute_type_id' is not a 'biolink:association_slot'
+            # Query 36: 'attribute_type_id' is not a 'biolink:association_slot'
             #           (biolink:synonym is a node property) but...
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3632,27 +3659,27 @@
             # ...since Biolink Model validation is tagged as 'suppress',
             # we don't expect any validation output here?
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 36: Knowledge Graph dangling nodes error
+            # Query 37: Knowledge Graph dangling nodes error
             {
                 # Sample nodes with extra  unused node
                 'nodes': SAMPLE_NODES_WITH_UNUSED_NODE,
                 # Sample edge
                 'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
             },
             "warning.knowledge_graph.nodes.dangling"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 37: Knowledge Graph edge duplicated Knowledge Level
+            # Query 38: Knowledge Graph edge duplicated Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         DEFAULT_KL,
                         DEFAULT_AT
@@ -3660,30 +3687,30 @@
                 )
             },
             "error.knowledge_graph.edge.knowledge_level.duplicated"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 38: Knowledge Graph edge missing Knowledge Level
+            # Query 39: Knowledge Graph edge missing Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_AT
                     ]
                 )
             },
             # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
             "warning.knowledge_graph.edge.knowledge_level.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 39: Knowledge Graph edge invalid Knowledge Level
+            # Query 40: Knowledge Graph edge invalid Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         {
                            "attribute_type_id": "biolink:knowledge_level",
                            "value": "not-a-knowledge-level"
@@ -3693,15 +3720,15 @@
                 )
             },
             "error.knowledge_graph.edge.knowledge_level.invalid"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 40: Knowledge Graph edge duplicated Agent Type
+            # Query 41: Knowledge Graph edge duplicated Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         DEFAULT_AT,
                         DEFAULT_AT
@@ -3709,30 +3736,30 @@
                 )
             },
             "error.knowledge_graph.edge.agent_type.duplicated"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 41: Knowledge Graph edge missing Agent Type
+            # Query 42: Knowledge Graph edge missing Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL
                     ]
                 )
             },
             # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
             "warning.knowledge_graph.edge.agent_type.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 42: Knowledge Graph edge invalid Agent Type
+            # Query 43: Knowledge Graph edge invalid Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         {
                            "attribute_type_id": "biolink:agent_type",
@@ -3742,15 +3769,15 @@
                 )
             },
             "error.knowledge_graph.edge.agent_type.invalid"
         ),
         (
             "4.1.6",
 
-            # Query 43: Sample full valid TRAPI Knowledge Graph
+            # Query 44: Sample full valid TRAPI Knowledge Graph
             {
                 # Sample nodes
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 # Sample edge
                 'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
             },
             ""
@@ -3759,15 +3786,18 @@
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(
         biolink_version: str,
         graph_data: Dict,
         code: str
 ):
     validator = BiolinkValidator(biolink_version=biolink_version)
-    validator.check_biolink_model_compliance(graph=graph_data, graph_type=TRAPIGraphType.Knowledge_Graph)
+    validator.check_biolink_model_compliance(
+        graph=graph_data,
+        graph_type=TRAPIGraphType.Knowledge_Graph
+    )
     check_messages(validator, code)
 
 
 MESSAGE_EDGE_WITHOUT_ATTRIBUTES = {
     "nodes": SIMPLE_SAMPLE_NODES,
     "edges": {
         "edge_1": {
```

### Comparing `reasoner_validator-4.1.7/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.8/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_response_validator.py` & `reasoner_validator-4.1.8/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_semver.py` & `reasoner_validator-4.1.8/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.8/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_validate.py` & `reasoner_validator-4.1.8/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_validation_report.py` & `reasoner_validator-4.1.8/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/tests/test_workflows.py` & `reasoner_validator-4.1.8/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.7/PKG-INFO` & `reasoner_validator-4.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.7
+Version: 4.1.8
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bioregistry (>=0.11.1,<0.12.0)
-Requires-Dist: bmt (>=1.4.0,<2.0.0)
+Requires-Dist: bmt (>=1.4.1,<2.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/NCATSTranslator/reasoner-validator/issues
 Project-URL: Change Log, https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md
```

