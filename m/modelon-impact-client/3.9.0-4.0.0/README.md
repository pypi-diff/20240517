# Comparing `tmp/modelon_impact_client-3.9.0.tar.gz` & `tmp/modelon_impact_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-3.9.0.tar", max compression
+gzip compressed data, was "modelon_impact_client-4.0.0.tar", max compression
```

## Comparing `modelon_impact_client-3.9.0.tar` & `modelon_impact_client-4.0.0.tar`

### file list

```diff
@@ -1,82 +1,79 @@
--rw-r--r--   0        0        0     1479 2024-02-15 04:09:47.458728 modelon_impact_client-3.9.0/LICENSE.md
--rw-r--r--   0        0        0     2748 2024-02-15 04:09:47.470728 modelon_impact_client-3.9.0/README.md
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.413728 modelon_impact_client-3.9.0/modelon/__init__.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.454728 modelon_impact_client-3.9.0/modelon/impact/__init__.py
--rw-r--r--   0        0        0     1035 2024-02-15 04:09:47.448728 modelon_impact_client-3.9.0/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    26054 2024-02-15 04:09:47.418727 modelon_impact_client-3.9.0/modelon/impact/client/client.py
--rw-r--r--   0        0        0     1577 2024-02-15 04:09:47.470728 modelon_impact_client-3.9.0/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1937 2024-02-15 04:09:47.419728 modelon_impact_client-3.9.0/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2024-02-15 04:09:47.435728 modelon_impact_client-3.9.0/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      640 2024-02-15 04:09:47.408728 modelon_impact_client-3.9.0/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    24785 2024-02-15 04:09:47.468728 modelon_impact_client-3.9.0/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     2260 2024-02-15 04:09:47.486728 modelon_impact_client-3.9.0/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     6622 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    18420 2024-02-15 04:09:47.425728 modelon_impact_client-3.9.0/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     2512 2024-02-15 04:09:47.408728 modelon_impact_client-3.9.0/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.485728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/__init__.py
--rw-r--r--   0        0        0      180 2024-02-15 04:09:47.399727 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/case.py
--rw-r--r--   0        0        0      200 2024-02-15 04:09:47.454728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/custom_function.py
--rw-r--r--   0        0        0      366 2024-02-15 04:09:47.445728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/experiment.py
--rw-r--r--   0        0        0      192 2024-02-15 04:09:47.449728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/external_result.py
--rw-r--r--   0        0        0      186 2024-02-15 04:09:47.446728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/model.py
--rw-r--r--   0        0        0      190 2024-02-15 04:09:47.436728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/model_executable.py
--rw-r--r--   0        0        0      190 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/workspace.py
--rw-r--r--   0        0        0      156 2024-02-15 04:09:47.440728 modelon_impact_client-3.9.0/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    16772 2024-02-15 04:09:47.426728 modelon_impact_client-3.9.0/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0    12111 2024-02-15 04:09:47.417728 modelon_impact_client-3.9.0/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    12804 2024-02-15 04:09:47.483728 modelon_impact_client-3.9.0/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1988 2024-02-15 04:09:47.445728 modelon_impact_client-3.9.0/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0     1479 2024-02-15 04:09:47.400727 modelon_impact_client-3.9.0/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    34034 2024-02-15 04:09:47.475728 modelon_impact_client-3.9.0/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1366 2024-02-15 04:09:47.422728 modelon_impact_client-3.9.0/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.409727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     5284 2024-02-15 04:09:47.494728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0     4039 2024-02-15 04:09:47.419728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0    10243 2024-02-15 04:09:47.401727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0    12627 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/fmu_based.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.455728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/__init__.py
--rw-r--r--   0        0        0      507 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/definition.py
--rw-r--r--   0        0        0      409 2024-02-15 04:09:47.421728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/expansion.py
--rw-r--r--   0        0        0      188 2024-02-15 04:09:47.390727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/extension.py
--rw-r--r--   0        0        0    18531 2024-02-15 04:09:47.426728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/model_based.py
--rw-r--r--   0        0        0     4699 2024-02-15 04:09:47.405727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0      643 2024-02-15 04:09:47.409727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       65 2024-02-15 04:09:47.492728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/__init__.py
--rw-r--r--   0        0        0     2976 2024-02-15 04:09:47.461728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/authorize.py
--rw-r--r--   0        0        0      281 2024-02-15 04:09:47.499729 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/exceptions.py
--rw-r--r--   0        0        0     2895 2024-02-15 04:09:47.422728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/sal.py
--rw-r--r--   0        0        0       79 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5814 2024-02-15 04:09:47.428728 modelon_impact_client-3.9.0/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2440 2024-02-15 04:09:47.447728 modelon_impact_client-3.9.0/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2503 2024-02-15 04:09:47.448728 modelon_impact_client-3.9.0/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2245 2024-02-15 04:09:47.410728 modelon_impact_client-3.9.0/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2409 2024-02-15 04:09:47.450728 modelon_impact_client-3.9.0/modelon/impact/client/operations/external_result_import.py
--rw-r--r--   0        0        0     2720 2024-02-15 04:09:47.440728 modelon_impact_client-3.9.0/modelon/impact/client/operations/fmu_import.py
--rw-r--r--   0        0        0     5846 2024-02-15 04:09:47.492728 modelon_impact_client-3.9.0/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0     2685 2024-02-15 04:09:47.504729 modelon_impact_client-3.9.0/modelon/impact/client/operations/project_import.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.415727 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2600 2024-02-15 04:09:47.493728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3627 2024-02-15 04:09:47.494728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2470 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3770 2024-02-15 04:09:47.472728 modelon_impact_client-3.9.0/modelon/impact/client/options.py
--rw-r--r--   0        0        0     5373 2024-02-15 04:09:47.452728 modelon_impact_client-3.9.0/modelon/impact/client/published_workspace_client.py
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.400727 modelon_impact_client-3.9.0/modelon/impact/client/py.typed
--rw-r--r--   0        0        0        0 2024-02-15 04:09:47.459728 modelon_impact_client-3.9.0/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      132 2024-02-15 04:09:47.455728 modelon_impact_client-3.9.0/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1544 2024-02-15 04:09:47.430728 modelon_impact_client-3.9.0/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      671 2024-02-15 04:09:47.395727 modelon_impact_client-3.9.0/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     6787 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      630 2024-02-15 04:09:47.418727 modelon_impact_client-3.9.0/modelon/impact/client/sal/exports.py
--rw-r--r--   0        0        0     1476 2024-02-15 04:09:47.500728 modelon_impact_client-3.9.0/modelon/impact/client/sal/external_result.py
--rw-r--r--   0        0        0     3305 2024-02-15 04:09:47.452728 modelon_impact_client-3.9.0/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0      476 2024-02-15 04:09:47.503728 modelon_impact_client-3.9.0/modelon/impact/client/sal/imports.py
--rw-r--r--   0        0        0     3084 2024-02-15 04:09:47.472728 modelon_impact_client-3.9.0/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4883 2024-02-15 04:09:47.464728 modelon_impact_client-3.9.0/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     5097 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     5114 2024-02-15 04:09:47.446728 modelon_impact_client-3.9.0/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     5082 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      885 2024-02-15 04:09:47.402727 modelon_impact_client-3.9.0/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      454 2024-02-15 04:09:47.435728 modelon_impact_client-3.9.0/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0    12555 2024-02-15 04:09:47.431728 modelon_impact_client-3.9.0/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0     1440 2024-02-15 04:13:33.738229 modelon_impact_client-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1479 2024-05-17 04:17:21.438211 modelon_impact_client-4.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3700 2024-05-17 04:17:21.449211 modelon_impact_client-4.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.324210 modelon_impact_client-4.0.0/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.156208 modelon_impact_client-4.0.0/modelon/impact/__init__.py
+-rw-r--r--   0        0        0     1035 2024-05-17 04:17:21.417211 modelon_impact_client-4.0.0/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    28159 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/client.py
+-rw-r--r--   0        0        0     1949 2024-05-17 04:17:21.218209 modelon_impact_client-4.0.0/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1937 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2024-05-17 04:17:21.398211 modelon_impact_client-4.0.0/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-17 04:17:21.322210 modelon_impact_client-4.0.0/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    27437 2024-05-17 04:17:21.216209 modelon_impact_client-4.0.0/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2260 2024-05-17 04:17:21.233209 modelon_impact_client-4.0.0/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     8204 2024-05-17 04:17:21.080208 modelon_impact_client-4.0.0/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    26183 2024-05-17 04:17:21.379211 modelon_impact_client-4.0.0/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2512 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.481212 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-17 04:17:21.307210 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      200 2024-05-17 04:17:21.155208 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0     1305 2024-05-17 04:17:21.405211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2024-05-17 04:17:21.418211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2024-05-17 04:17:21.140208 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2024-05-17 04:17:21.398211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2024-05-17 04:17:21.139208 modelon_impact_client-4.0.0/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16740 2024-05-17 04:17:21.380211 modelon_impact_client-4.0.0/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    13656 2024-05-17 04:17:21.368211 modelon_impact_client-4.0.0/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    13156 2024-05-17 04:17:21.224209 modelon_impact_client-4.0.0/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1988 2024-05-17 04:17:21.140208 modelon_impact_client-4.0.0/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1479 2024-05-17 04:17:21.316210 modelon_impact_client-4.0.0/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    39729 2024-05-17 04:17:21.476212 modelon_impact_client-4.0.0/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1531 2024-05-17 04:17:21.372211 modelon_impact_client-4.0.0/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2024-05-17 04:17:21.243209 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     4039 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    11525 2024-05-17 04:17:21.029207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    13950 2024-05-17 04:17:21.446211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.157208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2024-05-17 04:17:21.081208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      188 2024-05-17 04:17:21.017207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    21122 2024-05-17 04:17:21.381211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     2090 2024-05-17 04:17:21.202209 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/modifiers.py
+-rw-r--r--   0        0        0     7944 2024-05-17 04:17:21.042207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0     1018 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       79 2024-05-17 04:17:21.324210 modelon_impact_client-4.0.0/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5814 2024-05-17 04:17:21.382211 modelon_impact_client-4.0.0/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2440 2024-05-17 04:17:21.141208 modelon_impact_client-4.0.0/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2503 2024-05-17 04:17:21.141208 modelon_impact_client-4.0.0/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2245 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2409 2024-05-17 04:17:21.420211 modelon_impact_client-4.0.0/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2720 2024-05-17 04:17:21.131208 modelon_impact_client-4.0.0/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5846 2024-05-17 04:17:21.486212 modelon_impact_client-4.0.0/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2634 2024-05-17 04:17:21.299210 modelon_impact_client-4.0.0/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.367210 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2600 2024-05-17 04:17:21.486212 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3627 2024-05-17 04:17:21.487212 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2470 2024-05-17 04:17:21.447211 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3770 2024-05-17 04:17:21.474212 modelon_impact_client-4.0.0/modelon/impact/client/options.py
+-rw-r--r--   0        0        0     5697 2024-05-17 04:17:21.145208 modelon_impact_client-4.0.0/modelon/impact/client/published_workspace_client.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.028207 modelon_impact_client-4.0.0/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2024-05-17 04:17:21.440211 modelon_impact_client-4.0.0/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-17 04:17:21.156208 modelon_impact_client-4.0.0/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1544 2024-05-17 04:17:21.093208 modelon_impact_client-4.0.0/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2024-05-17 04:17:21.302210 modelon_impact_client-4.0.0/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6787 2024-05-17 04:17:21.447211 modelon_impact_client-4.0.0/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      630 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1476 2024-05-17 04:17:21.278210 modelon_impact_client-4.0.0/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3346 2024-05-17 04:17:21.421211 modelon_impact_client-4.0.0/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      476 2024-05-17 04:17:21.298210 modelon_impact_client-4.0.0/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3084 2024-05-17 04:17:21.218209 modelon_impact_client-4.0.0/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4883 2024-05-17 04:17:21.203209 modelon_impact_client-4.0.0/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     5353 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5114 2024-05-17 04:17:21.407211 modelon_impact_client-4.0.0/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     3284 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      885 2024-05-17 04:17:21.319210 modelon_impact_client-4.0.0/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      454 2024-05-17 04:17:21.384211 modelon_impact_client-4.0.0/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0    13616 2024-05-17 04:17:21.383211 modelon_impact_client-4.0.0/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1479 2024-05-17 04:23:56.357321 modelon_impact_client-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 modelon_impact_client-4.0.0/PKG-INFO
```

### Comparing `modelon_impact_client-3.9.0/LICENSE.md` & `modelon_impact_client-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/README.md` & `modelon_impact_client-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,112 @@
 # Modelon-impact-client
