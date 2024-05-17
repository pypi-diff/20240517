# Comparing `tmp/cnl2asp-1.3.2.tar.gz` & `tmp/cnl2asp-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2asp-1.3.2.tar", last modified: Wed Apr 24 14:48:04 2024, max compression
+gzip compressed data, was "cnl2asp-1.3.3.tar", last modified: Fri May 17 08:43:55 2024, max compression
```

## Comparing `cnl2asp-1.3.2.tar` & `cnl2asp-1.3.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/
--rw-rw-r--   0 simone    (1000) simone    (1000)    11357 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/LICENSE
--rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      922 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     1128 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.073338 cnl2asp-1.3.2/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.073338 cnl2asp-1.3.2/src/cnl2asp/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1517 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_aggregate.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4505 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_atom.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1837 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_attribute.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1594 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_conjunction.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      471 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_element.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1060 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_encoding.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     6394 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_operation.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      510 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_program.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4703 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_rule.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      414 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_temporal_formula.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8020 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      561 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1638 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      609 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    10236 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/cnl2asp.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/converter/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    25041 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/asp_converter.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     7333 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/cnl2json_converter.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4916 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/converter_interface.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/exception/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/exception/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2369 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/exception/cnl2asp_exceptions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    16830 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/grammar.lark
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/parser/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     3199 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/command.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    45312 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/parser.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     7027 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/proposition_builder.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/specification/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1103 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/aggregate_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4080 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/attribute_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      741 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      540 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/constant_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    13928 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/entity_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1667 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/name_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3215 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/operation_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1122 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/problem.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11502 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/proposition.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1081 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/relation_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3963 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/signaturemanager.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1288 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/specification.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/utility/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/utility/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      933 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/utility/utility.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp.egg-info/
--rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     2031 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       49 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       30 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.052956 cnl2asp-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.056956 cnl2asp-1.3.3/src/cnl2asp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.056956 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1517 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_aggregate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_atom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1837 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_attribute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_conjunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_encoding.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6550 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      510 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_program.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4703 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_temporal_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.056956 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/cnl2asp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp/converter/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/converter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25041 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/converter/asp_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/converter/cnl2json_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/converter/converter_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/exception/cnl2asp_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/grammar.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp/parser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/parser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3199 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/parser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45312 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/parser/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7027 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/parser/proposition_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/aggregate_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/attribute_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/constant_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/entity_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/name_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/operation_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/proposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/relation_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/signaturemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-17 08:43:51.000000 cnl2asp-1.3.3/src/cnl2asp/utility/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:43:55.060956 cnl2asp-1.3.3/src/cnl2asp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 08:43:55.000000 cnl2asp-1.3.3/src/cnl2asp.egg-info/top_level.txt
```

### Comparing `cnl2asp-1.3.2/LICENSE` & `cnl2asp-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/PKG-INFO` & `cnl2asp-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.2
+Version: 1.3.3
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.2/README.md` & `cnl2asp-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/setup.py` & `cnl2asp-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from textwrap import dedent
 
 from setuptools import setup, find_packages
 
 setup(
     name='cnl2asp',
-    version='1.3.2',
+    version='1.3.3',
     description='A tool for converting a Controlled Natural Language based on English into Answer Set Programming',
     long_description=dedent('''\
                             A tool for converting a Controlled Natural Language based on English into Answer Set Programming
                             
                             Documentation is available at:
                             https://dodaro.github.io/cnl2asp/
                             '''),
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_aggregate.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_aggregate.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_atom.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_atom.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_attribute.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_attribute.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_conjunction.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_conjunction.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_encoding.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_encoding.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_operation.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
     def __str__(self) -> str:
         if len(self.operands) > 1:
             return f'{super(ASPTemporalOperation, self).__str__()}'
         else:
             string = ''
             string += f'{self._operator_to_symbol(self.operator)} '
             operand = str(self.operands[0])
-            if not isinstance(operand, ASPOperation):
+            if not isinstance(self.operands[0], ASPOperation) or (isinstance(self.operands[0], ASPOperation) and len(self.operands[0].operands) == 1):
+                # operation of a single operand or an atom
                 string += operand
             else:
                 string += f'({operand})'
             return string
 
 
     def temporal_formula_string(self) -> str:
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_rule.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/asp_rule.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py` & `cnl2asp-1.3.3/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,10 +13,10 @@
         self.encoding = encoding
 
     def solve(self):
         with tempfile.NamedTemporaryFile(mode="w") as file:
             file.write(self.encoding)
             file.seek(0)
             sys.stdout = telingo_result = StringIO()
-            clingo.clingo_main(telingo.TelApp(), [file.name, "--verbose=0", "--quiet=1,2,2", "--warn=none"])
+            clingo.clingo_main(telingo.Application(), [file.name, "--verbose=0", "--quiet=1,2,2", "--warn=none"])
             sys.stdout = sys.__stdout__
             return telingo_result.getvalue()
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/cnl2asp.py` & `cnl2asp-1.3.3/src/cnl2asp/cnl2asp.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/converter/asp_converter.py` & `cnl2asp-1.3.3/src/cnl2asp/converter/asp_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/converter/cnl2json_converter.py` & `cnl2asp-1.3.3/src/cnl2asp/converter/cnl2json_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/converter/converter_interface.py` & `cnl2asp-1.3.3/src/cnl2asp/converter/converter_interface.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/exception/cnl2asp_exceptions.py` & `cnl2asp-1.3.3/src/cnl2asp/exception/cnl2asp_exceptions.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/grammar.lark` & `cnl2asp-1.3.3/src/cnl2asp/grammar.lark`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 _CNL_CONTAINS: "contains"
 complex_concept_elements_definition: STRING _CNL_CONTAINS string_list
 
 implicit_definition_proposition: constant_definition_clause -> constant_implicit_definition_proposition
                                  | simple_definition
                                  | compounded_range_clause
                                  | compounded_match_clause
-                                 | enumerative_definition_clause
+                                 | enumerative_definition_clause [terminal_clauses]
 _CNL_CONSTANT: "constant"
 cnl_is_a_constant: _CNL_IS " " _CNL_A " " _CNL_CONSTANT
 _CNL_EQUAL: "equal"
 _CNL_EQUAL_TO: _CNL_EQUAL " " _CNL_TO
 constant_definition_clause.1: STRING cnl_is_a_constant [_CNL_EQUAL_TO STRING]
 
 _CNL_AN: "an"i
@@ -90,15 +90,15 @@
 _CNL_THAT: "that"
 _CNL_ARE: "are"
 _CNL_RESPECTIVELY: "respectively"
 cnl_that_are_equal_to_respectively: _CNL_THAT " " _CNL_ARE " " _CNL_EQUAL_TO " " _CNL_RESPECTIVELY
 cnl_that_is_equal_to_respectively: _CNL_THAT " " _CNL_IS " " _CNL_EQUAL_TO " " _CNL_RESPECTIVELY
 _CNL_ALSO: "also"
 compounded_match_tail: _CNL_AND _CNL_HAS STRING (cnl_that_are_equal_to_respectively | cnl_that_is_equal_to_respectively) string_list (_CNL_AND _CNL_ALSO STRING (cnl_that_are_equal_to_respectively | cnl_that_is_equal_to_respectively) string_list)*
-enumerative_definition_clause: entity verb [conjunctive_object_list] [terminal_clauses]
+enumerative_definition_clause: entity verb [conjunctive_object_list]
 
 standard_proposition: whenever_then_clause_proposition
                     | fact_proposition
                     | quantified_choice_proposition
                     | constraint_proposition
                     | weak_constraint_proposition
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/parser/command.py` & `cnl2asp-1.3.3/src/cnl2asp/parser/command.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/parser/parser.py` & `cnl2asp-1.3.3/src/cnl2asp/parser/parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/parser/proposition_builder.py` & `cnl2asp-1.3.3/src/cnl2asp/parser/proposition_builder.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/aggregate_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/aggregate_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/attribute_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/attribute_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/constant_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/constant_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/entity_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/entity_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/name_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/name_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/operation_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/operation_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.negated = False
         if self.operation == Operators.BETWEEN:
             operands = self.between_operator(operands)
         for operand in operands:
             if not isinstance(operand, Component):
                 operand = ValueComponent(operand)
             self.operands.append(operand)
+        self.auxiliary_verb = None
 
 
     def between_operator(self, operands):
         operands = list(operands)
         if self.operation == Operators.BETWEEN:
             self.operation = Operators.LESS_THAN_OR_EQUAL_TO
         elif self.operation == Operators.NOTBETWEEN:
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/problem.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/problem.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/proposition.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/proposition.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def convert(self, converter: Converter) -> NewKnowledgeConverter:
         return converter.convert_new_knowledge(self)
 
     def copy(self):
         return NewKnowledgeComponent(self.new_entity.copy(), self.condition.copy(), self.subject, self.auxiliary_verb, self.objects)
 
     def get_entities(self) -> list[EntityComponent]:
-        entities = [self.new_entity]
+        entities = self.new_entity.get_entities()
         for entity in self.condition.get_entities():
             entities.append(entity)
         return entities
 
     def get_entities_to_link_with_new_knowledge(self) -> list[EntityComponent]:
         entities = [self.new_entity]
         for entity in self.condition.get_entities_to_link_with_new_knowledge():
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/relation_component.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/relation_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/signaturemanager.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/signaturemanager.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/specification/specification.py` & `cnl2asp-1.3.3/src/cnl2asp/specification/specification.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp/utility/utility.py` & `cnl2asp-1.3.3/src/cnl2asp/utility/utility.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.2/src/cnl2asp.egg-info/PKG-INFO` & `cnl2asp-1.3.3/src/cnl2asp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.2
+Version: 1.3.3
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.2/src/cnl2asp.egg-info/SOURCES.txt` & `cnl2asp-1.3.3/src/cnl2asp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

