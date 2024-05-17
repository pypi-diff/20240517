# Comparing `tmp/onediff-1.0.0.dev202405150127.tar.gz` & `tmp/onediff-1.1.0.dev202405160127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202405150127.tar", last modified: Wed May 15 01:27:58 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405160127.tar", last modified: Thu May 16 01:27:52 2024, max compression
```

## Comparing `onediff-1.0.0.dev202405150127.tar` & `onediff-1.1.0.dev202405160127.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.752598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.752598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.008592 onediff-1.1.0.dev202405160127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-16 01:27:52.008592 onediff-1.1.0.dev202405160127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:27:52.008592 onediff-1.1.0.dev202405160127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.992592 onediff-1.1.0.dev202405160127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77140 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:51.996592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/nexfort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/core/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/core/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/nexfort/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.000592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.004592 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.004592 onediff-1.1.0.dev202405160127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.004592 onediff-1.1.0.dev202405160127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.004592 onediff-1.1.0.dev202405160127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.008592 onediff-1.1.0.dev202405160127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-16 01:27:51.000000 onediff-1.1.0.dev202405160127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-16 01:27:51.000000 onediff-1.1.0.dev202405160127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:27:51.000000 onediff-1.1.0.dev202405160127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 01:27:51.000000 onediff-1.1.0.dev202405160127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:27:51.000000 onediff-1.1.0.dev202405160127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:52.008592 onediff-1.1.0.dev202405160127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-16 01:27:46.000000 onediff-1.1.0.dev202405160127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202405150127/LICENSE` & `onediff-1.1.0.dev202405160127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/PKG-INFO` & `onediff-1.1.0.dev202405160127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405150127
+Version: 1.1.0.dev202405160127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
+Author-email: contact@siliconflow.com
+License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405150127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405160127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
-caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
+contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
```

### Comparing `onediff-1.0.0.dev202405150127/README.md` & `onediff-1.1.0.dev202405160127/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/setup.py` & `onediff-1.1.0.dev202405160127/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
 setup(
     name="onediff",
     version=get_version(),
     description="an out-of-the-box acceleration library for diffusion models",
     url="https://github.com/siliconflow/onediff",
     author="OneDiff contributors",
-    license="Apache",
-    author_email="caishenghang@oneflow.org",
+    license="Apache-2.0",
+    license_files=('LICENSE',),
+    author_email="contact@siliconflow.com",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.8.0",
     install_requires=[
         "transformers>=4.27.1",
         "diffusers>=0.19.3",
         "accelerate",
```

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,17 @@
 
         return tensor
 
     def get_attention_scores(self, query, key, attention_mask=None):
         if self.upcast_attention and parse_boolean_from_env(
             "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION", True
         ):
-            set_boolean_env_var("ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION", False)
+            set_boolean_env_var(
+                "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION", False
+            )
         dtype = query.dtype
         # if self.upcast_attention:
         #     query = query.float()
         #     key = key.float()
 
         if attention_mask is None:
             baddbmm_input = torch.empty(
```

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from onediff.infer_compiler import register
+from onediff.infer_compiler.transform import register
 
 import oneflow as flow
 import diffusers_enterprise_lite
 
 torch2oflow_class_map = {
     diffusers_enterprise_lite.ProxyFakeModule: diffusers_enterprise_lite.OneFlowFakeHPCModule,
     diffusers_enterprise_lite.ProxyDynamicConvModule: diffusers_enterprise_lite.OneFlowDynamicHPCConvModule,
```

### Comparing `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405160127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from onediff.infer_compiler import register
+from onediff.infer_compiler.transform import register
 
 import oneflow as flow
 import onediff_quant
 
 torch2oflow_class_map = {
     onediff_quant.FakeQuantModule: onediff_quant.OneFlowFakeQuantModule,
     onediff_quant.StaticQuantConvModule: onediff_quant.OneFlowStaticQuantConvModule,
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import torch
 from .registry import register_backend
-from ..utils.options import CompileOptions
-from ..utils.param_utils import state_update_hook, init_state_update_attr, forward_pre_check_and_update_state_hook, forward_generate_constant_folding_info_hook
 
 
 @register_backend("oneflow")
 def compile(torch_module: torch.nn.Module, *, options=None):
     """
     Transform a torch nn.Module to oneflow.nn.Module, then optimize it with oneflow.nn.Graph.
     Args:
@@ -17,21 +15,29 @@
                      default True.
         - 'use_graph' whether to optimize with oneflow.nn.Graph, default True.
         - 'debug' which config the nn.Graph debug level, default -1(no debug info), max 3(max debug info).
         - 'size' which config the cache size when cache is enabled. Note that after onediff v0.12, cache is default disabled.
         - 'graph_file' (None) generates a compilation cache file. If the file exists, loading occurs; if not, the compilation result is saved after the first run.
         - 'graph_file_device' (None) sets the device for the graph file, default None.  If set, the compilation result will be converted to the specified device.
     """
-    from ..transform.custom_transform import set_default_registry
     from ..oneflow.deployable_module import OneflowDeployableModule
     from ..oneflow.utils import get_mixed_deployable_module
+    from ..transform.custom_transform import set_default_registry
+    from ..utils import CompileOptions, set_oneflow_env_vars
+    from ..utils.param_utils import (
+        state_update_hook,
+        init_state_update_attr,
+        forward_pre_check_and_update_state_hook,
+        forward_generate_constant_folding_info_hook,
+    )
 
     set_default_registry()
 
     options = options if options is not None else CompileOptions()
+    set_oneflow_env_vars(options.oneflow)
 
     def wrap_module(module):
         if isinstance(module, OneflowDeployableModule):
             assert not module._is_raw_deployable_module
             return module.__class__.from_existing(
                 module, options.dynamic, options.oneflow
             )
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import inspect
 import os
 import torch
 from oneflow.mock_torch import enable
 from oneflow.mock_torch.mock_importer import _importer
 from .import_module_utils import import_module_from_path
 from ..utils.log_utils import logger
+from ..utils.patch_for_compiler import *
 
 __all__ = ["DynamicMockModule"]
 
 
 def _get_module(full_name: str):
     try:
         attrs = full_name.split(".")
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import types
 import torch
 import oneflow as flow
 
+from ..core.deployable_module import DeployableModule
 from ..transform.manager import transform_mgr
 from ..utils.oneflow_exec_mode import oneflow_exec_mode, oneflow_exec_mode_enabled
 from ..utils.args_tree_util import input_output_processor
 from ..utils.log_utils import logger
-from ..utils.param_utils import parse_device, check_device
+from ..utils.param_utils import parse_device, check_device, generate_constant_folding_info
 from ..utils.graph_management_utils import graph_file_management
 from ..utils.online_quantization_utils import quantize_and_deploy_wrapper
 from ..utils.options import OneflowCompileOptions
-from ..deployable_module import DeployableModule
 
 from .utils import handle_deployable_exception, get_mixed_dual_module, get_oneflow_graph
 
 
 class OneflowDeployableModule(DeployableModule):
     def __init__(
         self, torch_module, oneflow_module, dynamic=True, options=None,
@@ -145,14 +145,15 @@
     def __getattr__(self, name):
         return getattr(self._deployable_module_model, name)
 
     def load_graph(self, file_path, device=None, run_warmup=True, *, state_dict=None):
         self.get_graph().load_graph(
             file_path, device, run_warmup, state_dict=state_dict
         )
+        generate_constant_folding_info(self)
 
     def save_graph(self, file_path, *, process_state_dict=lambda x: x):
         self.get_graph().save_graph(file_path, process_state_dict=process_state_dict)
 
     def extra_repr(self) -> str:
         return self._deployable_module_model.extra_repr()
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import warnings
 from typing import Union, List
 from collections import defaultdict
 import torch
-from onediff.infer_compiler.deployable_module import DeployableModule
+from onediff.infer_compiler import DeployableModule
 
 _nested_counter = defaultdict(lambda: 0)
 
 
 class TensorInplaceAssign:
     r"""
     This class is used as a context manager, instantiated with either a `torch.nn.Module` or
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import oneflow as flow
-
 _ONEFLOW_EXEC_MODE = False
 
 
 class oneflow_exec_mode(object):
     def __init__(self, enabled=None):
         if enabled is not None:
             self.enabled = enabled
         else:
             self.enabled = True
 
     def __enter__(self):
+        import oneflow as flow
+
         global _ONEFLOW_EXEC_MODE
         self.prev_mode = _ONEFLOW_EXEC_MODE
         _ONEFLOW_EXEC_MODE = self.enabled
         self.prev_grad_mode = flow.is_grad_enabled()
         _ = flow.set_grad_enabled(False)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        import oneflow as flow
+
         global _ONEFLOW_EXEC_MODE
         _ONEFLOW_EXEC_MODE = self.prev_mode
         _ = flow.set_grad_enabled(self.prev_grad_mode)
 
 
 def oneflow_exec_mode_enabled():
     global _ONEFLOW_EXEC_MODE
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 
 STATE_UPDATED_ATTR = "_onediff_state_updated"
 CONSTANT_FOLDING_INFO_ATTR = "_onediff_constant_folding_info"
 GRAPH_RELATED_TENSOR_ATTR = "_onediff_graph_related_tensor"
 
 
 def init_state_update_attr(module: torch.nn.Module):
-    from onediff.infer_compiler.deployable_module import DeployableModule
+    from onediff.infer_compiler import DeployableModule
 
     if isinstance(module, DeployableModule):
         module = module._torch_module
     if not isinstance(module, torch.nn.Module):
         raise TypeError(f"module must be a torch.nn.Module, got {type(module)}")
     setattr(module, STATE_UPDATED_ATTR, False)
 
 
 def set_constant_folded_conv_attr(
     deployable_module, constant_folding_info: Dict[str, flow.Tensor] = None
 ) -> None:
-    from onediff.infer_compiler.deployable_module import DeployableModule
+    from onediff.infer_compiler import DeployableModule
 
     if not isinstance(deployable_module, DeployableModule):
         raise TypeError(
             f"deployable_model must be a DeployableModule, got {type(deployable_module)}"
         )
 
     constant_folding_info = constant_folding_info or get_constant_folding_info(
@@ -86,15 +86,15 @@
     # to 'input_blocks.10.0.in_layers.2.weight'
     def convert_var_name(s: str, prefix="variable_transpose_"):
         s = removeprefix(s, prefix)
         s = re.sub(r"_[0-9]+$", "", s)
         s = removeprefix(s, "model.")
         return s
 
-    from onediff.infer_compiler.deployable_module import DeployableModule
+    from onediff.infer_compiler import DeployableModule
 
     if not isinstance(deployable_module, DeployableModule):
         raise TypeError(
             f"deployable_model must be a DeployableModule, got {type(deployable_module)}"
         )
     if torch_module is None:
         torch_module = deployable_module._torch_module
@@ -111,15 +111,15 @@
     setattr(deployable_module, CONSTANT_FOLDING_INFO_ATTR, result)
     set_constant_folded_conv_attr(deployable_module, result)
 
 
 def update_graph_with_constant_folding_info(
     module: torch.nn.Module, info: Dict[str, flow.Tensor] = None
 ) -> None:
-    from onediff.infer_compiler.deployable_module import DeployableModule
+    from onediff.infer_compiler import DeployableModule
 
     if isinstance(module, DeployableModule):
         if info is None:
             info = get_constant_folding_info(module)
         module = module._torch_module
     if info is None:
         return
@@ -142,15 +142,15 @@
         return
     target_tensor.copy_(
         flow.utils.tensor.from_torch(module.weight.data.permute(0, 2, 3, 1))
     )
 
 
 def get_constant_folding_info(module) -> Union[Dict[str, flow.Tensor], None]:
-    from onediff.infer_compiler.deployable_module import DeployableModule
+    from onediff.infer_compiler import DeployableModule
 
     if not isinstance(module, DeployableModule):
         raise TypeError(f"module must be a DeployableModule, got {type(module)}")
     return getattr(module, CONSTANT_FOLDING_INFO_ATTR, None)
 
 
 def state_update_hook(module, incompatible_keys):
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.1.0.dev202405160127/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405160127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405160127/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405160127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405160127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405160127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405160127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405160127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405160127/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405150127
+Version: 1.1.0.dev202405160127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
+Author-email: contact@siliconflow.com
+License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405150127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405160127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
-caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
+contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
```

### Comparing `onediff-1.0.0.dev202405150127/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405160127/src/onediff.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 src/onediff/__init__.py
 src/onediff.egg-info/PKG-INFO
 src/onediff.egg-info/SOURCES.txt
 src/onediff.egg-info/dependency_links.txt
 src/onediff.egg-info/requires.txt
 src/onediff.egg-info/top_level.txt
 src/onediff/infer_compiler/__init__.py
-src/onediff/infer_compiler/deployable_module.py
-src/onediff/infer_compiler/with_fx_graph.py
-src/onediff/infer_compiler/with_fx_interpreter.py
-src/onediff/infer_compiler/with_onediff_compile.py
 src/onediff/infer_compiler/backends/__init__.py
+src/onediff/infer_compiler/backends/nexfort.py
 src/onediff/infer_compiler/backends/oneflow.py
 src/onediff/infer_compiler/backends/registry.py
+src/onediff/infer_compiler/core/__init__.py
+src/onediff/infer_compiler/core/deployable_module.py
+src/onediff/infer_compiler/core/with_onediff_compile.py
 src/onediff/infer_compiler/import_tools/__init__.py
 src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
 src/onediff/infer_compiler/import_tools/format_utils.py
 src/onediff/infer_compiler/import_tools/import_module_utils.py
 src/onediff/infer_compiler/import_tools/importer.py
+src/onediff/infer_compiler/nexfort/__init__.py
+src/onediff/infer_compiler/nexfort/deployable_module.py
 src/onediff/infer_compiler/oneflow/__init__.py
 src/onediff/infer_compiler/oneflow/config.py
 src/onediff/infer_compiler/oneflow/deployable_module.py
 src/onediff/infer_compiler/oneflow/dual_module.py
 src/onediff/infer_compiler/oneflow/graph.py
 src/onediff/infer_compiler/oneflow/utils.py
 src/onediff/infer_compiler/transform/__init__.py
```

### Comparing `onediff-1.0.0.dev202405150127/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405160127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405160127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405150127/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405160127/tests/test_quantitative_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from skimage.metrics import structural_similarity as ssim
 from PIL import Image
 import numpy as np
 import unittest
 
-class  QuantizeQuality(unittest.TestCase):
+class QuantizeQuality(unittest.TestCase):
 
     def test_validate(self):
         image1 = np.array(Image.open('/share_nfs/civitai/20240407-163408.jpg').convert('RGB'))
         image2 = np.array(Image.open('/src/onediff/output_enterprise_sd.png').convert('RGB'))
         # Calculate SSIM
         ssim_index = ssim(image1, image2, multichannel=True, win_size=3)
         print("SSIM:", ssim_index)
```

### Comparing `onediff-1.0.0.dev202405150127/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405160127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

