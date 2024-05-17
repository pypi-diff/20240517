# Comparing `tmp/splight_cli-4.8.0.tar.gz` & `tmp/splight_cli-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight_cli-4.8.0.tar", max compression
+gzip compressed data, was "splight_cli-4.9.0.tar", max compression
```

## Comparing `splight_cli-4.8.0.tar` & `splight_cli-4.9.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    16636 2024-02-15 19:15:41.072340 splight_cli-4.8.0/README.md
--rw-r--r--   0        0        0     1296 2024-02-15 19:15:41.072340 splight_cli-4.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/__init__.py
--rw-r--r--   0        0        0     1133 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/cli.py
--rw-r--r--   0        0        0     3760 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/__init__.py
--rw-r--r--   0        0        0     6551 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/component.py
--rw-r--r--   0        0        0     1468 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/exceptions.py
--rw-r--r--   0        0        0     1711 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/loaders.py
--rw-r--r--   0        0        0     1335 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/.splightignore
--rw-r--r--   0        0        0       52 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/Initialization
--rw-r--r--   0        0        0      113 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/README.md
--rw-r--r--   0        0        0     2554 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/auto_readme.md
--rw-r--r--   0        0        0     2126 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/main.py
--rw-r--r--   0        0        0     2752 2024-02-15 19:15:41.072340 splight_cli-4.8.0/splight_cli/component/templates/spec.json
--rw-r--r--   0        0        0      614 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/component/templates/tests.py
--rw-r--r--   0        0        0        0 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/component/tests/__init__.py
--rw-r--r--   0        0        0     2078 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/component/tests/test_component_manager.py
--rw-r--r--   0        0        0     3836 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/component/utils.py
--rw-r--r--   0        0        0     2678 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/config/__init__.py
--rw-r--r--   0        0        0     1605 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/constants.py
--rw-r--r--   0        0        0      792 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/context/__init__.py
--rw-r--r--   0        0        0      383 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/context/context.py
--rw-r--r--   0        0        0     3919 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/context/workspace.py
--rw-r--r--   0        0        0     1016 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/__init__.py
--rw-r--r--   0        0        0     2004 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/alert/__init__.py
--rw-r--r--   0        0        0     1989 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/asset/__init__.py
--rw-r--r--   0        0        0     2042 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/attribute/__init__.py
--rw-r--r--   0        0        0     3848 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/component/__init__.py
--rw-r--r--   0        0        0     2126 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/datalake/__init__.py
--rw-r--r--   0        0        0     2307 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/file/__init__.py
--rw-r--r--   0        0        0      220 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/manager/__init__.py
--rw-r--r--   0        0        0     1280 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/manager/exceptions.py
--rw-r--r--   0        0        0    24434 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/manager/manager.py
--rw-r--r--   0        0        0     1196 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/manager/tests/test_datalake_manager.py
--rw-r--r--   0        0        0     1679 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/manager/tests/test_resource_manager.py
--rw-r--r--   0        0        0     2022 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/engine/secret/__init__.py
--rw-r--r--   0        0        0      412 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/hub/__init__.py
--rw-r--r--   0        0        0     2000 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/hub/component/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/hub/component/exceptions.py
--rw-r--r--   0        0        0     4659 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/hub/component/hub_manager.py
--rw-r--r--   0        0        0     4443 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/hub/component/tests/test_hub_manager.py
--rw-r--r--   0        0        0      720 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/settings.py
--rw-r--r--   0        0        0     3165 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/__init__.py
--rw-r--r--   0        0        0     6402 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/apply_exec.py
--rw-r--r--   0        0        0     1272 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/destroyer.py
--rw-r--r--   0        0        0       89 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/exceptions.py
--rw-r--r--   0        0        0     2710 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/importer.py
--rw-r--r--   0        0        0     1125 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/models.py
--rw-r--r--   0        0        0     4229 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/plan_exec.py
--rw-r--r--   0        0        0    12850 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/replacer.py
--rw-r--r--   0        0        0    18167 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/solution.py
--rw-r--r--   0        0        0    12748 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/solution_checker.py
--rw-r--r--   0        0        0    22432 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/tests/constants.py
--rw-r--r--   0        0        0     8164 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/tests/test_apply.py
--rw-r--r--   0        0        0     3254 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/tests/test_destroy.py
--rw-r--r--   0        0        0     5541 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/tests/test_import.py
--rw-r--r--   0        0        0     2078 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/tests/test_plan.py
--rw-r--r--   0        0        0     1756 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/solution/utils.py
--rw-r--r--   0        0        0        0 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/tests/test_component/Initialization
--rw-r--r--   0        0        0       17 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/tests/test_component/README.md
--rw-r--r--   0        0        0       55 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/tests/test_component/main.py
--rw-r--r--   0        0        0     1451 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/tests/test_component/spec.json
--rw-r--r--   0        0        0        0 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/tests/test_component/tests.py
--rw-r--r--   0        0        0      352 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/__init__.py
--rw-r--r--   0        0        0     2951 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/input.py
--rw-r--r--   0        0        0      418 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/json.py
--rw-r--r--   0        0        0     1884 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/loader.py
--rw-r--r--   0        0        0     1079 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/pprint.py
--rw-r--r--   0        0        0      461 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/template.py
--rw-r--r--   0        0        0      754 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/utils/yaml.py
--rw-r--r--   0        0        0       78 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/version.py
--rw-r--r--   0        0        0     2839 2024-02-15 19:15:41.076340 splight_cli-4.8.0/splight_cli/workspace/__init__.py
--rw-r--r--   0        0        0    17637 1970-01-01 00:00:00.000000 splight_cli-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0    16636 2024-02-22 14:20:36.746669 splight_cli-4.9.0/README.md
+-rw-r--r--   0        0        0     1296 2024-02-22 14:20:36.750669 splight_cli-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/__init__.py
+-rw-r--r--   0        0        0     1133 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/cli.py
+-rw-r--r--   0        0        0     3760 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/__init__.py
+-rw-r--r--   0        0        0     6551 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/component.py
+-rw-r--r--   0        0        0     1468 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/exceptions.py
+-rw-r--r--   0        0        0     1711 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/loaders.py
+-rw-r--r--   0        0        0     1335 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/.splightignore
+-rw-r--r--   0        0        0       52 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/Initialization
+-rw-r--r--   0        0        0      113 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/README.md
+-rw-r--r--   0        0        0     2554 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/auto_readme.md
+-rw-r--r--   0        0        0     2126 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/main.py
+-rw-r--r--   0        0        0     1991 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/spec.json
+-rw-r--r--   0        0        0      614 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/templates/tests.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/tests/__init__.py
+-rw-r--r--   0        0        0     1943 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/tests/test_component_manager.py
+-rw-r--r--   0        0        0     3726 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/component/utils.py
+-rw-r--r--   0        0        0     2678 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/config/__init__.py
+-rw-r--r--   0        0        0     1605 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/constants.py
+-rw-r--r--   0        0        0      792 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/context/__init__.py
+-rw-r--r--   0        0        0      383 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/context/context.py
+-rw-r--r--   0        0        0     3919 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/context/workspace.py
+-rw-r--r--   0        0        0     1016 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/__init__.py
+-rw-r--r--   0        0        0     2004 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/alert/__init__.py
+-rw-r--r--   0        0        0     1989 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/asset/__init__.py
+-rw-r--r--   0        0        0     2042 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/attribute/__init__.py
+-rw-r--r--   0        0        0     3848 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/component/__init__.py
+-rw-r--r--   0        0        0     2126 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/datalake/__init__.py
+-rw-r--r--   0        0        0     2307 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/file/__init__.py
+-rw-r--r--   0        0        0      220 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/manager/__init__.py
+-rw-r--r--   0        0        0     1280 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/manager/exceptions.py
+-rw-r--r--   0        0        0    24344 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/manager/manager.py
+-rw-r--r--   0        0        0     1196 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/manager/tests/test_datalake_manager.py
+-rw-r--r--   0        0        0     1679 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/manager/tests/test_resource_manager.py
+-rw-r--r--   0        0        0     2022 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/engine/secret/__init__.py
+-rw-r--r--   0        0        0      412 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/hub/__init__.py
+-rw-r--r--   0        0        0     2000 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/hub/component/__init__.py
+-rw-r--r--   0        0        0     1264 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/hub/component/exceptions.py
+-rw-r--r--   0        0        0     4659 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/hub/component/hub_manager.py
+-rw-r--r--   0        0        0     4443 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/hub/component/tests/test_hub_manager.py
+-rw-r--r--   0        0        0      720 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/settings.py
+-rw-r--r--   0        0        0     3165 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/__init__.py
+-rw-r--r--   0        0        0     6402 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/apply_exec.py
+-rw-r--r--   0        0        0     1272 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/destroyer.py
+-rw-r--r--   0        0        0       89 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/exceptions.py
+-rw-r--r--   0        0        0     2710 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/importer.py
+-rw-r--r--   0        0        0     1125 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/models.py
+-rw-r--r--   0        0        0     4229 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/plan_exec.py
+-rw-r--r--   0        0        0    12850 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/replacer.py
+-rw-r--r--   0        0        0    18167 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/solution.py
+-rw-r--r--   0        0        0    12748 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/solution_checker.py
+-rw-r--r--   0        0        0    22320 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/tests/constants.py
+-rw-r--r--   0        0        0     8164 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/tests/test_apply.py
+-rw-r--r--   0        0        0     3254 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/tests/test_destroy.py
+-rw-r--r--   0        0        0     5541 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/tests/test_import.py
+-rw-r--r--   0        0        0     2078 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/tests/test_plan.py
+-rw-r--r--   0        0        0     1756 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/solution/utils.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/tests/test_component/Initialization
+-rw-r--r--   0        0        0       17 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/tests/test_component/README.md
+-rw-r--r--   0        0        0       55 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/tests/test_component/main.py
+-rw-r--r--   0        0        0     1210 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/tests/test_component/spec.json
+-rw-r--r--   0        0        0        0 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/tests/test_component/tests.py
+-rw-r--r--   0        0        0      352 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2951 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/input.py
+-rw-r--r--   0        0        0      418 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/json.py
+-rw-r--r--   0        0        0     1884 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/loader.py
+-rw-r--r--   0        0        0     1079 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/pprint.py
+-rw-r--r--   0        0        0      461 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/template.py
+-rw-r--r--   0        0        0      754 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/utils/yaml.py
+-rw-r--r--   0        0        0       78 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/version.py
+-rw-r--r--   0        0        0     2839 2024-02-22 14:20:36.750669 splight_cli-4.9.0/splight_cli/workspace/__init__.py
+-rw-r--r--   0        0        0    17637 1970-01-01 00:00:00.000000 splight_cli-4.9.0/PKG-INFO
```

### Comparing `splight_cli-4.8.0/README.md` & `splight_cli-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/pyproject.toml` & `splight_cli-4.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "splight-cli"
-version = "4.8.0"
+version = "4.9.0"
 description = "Splight Command Line Interface"
 authors = ["Splight Dev <dev@splight-ae.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 case-converter = "1.1.0"
 click = "8.0.4"
 click-default-group = "1.2.2"
 setuptools = "60.9.3"
-splight-lib = "^5.1.0"
+splight-lib = "^5.2.2"
 py7zr = "0.20.8"
 typer = "0.9.0"
 colorama = "0.4.4"
 requests = "2.31.0"
 PyYAML = "6.0.1"
 rich = "13.0.1"
 pathspec = "0.11.1"
```

### Comparing `splight_cli-4.8.0/splight_cli/cli.py` & `splight_cli-4.9.0/splight_cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/__init__.py` & `splight_cli-4.9.0/splight_cli/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/component.py` & `splight_cli-4.9.0/splight_cli/component/component.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/exceptions.py` & `splight_cli-4.9.0/splight_cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/loaders.py` & `splight_cli-4.9.0/splight_cli/component/loaders.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/templates/.splightignore` & `splight_cli-4.9.0/splight_cli/component/templates/.splightignore`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/templates/auto_readme.md` & `splight_cli-4.9.0/splight_cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/templates/main.py` & `splight_cli-4.9.0/splight_cli/component/templates/main.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/templates/spec.json` & `splight_cli-4.9.0/splight_cli/component/templates/spec.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'delete': "['commands', 'bindings']"}*

```diff
@@ -1,38 +1,8 @@
 {
-    "bindings": [
-        {
-            "name": "handle_myasset_create",
-            "object_action": "CREATE",
-            "object_type": "MyAsset"
-        },
-        {
-            "name": "handle_myasset_create",
-            "object_action": "UPDATE",
-            "object_type": "MyAsset"
-        },
-        {
-            "name": "handle_myasset_delete",
-            "object_action": "DELETE",
-            "object_type": "MyAsset"
-        }
-    ],
-    "commands": [
-        {
-            "fields": [
-                {
-                    "name": "asset",
-                    "required": true,
-                    "type": "MyAsset",
-                    "value": null
-                }
-            ],
-            "name": "command_myasset_print"
-        }
-    ],
     "component_type": "connector",
     "custom_types": [
         {
             "fields": [
                 {
                     "name": "asset",
                     "required": true,
```

### Comparing `splight_cli-4.8.0/splight_cli/component/templates/tests.py` & `splight_cli-4.9.0/splight_cli/component/templates/tests.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/component/tests/test_component_manager.py` & `splight_cli-4.9.0/splight_cli/component/tests/test_component_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,15 @@
             },
             {"name": "Bool", "type": "bool", "required": True, "value": True},
             {"name": "Float", "type": "float", "required": True, "value": 1.0},
         ],
         "output": [
             {"name": "Test", "fields": [{"name": "Asset", "type": "Asset"}]}
         ],
-        "commands": [
-            {"name": "Hello", "fields": [{"name": "message", "type": "str"}]}
-        ],
         "tags": ["tag1", "tag2", "tag3"],
-        "bindings": [],
         "endpoints": [{"name": "proxy", "port": 1080}],
     }
 )
 
 
 @dataclass
 class SubprocessOutput:
```

### Comparing `splight_cli-4.8.0/splight_cli/component/utils.py` & `splight_cli-4.9.0/splight_cli/component/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,15 @@
             "id": component_id,
             "name": json_spec.get("name"),
             "version": f"{json_spec['name']}-{json_spec['version']}",
             "custom_types": json_spec.get("custom_types", []),
             "component_type": json_spec.get("component_type", "connector"),
             "input": json_spec.get("input", []),
             "output": json_spec.get("output", []),
-            "commands": json_spec.get("commands", []),
             "endpoints": json_spec.get("endpoints", []),
-            "bindings": json_spec.get("bindings", []),
         }
     }
     return component_id, component
 
 
 def generate_component_object(
     custom_type: Dict[str, Any],
```

### Comparing `splight_cli-4.8.0/splight_cli/config/__init__.py` & `splight_cli-4.9.0/splight_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/constants.py` & `splight_cli-4.9.0/splight_cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/context/__init__.py` & `splight_cli-4.9.0/splight_cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/context/workspace.py` & `splight_cli-4.9.0/splight_cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/alert/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/asset/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/attribute/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/component/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/datalake/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/file/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/file/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/manager/exceptions.py` & `splight_cli-4.9.0/splight_cli/engine/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/manager/manager.py` & `splight_cli-4.9.0/splight_cli/engine/manager/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,18 +626,16 @@
     ):
         self._console.print(
             "Creating new component"
             f" {from_component.name}-{hub_component.version}"
         )
         new_component = Component(
             name=f"{from_component.name}-{hub_component.version}",
-            bindings=hub_component.bindings,
             version=f"{hub_component.name}-{hub_component.version}",
             endpoints=hub_component.endpoints,
-            commands=hub_component.commands,
             component_type=hub_component.component_type,
             output=hub_component.output,
             description=hub_component.description,
             custom_types=hub_component.custom_types,
             input=inputs,
         )
         try:
```

### Comparing `splight_cli-4.8.0/splight_cli/engine/manager/tests/test_datalake_manager.py` & `splight_cli-4.9.0/splight_cli/engine/manager/tests/test_datalake_manager.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/manager/tests/test_resource_manager.py` & `splight_cli-4.9.0/splight_cli/engine/manager/tests/test_resource_manager.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/engine/secret/__init__.py` & `splight_cli-4.9.0/splight_cli/engine/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/hub/component/__init__.py` & `splight_cli-4.9.0/splight_cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/hub/component/exceptions.py` & `splight_cli-4.9.0/splight_cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/hub/component/hub_manager.py` & `splight_cli-4.9.0/splight_cli/hub/component/hub_manager.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/hub/component/tests/test_hub_manager.py` & `splight_cli-4.9.0/splight_cli/hub/component/tests/test_hub_manager.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/settings.py` & `splight_cli-4.9.0/splight_cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/__init__.py` & `splight_cli-4.9.0/splight_cli/solution/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/apply_exec.py` & `splight_cli-4.9.0/splight_cli/solution/apply_exec.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/destroyer.py` & `splight_cli-4.9.0/splight_cli/solution/destroyer.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/importer.py` & `splight_cli-4.9.0/splight_cli/solution/importer.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/models.py` & `splight_cli-4.9.0/splight_cli/solution/models.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/plan_exec.py` & `splight_cli-4.9.0/splight_cli/solution/plan_exec.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/replacer.py` & `splight_cli-4.9.0/splight_cli/solution/replacer.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/solution.py` & `splight_cli-4.9.0/splight_cli/solution/solution.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/solution_checker.py` & `splight_cli-4.9.0/splight_cli/solution/solution_checker.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/tests/constants.py` & `splight_cli-4.9.0/splight_cli/solution/tests/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,14 @@
             "name": "test_asset",
             "tags": [],
             "verified": False,
         }
     ],
     "components": [
         {
-            "bindings": [],
-            "commands": [],
             "component_type": "algorithm",
             "custom_types": [],
             "endpoints": [],
             "id": None,
             "input": [],
             "name": "test_forecast",
             "output": [],
@@ -320,16 +318,14 @@
             "name": "test_asset",
             "tags": [],
             "verified": False,
         }
     ],
     "components": [
         {
-            "bindings": [],
-            "commands": [],
             "component_type": "algorithm",
             "custom_types": [],
             "endpoints": [],
             "id": "5fcca841-8e80-4f5f-b941-763353c30e9b",
             "input": [],
             "name": "test_forecast",
             "output": [],
```

### Comparing `splight_cli-4.8.0/splight_cli/solution/tests/test_apply.py` & `splight_cli-4.9.0/splight_cli/solution/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/tests/test_destroy.py` & `splight_cli-4.9.0/splight_cli/solution/tests/test_destroy.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/tests/test_import.py` & `splight_cli-4.9.0/splight_cli/solution/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/tests/test_plan.py` & `splight_cli-4.9.0/splight_cli/solution/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/solution/utils.py` & `splight_cli-4.9.0/splight_cli/solution/utils.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/tests/test_component/spec.json` & `splight_cli-4.9.0/splight_cli/tests/test_component/spec.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': "['commands', 'bindings']"}*

```diff
@@ -1,20 +1,8 @@
 {
-    "bindings": [],
-    "commands": [
-        {
-            "fields": [
-                {
-                    "name": "message",
-                    "type": "str"
-                }
-            ],
-            "name": "Hello"
-        }
-    ],
     "component_id": "ee21534f-b80b-4f84-a84f-53ce3812fa4c",
     "component_type": "algorithm",
     "custom_types": [],
     "endpoints": [
         {
             "name": "proxy",
             "port": 1080
```

### Comparing `splight_cli-4.8.0/splight_cli/utils/input.py` & `splight_cli-4.9.0/splight_cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/utils/loader.py` & `splight_cli-4.9.0/splight_cli/utils/loader.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/utils/pprint.py` & `splight_cli-4.9.0/splight_cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/utils/yaml.py` & `splight_cli-4.9.0/splight_cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/splight_cli/workspace/__init__.py` & `splight_cli-4.9.0/splight_cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_cli-4.8.0/PKG-INFO` & `splight_cli-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-cli
-Version: 4.8.0
+Version: 4.9.0
 Summary: Splight Command Line Interface
 Author: Splight Dev
 Author-email: dev@splight-ae.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Requires-Dist: mock (>=5.1.0,<6.0.0)
 Requires-Dist: packaging (==23.0)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: py7zr (==0.20.8)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.0.1)
 Requires-Dist: setuptools (==60.9.3)
-Requires-Dist: splight-lib (>=5.1.0,<6.0.0)
+Requires-Dist: splight-lib (>=5.2.2,<6.0.0)
 Requires-Dist: typer (==0.9.0)
 Description-Content-Type: text/markdown
 
 # Splight CLI
 
 ![snyk_code](https://github.com/splightplatform/splight-cli/blob/gh-pages/snyk_code.svg?raw=True)
 ![snyk_dependencies](https://github.com/splightplatform/splight-cli/blob/gh-pages/snyk_dependencies.svg?raw=True)
```