+
 Client library for easy scripting against Modelon Impact
 
 ## Installation
 
 For installation instructions and requirements, please refer to the [documentation](https://modelon-impact-client.readthedocs.io).
 
 ## Develop
 
 ### Devcontainer
+
 If you are developing with VS Code you can use the devcontainer which gives gives you a ready to use environment for development. Just click the "Reopen in Container" button after opening the project in VS Code.
 
 #### Tips and tricks
+
 It is possible to run the 'make' commands listed bellow using the devcontainer. It will detect being in a container and bypass Docker parts of the commands.
 
 You can open a project with the dev-container directly without having to open and then re-load. Standing in the project directory you can run:
+
 ```
 devcontainer open .
 ```
+
 Note that this requires the [devcontainer-cli](https://code.visualstudio.com/docs/remote/devcontainer-cli).
 
 You can add your own extensions to devcontainers. These extensions will be added for all devcontainers. First open your 'settings' as JSON. Then, to add for example the "GitLens" extension, put the following at the bottom of the settings:
+
 ```
     ...
     "remote.containers.defaultExtensions": ["eamodio.gitlens"]
 }
 ```
+
 VS Code also have a `'Install Local Extensions in 'Remote'` command, but it must be repeated for each devcontainer and everytime a devcontainer is re-built.
 
 ### Creating a shell
+
 Modelon-impact-client is developed using a Docker container for all build tools.
 You can get a shell into said container by running:
 
 ```
 make shell
 ```
 
 ### Manage dependencies
-Dependencies are managed by poetry. Add dependencies by running 
+
+Dependencies are managed by poetry. Add dependencies by running
 `poetry add <package>`  or `poetry add <package> --dev` inside the shell
 
 ### Running tests
 
 Tests are executed by running `make test`. You can also run `make test-watch` to get a watcher
 that continuously re-runs the tests.
 
 ### Running lint
+
 ```
 make lint
 ```
 
 ## Build
 
 Building modelon-impact-client is done by running
 
 ```
 make wheel
 ```
 
+## Test
+
+The tests for modelon-impact-client could be run by executing
+
+```
+make test
+```
+
+### VCR test
+
+Vcrpy(https://vcrpy.readthedocs.io/en/latest/) is used to mock the http requests and
+responses for some of the tests. VCR.py records all HTTP interactions that take place
+in a flat file called a 'cassette'. These files could are stored in the `impact-client-python/tests/fixtures/vcr_cassettes` folder. When an API response/request body is updated on MI, these files need to be regenerated. To regenerate these file, follow the following steps:
+
+1. Start Modelon impact cloud - https://impact.modelon.cloud.
+2. Generate an MI api key and JH token and store them in secrets folder. See [Readme](.secrets/README.md) for more information.
+3. Delete the cassette file you wish to regenerate from `impact-client-python/tests/fixtures/vcr_cassettes` folder.
+4. The file could now be regenrated by executing
+
+```
+make regenerate-cassette
+```
+
 ## Release
 
 The modelon-impact-client build process is a fully automated using `Semantic-release`.
 
 Automation is enabled for:
+
 - Bumping version
 - Generate changelog
 
 This is done based on git commit semantics as described here: https://semantic-release.gitbook.io/semantic-release/
 
 To make a new release simply run:
+
 ```
 make publish
 ```
 
 This command will detect what branch you are on and your git history and make a appropriate release.
 
 Current configuration can be found in `.releaserc` and specifies that commits to branch `master` should be released and
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/__init__.py` & `modelon_impact_client-4.0.0/modelon/impact/client/__init__.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/client.py` & `modelon_impact_client-4.0.0/modelon/impact/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 import enum
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 from semantic_version import SimpleSpec, Version  # type: ignore
 
-import modelon.impact.client.jupyterhub
 import modelon.impact.client.sal.exceptions
-import modelon.impact.client.sal.service
 from modelon.impact.client import exceptions
-from modelon.impact.client.configuration import get_client_interactive, get_client_url
+from modelon.impact.client.configuration import (
+    Experimental,
+    get_client_interactive,
+    get_client_url,
+)
 from modelon.impact.client.credential_manager import CredentialManager
+from modelon.impact.client.entities.case import Case
 from modelon.impact.client.entities.experiment import Experiment
+from modelon.impact.client.entities.interfaces.case import CaseReference
+from modelon.impact.client.entities.interfaces.experiment import ExperimentReference
 from modelon.impact.client.entities.model_executable import ModelExecutable
 from modelon.impact.client.entities.project import (
     Project,
     ProjectType,
     StorageLocation,
     VcsUri,
 )
@@ -28,23 +33,24 @@
 from modelon.impact.client.operations.project_import import ProjectImportOperation
 from modelon.impact.client.operations.workspace.conversion import (
     WorkspaceConversionOperation,
 )
 from modelon.impact.client.operations.workspace.imports import WorkspaceImportOperation
 from modelon.impact.client.published_workspace_client import PublishedWorkspacesClient
 from modelon.impact.client.sal.context import Context
+from modelon.impact.client.sal.service import Service, is_jupyterhub_url
 from modelon.impact.client.sal.uri import URI
 
 logger = logging.getLogger(__name__)
 
 
 @enum.unique
 class ExecutionKind(enum.Enum):
-    COMPILATION = 'COMPILATION'
-    EXPERIMENT = 'EXPERIMENT'
+    COMPILATION = "COMPILATION"
+    EXPERIMENT = "EXPERIMENT"
 
 
 @dataclass
 class Execution:
     kind: ExecutionKind
     workspace_id: str
     id: str
@@ -66,15 +72,15 @@
 
 @dataclass
 class Selection:
     entry_id: str
     project: Project
 
     def to_dict(self) -> Dict[str, Any]:
-        return {'id': self.entry_id, 'project': {'id': self.project.id}}
+        return {"id": self.entry_id, "project": {"id": self.project.id}}
 
 
 @dataclass
 class ProjectMatching:
     entry_id: str
     vcs_uri: str
     projects: List[Project]
@@ -128,15 +134,15 @@
             vcs_uri = f"{' ' * len(choice)} Project URI: {str(project.vcs_uri)}"
             print("_" * 60)
             print(f"{choice} Project name: {project.definition.name}")
             print(vcs_uri)
 
         while True:
             try:
-                chosen_index = int(input('\nPlease enter one of the above choices:-'))
+                chosen_index = int(input("\nPlease enter one of the above choices:-"))
                 selection = self.get_selection(index=chosen_index)
                 break
             except (KeyError, ValueError, IndexError):
                 allowed_choices = map(str, range(len(self.projects)))
                 print(
                     f"Invalid choice. Please select one of {','.join(allowed_choices)}!"
                 )
@@ -212,77 +218,58 @@
         from modelon.impact.client import Client
 
         client = Client(url=impact_url)
         client = Client(url=impact_url, interactive=True)
 
     """
 
-    _SUPPORTED_VERSION_RANGE = ">=4.0.0,<5.0.0"
+    _SUPPORTED_VERSION_RANGE = ">=4.11.0,<5.0.0"
 
     def __init__(
         self,
         url: Optional[str] = None,
         interactive: Optional[bool] = None,
         credential_manager: Optional[CredentialManager] = None,
         context: Optional[Context] = None,
-        jupyterhub_credential_manager: Optional[CredentialManager] = None,
     ):
         if url is None:
             url = get_client_url()
 
         if interactive is None:
             interactive = get_client_interactive()
 
         self._uri = URI(url)
-        self._sal = modelon.impact.client.sal.service.Service(self._uri, context)
-
-        if self._sal.is_jupyterhub_url():
-            logger.info(
-                "API response indicates that the URL '%s' hosts a JupyterHub.",
-                str(self._uri),
-            )
-            self._uri, jupyter_context = modelon.impact.client.jupyterhub.authorize(
-                self._uri,
-                interactive,
-                context,
-                jupyterhub_credential_manager,
-            )
-            self._sal = modelon.impact.client.sal.service.Service(
-                self._uri, jupyter_context
-            )
-
-        self._validate_compatible_api_version()
-
         if credential_manager is None:
-            help_hint = f"can be generated at {self._uri / 'admin/keys'}"
+            uri = (
+                self._uri / "user-redirect/impact"
+                if is_jupyterhub_url(self._uri)
+                else self._uri
+            )
+            help_hint = f"can be generated at {uri / 'admin/keys'}"
             help_text = f"Enter Modelon Impact API key ({help_hint}):"
             credential_manager = CredentialManager(interactive_help_text=help_text)
         self._credential_manager = credential_manager
 
         try:
-            api_key = self._authenticate_against_api(interactive)
+            self._sal = self._get_authenticated_service(interactive, self._uri, context)
         except modelon.impact.client.sal.exceptions.HTTPError:
             if interactive:
                 logger.warning(
                     "The provided Modelon Impact API key is not valid, "
                     "please enter a new key"
                 )
                 api_key = self._credential_manager.get_key_from_prompt()
-                api_key = self._authenticate_against_api(interactive, api_key=api_key)
+                self._sal = self._get_authenticated_service(
+                    interactive, self._uri, context, api_key=api_key
+                )
             else:
                 raise
 
-        self._sal.add_login_retry_with(api_key)
-
-        resp = self._sal.users.get_me()
-        if 'license' not in resp['data']:
-            raise exceptions.NoAssignedLicenseError(
-                "No assigned license during login. Either out of floating Deployment "
-                "Add-on licenses or your assigned user license could not be validated"
-            )
+        # TODO Update to use the unprotected API route https://impact.modelon.cloud/api
+        self._validate_compatible_api_version()
 
     def _validate_compatible_api_version(self) -> None:
         try:
             version = self._sal.api_get_metadata()["version"]
         except modelon.impact.client.sal.exceptions.CommunicationError as exce:
             raise modelon.impact.client.sal.exceptions.NoResponseFetchVersionError(
                 f"No response from url {self._uri}, "
@@ -293,33 +280,43 @@
             raise exceptions.UnsupportedSemanticVersionError(
                 f"Version '{version}' of the HTTP REST API is not supported, "
                 f"must be in the range '{self._SUPPORTED_VERSION_RANGE}'! "
                 "Updgrade or downgrade this package to a version "
                 f"that supports version '{version}' of the HTTP REST API."
             )
 
-    def _authenticate_against_api(
-        self, interactive: bool, api_key: Optional[str] = None
-    ) -> Optional[str]:
+    def _get_authenticated_service(
+        self,
+        interactive: bool,
+        uri: URI,
+        context: Optional[Context] = None,
+        api_key: Optional[str] = None,
+    ) -> Service:
         if not api_key:
             api_key = self._credential_manager.get_key(interactive=interactive)
 
         if not api_key:
-            logger.warning(
-                "No Modelon Impact API key could be found, "
-                "will log in as anonymous user. Permissions may be limited"
+            raise exceptions.AuthenticationError(
+                "Authentication failed! No Modelon Impact API key could be found"
             )
+        # TODO: Do we need a key validation API?
+        sal = Service(uri, api_key, context)
+        resp = sal.users.get_me()
 
-        self._sal.api_login(api_key=api_key)
         if api_key and interactive:
             # Save the api_key for next time if
             # running interactively and login was successfully
             self._credential_manager.write_key_to_file(api_key)
 
-        return api_key
+        if "license" not in resp["data"]:
+            raise exceptions.NoAssignedLicenseError(
+                "No assigned license during login. Either out of floating Deployment "
+                "Add-on licenses or your assigned user license could not be validated"
+            )
+        return sal
 
     def get_workspace(self, workspace_id: str) -> Workspace:
         """Returns a Workspace class object.
 
         Args:
             workspace_id: The ID of the workspace.
 
@@ -348,15 +345,15 @@
             workspaces = client.get_workspace_by_name('TestWorkspace')
 
         """
         resp = self._sal.workspace.workspaces_get()
         return [
             Workspace(item["id"], self._sal)
             for item in resp["data"]["items"]
-            if item['definition']['name'] == workspace_name
+            if item["definition"]["name"] == workspace_name
         ]
 
     def get_workspaces(
         self,
         only_app_mode: bool = False,
         name: Optional[str] = None,
         sharing_id: Optional[str] = None,
@@ -416,15 +413,14 @@
 
         """
         resp = self._sal.project.project_get(
             project_id, vcs_info=vcs_info, size_info=False
         )
         return Project(
             resp["id"],
-            resp["definition"],
             resp["projectType"],
             resp["storageLocation"],
             VcsUri.from_dict(resp["vcsUri"]) if resp.get("vcsUri") else None,
             self._sal,
         )
 
     def get_projects(
@@ -462,15 +458,14 @@
             vcs_info=vcs_info,
             project_type=project_type,
             storage_location=storage_location,
         )
         return [
             Project(
                 item["id"],
-                item["definition"],
                 item["projectType"],
                 item["storageLocation"],
                 VcsUri.from_dict(item["vcsUri"]) if item.get("vcsUri") else None,
                 self._sal,
             )
             for item in resp["data"]["items"]
         ]
@@ -619,26 +614,25 @@
                 shared_definition, selections
             ).wait()
 
         """
         project_matchings = []
         matchings = self._sal.workspace.get_project_matchings(
             {"definition": shared_definition.to_dict()}
-        )['data']['vcs']
+        )["data"]["vcs"]
         for entry in matchings:
             projects = [
                 Project(
                     project["id"],
-                    project["definition"],
                     project["projectType"],
                     project["storageLocation"],
                     VcsUri.from_dict(project["vcsUri"]),
                     self._sal,
                 )
-                for project in entry['projects']
+                for project in entry["projects"]
             ]
 
             project_matchings.append(
                 ProjectMatching(
                     entry["entryId"], str(VcsUri.from_dict(entry["uri"])), projects
                 )
             )
@@ -721,7 +715,94 @@
         Example::
 
             pw_client = client.get_published_workspaces_client()
             pw_client.get_by_id("2h98hciwsniucwincj")
 
         """
         return PublishedWorkspacesClient(self._sal)
+
+    def get_me(self) -> User:
+        """Return the User class object for the logged in user.
+
+        Example::
+
+            user = client.get_me()
+            user_tenant_group_name = user.tenant.group_name
+
+        """
+        user = self._sal.users.get_me()["data"]
+        return User.from_dict(user)
+
+    @Experimental
+    def get_case_by_reference(self, reference: CaseReference) -> Case:
+        """Return the Case class object given a CaseReference class.
+
+        Args:
+            reference: A CaseReference class object.
+
+        Returns:
+            A Case class object.
+
+        Example::
+
+            case_def = case.get_definition()
+            baseline_case_ref = case_def.custom_function.parameter_values[
+                "baseline_case"]
+            case = client.get_case_by_reference(baseline_case_ref)
+
+        """
+        return Case.from_reference(reference)
+
+    @Experimental
+    def get_experiment_by_reference(self, reference: ExperimentReference) -> Experiment:
+        """Return the Experiment class object given a ExperimentReference class.
+
+        Args:
+            reference: An ExperimentReference class object.
+
+        Returns:
+            An Experiment class object.
+
+        Example::
+
+            exp_def = experiment.get_definition()
+            experiment_ref = exp_def.custom_function.parameter_values[
+                "reference_experiment"]
+            exp = client.get_experiment_by_reference(experiment_ref)
+
+        """
+        return Experiment.from_reference(reference)
+
+
+@dataclass
+class Tenant:
+    id: str
+    group_name: str
+
+    @classmethod
+    def from_dict(cls, tenant_data: Dict[str, Any]) -> Tenant:
+        return Tenant(id=tenant_data["id"], group_name=tenant_data["groupName"])
+
+
+@dataclass
+class User:
+    id: str
+    username: str
+    firstname: str
+    last_name: str
+    email: str
+    license: str
+    roles: List[str]
+    tenant: Tenant
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> User:
+        return User(
+            id=data["id"],
+            username=data["username"],
+            firstname=data["firstName"],
+            last_name=data["lastName"],
+            email=data["email"],
+            license=data["license"],
+            roles=data["roles"],
+            tenant=Tenant.from_dict(tenant_data=data["tenant"]),
+        )
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/configuration.py` & `modelon_impact_client-4.0.0/modelon/impact/client/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,24 @@
     Can be overridden by the environment variable IMPACT_PYTHON_CLIENT_EXPERIMENTAL.
 
     """
     experimental_env = os.environ.get("IMPACT_PYTHON_CLIENT_EXPERIMENTAL", "false")
     return experimental_env.lower() in ("1", "true")
 
 
+def get_client_experiments_v3_experimental() -> bool:
+    """If the client should use the new experimental V3 schema for experiments.
+
+    Can be overridden by the environment variable IMPACT_PYTHON_CLIENT_V3_EXPERIMENTS.
+
+    """
+    experimental_env = os.environ.get("IMPACT_PYTHON_CLIENT_V3_EXPERIMENTS", "false")
+    return experimental_env.lower() in ("1", "true")
+
+
 class Experimental:
     def __init__(self, fn: Callable):
         self.fn = fn
 
     def __set_name__(self, owner: str, name: str) -> None:
         if get_client_experimental():
             setattr(owner, name, self.fn)
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/credential_manager.py` & `modelon_impact_client-4.0.0/modelon/impact/client/credential_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return None
 
         with open(credentials_file, "r") as credentials:
             return credentials.read().strip()
 
     def get_key_from_prompt(self) -> str:
         key = getpass(self._interactive_help_text)
-        if key == '\x16':
+        if key == "\x16":
             # This is a getpass Windows bug...
             logger.error("Does not support Ctrl+V on Windows")
             return self.get_key_from_prompt()
 
         return key
 
     def write_key_to_file(self, api_key: str) -> None:
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/asserts.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/case.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/case.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,33 @@
 import os
 import tempfile
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Text, Tuple, Union
 
 from modelon.impact.client import exceptions
 from modelon.impact.client.entities.asserts import assert_successful_operation
+from modelon.impact.client.entities.custom_function import CustomFunction
 from modelon.impact.client.entities.external_result import ExternalResult
-from modelon.impact.client.entities.interfaces.case import CaseInterface
+from modelon.impact.client.entities.interfaces.case import CaseReference
 from modelon.impact.client.entities.log import Log
+from modelon.impact.client.entities.model import (
+    Model,
+    SimpleModelicaExperimentDefinition,
+)
 from modelon.impact.client.entities.model_executable import ModelExecutable
 from modelon.impact.client.entities.result import Result
 from modelon.impact.client.entities.status import CaseStatus
 from modelon.impact.client.operations.base import BaseOperation
 from modelon.impact.client.operations.case import CaseOperation
 from modelon.impact.client.sal.experiment import ResultFormat
 
 if TYPE_CHECKING:
     from modelon.impact.client.sal.experiment import ExperimentService
     from modelon.impact.client.sal.service import Service
+
 logger = logging.getLogger(__name__)
 
 
 def _assert_case_is_complete(
     status: CaseStatus, operation_name: str = "Operation"
 ) -> None:
     if status == CaseStatus.NOT_STARTED:
@@ -97,15 +103,15 @@
         """
         return self._datetime_finished
 
 
 class CaseAnalysis:
     """Class containing Case analysis configuration."""
 
-    __slots__ = ['_analysis']
+    __slots__ = ["_analysis"]
 
     def __init__(self, analysis: Dict[str, Any]):
         self._analysis = analysis
 
     @property
     def analysis_function(self) -> str:
         """Custom function name.
@@ -114,15 +120,15 @@
             The name of the custom function.
 
         Example::
 
             analysis_function = case.input.analysis.analysis_function
 
         """
-        return self._analysis['analysis_function']
+        return self._analysis["analysis_function"]
 
     @property
     def parameters(self) -> Dict[str, Any]:
         """Get or set parameters for the custom function. Parameters are a dictionary
         containing the custom function parameters.
 
         Example::
@@ -131,19 +137,19 @@
             case.input.analysis.parameters = {'start_time': 0, 'final_time': 90}
 
 
             # Get the custom function parameters
             parameters = case.input.analysis.parameters
 
         """
-        return self._analysis['parameters']
+        return self._analysis["parameters"]
 
     @parameters.setter
     def parameters(self, parameters: Dict[str, Any]) -> None:
-        self._analysis['parameters'] = parameters
+        self._analysis["parameters"] = parameters
 
     @property
     def simulation_options(self) -> Dict[str, Any]:
         """Get or set the simulation options. Options are key-value pairs of simulation
         options.
 
         Example::
@@ -151,19 +157,19 @@
             # Set the custom function parameters
             case.input.analysis.simulation_options = {'ncp': 600}
 
             # Get the custom function parameters
             simulation_options = case.input.analysis.simulation_options
 
         """
-        return self._analysis['simulation_options']
+        return self._analysis["simulation_options"]
 
     @simulation_options.setter
     def simulation_options(self, simulation_options: Dict[str, Any]) -> None:
-        self._analysis['simulation_options'] = simulation_options
+        self._analysis["simulation_options"] = simulation_options
 
     @property
     def solver_options(self) -> Dict[str, Any]:
         """Get or set the simulation options. Options are key-value pairs of solver
         options.
 
         Example::
@@ -172,19 +178,19 @@
             case.input.analysis.solver_options = {'atol': 1e-9}
 
 
             # Get the solver options
             solver_options = case.input.analysis.solver_options
 
         """
-        return self._analysis['solver_options']
+        return self._analysis["solver_options"]
 
     @solver_options.setter
     def solver_options(self, solver_options: Dict[str, Any]) -> None:
-        self._analysis['solver_options'] = solver_options
+        self._analysis["solver_options"] = solver_options
 
     @property
     def simulation_log_level(self) -> str:
         """Get or set the simulation log level. Supported options are- 'WARNING',
         'ERROR', 'DEBUG', 'INFO' and 'VERBOSE'.
 
         Example::
@@ -192,19 +198,19 @@
             # Set the solver options
             case.input.analysis.simulation_log_level = "WARNING"
 
             # Get the solver options
             simulation_log_level = case.input.analysis.simulation_log_level
 
         """
-        return self._analysis['simulation_log_level']
+        return self._analysis["simulation_log_level"]
 
     @simulation_log_level.setter
     def simulation_log_level(self, simulation_log_level: str) -> None:
-        self._analysis['simulation_log_level'] = simulation_log_level
+        self._analysis["simulation_log_level"] = simulation_log_level
 
 
 class CustomArtifact:
     """CustomArtifact class."""
 
     def __init__(
         self,
@@ -281,15 +287,15 @@
 
         return result_stream
 
 
 class CaseMeta:
     """Class containing Case meta."""
 
-    __slots__ = ['_data']
+    __slots__ = ["_data"]
 
     def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
     def label(self) -> str:
         """Get or set the label for the case.
@@ -299,32 +305,32 @@
             # Set the case label
             case.meta.label = 'Cruise condition'
 
             # Get the case label
             label = case.meta.label
 
         """
-        return self._data['label']
+        return self._data["label"]
 
     @label.setter
     def label(self, label: str) -> None:
-        self._data['label'] = label
+        self._data["label"] = label
 
 
 class CaseInput:
     """Class containing Case input."""
 
-    __slots__ = ['_data']
+    __slots__ = ["_data"]
 
     def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
     def analysis(self) -> CaseAnalysis:
-        return CaseAnalysis(self._data['analysis'])
+        return CaseAnalysis(self._data["analysis"])
 
     @property
     def parametrization(self) -> Dict[str, Any]:
         """Get or set the parametrization of the case. Parameterization is defined as a
         dict of key value pairs where key is variable name and value is the value to use
         for that variable.
 
@@ -334,50 +340,50 @@
             case.input.parametrization = {'PI.k': 120}
 
 
             # Get the case parametrization
             parametrization = case.input.parametrization
 
         """
-        return self._data['parametrization']
+        return self._data["parametrization"]
 
     @parametrization.setter
     def parametrization(self, parametrization: Dict[str, Any]) -> None:
-        self._data['parametrization'] = parametrization
+        self._data["parametrization"] = parametrization
 
     @property
     def fmu_id(self) -> str:
         """Reference ID to the compiled model used running the case."""
-        return self._data['fmu_id']
+        return self._data["fmu_id"]
 
     @property
     def structural_parametrization(self) -> Dict[str, Any]:
         """Structural parametrization of the case, a list of key value pairs where key
         is variable name and value is the value to use for that variable.
 
         These are values that cannot be applied to the FMU/Model after compilation.
 
         """
-        return self._data['structural_parametrization']
+        return self._data["structural_parametrization"]
 
     @property
     def fmu_base_parametrization(self) -> Dict[str, Any]:
         """This is some base parametrization that must be applied to the FMU for it to
         be valid running this case.
 
         It often comes as a result from of caching to reuse the FMU.
 
         """
-        return self._data['fmu_base_parametrization']
+        return self._data["fmu_base_parametrization"]
 
 
-class Case(CaseInterface):
+class Case(CaseReference):
     """Class containing Case functionalities."""
 
-    __slots__ = ['_case_id', '_workspace_id', '_exp_id', '_sal', '_info']
+    __slots__ = ["_case_id", "_workspace_id", "_exp_id", "_sal", "_info"]
 
     def __init__(
         self,
         case_id: str,
         workspace_id: str,
         exp_id: str,
         service: Service,
@@ -400,24 +406,14 @@
             self._info = self._sal.experiment.case_get(
                 self._workspace_id, self._exp_id, self.id
             )
 
         return self._info
 
     @property
-    def id(self) -> str:
-        """Case id."""
-        return self._case_id
-
-    @property
-    def experiment_id(self) -> str:
-        """Experiment id."""
-        return self._exp_id
-
-    @property
     def info(self) -> Dict[str, Any]:
         """Deprecated, use 'run_info' attribute."""
         logger.warning("This attribute is deprectated, use 'run_info' instead")
         return self._get_info(cached=False)
 
     @property
     def run_info(self) -> CaseRunInfo:
@@ -441,30 +437,30 @@
             case.input.parametrization = {'PI.k': 120}
             case.sync()
 
             help(case.input.analysis) # See help for attribute
             dir(case.input) # See nested attributes
 
         """
-        return CaseInput(self._info['input'])
+        return CaseInput(self._info["input"])
 
     @property
     def meta(self) -> CaseMeta:
         """Case meta attributes.
 
         Example::
 
             case.meta.label = 'Cruise condition'
             case.sync()
 
             help(case.meta) # See help for attribute
             dir(case.input) # See nested attributes
 
         """
-        return CaseMeta(self._info['meta'])
+        return CaseMeta(self._info["meta"])
 
     @property
     def initialize_from_case(self) -> Optional[Case]:
         """Get(if any) or set the case to initialize from.
 
         Example::
 
@@ -482,36 +478,36 @@
             case_init_successful = case_2.execute().wait()
 
 
             # Get the case set to initialize from
             initialized_from_case = case.initialize_from_case
 
         """
-        init_from_dict = self._info['input'].get('initialize_from_case')
+        init_from_dict = self._info["input"].get("initialize_from_case")
         if init_from_dict is None:
             return None
 
-        experiment_id = init_from_dict.get('experimentId')
-        case_id = init_from_dict.get('caseId')
+        experiment_id = init_from_dict.get("experimentId")
+        case_id = init_from_dict.get("caseId")
 
         case_data = self._sal.experiment.case_get(
             self._workspace_id, experiment_id, case_id
         )
         return Case(
             case_data["id"], self._workspace_id, experiment_id, self._sal, case_data
         )
 
     @initialize_from_case.setter
     def initialize_from_case(self, case: Case) -> None:
         if not isinstance(case, Case):
             raise TypeError("The value must be an instance of Case")
-        self._assert_unique_case_initialization('initialize_from_external_result')
-        self._info['input']['initialize_from_case'] = {
-            'experimentId': case.experiment_id,
-            'caseId': case.id,
+        self._assert_unique_case_initialization("initialize_from_external_result")
+        self._info["input"]["initialize_from_case"] = {
+            "experimentId": case.experiment_id,
+            "caseId": case.id,
         }
 
     @property
     def initialize_from_external_result(self) -> Optional[ExternalResult]:
         """Get(if any) or set the external result file to initialize from.
 
         Example::
@@ -528,29 +524,29 @@
             case_init_successful = case_2.execute().wait()
 
 
             # Get the external result file to initialize from
             initialize_from_external_result = case.initialize_from_external_result
 
         """
-        init_from_dict = self._info['input'].get('initialize_from_external_result')
+        init_from_dict = self._info["input"].get("initialize_from_external_result")
 
         if init_from_dict is None:
             return None
 
-        result_id = init_from_dict.get('uploadId')
+        result_id = init_from_dict.get("uploadId")
 
         return ExternalResult(result_id, self._sal)
 
     @initialize_from_external_result.setter
     def initialize_from_external_result(self, result: ExternalResult) -> None:
         if not isinstance(result, ExternalResult):
             raise TypeError("The value must be an instance of ExternalResult")
-        self._assert_unique_case_initialization('initialize_from_case')
-        self._info['input']['initialize_from_external_result'] = {"uploadId": result.id}
+        self._assert_unique_case_initialization("initialize_from_case")
+        self._info["input"]["initialize_from_external_result"] = {"uploadId": result.id}
 
     def is_successful(self) -> bool:
         """Returns True if a case has completed successfully.
 
         Returns:
             True, if the case has executed successfully, False,
             if the case has failed execution.
@@ -576,15 +572,15 @@
         """
         return Log(
             self._sal.experiment.case_get_log(
                 self._workspace_id, self._exp_id, self._case_id
             )
         )
 
-    def get_result(self, format: str = 'mat') -> Tuple[Union[bytes, Text], str]:
+    def get_result(self, format: str = "mat") -> Tuple[Union[bytes, Text], str]:
         """Returns the result stream and the file name for a finished case.
 
         Args:
             format: The file format to download the result in. The only possible values
                 are 'mat' and 'csv'. Default: 'mat'
 
         Returns:
@@ -676,17 +672,17 @@
         )
         meta = next(
             (meta for meta in resp["data"]["items"] if meta["id"] == artifact_id),
             None,
         )
         if not meta:
             raise exceptions.NoSuchCustomArtifactError(
-                f'No custom artifact found with ID: {artifact_id}.'
+                f"No custom artifact found with ID: {artifact_id}."
             )
-        return meta['downloadAs']
+        return meta["downloadAs"]
 
     def get_artifacts(self) -> List[CustomArtifact]:
         """Returns a list of CustomArtifact classes for a finished case.
 
         Returns:
             A list of CustomArtifact class objects.
 
@@ -704,16 +700,16 @@
             self._workspace_id, self._exp_id, self._case_id
         )
         return [
             CustomArtifact(
                 self._workspace_id,
                 self.experiment_id,
                 self._case_id,
-                meta['id'],
-                meta['downloadAs'],
+                meta["id"],
+                meta["downloadAs"],
                 self._sal.experiment,
             )
             for meta in resp["data"]["items"]
         ]
 
     def get_fmu(
         self,
@@ -727,15 +723,20 @@
 
             case = experiment.get_case('case_1')
             fmu = case.get_fmu()
             fmus = set(case.get_fmu() for case in exp.get_cases())
 
         """
         fmu_id = self.input.fmu_id
-
+        if not fmu_id:
+            custom_function = self._get_custom_function()
+            for param in custom_function.parameter_values.values():
+                if isinstance(param, CaseReference):
+                    case = self.from_reference(param)
+                    fmu_id = case.input.fmu_id
         return ModelExecutable(self._workspace_id, fmu_id, self._sal)
 
     def sync(self) -> None:
         """Sync case state against server, pushing any changes that has been done to the
         object client side.
 
         Example::
@@ -778,20 +779,83 @@
                 self._workspace_id, self._exp_id, [self._case_id]
             ),
             self._case_id,
             self._sal,
             Case.from_operation,
         )
 
+    def _get_custom_function(self) -> CustomFunction:
+        custom_function_meta = self._sal.custom_function.custom_function_get(
+            self._workspace_id, self.input.analysis.analysis_function
+        )
+        custom_function_params = self.input.analysis.parameters
+        return CustomFunction(
+            self._workspace_id,
+            custom_function_meta["name"],
+            custom_function_meta["parameters"],
+            self._sal,
+        ).with_parameters(**custom_function_params)
+
+    def get_definition(self) -> SimpleModelicaExperimentDefinition:
+        """Get an experiment definition that can be used to reproduce this case result.
+
+        Returns:
+            An instance of SimpleModelicaExperimentDefinition class.
+
+        Example::
+
+            definition = case.get_definition()
+
+        """
+        custom_function = self._get_custom_function()
+        fmu = self.get_fmu()
+        model = Model(
+            fmu.input.class_name,
+            workspace_id=self._workspace_id,
+            project_id="",
+            service=self._sal,
+        )
+        definition = SimpleModelicaExperimentDefinition(
+            model=model,
+            custom_function=custom_function,
+            compiler_options=fmu.input.compiler_options,
+            fmi_target=fmu.input.fmi_target,
+            fmi_version=fmu.input.fmi_version,
+            platform=fmu.input.platform,
+            compiler_log_level=fmu.input.compiler_log_level,
+            runtime_options=fmu.input.runtime_options,
+            solver_options=self.input.analysis.solver_options,
+            simulation_options=self.input.analysis.simulation_options,
+            simulation_log_level=self.input.analysis.simulation_log_level,
+            initialize_from=self.initialize_from_case
+            or self.initialize_from_external_result,
+        )
+        modifiers = {
+            **self.input.structural_parametrization,
+            **self.input.parametrization,
+        }
+        definition = definition.with_modifiers(modifiers=modifiers)
+        return definition
+
     def _assert_unique_case_initialization(self, unsupported_init: str) -> None:
-        if self._info['input'][unsupported_init]:
+        if self._info["input"][unsupported_init]:
             raise ValueError(
                 "A case cannot use both 'initialize_from_case' and "
                 "'initialize_from_external_result' to specify what to initialize from! "
                 f"To resolve this, set the '{unsupported_init}' attribute "
                 "to None and re-try."
             )
 
     @classmethod
     def from_operation(cls, operation: BaseOperation[Case], **kwargs: Any) -> Case:
         assert isinstance(operation, CaseOperation)
         return cls(**kwargs, service=operation._sal)
+
+    @classmethod
+    def from_reference(cls, reference: CaseReference) -> Case:
+        return cls(
+            case_id=reference._case_id,
+            workspace_id=reference._workspace_id,
+            exp_id=reference._exp_id,
+            service=reference._sal,
+            info=reference._info,
+        )
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/content.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/content.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     from modelon.impact.client.operations.base import BaseOperation
 
 
 @enum.unique
 class ContentType(enum.Enum):
     """Supported content types in a project."""
 
-    MODELICA = 'MODELICA'
-    VIEWS = 'VIEWS'
-    FAVORITES = 'FAVORITES'
-    CUSTOM_FUNCTIONS = 'CUSTOM_FUNCTIONS'
-    REFERENCE_RESULTS = 'REFERENCE_RESULTS'
-    EXPERIMENT_DEFINITIONS = 'EXPERIMENT_DEFINITIONS'
-    GENERIC = 'GENERIC'
+    MODELICA = "MODELICA"
+    VIEWS = "VIEWS"
+    FAVORITES = "FAVORITES"
+    CUSTOM_FUNCTIONS = "CUSTOM_FUNCTIONS"
+    REFERENCE_RESULTS = "REFERENCE_RESULTS"
+    EXPERIMENT_DEFINITIONS = "EXPERIMENT_DEFINITIONS"
+    GENERIC = "GENERIC"
 
 
 class ProjectContent:
     """Content entry in a project."""
 
     def __init__(self, content: Dict[str, str], project_id: str, service: Service):
         self._content = content
@@ -41,34 +41,34 @@
     @property
     def relpath(self) -> Path:
         """Relative path in the project.
 
         Can be file (e.g., SomeLib.mo) or folder
 
         """
-        return Path(self._content['relpath'])
+        return Path(self._content["relpath"])
 
     @property
     def content_type(self) -> ContentType:
         """Type of content."""
-        return ContentType(self._content['contentType'])
+        return ContentType(self._content["contentType"])
 
     @property
     def id(self) -> str:
         """Content ID."""
-        return self._content['id']
+        return self._content["id"]
 
     @property
     def name(self) -> Optional[str]:
         """Modelica library name."""
-        return self._content.get('name')
+        return self._content.get("name")
 
     @property
     def default_disabled(self) -> str:
-        return self._content['defaultDisabled']
+        return self._content["defaultDisabled"]
 
     def delete(self) -> None:
         """Deletes a project content.
 
         Example::
 
             content.delete()
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,35 @@
 import enum
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from modelon.impact.client import exceptions
 from modelon.impact.client.entities.asserts import assert_variable_in_result
 from modelon.impact.client.entities.case import Case
-from modelon.impact.client.entities.interfaces.experiment import ExperimentInterface
+from modelon.impact.client.entities.custom_function import CustomFunction
+from modelon.impact.client.entities.external_result import ExternalResult
+from modelon.impact.client.entities.interfaces.experiment import ExperimentReference
+from modelon.impact.client.entities.model import (
+    Model,
+    SimpleModelicaExperimentDefinition,
+)
+from modelon.impact.client.entities.model_executable import (
+    ModelExecutable,
+    SimpleFMUExperimentDefinition,
+)
 from modelon.impact.client.entities.status import ExperimentStatus
+from modelon.impact.client.experiment_definition.expansion import (
+    ExpansionAlgorithm,
+    FullFactorial,
+    LatinHypercube,
+    Sobol,
+)
+from modelon.impact.client.experiment_definition.extension import (
+    SimpleExperimentExtension,
+)
 from modelon.impact.client.operations import experiment
 from modelon.impact.client.options import (
     CompilerOptions,
     RuntimeOptions,
     SimulationOptions,
     SolverOptions,
 )
@@ -20,14 +39,18 @@
 if TYPE_CHECKING:
     from modelon.impact.client.operations.base import BaseOperation
     from modelon.impact.client.sal.service import Service
 
 logger = logging.getLogger(__name__)
 
 ScalarValue = Union[float, int, str]
+ValidExperimentDefinitions = Union[
+    SimpleModelicaExperimentDefinition,
+    SimpleFMUExperimentDefinition,
+]
 
 
 @enum.unique
 class _TrajectoryResponseFormat(enum.Enum):
     V1 = "application/vnd.impact.trajectories.v1+json"
     V2 = "application/vnd.impact.trajectories.v2+json"
 
@@ -67,16 +90,16 @@
         ]
 
 
 @enum.unique
 class _Workflow(enum.Enum):
     """Workflow type."""
 
-    FMU_BASED = 'FMU_BASED'
-    CLASS_BASED = 'CLASS_BASED'
+    FMU_BASED = "FMU_BASED"
+    CLASS_BASED = "CLASS_BASED"
 
 
 def _assert_experiment_is_complete(
     status: ExperimentStatus, operation_name: str = "Operation"
 ) -> None:
     if status == ExperimentStatus.NOTSTARTED:
         raise exceptions.OperationNotCompleteError.for_operation(operation_name, status)
@@ -167,41 +190,33 @@
 
     @property
     def label(self) -> Optional[str]:
         """Experiment label."""
         return self._meta_data.get("label")
 
 
-class Experiment(ExperimentInterface):
+class Experiment(ExperimentReference):
     """Class containing Experiment functionalities."""
 
     def __init__(
         self,
         workspace_id: str,
         exp_id: str,
         service: Service,
         info: Optional[Dict[str, Any]] = None,
     ):
-        self._exp_id = exp_id
-        self._workspace_id = workspace_id
-        self._sal = service
-        self._info = info
+        super().__init__(workspace_id, exp_id, service, info)
         self._fmu_info: Optional[Dict[str, Any]] = None
 
     def __eq__(self, obj: object) -> bool:
         return isinstance(obj, Experiment) and obj._exp_id == self._exp_id
 
     def __repr__(self) -> str:
         return f"Experiment with id '{self._exp_id}'"
 
-    @property
-    def id(self) -> str:
-        """Experiment id."""
-        return self._exp_id
-
     def _get_info(self, cached: bool = True) -> Dict[str, Any]:
         if not cached or self._info is None:
             self._info = self._sal.workspace.experiment_get(
                 self._workspace_id, self._exp_id
             )
 
         return self._info
@@ -447,16 +462,15 @@
     def get_last_point(
         self, variables: Optional[List[str]] = None
     ) -> ExperimentResultPoint:
         """Returns a ExperimentResultPoint class for a list of result variables for all
         the cases.
 
         Args:
-            variables: An optional list of result variables to fetch
-            trajectories for.
+            variables: An optional list of variables to fetch results for.
 
         Returns:
             An ExperimentResultPoint class object.
 
         Raises:
             OperationNotCompleteError if simulation process is in progress.
             OperationFailureError if simulation process was cancelled.
@@ -495,20 +509,27 @@
         Example::
 
             experiment.delete()
 
         """
         self._sal.experiment.experiment_delete(self._workspace_id, self._exp_id)
 
+    @property
+    def label(self) -> Optional[str]:
+        """Returns the experiment label if it exists."""
+        return self.metadata.label
+
     def set_label(self, label: str) -> None:
-        """Sets a label (string) for an experiment to distinguish it.
+        """Sets a label (string) for an experiment to distinguish it. To get the label,
+        you could call the experiment.label property.
 
         Example::
 
             experiment.set_label("Engine run with Oil type B")
+            label = experiment.label
 
         """
         self._sal.experiment.experiment_set_label(
             self._workspace_id, self._exp_id, label
         )
 
     @classmethod
@@ -534,42 +555,197 @@
         return _Workflow.CLASS_BASED if model.get("modelica") else _Workflow.FMU_BASED
 
     def get_class_name(self) -> str:
         """Return the model class name."""
         model = self._get_info()["experiment"]["base"]["model"]
         if self._get_workflow() == _Workflow.CLASS_BASED:
             return model["modelica"]["className"]
-        return self._get_fmu_info(model["fmu"]["id"])['input']["class_name"]
+        return self._get_fmu_info(model["fmu"]["id"])["input"]["class_name"]
 
     def get_compiler_options(self) -> CompilerOptions:
         """Return a CompilerOptions object."""
         model = self._get_info()["experiment"]["base"]["model"]
         if self._get_workflow() == _Workflow.CLASS_BASED:
             return CompilerOptions(
                 model["modelica"].get("compilerOptions", {}), self.custom_function
             )
-        fmu_info = self._get_fmu_info(model["fmu"]["id"])['input']
+        fmu_info = self._get_fmu_info(model["fmu"]["id"])["input"]
         return CompilerOptions(
             fmu_info.get("compiler_options", {}), self.custom_function
         )
 
     def get_runtime_options(self) -> RuntimeOptions:
         """Return a RuntimeOptions object."""
         model = self._get_info()["experiment"]["base"]["model"]
         if self._get_workflow() == _Workflow.CLASS_BASED:
             return RuntimeOptions(
                 model["modelica"].get("runtimeOptions", {}), self.custom_function
             )
-        fmu_info = self._get_fmu_info(model["fmu"]["id"])['input']
+        fmu_info = self._get_fmu_info(model["fmu"]["id"])["input"]
         return RuntimeOptions(fmu_info.get("runtime_options", {}), self.custom_function)
 
     def get_simulation_options(self) -> SimulationOptions:
         """Return a SimulationOptions object."""
         analysis = self._get_info()["experiment"]["base"]["analysis"]
         return SimulationOptions(
             analysis.get("simulationOptions", {}), self.custom_function
         )
 
     def get_solver_options(self) -> SolverOptions:
         """Return a SolverOptions object."""
         analysis = self._get_info()["experiment"]["base"]["analysis"]
         return SolverOptions(analysis.get("solverOptions", {}), self.custom_function)
+
+    def _get_initialize_from_case(self, experiment_id: str, case_id: str) -> Case:
+        case_data = self._sal.experiment.case_get(
+            self._workspace_id, experiment_id, case_id
+        )
+        return Case(
+            case_data["id"], self._workspace_id, experiment_id, self._sal, case_data
+        )
+
+    def _get_initialize_from_experiment(self, experiment_id: str) -> Experiment:
+        resp = self._sal.workspace.experiment_get(self._workspace_id, experiment_id)
+        return Experiment(self._workspace_id, resp["id"], self._sal, resp)
+
+    def _get_initialize_from(
+        self, modifiers: Dict[str, Any]
+    ) -> Optional[Union[Case, Experiment, ExternalResult]]:
+        if "initializeFrom" in modifiers:
+            exp_id = modifiers["initializeFrom"]
+            return self._get_initialize_from_experiment(exp_id)
+        elif "initializeFromCase" in modifiers:
+            case_id = modifiers["initializeFromCase"]["caseId"]
+            exp_id = modifiers["initializeFromCase"]["experimentId"]
+            return self._get_initialize_from_case(exp_id, case_id)
+        elif "initializeFromExternalResult" in modifiers:
+            ext_result_id = modifiers["initializeFromExternalResult"]
+            return ExternalResult(result_id=ext_result_id, service=self._sal)
+        return None
+
+    def _get_extension_initialize_from(
+        self, modifiers: Dict[str, Any]
+    ) -> Optional[Union[Case, Experiment]]:
+        if "initializeFrom" in modifiers:
+            exp_id = modifiers["initializeFrom"]
+            return self._get_initialize_from_experiment(exp_id)
+        elif "initializeFromCase" in modifiers:
+            case_id = modifiers["initializeFromCase"]["caseId"]
+            exp_id = modifiers["initializeFromCase"]["experimentId"]
+            return self._get_initialize_from_case(exp_id, case_id)
+        return None
+
+    def get_definition(self) -> ValidExperimentDefinitions:
+        """Get an experiment definition that can be used to reproduce this experiment
+        result.
+
+        Returns:
+            An instance of SimpleFMUExperimentDefinition or
+            SimpleModelicaExperimentDefinition class.
+
+        Example::
+
+            definition = experiment.get_definition()
+
+        """
+        base = self._get_info(cached=False)["experiment"]["base"]
+        analysis = base["analysis"]
+        custom_function = self._get_custom_function(analysis)
+        if self._get_workflow() == _Workflow.CLASS_BASED:
+            model = Model(
+                self.get_class_name(),
+                workspace_id=self._workspace_id,
+                project_id="",
+                service=self._sal,
+            )
+            modelica = base["model"]["modelica"]
+            definition = SimpleModelicaExperimentDefinition(
+                model=model,
+                custom_function=custom_function,
+                compiler_options=self.get_compiler_options(),
+                fmi_target=modelica["fmiTarget"],
+                fmi_version=modelica["fmiVersion"],
+                platform=modelica["platform"],
+                compiler_log_level=modelica["compilerLogLevel"],
+                runtime_options=self.get_runtime_options(),
+                solver_options=self.get_solver_options(),
+                simulation_options=self.get_simulation_options(),
+                simulation_log_level=analysis["simulationLogLevel"],
+                initialize_from=self._get_initialize_from(base["modifiers"]),
+            )
+            expansion = base.get("expansion", {})
+            expansion = self._get_expansion_algorithm(
+                expansion.get("algorithm"), expansion.get("parameters", {})
+            )
+            definition = definition.with_expansion(expansion=expansion)
+        else:
+            fmu_id = base["model"]["fmu"]["id"]
+            definition = SimpleFMUExperimentDefinition(
+                fmu=ModelExecutable(self._workspace_id, fmu_id, self._sal),
+                custom_function=custom_function,
+                solver_options=self.get_solver_options(),
+                simulation_options=self.get_simulation_options(),
+                simulation_log_level=analysis["simulationLogLevel"],
+                initialize_from=self._get_initialize_from(base["modifiers"]),
+            )  # type: ignore
+        modifiers = base["modifiers"]["variables"]
+        definition = definition.with_modifiers(modifiers=modifiers)
+        extensions = self._get_info()["experiment"].get("extensions")
+        if extensions:
+            sim_exts = []
+            for extension in extensions:
+                analysis = extension.get("analysis", {})
+                sim_ext = SimpleExperimentExtension(
+                    parameter_modifiers=analysis.get("parameters"),
+                    solver_options=analysis.get("solverOptions"),
+                    simulation_options=analysis.get("simulationOptions"),
+                    simulation_log_level=analysis.get("simulationLogLevel"),
+                    initialize_from=self._get_extension_initialize_from(
+                        extension["modifiers"]
+                    )
+                    if extension.get("modifiers")
+                    else None,
+                )
+                sim_ext = sim_ext.with_modifiers(
+                    modifiers=extension.get("modifiers", {}).get("variables")
+                )
+                case_data = extension.get("caseData", [])
+                case_labels = [data.get("label") for data in case_data]
+                if case_labels:
+                    case_label = case_labels[0]
+                    sim_ext = sim_ext.with_case_label(case_label)
+                sim_exts.append(sim_ext)
+            definition = definition.with_extensions(sim_exts)
+        return definition
+
+    def _get_custom_function(self, analysis: Dict[str, Any]) -> CustomFunction:
+        custom_function_meta = self._sal.custom_function.custom_function_get(
+            self._workspace_id, self.custom_function
+        )
+        custom_function_params = analysis["parameters"]
+        return CustomFunction(
+            self._workspace_id,
+            custom_function_meta["name"],
+            custom_function_meta["parameters"],
+            self._sal,
+        ).with_parameters(**custom_function_params)
+
+    def _get_expansion_algorithm(
+        self, algorithm: str, parameters: Dict[str, Any]
+    ) -> ExpansionAlgorithm:
+        if algorithm == "SOBOL":
+            return Sobol(samples=parameters["samples"])
+        elif algorithm == "LATINHYPERCUBE":
+            return LatinHypercube(
+                samples=parameters["samples"], seed=parameters.get("seed")
+            )
+        else:
+            return FullFactorial()
+
+    @classmethod
+    def from_reference(cls, reference: ExperimentReference) -> Experiment:
+        return cls(
+            workspace_id=reference._workspace_id,
+            exp_id=reference._exp_id,
+            service=reference._sal,
+            info=reference._info,
+        )
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/external_result.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/model.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,30 +343,29 @@
 
         """
         resp = self._sal.project.project_get(
             self._project_id, vcs_info=False, size_info=False
         )
         project = Project(
             resp["id"],
-            resp["definition"],
             resp["projectType"],
             resp["storageLocation"],
             None,
             self._sal,
         )
         modelica_content = project.get_modelica_library_by_name(self._class_name)
         if not modelica_content:
             raise ValueError(
                 f"No modelica package with name {self._class_name} exists "
                 f"in the Project - '{project.name}'"
             )
         class_name = class_name or ".".join(
             [
                 self._class_name,
-                os.path.split(fmu_path)[-1].strip('.fmu'),
+                os.path.split(fmu_path)[-1].strip(".fmu"),
             ]
         )
         resp = self._sal.project.fmu_import(
             self._project_id,
             modelica_content.id,
             fmu_path,
             class_name,
@@ -374,15 +373,15 @@
             include_patterns,
             exclude_patterns,
             top_level_inputs,
             step_size=step_size,
         )
 
         return FMUImportOperation[Model](
-            resp['data']['location'],
+            resp["data"]["location"],
             self._workspace_id,
             self._project_id,
             self._sal,
             Model.from_operation,
         )
 
     @classmethod
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/model_executable.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/model_executable.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             model_description.show()
             model_description.download()
 
         """
         if path is None:
             path = os.path.join(tempfile.gettempdir(), "impact-downloads")
         os.makedirs(path, exist_ok=True)
-        artifact_path = os.path.join(path, 'modelDescription.xml')
+        artifact_path = os.path.join(path, "modelDescription.xml")
         with open(artifact_path, mode="w", encoding="utf-8") as f:
             f.write(self)
         return artifact_path
 
 
 class ModelExecutableRunInfo:
     def __init__(self, status: ModelExecutableStatus, errors: List[str]):
@@ -108,14 +108,58 @@
 
         Is empty unless 'status' attribute is 'FAILED'
 
         """
         return self._errors
 
 
+class ModelExecutableInput:
+    """Class containing ModelExecutable input."""
+
+    __slots__ = ["_data"]
+
+    def __init__(self, data: Dict[str, Any]):
+        self._data = data
+
+    @property
+    def class_name(self) -> str:
+        """Returns the model class name."""
+        return self._data["class_name"]
+
+    @property
+    def compiler_log_level(self) -> str:
+        """Returns the compiler log level."""
+        return self._data["compiler_log_level"]
+
+    @property
+    def compiler_options(self) -> Dict[str, Any]:
+        """Returns the compiler options dict."""
+        return self._data["compiler_options"]
+
+    @property
+    def runtime_options(self) -> Dict[str, Any]:
+        """Returns the runtime options dict."""
+        return self._data["runtime_options"]
+
+    @property
+    def fmi_target(self) -> str:
+        """Returns the FMI target."""
+        return self._data["fmi_target"]
+
+    @property
+    def fmi_version(self) -> str:
+        """Returns the FMI version."""
+        return self._data["fmi_version"]
+
+    @property
+    def platform(self) -> str:
+        """Returns the platform the FMU was compiled for."""
+        return self._data["platform"]
+
+
 class ModelExecutable(ModelExecutableInterface):
     """Class containing ModelExecutable functionalities."""
 
     def __init__(
         self,
         workspace_id: str,
         fmu_id: str,
@@ -176,14 +220,28 @@
         """
         assert_successful_operation(self.is_successful(), "Compilation")
         parameter_state = {"parameterState": self._variable_modifiers()}
         return self._sal.model_executable.ss_fmu_metadata_get(
             self._workspace_id, self._fmu_id, parameter_state
         )
 
+    @property
+    def input(self) -> ModelExecutableInput:
+        """ModelExecutable input attributes.
+
+        Example::
+
+            compiled_platform = fmu.input.platform
+
+            help(fmu.input.platform) # See help for attribute
+            dir(fmu.input) # See nested attributes
+
+        """
+        return ModelExecutableInput(self._get_info()["input"])
+
     def get_class_name(self) -> str:
         """Return the model class name."""
         return self._get_info()["input"]["class_name"]
 
     def is_successful(self) -> bool:
         """Returns True if the model has compiled successfully. Use the 'run_info'
         attribute to get more info.
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/project.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 from modelon.impact.client.options import ProjectExecutionOptions
 from modelon.impact.client.sal.service import Service
 
 if TYPE_CHECKING:
     from modelon.impact.client.operations.base import BaseOperation
 
 logger = logging.getLogger(__name__)
-RepoURL = Union['GitRepoURL', 'SvnRepoURL']
+RepoURL = Union["GitRepoURL", "SvnRepoURL"]
 
 
 @enum.unique
 class ProjectType(enum.Enum):
     """Type of project."""
 
-    LOCAL = 'LOCAL'
-    RELEASED = 'RELEASED'
-    SYSTEM = 'SYSTEM'
+    LOCAL = "LOCAL"
+    RELEASED = "RELEASED"
+    SYSTEM = "SYSTEM"
 
 
 @enum.unique
 class StorageLocation(enum.Enum):
     """The storage location of the project."""
 
-    APPMODE = 'APPMODE'
-    USERSPACE = 'USERSPACE'
-    SYSTEM = 'SYSTEM'
+    APPMODE = "APPMODE"
+    USERSPACE = "USERSPACE"
+    SYSTEM = "SYSTEM"
 
 
 @dataclass
 class GitRepoURL:
     """GitRepoURL represents a project referenced in a git repository String
     representation is url[@[refname][:sha1]]"""
 
@@ -51,19 +51,19 @@
 
     sha1: str = ""
     """Commit hash."""
 
     def __str__(self) -> str:
         repo_url = self.url
         if self.refname or self.sha1:
-            repo_url += '@'
+            repo_url += "@"
         if self.refname:
             repo_url += self.refname
         if self.sha1:
-            repo_url += ':' + self.sha1
+            repo_url += ":" + self.sha1
         return repo_url
 
     @classmethod
     def from_dict(cls, data: Any) -> GitRepoURL:
         return cls(
             url=data.get("url"), refname=data.get("refname"), sha1=data.get("sha1")
         )
@@ -96,26 +96,26 @@
             and self.branch == other.branch
             and self.url_from_root == other.url_from_root
         )
 
     def get_rev(self) -> str:
         rev = self.rev
         if rev == "":
-            return 'HEAD'
+            return "HEAD"
         return rev
 
     def __str__(self) -> str:
         segments = [self.root_url]
         if self.branch:
             segments.append(self.branch)
         if self.url_from_root:
             segments.append(self.url_from_root)
-        repo_url = '/'.join(segments)
+        repo_url = "/".join(segments)
         if self.rev:
-            repo_url += '@' + self.rev
+            repo_url += "@" + self.rev
         return repo_url
 
     @classmethod
     def from_dict(cls, data: Any) -> SvnRepoURL:
         return cls(
             root_url=data.get("rootUrl"),
             branch=data.get("branch"),
@@ -143,15 +143,15 @@
     def from_dict(cls, data: Any) -> VcsUri:
         repo_url = data.get("repoUrl")
         service_kind = data.get("serviceKind")
         return cls(
             service_kind=service_kind,
             service_url=data.get("serviceUrl"),
             repourl=GitRepoURL.from_dict(repo_url)
-            if service_kind.lower() == 'git'
+            if service_kind.lower() == "git"
             else SvnRepoURL.from_dict(repo_url),
             protocol=data.get("protocol"),
             subdir=data.get("subdir"),
         )
 
 
 class ProjectDependency:
@@ -159,20 +159,20 @@
 
     def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
     def name(self) -> Optional[str]:
         """The name of the project dependency."""
-        return self._data.get('name')
+        return self._data.get("name")
 
     @property
     def version_specifier(self) -> Optional[str]:
         """Version specifier."""
-        return self._data.get('versionSpecifier')
+        return self._data.get("versionSpecifier")
 
 
 class ProjectDefinition:
     """Impact project definition."""
 
     def __init__(self, data: Dict[str, Any]):
         self._data = data
@@ -187,53 +187,47 @@
 
     @property
     def format(self) -> str:
         return self._data["format"]
 
     @property
     def dependencies(self) -> List[ProjectDependency]:
-        dependencies = self._data.get('dependencies', [])
+        dependencies = self._data.get("dependencies", [])
         return [ProjectDependency(dependency) for dependency in dependencies]
 
     @property
     def content(self) -> list:
-        return self._data.get('content', [])
+        return self._data.get("content", [])
 
     @property
     def execution_options(self) -> List[ProjectExecutionOptions]:
-        execution_options = self._data.get('executionOptions', [])
+        execution_options = self._data.get("executionOptions", [])
         return [
             ProjectExecutionOptions(
-                execution_option, execution_option['customFunction']
+                execution_option, execution_option["customFunction"]
             )
             for execution_option in execution_options
         ]
 
     def to_dict(self) -> Dict[str, Any]:
         return self._data
 
 
 class Project:
     """Class containing Project functionalities."""
 
     def __init__(
         self,
         project_id: str,
-        project_definition: Union[ProjectDefinition, Dict[str, Any]],
         project_type: Union[ProjectType, str],
         storage_location: Union[StorageLocation, str],
         vcs_uri: Optional[VcsUri],
         service: Service,
     ):
         self._project_id = project_id
-        self._project_definition = (
-            ProjectDefinition(project_definition)
-            if isinstance(project_definition, dict)
-            else project_definition
-        )
         self._vcs_uri = vcs_uri or None
         self._project_type = (
             ProjectType(project_type) if isinstance(project_type, str) else project_type
         )
         self._storage_location = (
             StorageLocation(storage_location)
             if isinstance(storage_location, str)
@@ -257,34 +251,55 @@
         """Project name."""
         return self.definition.name
 
     @property
     def size(self) -> float:
         """Project size in bytes."""
         return self._sal.project.project_get(self.id, vcs_info=False, size_info=True)[
-            'size'
+            "size"
         ]
 
     @property
     def definition(self) -> ProjectDefinition:
-        return self._project_definition
+        """Project definition."""
+        definition = self._sal.project.project_get(
+            project_id=self.id, size_info=False, vcs_info=False
+        )["definition"]
+        return ProjectDefinition(definition)
 
     @property
     def vcs_uri(self) -> Optional[VcsUri]:
         """Project vcs uri."""
         return self._vcs_uri
 
     @property
     def project_type(self) -> ProjectType:
         return self._project_type
 
     @property
     def storage_location(self) -> StorageLocation:
         return self._storage_location
 
+    def rename(self, new_name: str) -> None:
+        """Renames a project.
+
+        Args:
+            name: The new name for the project.
+
+        Example::
+
+            project.rename('renamed project')
+
+        """
+        prj_data = self._sal.project.project_get(
+            project_id=self.id, vcs_info=False, size_info=False
+        )
+        prj_data["definition"]["name"] = new_name
+        self._sal.project.project_put(self.id, prj_data)
+
     def delete(self) -> None:
         """Deletes a project.
 
         Example::
 
             project.delete()
 
@@ -299,16 +314,15 @@
 
         Example::
 
             project.get_contents()
 
         """
         return [
-            self._get_project_content(content)
-            for content in self._project_definition.content
+            self._get_project_content(content) for content in self.definition.content
         ]
 
     def get_content(self, content_id: str) -> ProjectContent:
         """Gets the project content with the given ID.
 
         Args:
             content_id: The ID of the workspace.
@@ -377,15 +391,15 @@
             project.import_content('/home/test.mo', ContentType.MODELICA).wait()
 
         """
         resp = self._sal.project.project_content_upload(
             path_to_content, self._project_id, content_type.value
         )
         return ContentImportOperation[ProjectContent](
-            resp['data']['location'], self._sal, ProjectContent.from_operation
+            resp["data"]["location"], self._sal, ProjectContent.from_operation
         )
 
     def import_modelica_library(self, path_to_lib: str) -> ContentImportOperation:
         """Uploads/adds a non-encrypted Modelica library or a Modelica model to the
         project.
 
         Args:
@@ -395,15 +409,15 @@
 
         Example::
 
             content  = project.import_modelica_library('A.mo').wait()
             content  = project.import_modelica_library('B.zip').wait()
 
         """
-        if Path(path_to_lib).suffix.lower() not in ['.mo', '.zip']:
+        if Path(path_to_lib).suffix.lower() not in [".mo", ".zip"]:
             raise ValueError(
                 "Only '.mo' or '.zip' file extension are supported for uploading "
                 "Modelica content into project."
             )
         return self.import_content(path_to_lib, ContentType.MODELICA)
 
     def get_options(
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/result.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/status.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/status.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     CANCELLED = "cancelled"
     """Status for experiment execution that has not yet started."""
 
     NOT_STARTED = "not_started"
     """Status for experiment execution that has not yet started."""
 
-    STARTED = 'started'
+    STARTED = "started"
     """Status for case that has  started execution."""
 
 
 class ExperimentStatus(Enum):
     """Class representing an enumeration for the possible experiment run info states."""
 
     NOTSTARTED = "not_started"
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-4.0.0/modelon/impact/client/entities/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
 import enum
 import json
 import logging
 import os
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from modelon.impact.client.configuration import Experimental
 from modelon.impact.client.entities.custom_function import CustomFunction
 from modelon.impact.client.entities.experiment import Experiment
 from modelon.impact.client.entities.external_result import ExternalResult
 from modelon.impact.client.entities.interfaces.workspace import WorkspaceInterface
 from modelon.impact.client.entities.model import Model
 from modelon.impact.client.entities.model_executable import ModelExecutable
 from modelon.impact.client.entities.project import Project, VcsUri
+from modelon.impact.client.exceptions import (
+    NoAssociatedPublishedWorkspaceError,
+    RemotePublishedWorkspaceLinkError,
+)
 from modelon.impact.client.experiment_definition.interfaces.definition import (
     BaseExperimentDefinition,
 )
 from modelon.impact.client.operations.experiment import ExperimentOperation
 from modelon.impact.client.operations.external_result_import import (
     ExternalResultImportOperation,
 )
@@ -27,23 +31,24 @@
     WorkspaceConversionOperation,
 )
 from modelon.impact.client.operations.workspace.exports import (
     Export,
     WorkspaceExportOperation,
 )
 from modelon.impact.client.operations.workspace.imports import WorkspaceImportOperation
+from modelon.impact.client.sal.exceptions import HTTPError
 from modelon.impact.client.sal.service import Service
 
 if TYPE_CHECKING:
     from modelon.impact.client.operations.base import BaseOperation
 
 logger = logging.getLogger(__name__)
 
 ExperimentDefinition = Union[
-    Type[BaseExperimentDefinition],
+    BaseExperimentDefinition,
     Dict[str, Any],
 ]
 
 
 @dataclass
 class AccessSettings:
     group_names: Optional[List[str]] = None
@@ -115,72 +120,63 @@
 class PublishedWorkspaceUploadStatus(enum.Enum):
     INITIALIZING = "initializing"
     CREATED = "created"
     DELETING = "deleting"
 
 
 @dataclass
+class AppMode:
+    model: str
+
+
+@dataclass
 class PublishedWorkspaceDefinition:
     name: str
     tenant_id: str
     size: int
     status: PublishedWorkspaceUploadStatus
     owner_username: str
     created_at: int
+    app_mode: Optional[AppMode] = None
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> PublishedWorkspaceDefinition:
         return cls(
             name=data["workspaceName"],
             tenant_id=data["tenantId"],
             size=data["size"],
             status=PublishedWorkspaceUploadStatus(data["status"]),
             owner_username=data["ownerUsername"],
             created_at=data["createdAt"],
+            app_mode=AppMode(data["appMode"]["model"]) if data.get("appMode") else None,
         )
 
 
 @dataclass
 class PublishedWorkspaceRequester:
     id: str
     username: str
 
     @classmethod
     def from_dict(cls, userdata: Dict[str, Any]) -> PublishedWorkspaceRequester:
         return cls(id=userdata["id"], username=userdata["username"])
 
 
 @dataclass
-class PublishedWorkspacePermission:
-    id: str
-    name: str
-
-    @classmethod
-    def from_dict(cls, permissions: Dict[str, Any]) -> PublishedWorkspacePermission:
-        return cls(id=permissions["id"], name=permissions["name"])
-
-
-@dataclass
 class PublishedWorkspaceACL:
-    role_permissions: List[PublishedWorkspacePermission]
-    group_permissions: List[PublishedWorkspacePermission]
+    role_names: List[str]
+    group_names: List[str]
     shared_with: List[PublishedWorkspaceRequester]
     requested_by: List[PublishedWorkspaceRequester]
 
     @classmethod
     def from_dict(cls, acl: Dict[str, Any]) -> PublishedWorkspaceACL:
         return cls(
-            role_permissions=[
-                PublishedWorkspacePermission.from_dict(permission)
-                for permission in acl["rolePermissions"]
-            ],
-            group_permissions=[
-                PublishedWorkspacePermission.from_dict(permission)
-                for permission in acl["groupPermissions"]
-            ],
+            role_names=acl["roleNames"],
+            group_names=acl["groupNames"],
             shared_with=[
                 PublishedWorkspaceRequester.from_dict(requester)
                 for requester in acl["sharedWith"]
             ],
             requested_by=[
                 PublishedWorkspaceRequester.from_dict(requester)
                 for requester in acl["requestedBy"]
@@ -261,51 +257,81 @@
             username: Username of the user to grant access rights to.
 
         Example::
 
             published_workspace.grant_user_access('sasuke')
 
         """
-        self._sal.workspace.grant_published_workspace_access(self._id, username)
+        self._sal.workspace.grant_user_access(self._id, username)
 
     @Experimental
-    def grant_community_access(self) -> None:
-        """Grant community access for the published workspace.
+    def revoke_user_access(self, username: str) -> None:
+        """Revoke access for the published workspace.
+
+        Args:
+            username: Username of the user to revoke access rights from.
 
         Example::
 
-            published_workspace.grant_community_access()
+            published_workspace.revoke_user_access('naruto')
 
         """
-        self._sal.workspace.grant_community_access(self._id)
+        self._sal.workspace.revoke_user_access(self._id, username)
 
     @Experimental
-    def revoke_community_access(self) -> None:
-        """Revoke community access for the published workspace.
+    def grant_group_access(self, group_name: Optional[str] = None) -> None:
+        """Grant group access for the published workspace.
+
+        Args:
+            group_name: Name of the group to grant access rights to. If not
+            specified, the workspace is shared with the group the published workspace
+            owner belongs to.
 
         Example::
 
-            published_workspace.revoke_community_access()
+            published_workspace.grant_group_access('impact-tenant-org1')
 
         """
-        self._sal.workspace.revoke_community_access(self._id)
+        self._sal.workspace.grant_group_access(self._id, group_name)
 
     @Experimental
-    def revoke_access(self, username: str) -> None:
-        """Revoke access for the published workspace.
+    def revoke_group_access(self, group_name: str) -> None:
+        """Revoke group access for the published workspace.
 
         Args:
-            username: Username of the user to revoke access rights from.
+            group_name: Name of the group to revoke access rights from.
+
+        Example::
+
+            published_workspace.revoke_group_access('impact-tenant-org1')
+
+        """
+        self._sal.workspace.revoke_group_access(self._id, group_name)
+
+    @Experimental
+    def grant_community_access(self) -> None:
+        """Grant community access for the published workspace.
 
         Example::
 
-            published_workspace.grant_access('naruto')
+            published_workspace.grant_community_access()
 
         """
-        self._sal.workspace.revoke_published_workspace_access(self._id, username)
+        self._sal.workspace.grant_community_access(self._id)
+
+    @Experimental
+    def revoke_community_access(self) -> None:
+        """Revoke community access for the published workspace.
+
+        Example::
+
+            published_workspace.revoke_community_access()
+
+        """
+        self._sal.workspace.revoke_community_access(self._id)
 
     def _get_latest_local_workspace(self) -> Optional[Workspace]:
         resp = self._sal.workspace.workspaces_get(sharing_id=self._id)
         workspaces = [
             Workspace(item["id"], self._sal) for item in resp["data"]["items"]
         ]
         if not workspaces:
@@ -328,17 +354,16 @@
             update_if_available: If true, the workspace is updated with the
             latest copy from the cloud. Default is False.
 
         Returns:
             The workspace class object.
 
         Example::
-
-            published_workspace = client.get_published_workspaces(owner="username",
-                name="A Workspace")[0]
+            pw_client = client.get_published_workspaces_client()
+            published_workspace = pw_client.find(owner="sasuke", name="A workspace")[0]
             workspace = published_workspace.import_to_userspace()
 
         """
         local_workspace = self._get_latest_local_workspace()
         if local_workspace:
             logger.info(
                 f"Local imports of workspace with sharing ID {self._id} exists."
@@ -383,16 +408,16 @@
         """Returns the access control list for the published workspace.
 
         Returns:
             The PublishedWorkspaceACL class object.
 
         Example::
 
-            published_workspace = client.get_published_workspaces(owner="username",
-                name="A Workspace")[0]
+            pw_client = client.get_published_workspaces_client()
+            published_workspace = pw_client.find(owner="sasuke", name="A workspace")[0]
             published_workspace_acl = published_workspace.get_access_control_list()
 
             published_workspace_shared_with = published_workspace_acl.shared_with
             published_workspace_requested_by = published_workspace_acl.requested_by
 
         """
         data = self._sal.workspace.get_published_workspace_acl(self.id)
@@ -429,14 +454,97 @@
         return OwnerData(self._data["owner"])
 
     @property
     def created_at(self) -> int:
         return self._data["createdAt"]
 
 
+class ReceivedFromWorkspace:
+    def __init__(self, workspace: Workspace) -> None:
+        self._workspace = workspace
+        self._received_from = self._workspace.definition.received_from
+        if not self._received_from:
+            raise NoAssociatedPublishedWorkspaceError(
+                "The workspace has no link to a published workspace."
+            )
+
+    @property
+    def metadata(self) -> ReceivedFrom:
+        """Reference metadata for the published workspace."""
+        assert self._received_from
+        return self._received_from
+
+    def get_workspace(self) -> Optional[PublishedWorkspace]:
+        """Return the published workspace from which the workspace was imported from.
+        Returns None if workspace is not linked to any published workspace.
+
+        Returns:
+            An PublishedWorkspace class object.
+
+        Example::
+
+            published_ws = workspace.received_from.get_workspace()
+
+        """
+        try:
+            sharing_id = self.metadata.sharing_id
+            data = self._workspace._sal.workspace.get_published_workspace(sharing_id)
+        except HTTPError as e:
+            logger.warning(
+                f"Published workspace with ID: {sharing_id} doesn't exist. Cause{e}"
+            )
+            return None
+        definition = PublishedWorkspaceDefinition.from_dict(data)
+        return PublishedWorkspace(
+            data["id"], definition=definition, service=self._workspace._sal
+        )
+
+    def has_updates(self) -> Optional[bool]:
+        """Return True if there are updates available for the published workspace
+        corresponding to the local workspace(if any) else False.
+
+        Example::
+
+            has_updates = workspace.received_from.has_updates()
+
+        """
+        pw = self.get_workspace()
+        if not pw:
+            return None
+        local_ws_created_at = self.metadata.created_at  # type: ignore
+        return pw.created_at != local_ws_created_at
+
+    def _import_to_userspace(self, sharing_id: str) -> Workspace:
+        resp = self._workspace._sal.workspace.import_from_cloud(
+            sharing_id, self._workspace.id
+        )
+        return WorkspaceImportOperation[Workspace](
+            resp["data"]["location"],
+            self._workspace._sal,
+            Workspace.from_import_operation,
+        ).wait()
+
+    def update_userspace(self) -> Workspace:
+        """Returns the workspaces updated from the latest published one.
+
+        Example::
+
+            updated_workspace = workspace.received_from.update_userspace()
+
+        """
+        logger.info("Updating the workspace to the latest published workspace.")
+        pub_ws = self.get_workspace()
+        if not pub_ws:
+            raise NoAssociatedPublishedWorkspaceError(
+                "No published workspace found that are "
+                f"associated with local workspace with ID: {self._workspace.id}"
+            )
+        return self._import_to_userspace(sharing_id=pub_ws.id)
+
+
 class WorkspaceDefinition:
     def __init__(self, data: Any) -> None:
         self._data = data
 
     @property
     def name(self) -> str:
         """Workspace name."""
@@ -694,23 +802,23 @@
             An WorkspaceExportOperation class object.
 
         Example::
 
             path = workspace.export().wait().download_as('/home/workspace.zip')
 
             # Publish a workspace
-            path = workspace.export(publish=True,
-                class_path='Modelica.Blocks.Examples.PID_Controller')
+            workspace.export(publish=True,
+                class_path='Modelica.Blocks.Examples.PID_Controller').wait()
 
             # Publish a workspace without sharing with group
             from modelon.impact.client import AccessSettings
 
-            path = workspace.export(publish=True,
+            workspace.export(publish=True,
                 class_path='Modelica.Blocks.Examples.PID_Controller',
-                access=AccessSettings(group_names=[])
+                access=AccessSettings(group_names=[]).wait()
             )
 
         """
         if access:
             access_settings = {"groupNames": access.group_names}
         else:
             access_settings = None
@@ -933,15 +1041,14 @@
         """
         resp = self._sal.workspace.projects_get(
             self._workspace_id, vcs_info=vcs_info, include_disabled=include_disabled
         )
         projects = [
             Project(
                 item["id"],
-                item["definition"],
                 item["projectType"],
                 item["storageLocation"],
                 VcsUri.from_dict(item["vcsUri"]) if item.get("vcsUri") else None,
                 self._sal,
             )
             for item in resp["data"]["items"]
         ]
@@ -968,15 +1075,14 @@
         """
         resp = self._sal.workspace.dependencies_get(
             self._workspace_id, vcs_info, include_disabled
         )
         return [
             Project(
                 item["id"],
-                item["definition"],
                 item["projectType"],
                 item["storageLocation"],
                 VcsUri.from_dict(item["vcsUri"]) if item.get("vcsUri") else None,
                 self._sal,
             )
             for item in resp["data"]["items"]
         ]
@@ -991,15 +1097,14 @@
 
             project = workspace.create_project("test")
 
         """
         resp = self._sal.workspace.project_create(self._workspace_id, name)
         return Project(
             resp["id"],
-            resp["definition"],
             resp["projectType"],
             resp["storageLocation"],
             VcsUri.from_dict(resp["vcsUri"]) if resp.get("vcsUri") else None,
             self._sal,
         )
 
     def get_default_project(self) -> Project:
@@ -1021,15 +1126,14 @@
         resp = self._sal.project.project_get(
             default_project_id,
             vcs_info=True,
             size_info=False,
         )
         return Project(
             resp["id"],
-            resp["definition"],
             resp["projectType"],
             resp["storageLocation"],
             VcsUri.from_dict(resp["vcsUri"]) if resp.get("vcsUri") else None,
             self._sal,
         )
 
     def get_shared_definition(self, strict: bool = False) -> WorkspaceDefinition:
@@ -1109,7 +1213,63 @@
 
     @classmethod
     def from_conversion_operation(
         cls, operation: BaseOperation[Workspace], **kwargs: Any
     ) -> Workspace:
         assert isinstance(operation, WorkspaceConversionOperation)
         return cls(**kwargs, service=operation._sal)
+
+    @property
+    def received_from(self) -> ReceivedFromWorkspace:
+        """Returns an instance of ReceivedFromWorkspace class."""
+        return ReceivedFromWorkspace(self)
+
+    def get_published_workspace(
+        self, model_name: Optional[str] = None
+    ) -> Optional[PublishedWorkspace]:
+        """Returns the published workspace with the name matching this workspace.
+
+        Args:
+            model_name: Class path of the Modelica model. If specified,
+             an app mode published workspace corresponding to the local workspace
+             is returned(if it exists).
+
+        Returns:
+            An PublishedWorkspace class object.
+
+        Example::
+
+            published_ws = workspace.get_published_workspace()
+
+        """
+        recieved_from = self.definition.received_from
+        if recieved_from:
+            raise RemotePublishedWorkspaceLinkError(
+                "This workspace is imported from published workspace with ID:"
+                f"{recieved_from.sharing_id}. Use received_from.get_workspace()"
+                " to retrieve the information"
+            )
+        user = self._sal.users.get_me()["data"]
+        published_workspaces = self._sal.workspace.get_published_workspaces(
+            name=self.name,
+            owner_username=user["username"],
+            type=PublishedWorkspaceType.APP_MODE.value
+            if model_name
+            else PublishedWorkspaceType.ARCHIVE.value,
+        )["data"]["items"]
+        if model_name:
+            published_workspaces = [
+                pw
+                for pw in published_workspaces
+                if pw.get("appMode", {}).get("model") == model_name
+            ]
+        if not published_workspaces:
+            logger.warning(
+                "No published workspace corresponding to the local workspace with"
+                f" ID: {self.id} exist!"
+            )
+            return None
+        return PublishedWorkspace(
+            published_workspaces[0]["id"],
+            definition=PublishedWorkspaceDefinition.from_dict(published_workspaces[0]),
+            service=self._sal,
+        )
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/exceptions.py` & `modelon_impact_client-4.0.0/modelon/impact/client/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,7 +70,19 @@
 
 class ExternalResultUploadError(Error):
     pass
 
 
 class NoSuchCustomArtifactError(Error):
     pass
+
+
+class NoAssociatedPublishedWorkspaceError(Error):
+    pass
+
+
+class RemotePublishedWorkspaceLinkError(Error):
+    pass
+
+
+class AuthenticationError(Error):
+    pass
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/asserts.py` & `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/expansion.py` & `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/expansion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from modelon.impact.client.entities.interfaces.case import CaseInterface
 from modelon.impact.client.entities.interfaces.experiment import ExperimentInterface
 from modelon.impact.client.experiment_definition.interfaces.extension import (
     BaseExperimentExtension,
 )
+from modelon.impact.client.experiment_definition.modifiers import (
+    Modifier,
+    ensure_as_modifier,
+    modifiers_to_dict,
+)
 from modelon.impact.client.experiment_definition.operators import Operator
 from modelon.impact.client.experiment_definition.util import (
     case_to_identifier_dict,
+    custom_function_parameters_to_dict,
     get_options,
 )
 
 if TYPE_CHECKING:
     from modelon.impact.client.entities.case import Case
     from modelon.impact.client.entities.experiment import Experiment
 
@@ -90,18 +96,48 @@
         _validate_initialize_from(initialize_from)
         self._parameter_modifiers = (
             {} if parameter_modifiers is None else parameter_modifiers
         )
         self._solver_options = get_options(dict, solver_options)
         self._simulation_options = get_options(dict, simulation_options)
         self._simulation_log_level = simulation_log_level
-        self._variable_modifiers: Dict[str, Any] = {}
+        self._variable_modifiers: Dict[str, Modifier] = {}
         self._initialize_from = initialize_from
         self._case_label: Optional[str] = None
 
+    @property
+    def simulation_options(self) -> Dict[str, Any]:
+        "Returns the simulation options as a dict."
+        return self._simulation_options
+
+    @property
+    def solver_options(self) -> Dict[str, Any]:
+        "Returns the solver options as a dict."
+        return self._solver_options
+
+    @property
+    def simulation_log_level(self) -> Optional[str]:
+        "Returns the simulation log level, if set."
+        return self._simulation_log_level
+
+    @property
+    def modifiers(self) -> Dict[str, Any]:
+        "Returns the variable modifiers dict."
+        return self._variable_modifiers
+
+    @property
+    def case_label(self) -> Optional[str]:
+        "Returns the case label if any set."
+        return self._case_label
+
+    @property
+    def initialize_from(self) -> Optional[CaseOrExperiment]:
+        "Returns the case or experiment the experiment extension was initialized from."
+        return self._initialize_from
+
     def with_modifiers(
         self, modifiers: Optional[Dict[str, Any]] = None, **modifiers_kwargs: Any
     ) -> SimpleExperimentExtension:
         """Sets the modifiers variables for an experiment extension.
 
         Args:
             modifiers: A dictionary of variable modifiers.
@@ -134,18 +170,18 @@
             self._simulation_log_level,
             self._initialize_from,
         )
         new._case_label = self._case_label
         for variable, value in modifiers_aggregate.items():
             if isinstance(value, Operator):
                 raise ValueError(
-                    "Range operator is not supported when using extentions"
+                    "Operators are not supported when using extentions"
                     " in the experiment"
                 )
-            new._variable_modifiers[variable] = value
+            new._variable_modifiers[variable] = ensure_as_modifier(value)
         return new
 
     def with_case_label(self, case_label: str) -> SimpleExperimentExtension:
         """Sets the case label for an experiment extension.
 
         Args:
             case_label: A case label string.
@@ -172,18 +208,14 @@
             self._initialize_from,
         )
         new._variable_modifiers = self._variable_modifiers
         new._case_label = case_label
 
         return new
 
-    @property
-    def initialize_from(self) -> Optional[CaseOrExperiment]:
-        return self._initialize_from
-
     def with_initialize_from(
         self, entity: Optional[CaseOrExperiment] = None
     ) -> SimpleExperimentExtension:
         """Sets the experiment or case to initialize from for an experiment extension.
 
         Args:
             entity: An instance of Case or Experiment classes.
@@ -231,19 +263,23 @@
             ).with_modifiers({'PI.k': 40})
             simulate_ext.to_dict()
 
         """
         ext_dict: Dict[str, Any] = {}
         if self._variable_modifiers:
             ext_dict.setdefault("modifiers", {})
-            ext_dict["modifiers"]["variables"] = self._variable_modifiers
+            variable_modifiers = modifiers_to_dict(self._variable_modifiers)
+            ext_dict["modifiers"]["variables"] = variable_modifiers
 
         if self._parameter_modifiers:
             ext_dict.setdefault("analysis", {})
-            ext_dict["analysis"]["parameters"] = self._parameter_modifiers
+            custom_function_parameters = custom_function_parameters_to_dict(
+                self._parameter_modifiers
+            )
+            ext_dict["analysis"]["parameters"] = custom_function_parameters
 
         if self._solver_options:
             ext_dict.setdefault("analysis", {})
             ext_dict["analysis"]["solverOptions"] = self._solver_options
 
         if self._simulation_options:
             ext_dict.setdefault("analysis", {})
@@ -253,14 +289,15 @@
             ext_dict.setdefault("analysis", {})
             ext_dict["analysis"]["simulationLogLevel"] = self._simulation_log_level
 
         if isinstance(self.initialize_from, ExperimentInterface):
             ext_dict.setdefault("modifiers", {})
             ext_dict["modifiers"]["initializeFrom"] = self.initialize_from.id
         elif isinstance(self.initialize_from, CaseInterface):
+            ext_dict.setdefault("modifiers", {})
             ext_dict["modifiers"]["initializeFromCase"] = case_to_identifier_dict(
                 self.initialize_from
             )
 
         if self._case_label:
             ext_dict["caseData"] = [{"label": self._case_label}]
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/fmu_based.py` & `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/fmu_based.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,55 @@
         )
 
         self._simulation_log_level = simulation_log_level
         self._initialize_from = initialize_from
         self._variable_modifiers = fmu._variable_modifiers()
         self._extensions: List[SimpleExperimentExtension] = []
 
+    @property
+    def fmu(self) -> ModelExecutable:
+        """Returns the ModelExecutable class."""
+        return self._fmu
+
+    @property
+    def modifiers(self) -> Dict[str, Any]:
+        """Returns the variable modifiers dict."""
+        return self._variable_modifiers
+
+    @property
+    def simulation_options(self) -> Dict[str, Any]:
+        """Returns the simulation options as a dict."""
+        return self._simulation_options
+
+    @property
+    def solver_options(self) -> Dict[str, Any]:
+        """Returns the solver options as a dict."""
+        return self._solver_options
+
+    @property
+    def simulation_log_level(self) -> str:
+        """Returns the simulation log level."""
+        return self._simulation_log_level
+
+    @property
+    def custom_function(self) -> CustomFunction:
+        """Returns the custom function class."""
+        return self._custom_function
+
+    @property
+    def extensions(self) -> List[SimpleExperimentExtension]:
+        """Returns the list of experiment extensions."""
+        return self._extensions
+
+    @property
+    def initialize_from(self) -> Optional[CaseOrExperimentOrExternalResult]:
+        """Returns the case, experiment or result the experiment definition was
+        initialized from."""
+        return self._initialize_from
+
     def validate(self) -> None:
         add = set(self._variable_modifiers.keys()) - set(
             self._fmu.get_settable_parameters()
         )
         if add:
             raise KeyError(
                 f"Paramter(s) '{', '.join(add)}' {'are' if len(add)>1 else 'is'} "
@@ -151,14 +192,15 @@
             self._custom_function,
             self._solver_options,
             self._simulation_options,
             self._simulation_log_level,
             self._initialize_from,
         )
         new._extensions = self._extensions
+        new._variable_modifiers = self._variable_modifiers
         for variable, value in modifiers_aggregate.items():
             new._variable_modifiers[variable] = (
                 str(value) if isinstance(value, Operator) else value
             )
         return new
 
     def with_extensions(
@@ -247,23 +289,26 @@
                 .with_values(ncp=500)
             solver_options = {'atol':1e-8}
             simulate_def = fmu.new_experiment_definition(custom_function,
             solver_options, simulation_options)
             simulate_def.to_dict()
 
         """
+        custom_function_parameters = (
+            self._custom_function.parameter_values.as_raw_dict()
+        )
         exp_dict: Dict[str, Any] = {
             "experiment": {
                 "version": 2,
                 "base": {
                     "model": {"fmu": {"id": self._fmu.id}},
                     "modifiers": {"variables": self._variable_modifiers},
                     "analysis": {
                         "type": self._custom_function.name,
-                        "parameters": self._custom_function.parameter_values,
+                        "parameters": custom_function_parameters,
                         "simulationOptions": self._simulation_options,
                         "solverOptions": self._solver_options,
                         "simulationLogLevel": self._simulation_log_level,
                     },
                 },
                 "extensions": [ext.to_dict() for ext in self._extensions],
             }
@@ -278,18 +323,14 @@
             ] = case_to_identifier_dict(self.initialize_from)
         elif isinstance(self.initialize_from, ExternalResultInterface):
             exp_dict["experiment"]["base"]["modifiers"][
                 "initializeFromExternalResult"
             ] = self.initialize_from.id
         return exp_dict
 
-    @property
-    def initialize_from(self) -> Optional[CaseOrExperimentOrExternalResult]:
-        return self._initialize_from
-
     def with_initialize_from(
         self, entity: Optional[CaseOrExperimentOrExternalResult] = None
     ) -> SimpleFMUExperimentDefinition:
         """Sets the experiment or case to initialize from for an experiment.
 
         Args:
             entity: An instance of Case or Experiment or ExternalResult."
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/model_based.py` & `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/model_based.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
+from modelon.impact.client.configuration import get_client_experiments_v3_experimental
 from modelon.impact.client.entities.interfaces.case import CaseInterface
 from modelon.impact.client.entities.interfaces.experiment import ExperimentInterface
 from modelon.impact.client.entities.interfaces.external_result import (
     ExternalResultInterface,
 )
 from modelon.impact.client.experiment_definition.asserts import (
     assert_valid_args,
@@ -20,17 +21,22 @@
 )
 from modelon.impact.client.experiment_definition.extension import (
     SimpleExperimentExtension,
 )
 from modelon.impact.client.experiment_definition.interfaces.definition import (
     BaseExperimentDefinition,
 )
-from modelon.impact.client.experiment_definition.operators import Operator
+from modelon.impact.client.experiment_definition.modifiers import (
+    Modifier,
+    ensure_as_modifier,
+    modifiers_to_dict,
+)
 from modelon.impact.client.experiment_definition.util import (
     case_to_identifier_dict,
+    custom_function_parameters_to_dict,
     get_options,
 )
 
 if TYPE_CHECKING:
     from modelon.impact.client.entities.case import Case
     from modelon.impact.client.entities.custom_function import CustomFunction
     from modelon.impact.client.entities.experiment import Experiment
@@ -144,17 +150,93 @@
             custom_function.get_solver_options, solver_options
         )
         self._simulation_options = get_options(
             custom_function.get_simulation_options, simulation_options
         )
         self._simulation_log_level = simulation_log_level
         self._initialize_from = initialize_from
-        self._variable_modifiers: Dict[str, Any] = {}
+        self._variable_modifiers: Dict[str, Modifier] = {}
         self._extensions: List[SimpleExperimentExtension] = []
-        self._expansion = FullFactorial()
+        self._expansion: ExpansionAlgorithm = FullFactorial()
+
+    @property
+    def modifiers(self) -> Dict[str, Any]:
+        """Returns the variable modifiers dict."""
+        return self._variable_modifiers
+
+    @property
+    def model(self) -> Model:
+        """Returns the Model class."""
+        return self._model
+
+    @property
+    def fmi_target(self) -> str:
+        """Returns the FMI target."""
+        return self._fmi_target
+
+    @property
+    def fmi_version(self) -> str:
+        """Returns the FMI version."""
+        return self._fmi_version
+
+    @property
+    def platform(self) -> str:
+        """Returns the platform to compile FMU for."""
+        return self._platform
+
+    @property
+    def compiler_log_level(self) -> str:
+        """Returns the compiler log level."""
+        return self._compiler_log_level
+
+    @property
+    def compiler_options(self) -> Dict[str, Any]:
+        """Returns the compiler options as a dict."""
+        return self._compiler_options
+
+    @property
+    def runtime_options(self) -> Dict[str, Any]:
+        """Returns the runtime options as a dict."""
+        return self._runtime_options
+
+    @property
+    def simulation_options(self) -> Dict[str, Any]:
+        """Returns the simulation options as a dict."""
+        return self._simulation_options
+
+    @property
+    def solver_options(self) -> Dict[str, Any]:
+        """Returns the solver options as a dict."""
+        return self._solver_options
+
+    @property
+    def simulation_log_level(self) -> str:
+        """Returns the simulation log level."""
+        return self._simulation_log_level
+
+    @property
+    def custom_function(self) -> CustomFunction:
+        """Returns the custom function class."""
+        return self._custom_function
+
+    @property
+    def extensions(self) -> List[SimpleExperimentExtension]:
+        """Returns the list of experiment extensions."""
+        return self._extensions
+
+    @property
+    def expansion(self) -> ExpansionAlgorithm:
+        """Returns the expansion algorithm class."""
+        return self._expansion
+
+    @property
+    def initialize_from(self) -> Optional[CaseOrExperimentOrExternalResult]:
+        """Returns the case, experiment or result the experiment definition was
+        initialized from."""
+        return self._initialize_from
 
     def validate(self) -> None:
         raise NotImplementedError(
             "Validation is not supported for SimpleModelicaExperimentDefinition class"
         )
 
     def with_modifiers(
@@ -191,23 +273,22 @@
             solver_options=self._solver_options,
             simulation_options=self._simulation_options,
             simulation_log_level=self._simulation_log_level,
             initialize_from=self._initialize_from,
         )
         new._extensions = self._extensions
         new._expansion = self._expansion
+        new._variable_modifiers = self._variable_modifiers
 
-        for variable, value in modifiers.items():
-            new._variable_modifiers[variable] = (
-                str(value) if isinstance(value, Operator) else value
-            )
+        for name, value in modifiers.items():
+            new._variable_modifiers[name] = ensure_as_modifier(value)
         return new
 
     def with_expansion(
-        self, expansion: Optional[Type[ExpansionAlgorithm]] = None
+        self, expansion: Optional[ExpansionAlgorithm] = None
     ) -> SimpleModelicaExperimentDefinition:
         """Sets the expansion algorithm for an experiment.
 
         Args:
             expansion: An expansion algorithm. Available algorithms are LatinHypercube,
                 Sobol and FullFactorial.
                 Default: FullFactorial.
@@ -223,15 +304,15 @@
 
         """
         if not isinstance(expansion, ExpansionAlgorithm):
             raise TypeError(
                 f"The expansion argument is of type '{type(expansion)}' "
                 "which is not a subtype of 'ExpansionAlgorithm'!"
             )
-        expansion = expansion or FullFactorial()
+        new_expansion = expansion or FullFactorial()
         new = SimpleModelicaExperimentDefinition(
             model=self._model,
             custom_function=self._custom_function,
             compiler_options=self._compiler_options,
             fmi_target=self._fmi_target,
             fmi_version=self._fmi_version,
             platform=self._platform,
@@ -239,22 +320,18 @@
             runtime_options=self._runtime_options,
             solver_options=self._solver_options,
             simulation_options=self._simulation_options,
             simulation_log_level=self._simulation_log_level,
             initialize_from=self._initialize_from,
         )
         new._extensions = self._extensions
-        new._expansion = expansion
+        new._expansion = new_expansion
         new._variable_modifiers = self._variable_modifiers
         return new
 
-    @property
-    def initialize_from(self) -> Optional[CaseOrExperimentOrExternalResult]:
-        return self._initialize_from
-
     def with_initialize_from(
         self, entity: Optional[CaseOrExperimentOrExternalResult] = None
     ) -> SimpleModelicaExperimentDefinition:
         """Sets the experiment or case to initialize from for an experiment.
 
         Args:
             entity: An instance of Case or Experiment or ExternalResult.
@@ -394,33 +471,38 @@
                 solver_options=solver_options,
                 simulation_options=simulation_options
             )
             simulate_def.to_dict()
 
         """
 
+        version = 3 if get_client_experiments_v3_experimental() else 2
+        custom_function_parameters = custom_function_parameters_to_dict(
+            self._custom_function.parameter_values.as_raw_dict()
+        )
+        variable_modifiers = modifiers_to_dict(self._variable_modifiers)
         exp_dict: Dict[str, Any] = {
             "experiment": {
-                "version": 2,
+                "version": version,
                 "base": {
                     "model": {
                         "modelica": {
                             "className": self._model.name,
                             "compilerOptions": self._compiler_options,
                             "runtimeOptions": self._runtime_options,
                             "compilerLogLevel": self._compiler_log_level,
                             "fmiTarget": self._fmi_target,
                             "fmiVersion": self._fmi_version,
                             "platform": self._platform,
                         }
                     },
-                    "modifiers": {"variables": self._variable_modifiers},
+                    "modifiers": {"variables": variable_modifiers},
                     "analysis": {
                         "type": self._custom_function.name,
-                        "parameters": self._custom_function.parameter_values,
+                        "parameters": custom_function_parameters,
                         "simulationOptions": self._simulation_options,
                         "solverOptions": self._solver_options,
                         "simulationLogLevel": self._simulation_log_level,
                     },
                     "expansion": {"algorithm": str(self._expansion)},
                 },
                 "extensions": [ext.to_dict() for ext in self._extensions],
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/base.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     """Status for an operation that has been completed."""
 
 
 @enum.unique
 class AsyncOperationStatus(enum.Enum):
     """Defines all states for import."""
 
-    RUNNING = 'running'
+    RUNNING = "running"
     """Status for an async operation that is running."""
 
-    READY = 'ready'
+    READY = "ready"
     """Status for an async operation that is ready."""
 
-    ERROR = 'error'
+    ERROR = "error"
     """Status for an async operation that has errors."""
 
     def done(self) -> bool:
         return self in [AsyncOperationStatus.READY, AsyncOperationStatus.ERROR]
 
 
 class BaseOperation(Generic[Entity]):
@@ -125,15 +125,15 @@
                     f"Time exceeded the set timeout - {timeout}s! "
                     f"Present status of operation is {self.status.name}!"
                 )
 
             time.sleep(0.5)
 
     def cancel(self) -> None:
-        raise NotImplementedError('Cancel is not supported for this operation')
+        raise NotImplementedError("Cancel is not supported for this operation")
 
 
 class ExecutionOperation(BaseOperation[Entity]):
     """Execution operation class containing base functionality."""
 
     def is_complete(self) -> bool:
         """Returns True if the operation has completed.
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/case.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/content_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return (
             isinstance(obj, ContentImportOperation) and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Content import id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Project content import"
 
     def _info(self) -> Dict[str, Any]:
@@ -50,19 +50,19 @@
         """Returns a new ProjectContent class instance.
 
         Returns:
             A ProjectContent class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalContentImport(
                 f"Content import failed! Cause: {info['error'].get('message')}"
             )
-        project_id = self._location.split('/')[-3]
+        project_id = self._location.split("/")[-3]
         content_id = info["data"]["contentId"]
         resp = self._sal.project.project_content_get(project_id, content_id)
         return self._create_entity(self, content=resp, project_id=project_id)
 
     @property
     def status(self) -> AsyncOperationStatus:
         """Returns the upload status as an enumeration.
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/experiment.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/external_result_import.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/external_result_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             isinstance(obj, ExternalResultImportOperation)
             and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Result import id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Result import"
 
     def _info(self) -> Dict[str, Any]:
@@ -51,20 +51,20 @@
         """Returns a new ExternalResult class instance.
 
         Returns:
             A ExternalResult class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.ExternalResultUploadError(
                 f"External result upload failed! Cause: {info['error'].get('message')}"
             )
         resp = self._sal.external_result.get_uploaded_result(self.id)
-        return self._create_entity(self, result_id=resp['data']['id'])
+        return self._create_entity(self, result_id=resp["data"]["id"])
 
     @property
     def status(self) -> AsyncOperationStatus:
         """Returns the upload status as an enumeration.
 
         Returns:
             The AsyncOperationStatus enum. The status can have the enum values
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/fmu_import.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/fmu_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __eq__(self, obj: object) -> bool:
         return isinstance(obj, FMUImportOperation) and obj._location == self._location
 
     @property
     def id(self) -> str:
         """FMU import id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Model import"
 
     def _info(self) -> Dict[str, Any]:
@@ -58,15 +58,15 @@
         """Returns a new Model class instance.
 
         Returns:
             A Model class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalFMUImport(
                 f"FMU import failed! Cause: {info['error'].get('message')}"
             )
         if info.get("importWarnings"):
             logger.warning(f"Import Warnings: {'. '.join(info['importWarnings'])}")
 
         class_name = info["data"]["fmuClassPath"]
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/project_import.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/project_import.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return (
             isinstance(obj, ProjectImportOperation) and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Project import id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Project import"
 
     def _info(self) -> Dict[str, Any]:
@@ -50,24 +50,23 @@
         """Returns a new Project class instance.
 
         Returns:
             A Project class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalProjectImport(
                 f"Project import failed! Cause: {info['error'].get('message')}"
             )
         project_id = info["data"]["projectId"]
         resp = self._sal.project.project_get(project_id, False, False)
         return self._create_entity(
             self,
             project_id=resp["id"],
-            project_definition=resp["definition"],
             project_type=resp["projectType"],
             storage_location=resp["storageLocation"],
         )
 
     @property
     def status(self) -> AsyncOperationStatus:
         """Returns the upload status as an enumeration.
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             isinstance(obj, WorkspaceConversionOperation)
             and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Workspace conversion id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Workspace conversion"
 
     def _info(self) -> Dict[str, Any]:
@@ -53,15 +53,15 @@
         """Returns a Workspace class instance of the converted workspace.
 
         Returns:
             A Workspace class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalWorkspaceConversion(
                 f"Workspace conversion failed! Cause: {info['error'].get('message')}"
             )
 
         workspace_id = info["data"]["workspaceId"]
         resp = self._sal.workspace.workspace_get(workspace_id, False)
         return self._create_entity(
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/exports.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, export_service: ExportService, download_uri: str):
         self._export_sal = export_service
         self._download_uri = download_uri
 
     @property
     def id(self) -> str:
         """ID of the export."""
-        return self._download_uri.split('/')[-1]
+        return self._download_uri.split("/")[-1]
 
     def download_as(self, path_to_download: str) -> str:
         """Writes the binary archive to a file. Returns the path to downloaded archive.
 
         Args:
             path_to_download: The path to store the downloaded workspace.
 
@@ -72,15 +72,15 @@
             isinstance(obj, WorkspaceExportOperation)
             and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Workspace export id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Workspace export"
 
     def _info(self) -> Dict[str, Any]:
@@ -90,15 +90,15 @@
         """Returns a Export class instance.
 
         Returns:
             An Export class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalWorkspaceExport(
                 f"Workspace export failed! Cause: {info['error'].get('message')}"
             )
         return self._create_entity(self, download_uri=info["data"]["downloadUri"])
 
     @property
     def status(self) -> AsyncOperationStatus:
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             isinstance(obj, WorkspaceImportOperation)
             and obj._location == self._location
         )
 
     @property
     def id(self) -> str:
         """Workspace import id."""
-        return self._location.split('/')[-1]
+        return self._location.split("/")[-1]
 
     @property
     def name(self) -> str:
         """Return the name of operation."""
         return "Workspace import"
 
     def _info(self) -> Dict[str, Any]:
@@ -51,15 +51,15 @@
         """Returns a new Workspace class instance.
 
         Returns:
             A Workspace class instance.
 
         """
         info = self._info()
-        if info['status'] == AsyncOperationStatus.ERROR.value:
+        if info["status"] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalWorkspaceImport(
                 f"Workspace import failed! Cause: {info['error'].get('message')}"
             )
         workspace_id = info["data"]["workspaceId"]
         resp = self._sal.workspace.workspace_get(workspace_id, False)
         return self._create_entity(self, workspace_id=resp["id"])
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/options.py` & `modelon_impact_client-4.0.0/modelon/impact/client/options.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/published_workspace_client.py` & `modelon_impact_client-4.0.0/modelon/impact/client/published_workspace_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         *,
         name: str = "",
         first: int = 0,
         maximum: int = 20,
         has_data: bool = False,
         owner_username: str = "",
         type: Optional[PublishedWorkspaceType] = None,
+        group_name: Optional[str] = None,
     ) -> List[PublishedWorkspace]:
         """Returns a list of published workspaces. The snapshots could be filtered based
         on the key-worded arguments.
 
         Args:
             name: Name of the workspace.
             first: Index of first matching resource to return.
@@ -59,30 +60,39 @@
             status==PublishedWorkspaceUploadStatus.CREATED. If false
             returns everything.
             owner_username: If true, only workspaces published by the specified
             user are listed.
             type: Filter so only published workspace of a specified type are
                 returned. If not given all published workspace types are
                 returned.
+            group_name: Group name to query published workspaces for. Only
+                a user with impact-sys-admin role can query published workspaces
+                shared with a group other than his own.
 
         Returns:
             A list of published workspace class objects.
 
         Example::
 
             pw_client = client.get_published_workspaces_client()
             pw_client.find()
 
         """
         data = self._sal.workspace.get_published_workspaces(
-            name, first, maximum, has_data, owner_username, type.value if type else None
+            name,
+            first,
+            maximum,
+            has_data,
+            owner_username,
+            type.value if type else None,
+            group_name,
         )["data"]["items"]
         return [
             PublishedWorkspace(
-                item['id'],
+                item["id"],
                 definition=PublishedWorkspaceDefinition.from_dict(item),
                 service=self._sal,
             )
             for item in data
         ]
 
     def get_by_id(
@@ -100,22 +110,22 @@
         Example::
 
             pw_client = client.get_published_workspaces_client()
             pw_client.get("2h98hciwsniucwincj")
 
         """
         if request_if_no_access:
-            self._sal.workspace.request_published_workspace_access(sharing_id)
+            self._sal.workspace.request_user_access(sharing_id)
             logger.info(
                 "Access request sent for published workspaces with ID '%s'.", sharing_id
             )
             return None
         data = self._sal.workspace.get_published_workspace(sharing_id)
         definition = PublishedWorkspaceDefinition.from_dict(data)
-        return PublishedWorkspace(data['id'], definition=definition, service=self._sal)
+        return PublishedWorkspace(data["id"], definition=definition, service=self._sal)
 
     @Experimental
     def get_by_access_kind(
         self,
         access_kind: PublishedWorkspaceAccessKind = PublishedWorkspaceAccessKind.SHARED_BY_ME,  # noqa
         first: int = 0,
         maximum: int = 20,
@@ -141,22 +151,22 @@
 
         """
         data = self._sal.workspace.get_published_workspaces_by_kind(
             access_kind.value, first, maximum
         )["data"]["items"]
         return [
             PublishedWorkspaceAccess(
-                item['sharingId'],
-                item['requesterId'],
-                item['requesterUsername'],
+                item["sharingId"],
+                item["requesterId"],
+                item["requesterUsername"],
                 PublishedWorkspace(
-                    item['publishedWorkspace']['id'],
+                    item["publishedWorkspace"]["id"],
                     definition=PublishedWorkspaceDefinition.from_dict(
-                        item['publishedWorkspace']
+                        item["publishedWorkspace"]
                     ),
                     service=self._sal,
                 )
-                if 'publishedWorkspace' in item
+                if "publishedWorkspace" in item
                 else None,
             )
             for item in data
         ]
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     downloading results."""
 
     MAT = "mat"
     CSV = "csv"
 
     @classmethod
     def _missing_(cls, value: Any) -> Any:
-        if cls not in ['mat', 'csv']:
+        if cls not in ["mat", "csv"]:
             raise ValueError(
                 "Invalid result format! Allowed formats are 'mat' and 'csv."
             )
         return cls(value)
 
 
 class ExperimentService:
@@ -141,18 +141,18 @@
     ) -> Tuple[Union[Text, bytes], str]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}/result"
         ).resolve()
         if result_format == ResultFormat.CSV:
-            headers = {'Accept': 'text/csv'}
+            headers = {"Accept": "text/csv"}
             csv_resp = self._http_client.get_csv(url, headers=headers)
             return csv_resp.stream, csv_resp.file_name
-        headers = {'Accept': 'application/vnd.impact.mat.v1+octet-stream'}
+        headers = {"Accept": "application/vnd.impact.mat.v1+octet-stream"}
         mat_resp = self._http_client.get_mat(url, headers=headers)
         return mat_resp.stream, mat_resp.file_name
 
     def case_trajectories_get(
         self,
         workspace_id: str,
         experiment_id: str,
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/exports.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/external_result.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/external_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         }
         if label:
             options["name"] = label
         if description:
             options["description"] = description
         with open(path_to_result, "rb") as f:
             multipart_form_data = {
-                'file': f,
-                'options': json.dumps(options),
+                "file": f,
+                "options": json.dumps(options),
             }
             return self._http_client.post_json(url, files=multipart_form_data)
 
     def get_uploaded_result(self, result_id: str) -> Dict[str, Any]:
         url = (self._base_uri / f"api/external-result/{result_id}").resolve()
         return self._http_client.get_json(url)
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/http.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """HTTP client class."""
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
-from modelon.impact.client.jupyterhub.sal import JupyterContext
 from modelon.impact.client.sal.context import Context
 from modelon.impact.client.sal.request import (
     RequestCSV,
     RequestJSON,
     RequestMatStream,
     RequestOctetStream,
     RequestText,
@@ -17,16 +16,20 @@
     JSONResponse,
     MatStreamResponse,
     OctetStreamResponse,
 )
 
 
 class HTTPClient:
-    def __init__(self, context: Optional[Union[Context, JupyterContext]] = None):
+    def __init__(
+        self, api_key: Optional[str] = None, context: Optional[Context] = None
+    ):
         self._context = context if context else Context()
+        if api_key:
+            self._context.session.headers["impact-api-key"] = api_key
 
     def get_json(self, url: str, headers: Optional[Dict[str, Any]] = None) -> Any:
         return self.get_json_response(url, headers=headers).data
 
     def get_json_response(
         self, url: str, headers: Optional[Dict[str, Any]] = None
     ) -> JSONResponse:
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/project.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
     def projects_get(
         self,
         vcs_info: bool,
         project_type: Optional[ProjectType] = None,
         storage_location: Optional[StorageLocation] = None,
     ) -> Dict[str, Any]:
-        prj_type = '&type=' + project_type.value if project_type else ""
+        prj_type = "&type=" + project_type.value if project_type else ""
         stg_loc = (
-            '&storageLocation=' + storage_location.value if storage_location else ""
+            "&storageLocation=" + storage_location.value if storage_location else ""
         )
         url = (
             self._base_uri / f"api/projects?vcsInfo={vcs_info}{prj_type}{stg_loc}"
         ).resolve()
         return self._http_client.get_json(url)
 
     def project_get(
@@ -76,16 +76,16 @@
 
     def project_content_upload(
         self, path_to_result: str, project_id: str, content_type: str
     ) -> Dict[str, Any]:
         url = (self._base_uri / f"/api/projects/{project_id}/content-imports").resolve()
         with open(path_to_result, "rb") as f:
             multipart_form_data = {
-                'file': f,
-                'options': json.dumps({'contentType': content_type}),
+                "file": f,
+                "options": json.dumps({"contentType": content_type}),
             }
             return self._http_client.post_json(url, files=multipart_form_data)
 
     def project_content_get(self, project_id: str, content_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri / f"/api/projects/{project_id}/content/{content_id}"
         ).resolve()
@@ -118,16 +118,16 @@
         if exclude_patterns:
             options["excludePatterns"] = exclude_patterns
         if top_level_inputs:
             options["topLevelInputs"] = top_level_inputs
 
         with open(fmu_path, "rb") as f:
             multipart_form_data = {
-                'file': f,
-                'options': json.dumps(options),
+                "file": f,
+                "options": json.dumps(options),
             }
             return self._http_client.post_json(url, files=multipart_form_data)
 
     def import_from_zip(self, path_to_project: str) -> Dict[str, Any]:
         url = (self._base_uri / "api/project-imports").resolve()
         with open(path_to_project, "rb") as f:
             return self._http_client.post_json(url, files={"file": f})
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/request.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,33 +35,42 @@
         self.body = body
         self.files = files
         self.request_type = request_type
         self.headers = headers
 
     def execute(self, check_return: bool = True) -> Any:
         try:
+            extra_headers = self.headers or {}
+            headers = {**self.context.session.headers, **extra_headers}
             if self.method == "POST":
                 logger.debug("POST with JSON body: {}".format(self.body))
                 resp = self.context.session.post(
-                    self.url, json=self.body, files=self.files, headers=self.headers
+                    self.url,
+                    json=self.body,
+                    files=self.files,
+                    headers=headers,
                 )
             elif self.method == "GET":
-                resp = self.context.session.get(self.url, headers=self.headers)
+                resp = self.context.session.get(self.url, headers=headers)
             elif self.method == "PUT":
                 resp = self.context.session.put(
-                    self.url, json=self.body, headers=self.headers
+                    self.url,
+                    json=self.body,
+                    headers=headers,
                 )
             elif self.method == "PATCH":
                 resp = self.context.session.patch(
                     self.url,
                     json=self.body,
-                    headers=self.headers,
+                    headers=headers,
                 )
             elif self.method == "DELETE":
-                resp = self.context.session.delete(self.url, json=self.body)
+                resp = self.context.session.delete(
+                    self.url, json=self.body, headers=headers
+                )
             else:
                 raise NotImplementedError()
         except requests.exceptions.SSLError as exce:
             raise exceptions.SSLError(
                 "SSL error, could not verify connection. Please check that "
                 "certificates are setup correctly for the Modelon Impact server"
             ) from exce
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/response.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/response.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/uri.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/uri.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         self.content = content
 
     def resolve(self, **kwargs: Any) -> str:
         return self.content.format(**kwargs)
 
     def _with_path(self, path: str) -> URI:
-        return URI(urllib.parse.urljoin(self.content + "/", path.lstrip('/')))
+        return URI(urllib.parse.urljoin(self.content + "/", path.lstrip("/")))
 
     def __floordiv__(self, other: str) -> URI:
         return self._with_path(other)
 
     def __truediv__(self, other: str) -> URI:
         return self._with_path(other)
```

### Comparing `modelon_impact_client-3.9.0/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-4.0.0/modelon/impact/client/sal/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Workspace service module."""
 from typing import Any, Dict, List, Optional
 
+from modelon.impact.client.configuration import get_client_experiments_v3_experimental
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
 
 class WorkspaceService:
     def __init__(self, uri: URI, http_client: HTTPClient):
         self._base_uri = uri
         self._http_client = http_client
+        if get_client_experiments_v3_experimental():
+            self._experiment_schema = "application/vnd.impact.experiment.v3+json"
+        else:
+            self._experiment_schema = "application/vnd.impact.experiment.v2+json"
 
     def workspace_create(self, name: str) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspaces").resolve()
         return self._http_client.post_json(url, body={"new": {"name": name}})
 
     def workspace_delete(self, workspace_id: str) -> None:
         url = (self._base_uri / f"api/workspaces/{workspace_id}").resolve()
@@ -33,15 +38,15 @@
         query = {}
         if name:
             query["name"] = name
         if sharing_id:
             query["sharingId"] = sharing_id
         if only_app_mode:
             query["onlyAppMode"] = str(only_app_mode)
-        query_args = '&'.join(f'{key}={value}' for key, value in query.items())
+        query_args = "&".join(f"{key}={value}" for key, value in query.items())
         url = (self._base_uri / f"api/workspaces?{query_args}").resolve()
         return self._http_client.get_json(url)
 
     def projects_get(
         self, workspace_id: str, vcs_info: bool, include_disabled: bool
     ) -> Dict[str, Any]:
         url = (
@@ -73,23 +78,23 @@
         access_settings: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-exports").resolve()
         body = {"workspaceId": workspace_id, "publish": publish}
         if access_settings:
             body["access"] = access_settings
         if class_path:
-            body['appMode'] = {'model': class_path}
+            body["appMode"] = {"model": class_path}
         return self._http_client.post_json(url, body=body)
 
     def workspace_conversion_setup(
         self, workspace_id: str, backup_name: Optional[str]
     ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-conversions").resolve()
-        backup_data = {'backup': {'name': backup_name}} if backup_name else {}
-        body: Dict[str, Any] = {'data': {'workspaceId': workspace_id, **backup_data}}
+        backup_data = {"backup": {"name": backup_name}} if backup_name else {}
+        body: Dict[str, Any] = {"data": {"workspaceId": workspace_id, **backup_data}}
         return self._http_client.post_json(url, body=body)
 
     def get_workspace_conversion_status(self, location: str) -> Dict[str, Any]:
         url = (self._base_uri / location).resolve()
         return self._http_client.get_json(url)
 
     def fmus_get(self, workspace_id: str) -> Dict[str, Any]:
@@ -116,24 +121,24 @@
     ) -> Dict[str, Any]:
         class_path_query = f"?classPath={class_path}" if class_path else ""
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments{class_path_query}"
         ).resolve()
         return self._http_client.get_json(
-            url, headers={"Accept": "application/vnd.impact.experiment.v2+json"}
+            url, headers={"Accept": self._experiment_schema}
         )
 
     def experiment_get(self, workspace_id: str, experiment_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}"
         ).resolve()
         return self._http_client.get_json(
-            url, headers={"Accept": "application/vnd.impact.experiment.v2+json"}
+            url, headers={"Accept": self._experiment_schema}
         )
 
     def experiment_create(
         self,
         workspace_id: str,
         definition: Dict[str, Any],
         user_data: Optional[Dict[str, Any]] = None,
@@ -215,29 +220,32 @@
         self,
         name: str = "",
         first: int = 0,
         maximum: int = 20,
         has_data: bool = False,
         owner_username: str = "",
         type: Optional[str] = None,
+        group_name: Optional[str] = None,
     ) -> Dict[str, Any]:
         query = {}
         if name:
             query["workspaceName"] = name
         if has_data:
             query["hasData"] = str(has_data)
         if first > 0:
             query["first"] = str(first)
         if maximum >= 0:
             query["max"] = str(maximum)
         if owner_username:
             query["ownerUsername"] = owner_username
         if type:
             query["type"] = type
-        query_args = '&'.join(f'{key}={value}' for key, value in query.items())
+        if group_name:
+            query["groupName"] = group_name
+        query_args = "&".join(f"{key}={value}" for key, value in query.items())
         url = (self._base_uri / f"api/published-workspaces?{query_args}").resolve()
         resp = self._http_client.get_json_response(url)
         return resp.data
 
     def get_published_workspaces_by_kind(
         self,
         kind: str = "",
@@ -247,15 +255,15 @@
         query = {}
         if kind:
             query["kind"] = kind
         if first > 0:
             query["first"] = str(first)
         if maximum >= 0:
             query["max"] = str(maximum)
-        query_args = '&'.join(f'{key}={value}' for key, value in query.items())
+        query_args = "&".join(f"{key}={value}" for key, value in query.items())
         url = (
             self._base_uri / f"/api/published-workspaces/access/users?{query_args}"
         ).resolve()
         resp = self._http_client.get_json_response(url)
         return resp.data
 
     def get_published_workspace(self, sharing_id: str) -> Dict[str, Any]:
@@ -269,51 +277,68 @@
         ).resolve()
         resp = self._http_client.get_json_response(url)
         return resp.data
 
     def rename_published_workspace(self, sharing_id: str, workspace_name: str) -> None:
         url = (self._base_uri / f"api/published-workspaces/{sharing_id}").resolve()
         self._http_client.patch_json_no_response_body(
-            url, body={'workspaceName': workspace_name}
+            url, body={"workspaceName": workspace_name}
         )
 
-    def _access_request(
+    def _user_access_request(
         self, operation: str, sharing_id: str, username: Optional[str] = None
     ) -> None:
         url = (
             self._base_uri / f"api/published-workspaces/{sharing_id}/access/users"
         ).resolve()
         body = {"operation": operation}
         if username:
-            body['requesterUsername'] = username
+            body["requesterUsername"] = username
         self._http_client.patch_json_no_response_body(url, body=body)
 
-    def _community_access_request(
-        self, operation: str, sharing_id: str, username: Optional[str] = None
+    def _group_access_request(
+        self, operation: str, sharing_id: str, group_name: Optional[str] = None
     ) -> None:
         url = (
+            self._base_uri / f"api/published-workspaces/{sharing_id}/access/group"
+        ).resolve()
+        body = {"operation": operation}
+        if group_name:
+            body["groupName"] = group_name
+        self._http_client.patch_json_no_response_body(url, body=body)
+
+    def _community_access_request(self, operation: str, sharing_id: str) -> None:
+        url = (
             self._base_uri / f"api/published-workspaces/{sharing_id}/access/community"
         ).resolve()
         body = {"operation": operation}
         self._http_client.patch_json_no_response_body(url, body=body)
 
-    def request_published_workspace_access(self, sharing_id: str) -> None:
-        self._access_request('request', sharing_id)
+    def grant_group_access(
+        self, sharing_id: str, group_name: Optional[str] = None
+    ) -> None:
+        self._group_access_request("grant", sharing_id, group_name)
+
+    def revoke_group_access(self, sharing_id: str, group_name: str) -> None:
+        self._group_access_request("revoke", sharing_id, group_name)
+
+    def request_user_access(self, sharing_id: str) -> None:
+        self._user_access_request("request", sharing_id)
 
-    def grant_published_workspace_access(self, sharing_id: str, username: str) -> None:
-        self._access_request('grant', sharing_id, username)
+    def grant_user_access(self, sharing_id: str, username: str) -> None:
+        self._user_access_request("grant", sharing_id, username)
+
+    def revoke_user_access(self, sharing_id: str, username: str) -> None:
+        self._user_access_request("revoke", sharing_id, username)
 
     def grant_community_access(self, sharing_id: str) -> None:
-        self._community_access_request('grant', sharing_id)
+        self._community_access_request("grant", sharing_id)
 
     def revoke_community_access(self, sharing_id: str) -> None:
-        self._community_access_request('revoke', sharing_id)
-
-    def revoke_published_workspace_access(self, sharing_id: str, username: str) -> None:
-        self._access_request('revoke', sharing_id, username)
+        self._community_access_request("revoke", sharing_id)
 
     def delete_published_workspace(self, sharing_id: str) -> None:
         url = (self._base_uri / f"api/published-workspaces/{sharing_id}").resolve()
         self._http_client.delete_json(url)
 
     def update_workspace(
         self, workspace_id: str, data: Dict[str, Any]
```

### Comparing `modelon_impact_client-3.9.0/pyproject.toml` & `modelon_impact_client-4.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "3.9.0"
+version = "4.0.0"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
@@ -37,18 +37,20 @@
 docformatter = {extras = ["tomli"], version = "^1.7.5"}
 pytest = "^7.2.0"
 pytest-watch = "^4.2.0"
 pytest-cov = "^4.0.0"
 click = "^8.1.3"
 toml = "^0.10.2"
 requests_mock = "^1.10"
+vcrpy = "^6.0.1"
+pytest-vcr = "^1.0.2"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.1.1"
+sphinx-rtd-theme = "^2.0.0"
 sphinx-copybutton = "^0.5.1"
 sphinxcontrib-napoleon = "^0.7"
 sphinxcontrib-spelling = "^7.7.0"
 readthedocs-sphinx-search = "^0.3.1"
 sphinx-autodoc-typehints = "^1.22"
 
 [tool.docformatter]
```

### Comparing `modelon_impact_client-3.9.0/PKG-INFO` & `modelon_impact_client-4.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelon-impact-client
-Version: 3.9.0
+Version: 4.0.0
 Summary: Client library for easy scripting against Modelon Impact
 Home-page: https://www.modelon.com/modelon-impact
 License: BSD
 Keywords: impact,client,API
 Author: WEP
 Author-email: impact@modelon.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -19,83 +19,118 @@
 Requires-Dist: types-requests (>=2.27.30,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Project-URL: Documentation, https://modelon-impact-client.readthedocs.io
 Project-URL: Repository, https://github.com/modelon-community/impact-client-python
 Description-Content-Type: text/markdown
 
 # Modelon-impact-client
+
 Client library for easy scripting against Modelon Impact
 
 ## Installation
 
 For installation instructions and requirements, please refer to the [documentation](https://modelon-impact-client.readthedocs.io).
 
 ## Develop
 
 ### Devcontainer
+
 If you are developing with VS Code you can use the devcontainer which gives gives you a ready to use environment for development. Just click the "Reopen in Container" button after opening the project in VS Code.
 
 #### Tips and tricks
+
 It is possible to run the 'make' commands listed bellow using the devcontainer. It will detect being in a container and bypass Docker parts of the commands.
 
 You can open a project with the dev-container directly without having to open and then re-load. Standing in the project directory you can run:
+
 ```
 devcontainer open .
 ```
+
 Note that this requires the [devcontainer-cli](https://code.visualstudio.com/docs/remote/devcontainer-cli).
 
 You can add your own extensions to devcontainers. These extensions will be added for all devcontainers. First open your 'settings' as JSON. Then, to add for example the "GitLens" extension, put the following at the bottom of the settings:
+
 ```
     ...
     "remote.containers.defaultExtensions": ["eamodio.gitlens"]
 }
 ```
+
 VS Code also have a `'Install Local Extensions in 'Remote'` command, but it must be repeated for each devcontainer and everytime a devcontainer is re-built.
 
 ### Creating a shell
+
 Modelon-impact-client is developed using a Docker container for all build tools.
 You can get a shell into said container by running:
 
 ```
 make shell
 ```
 
 ### Manage dependencies
-Dependencies are managed by poetry. Add dependencies by running 
+
+Dependencies are managed by poetry. Add dependencies by running
 `poetry add <package>`  or `poetry add <package> --dev` inside the shell
 
 ### Running tests
 
 Tests are executed by running `make test`. You can also run `make test-watch` to get a watcher
 that continuously re-runs the tests.
 
 ### Running lint
+
 ```
 make lint
 ```
 
 ## Build
 
 Building modelon-impact-client is done by running
 
 ```
 make wheel
 ```
 
+## Test
+
+The tests for modelon-impact-client could be run by executing
+
+```
+make test
+```
+
+### VCR test
+
+Vcrpy(https://vcrpy.readthedocs.io/en/latest/) is used to mock the http requests and
+responses for some of the tests. VCR.py records all HTTP interactions that take place
+in a flat file called a 'cassette'. These files could are stored in the `impact-client-python/tests/fixtures/vcr_cassettes` folder. When an API response/request body is updated on MI, these files need to be regenerated. To regenerate these file, follow the following steps:
+
+1. Start Modelon impact cloud - https://impact.modelon.cloud.
+2. Generate an MI api key and JH token and store them in secrets folder. See [Readme](.secrets/README.md) for more information.
+3. Delete the cassette file you wish to regenerate from `impact-client-python/tests/fixtures/vcr_cassettes` folder.
+4. The file could now be regenrated by executing
+
+```
+make regenerate-cassette
+```
+
 ## Release
 
 The modelon-impact-client build process is a fully automated using `Semantic-release`.
 
 Automation is enabled for:
+
 - Bumping version
 - Generate changelog
 
 This is done based on git commit semantics as described here: https://semantic-release.gitbook.io/semantic-release/
 
 To make a new release simply run:
+
 ```
 make publish
 ```
 
 This command will detect what branch you are on and your git history and make a appropriate release.
 
 Current configuration can be found in `.releaserc` and specifies that commits to branch `master` should be released and
```

