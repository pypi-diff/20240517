# Comparing `tmp/onnxscript-0.1.0.dev20240515.tar.gz` & `tmp/onnxscript-0.1.0.dev20240516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240515.tar", last modified: Wed May 15 00:01:03 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240516.tar", last modified: Thu May 16 00:01:02 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240515.tar` & `onnxscript-0.1.0.dev20240516.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.269025 onnxscript-0.1.0.dev20240515/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.273025 onnxscript-0.1.0.dev20240515/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.273025 onnxscript-0.1.0.dev20240515/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.273025 onnxscript-0.1.0.dev20240515/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.273025 onnxscript-0.1.0.dev20240515/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.269025 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.273025 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.281026 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.269025 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.269025 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.281026 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.281026 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.281026 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.285025 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.285025 onnxscript-0.1.0.dev20240515/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2702 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    92963 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20889 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/_type_casting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58627 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.285025 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.289026 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.289026 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6735 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26344 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/bfloat16_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5171 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40099 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-15 00:01:03.000000 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-15 00:01:03.000000 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-15 00:01:03.000000 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-15 00:01:03.000000 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-15 00:01:03.000000 onnxscript-0.1.0.dev20240515/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-15 00:01:03.293026 onnxscript-0.1.0.dev20240515/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-15 00:00:45.000000 onnxscript-0.1.0.dev20240515/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.806840 onnxscript-0.1.0.dev20240516/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.806840 onnxscript-0.1.0.dev20240516/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.826840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.830841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.830841 onnxscript-0.1.0.dev20240516/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2702 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    93832 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2962 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20889 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_type_casting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58555 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.834841 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.842841 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.842841 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.846841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6735 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26344 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5171 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40099 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240515/LICENSE` & `onnxscript-0.1.0.dev20240516/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/PKG-INFO` & `onnxscript-0.1.0.dev20240516/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240515
+Version: 0.1.0.dev20240516
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/ebee154f631fefc2cd5a6006d611d135f1181d1c
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b77f39393b9bba2fbb69a8e972fc8a36d2e811fb
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240515/README.md` & `onnxscript-0.1.0.dev20240516/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "opset18",
     "opset19",
     "opset20",
     "opset_ai_onnx_ml1",
     "opset_ai_onnx_ml2",
     "opset_ai_onnx_ml3",
     "opset_ai_onnx_ml4",
+    "DEBUG",
 ]
 
 import importlib.metadata
 
 from .backend.onnx_export import export2python as proto2python
 from .main import export_onnx_lib, graph, script
 
@@ -118,12 +119,15 @@
 
 # isort: on
 
 from . import ir, optimizer, rewriter
 from ._internal.utils import external_tensor
 from .values import OnnxFunction, TracedOnnxFunction
 
+# Set DEBUG to True to enable additional debug checks
+DEBUG = False
+
 try:  # noqa: SIM105
     __version__ = importlib.metadata.version("onnxscript")
 except importlib.metadata.PackageNotFoundError:
     # package is not installed
     pass
