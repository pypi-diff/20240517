# Comparing `tmp/cnl2asp_test-3.0.3.tar.gz` & `tmp/cnl2asp_test-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2asp_test-3.0.3.tar", last modified: Thu May 16 22:41:01 2024, max compression
+gzip compressed data, was "cnl2asp_test-3.1.0.tar", last modified: Fri May 17 08:15:15 2024, max compression
```

## Comparing `cnl2asp_test-3.0.3.tar` & `cnl2asp_test-3.1.0.tar`

### file list

```diff
@@ -1,15 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:01.847200 cnl2asp_test-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 22:41:01.847200 cnl2asp_test-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 22:40:57.000000 cnl2asp_test-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:41:01.847200 cnl2asp_test-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 22:40:57.000000 cnl2asp_test-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:01.843200 cnl2asp_test-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:01.847200 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 22:41:01.000000 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 22:41:01.000000 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:41:01.000000 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 22:41:01.000000 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 22:41:01.000000 cnl2asp_test-3.0.3/src/cnl2asp_test.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:01.847200 cnl2asp_test-3.0.3/src/printer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:40:57.000000 cnl2asp_test-3.0.3/src/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 22:40:57.000000 cnl2asp_test-3.0.3/src/printer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.090587 cnl2asp_test-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-17 08:15:15.090587 cnl2asp_test-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:15:15.090587 cnl2asp_test-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.078588 cnl2asp_test-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.082588 cnl2asp_test-3.1.0/src/cnl2asp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.082588 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1517 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_aggregate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_atom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1837 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_attribute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_conjunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_encoding.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6550 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      510 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_program.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4703 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/asp_temporal_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.082588 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/cnl2asp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.082588 cnl2asp_test-3.1.0/src/cnl2asp/converter/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/converter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25772 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/converter/asp_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/converter/cnl2json_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/converter/converter_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.086588 cnl2asp_test-3.1.0/src/cnl2asp/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/exception/cnl2asp_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/grammar.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.086588 cnl2asp_test-3.1.0/src/cnl2asp/parser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/parser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3199 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/parser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46610 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/parser/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7027 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/parser/proposition_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.086588 cnl2asp_test-3.1.0/src/cnl2asp/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/aggregate_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/attribute_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/constant_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/entity_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/name_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/operation_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/proposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/relation_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/signaturemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.086588 cnl2asp_test-3.1.0/src/cnl2asp/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-17 08:15:07.000000 cnl2asp_test-3.1.0/src/cnl2asp/utility/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:15:15.090587 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 08:15:15.000000 cnl2asp_test-3.1.0/src/cnl2asp_test.egg-info/top_level.txt
```