```

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240516/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240516/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1353,26 +1353,37 @@
         "_type",
         "_uses",
         "doc_string",
     )
 
     def __init__(
         self,
-        producer: Node | None,
+        producer: Node | None = None,
         *,
-        index: int | None,
+        index: int | None = None,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
         doc_string: str | None = None,
         const_value: _protocols.TensorProtocol
         | Sequence[_protocols.TensorProtocol]
         | None = None,
     ) -> None:
-        # producer is None when the value is an input or an initializer
+        """Initialize a value.
+
+        Args:
+            producer: The node that produces the value.
+                It can be ``None`` when the value is initialized first than its producer.
+            index: The index of the output of the defining node.
+            name: The name of the value.
+            shape: The shape of the value.
+            type: The type of the value.
+            doc_string: The documentation string.
+            const_value: The constant tensor is the value constant.
+        """
         self._producer: Node | None = producer
         self._index: int | None = index
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
 
         self._name: str | None = name
         self._shape: Shape | None = shape
@@ -1402,15 +1413,19 @@
         type_text = str(self.type) if self.type is not None else "?"
 
         # Quote the name because in reality the names can have invalid characters
         # that make them hard to read
         return f"%{_quoted(value_name)}<{type_text},{shape_text}>"
 
     def producer(self) -> Node | None:
-        """The node that produces this value."""
+        """The node that produces this value.
+
+        When producer is ``None``, the value does not belong to a node, and is
+        typically a graph input or an initializer.
+        """
         return self._producer
 
     def index(self) -> int | None:
         """The index of the output of the defining node."""
         return self._index
 
     def uses(self) -> Collection[tuple[Node, int]]:
@@ -1546,17 +1561,15 @@
     def __init__(
         self,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
         doc_string: str | None = None,
     ) -> None:
-        super().__init__(
-            None, index=None, name=name, shape=shape, type=type, doc_string=doc_string
-        )
+        super().__init__(name=name, shape=shape, type=type, doc_string=doc_string)
 
 
 def _check_node_safe_to_remove(
     node: Node, to_remove: AbstractSet[Node], graph_outputs: AbstractSet[Value]
 ) -> None:
     """Check if a node is safe to remove.
 
@@ -1708,19 +1721,17 @@
     def _set_node_graph_to_self_and_assign_names(self, node: Node) -> Node:
         """Set the graph reference for the node and assign names to it and its outputs if they don't have one."""
         if node.graph is not None and node.graph is not self:
             raise ValueError(
                 f"The node '{node!r}' belongs to another graph. Please remove it first with Graph.remove()."
             )
         # Give the node and its output values names if they don't not have one
-        if node.name is None:
-            self._name_authority.name_node(node)
+        self._name_authority.register_or_name_node(node)
         for value in node._outputs:  # pylint: disable=protected-access
-            if value.name is None:
-                self._name_authority.name_value(value)
+            self._name_authority.register_or_name_value(value)
         node.graph = self
         return node
 
     def node(self, index_or_name: int | str, /) -> Node:
         """Get a node by index or name.
 
         This is an O(n) operation. Getting nodes on the ends of the graph (0 or -1) is O(1).
@@ -1762,26 +1773,30 @@
         # NOTE: This is a method specific to Graph, not required by the protocol unless proven
         return len(self)
 
     # Mutation methods
     def append(self, node: Node, /) -> None:
         """Append a node to the graph in O(1) time.
 
+        Unique names will be assigned to the node and its values if any name is ``None``.
+
         Args:
             node: The node to append.
 
         Raises:
             ValueError: If the node belongs to another graph.
         """
         self._set_node_graph_to_self_and_assign_names(node)
         self._nodes.append(node)
 
     def extend(self, nodes: Iterable[Node], /) -> None:
         """Extend the graph with the given nodes in O(#new_nodes) time.
 
+        Unique names will be assigned to the node and its values if any name is ``None``.
+
         Args:
             nodes: The nodes to extend the graph with.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
         nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in nodes]
@@ -1826,14 +1841,16 @@
             # Set attributes to remove the node from this graph
             node.graph = None
             self._nodes.remove(node)
 
     def insert_after(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
         """Insert new nodes after the given node in O(#new_nodes) time.
 
+        Unique names will be assigned to the node and its values if any name is ``None``.
+
         Args:
             node: The node to insert after.
             new_nodes: The new nodes to insert.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
@@ -1841,14 +1858,16 @@
             new_nodes = (new_nodes,)
         new_nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in new_nodes]
         self._nodes.insert_after(node, new_nodes)
 
     def insert_before(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
         """Insert new nodes before the given node in O(#new_nodes) time.
 
+        Unique names will be assigned to the node and its values if any name is ``None``.
+
         Args:
             node: The node to insert before.
             new_nodes: The new nodes to insert.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
```

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/_type_casting.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240516/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,15 +586,15 @@
     )
 
 
 def deserialize_value_info_proto(
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
-        value = _core.Value(None, index=None, name=proto.name)
+        value = _core.Value(name=proto.name)
     value.shape = deserialize_type_proto_for_shape(proto.type)
     value.type = deserialize_type_proto_for_type(proto.type)
     metadata_props = deserialize_metadata_props(proto.metadata_props)
     if metadata_props is not None:
         value.metadata_props.update(metadata_props)
     value.doc_string = _get_field(proto, "doc_string")
     return value
@@ -843,30 +843,30 @@
             )
             if len(scoped_values) > 1:
                 logger.warning(
                     "Caveat: The value is created in the subgraph. If "
                     "the node is referencing a value that is not in the current graph, "
                     "it is impossible to create it in the correct scope.",
                 )
-            value = _core.Value(None, index=None, name=input_name)
+            value = _core.Value(name=input_name)
             # Fill in shape/type information if they exist
             if input_name in value_info:
                 deserialize_value_info_proto(value_info[input_name], value)
             node_inputs.append(value)
             # We can only create the value in the current scope. If the subgraph is
             # referencing a value that is not in the current scope, it is impossible
             # to create it in the correct scope.
             scoped_values[-1][input_name] = value
 
     # Build the output values for the node.
     node_outputs: list[_core.Value] = []
     for output_name in proto.output:
         if output_name == "":
             # Empty output
-            node_outputs.append(_core.Value(None, index=None, name=""))
+            node_outputs.append(_core.Value(name=""))
             continue
 
         # 1. When the graph is unsorted, we may be able to find the output already created
         # as an input to some other nodes in the current scope.
         # Note that a value is always owned by the producing node. Even though a value
         # can be created when parsing inputs of other nodes, the new node created here
         # that produces the value will assume ownership. It is then impossible to transfer
@@ -876,15 +876,15 @@
         # a node to produce an output that is not in its own scope.
         current_scope = scoped_values[-1]
         if output_name in current_scope:
             value = current_scope[output_name]
         else:
             # 2. Common scenario: the graph is sorted and this is the first time we see the output.
             # Create the value and add it to the current scope.
-            value = _core.Value(None, index=None, name=output_name)
+            value = _core.Value(name=output_name)
             current_scope[output_name] = value
         # Fill in shape/type information if they exist
         if output_name in value_info:
             deserialize_value_info_proto(value_info[output_name], value)
         else:
             logger.debug(
                 "ValueInfoProto not found for output '%s' in node '%s' of type '%s'",
```

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240516/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/main.py` & `onnxscript-0.1.0.dev20240516/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240516/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 
 from onnxscript import ir
 
 logger = logging.getLogger(__name__)
-CREATED_CAST_BFLOAT16_NAME_SUFFIX = "_cast_bfloat16"
 
 
 def _convert_inputs_from_bfloat16_to_float16(value: ir.Input) -> None:
     if value.dtype != ir.DataType.BFLOAT16:
         return
     value.dtype = ir.DataType.FLOAT16
     _insert_cast_nodes_for_float16_to_bfloat16_to_inputs(value)
@@ -57,17 +56,14 @@
         op_type="Cast",
         inputs=[node.outputs[index]],
         num_outputs=1,
         attributes=[attr],
     )
     cast.outputs[0].dtype = ir.DataType.FLOAT16
     cast.outputs[0].shape = node.outputs[index].shape
-    # To prevent naming conflicts, we need to append suffix to the output name of the cast node
-    # TODO: Remove this after naming authority covers this case
-    cast.outputs[0].name = node.outputs[index].name + CREATED_CAST_BFLOAT16_NAME_SUFFIX  # type: ignore[operator]
     node.append(cast)
 
     assert node.graph is not None, "Node graph should not be None"
     # Update graph/function outputs
     for idx, graph_or_function_output in enumerate(node.graph.outputs):
         if graph_or_function_output == node.outputs[index]:
             node.graph.outputs[idx] = cast.outputs[0]
```

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240516/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240516/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240516/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240516/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240516/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript/values.py` & `onnxscript-0.1.0.dev20240516/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240516/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240515
+Version: 0.1.0.dev20240516
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/ebee154f631fefc2cd5a6006d611d135f1181d1c
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b77f39393b9bba2fbb69a8e972fc8a36d2e811fb
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240515/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240516/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/pyproject.toml` & `onnxscript-0.1.0.dev20240516/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240515/setup.py` & `onnxscript-0.1.0.dev20240516/setup.py`

 * *Files identical despite different names*

